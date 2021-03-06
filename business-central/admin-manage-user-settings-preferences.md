---
title: Behandle brukerinnstillinger og innstillinger i Dynamics 365 Business Central
description: Behandle brukerinnstillinger og innstillinger i Dynamics 365 Business Central.
author: sorenfriisalexandersen
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: user settings, preferences, language, region, time zone, regional settings
ms.date: 06/17/2020
ms.author: soalex
ms.openlocfilehash: 633a0872a878843f26d627dcd76e69d1c851ef8a
ms.sourcegitcommit: 3945f16d6d9c9853651e6291ce1465a44fd71fc8
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/17/2020
ms.locfileid: "3460423"
---
# <a name="manage-user-settings-and-preferences"></a>Behandle brukerinnstillinger og innstillinger

Du kan som administrator behandle brukerinnstillinger i [!INCLUDE[d365fin](includes/d365fin_md.md)], på samme måte som enkeltbrukere kan behandle sine egne innstillinger på siden **Mine innstillinger**.  

## <a name="types-of-user-settings"></a>Typer brukerinnstillinger

*Brukerinnstillinger* er ikke det samme som *brukeroppsett*, som er om brukeren som en enhet og brukerens tilgang i systemet. I tillegg har brukerinnstillinger ingenting å gjøre med en brukers tilpassing, for eksempel ved å gjøre endringer i brukergrensesnittet. Brukerinnstillinger bestemmer brukerens innstillinger på ulike deler av måten programmet vises for brukeren. Det følgende avsnittet inneholder de fem typene brukerinnstillinger og innstillinger som kan angis av enkeltbrukeren eller sentralt av administratoren:

- **Selskap**  

  Denne innstillingen bestemmer hvilket selskap som skal logges på ved neste pålogging. En bruker kan ha tilgang til flere selskaper og kan være aktive i flere selskaper.

- **Profil (roller)**  

  Profilen beskriver brukerens funksjon i selskapet, for eksempel *salgssjef*, *regnskapsfører* eller *innkjøper*. Profilen bestemmer deretter brukerens rollesenter, hjemmesiden som brukerne vil se når de logger på. Profilen påvirker ikke tilgangsrettigheter til funksjoner i [!INCLUDE[d365fin](includes/d365fin_md.md)].  

- **Lokal ID (områdeinnstillinger)**  

  Definerer hvordan datoer og numre presenteres i [!INCLUDE[d365fin](includes/d365fin_md.md)]-klienten, for eksempel om det skal brukes europeiske eller amerikanske datoformater, eller hvordan desimaltegn og tusenskilletegn skal vises i beløp. Hvis [!INCLUDE[d365fin](includes/d365fin_md.md)]-brukere synkroniseres fra Office 365, brukes områdeinnstillinger fra Office 365, og det antas at brukeren vil bruke de samme innstillingene i Office-produkter og [!INCLUDE[d365fin](includes/d365fin_md.md)]. En administrator eller bruker kan endre disse innstillingene manuelt i [!INCLUDE[d365fin](includes/d365fin_md.md)], men de tilbakestilles til verdien fra Office 365 når den neste synkroniseringen blir utført.

- **Språk**  

  Definerer programspråket som [!INCLUDE[d365fin](includes/d365fin_md.md)] presenterer tekst, titler og feilmeldinger i. Hvis [!INCLUDE[d365fin](includes/d365fin_md.md)]-brukere synkroniseres fra Office 365, brukes språkinnstillinger fra Office 365, og det antas at brukeren vil bruke de samme innstillingene i Office-produkter og [!INCLUDE[d365fin](includes/d365fin_md.md)]. En administrator eller bruker kan endre disse innstillingene manuelt i [!INCLUDE[d365fin](includes/d365fin_md.md)], men de tilbakestilles til verdien fra Office 365 når den neste synkroniseringen blir utført.

  Hvis språkinnstillingen fra Office 365 samsvarer med et språk som støttes i [!INCLUDE[d365fin](includes/d365fin_md.md)], velges dette språket for brukeren.  

  > [!NOTE]
  > Du må kanskje installere en språkapp for [!INCLUDE[d365fin](includes/d365fin_md.md)] for å kunne vise språket. Det er derfor en god praksis å installere de nødvendige språkappene før alle brukere logger på for første gang, slik at de får en god opplevelse den første dagen. Hvis du vil ha mer informasjon, kan du se listen over [språk som støttes](/dynamics365/business-central/dev-itpro/compliance/apptest-countries-and-translations).  
  
- **Tidssone**  

  Definerer tidssonen brukeren befinner seg i. Dette synkroniseres for øyeblikket ikke fra Office 365 og må angis manuelt.  

> [!NOTE]
> Hvis det gjøres en Office 365-brukersynkronisering mens brukerne er logget på [!INCLUDE[d365fin](includes/d365fin_md.md)], må disse brukerne oppdatere nettleseren eller logge av og på [!INCLUDE[d365fin](includes/d365fin_md.md)] for å se et mulig språk som er angitt av synkroniseringshandlingen.

## <a name="overview-of-all-user-settings"></a>Oversikt over alle brukerinnstillinger

Administratorer har muligheten til å angi eller endre disse innstillingene for brukere i hvert enkelt selskap. Dette gjør du på siden **Brukertilpassinger**. Oppføringer på denne siden vil gjenspeile de enkelte brukerens valg for innstillingene ovenfor, én oppføring per bruker. Når brukere endrer innstillingene på siden **Mine innstillinger**, vil disse endringene gjenspeiles i listen **Brukertilpassinger**. Administratorer kan også angi disse innstillingene for brukere før de logger på for første gang, slik at brukerne ikke trenger å gjøre det selv, noe som gir dem en bedre *Komme i gang*-opplevelse.

> [!NOTE]
> Brukertilpassinger har ikke noe å gjøre med *personlige*, enkle endringer en bruker kan gjøre i brukeropplevelsen.

## <a name="to-review-or-make-changes-to-user-settings"></a>Slik går du gjennom eller endrer brukerinnstillinger

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Ikonet Søk etter side eller rapport"), angi **Brukertilpassinger**, og velg deretter den relaterte koblingen.
2. Dette viser listen over brukere og tilhørende innstillinger. Hvis du vil endre en brukers innstillinger, klikker du på **bruker-ID-en** eller velger **Behandle** og deretter **Rediger**.
3. Kortet **Brukertilpassing** for den bestemte brukerens innstillinger vises, og eventuelle endringer kan gjøres.  

## <a name="see-also"></a>Se også

[Komme i gang](product-get-started.md)  
[Land-/områdetilgjengelighet og støttede oversettelser](/dynamics365/business-central/dev-itpro/compliance/apptest-countries-and-translations)  
[Endre språk og nasjonal innstilling](about-locale-language.md)  
