---
title: Feilsøke synkroniseringsfeil | Microsoft Docs
description: Gir veiledning for identifisering og løsing av synkroniseringsfeil.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: bholtorf
ms.openlocfilehash: 82b5f3ec52be27c4fbe60a6a63a0cfc5f6f1bd7c
ms.sourcegitcommit: d67328e1992c9a754b14c7267ab11312c80c38dd
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/01/2020
ms.locfileid: "3196546"
---
# <a name="troubleshooting-synchronization-errors"></a>Feilsøke synkroniseringsfeil
Mange bevegelige deler er involvert i integrasjon av [!INCLUDE[d365fin](includes/d365fin_md.md)] med Common Data Service, og noen ganger går det galt. I dette emnet omtales noen av de typiske feilene som oppstår, og det oppgis noen punkter for hvordan de skal løses.

Feil oppstår ofte enten på grunn av noe en bruker har gjort med koblede poster eller fordi noe er galt med hvordan integrasjonen er satt opp. Ved feil relatert til koblede poster kan brukere løse disse selv. Disse feilene skyldes handlinger som sletting av en post i én bedriftsapp, men ikke i begge bedriftsappene, og påfølgende synkronisering. Hvis du vil ha mer informasjon, kan du se [Vise statusen for en synkronisering](admin-how-to-view-synchronization-status.md).

## <a name="example"></a>Eksempel
Denne videoen viser et eksempel på hvordan du feilsøker feil som skjedde under synkronisering med Sales. Prosessen vil være den samme for alle integreringer. 

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2097304]

Feil som er relatert til hvordan integrasjonen er satt opp, må vanligvis håndteres av en administrator. Du kan se disse feilene på siden **Synkroniseringsfeil ved integrasjon**. Eksempler på noen vanlige problemer er:  
  
* Tillatelsene og rollene som er tilordnet til brukere, er ikke korrekte.  
* Administratorkontoen ble angitt som integrasjonsbrukeren.  
* Integrasjonsbrukerens passord er satt til å kreve en endring når brukeren logger seg på.  
* Valutakursene for valutaer er ikke angitt i én av appene.  
  
Du må løse feilene manuelt, men siden hjelper deg på noen måter. Eksempel:  

* Feltene **Kilde** og **Destinasjon** kan inneholde koblinger til posten der feilen ble funnet. Klikk på koblingen for å åpne posten og undersøke feilen.  
* Handlingene **Slett oppføringer eldre enn 7 dager** og **Slett alle oppføringer** rydder opp i listen. Vanligvis bruker du disse handlingene etter at du har løst årsaken til en feil som påvirker mange poster. Du må imidlertid være forsiktig. Disse handlingene kan slette feil som fremdeles er relevante.

Tidsangivelser av poster kan iblant forårsake konflikter. Tabellen "CDS-integreringspost" beholder tidsstempelene "Siste synkronisering endret den" og "Siste CDS-synkronisering endret den" for å få den siste integrasjonen gjort i begge retninger for en post. Disse tidsstemplene sammenlignes med tidsstempler i Business Central sentraler og salgsposter. I Business Central er tidsstempelet i tabellen for integreringspost.

Du kan filtrere på poster som skal synkroniseres ved å sammenligne posttidsstempler i tabellen "Tilordning for integreringstabell" i feltene "Filter for siste synkr.endr." og "Filter for siste synkr.endr. i intgr.tab."

Feilmeldingen om konflikt "Kan ikke oppdatere kundeposten fordi den har en senere endringsdato enn forretningsforbindelsesposten" eller "Kan ikke oppdatere forretningsforbindelsesposten fordi den har en senere endringsdato enn kundeposten" kan vises hvis en post har et tidsstempel som er større enn IntegrationTableMapping."Filter for siste synkr.endr.", men den ikke er nyere enn tidsstempelet for salgsintegreringsposten. Det betyr at kildeposten ble synkronisert manuelt, og ikke av posten i jobbkøen. 

Konflikten oppstår fordi målposten også ble endret – posttidsstemplet er nyere enn tidsstempelet for salgsintegrasjonsposten. Målkontrollen skjer bare for toveis tabeller. 

Disse postene flyttes nå til siden "Hoppet over synkroniserte poster", som du åpner fra siden Tilkoblingsoppsett for Microsoft Dynamics i Business Central. Der kan du angi endringene du vil beholde, og deretter synkronisere postene på nytt.

## <a name="see-also"></a>Se også
[Integrere med Common Data Service](admin-prepare-dynamics-365-for-sales-for-integration.md)  
[Sette opp brukerkontoer for integrasjon med Common Data Service](admin-setting-up-integration-with-dynamics-sales.md)  
[Sette opp en tilkobling til Common Data Service](admin-how-to-set-up-a-dynamics-crm-connection.md)  
[Sammenkoble og synkronisere poster manuelt](admin-how-to-couple-and-synchronize-records-manually.md)  
[Vise statusen for en synkronisering](admin-how-to-view-synchronization-status.md)  
