---
title: Angi flere rentesatser
description: "Du kan beregne rentebelastning med flere rentesatser for en bestemt periode. Renteberegningen fungerer på samme måte for alle rentebelastninger. Det er bare satsen for renten for en bestemt periode som varierer."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 3d4c111af62db5858b81b76f9f51a9093c01e5e6
ms.contentlocale: nb-no
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-multiple-interest-rates"></a>Angi flere rentesatser.
Flere rentesatser brukes for forskjellige perioder for forsinkede betalinger handelstransaksjoner. For eksempel angir en offentlig myndighet maksimal rente som kan pålegges for en kunde. Denne rentesatsen kan endres to ganger i året, 1. januar og 1. juli. Rentesatsen mellom bedrifter (B2B) avtales av partene, og det er ingen begrensning for denne kundegruppen. Annonsert sats er vanligvis 4 % mer enn vanlig bankrente.

Når du oppretter rentenotabetingelser og purrebetingelser for straff for forsinket betaling, kan du angi flere rentesatser slik at straffegebyret beregnes fra forskjellige renter i forskjellige perioder. Hvis du vil ha mer informasjon, kan du se [Innkreve utestående saldi](receivables-collect-outstanding-balances.md).

## <a name="to-set-up-multiple-interest-rates"></a>Angi flere rentesatser  
1.  Velg ikonet ![lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Rentenotabetingelser**, og velg deretter den relaterte koblingen.  
2.  I vinduet **Rentenotabetingelser** velger du den nødvendige rentebetingelsen, og deretter handlingen **Rentesatser**.  
3.  Fyll ut feltene etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  Velg **OK**.  
5.  Velg ikonet ![lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Purrebetingelser**, og velg deretter den relaterte koblingen.  
6.  I vinduet **Purrebetingelser** velger du den nødvendige purrebetingelsen, og deretter handlingen **Nivåer**.  
7.  I vinduet **Purregrader** velger du **Beregn renter**-feltet.  

Når du utsteder en rentenota, viser den rentebelastningene med flere rentesatser for en bestemt tidsperiode. Notaen inneholder også kontaktdetaljer for kunden, selskapet som utsteder notaen, tilleggsbeløpet og det totale beløpet. Åpningsposten på rentenotaen vises med fet skrift. Rentebelastningen beregnes med flere rentesatser for en bestemt tidsperiode, og skrives ut etter åpningsposten for rentenotaen.  

## <a name="see-also"></a>Se også  
[Innkreve utestående saldi](receivables-collect-outstanding-balances.md)  
[Konfigurere finans](finance-setup-finance.md)
