---
title: Levere varer| Microsoft-dokumentasjon
description: Avhengig av lageroppsettet kan du registrere levering på det tilknyttede utgående forretningsdokumentet direkte, for eksempel en ordre, eller du kan bruke lagerleveringsdokumenter som respekterer en arbeidsflyt og er integrert med ulike lageraktiviteter.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/03/2020
ms.author: edupont
ms.openlocfilehash: 9beffaa8e881717506d0c471b9e8bfb9feaf3168
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/09/2020
ms.locfileid: "3779137"
---
# <a name="ship-items"></a>Levere varer

Når du leverer varer fra et lager som ikke er definert til lagerleveringsbehandling, må du ganske enkelt registrere leveringen i det relaterte forretningsdokumentet, for eksempel en ordre, serviceordre, bestillingsretur eller utgående overføringsordre.

Når du leverer varer fra et lager som er definert til lagerleveringsbehandling, kan du levere varer bare på basis av kildedokumenter som andre enheter i selskapet har frigitt til lageret for behandling.

> [!NOTE]
> Hvis lageret bruker kryssoverføring og hyller, kan du for hver linje vise antall varer som er plassert i kryssoverføringshyllene. Programmet beregner disse antallene automatisk hver gang feltene på følgeseddelen oppdateres. Hvis dette er varer som gjelder for den leveringen du forbereder, kan du opprette en plukking for alle linjene, og deretter fullføre leveringen. Hvis du vil ha mer informasjon, kan du se [Kryssoverføre varer](warehouse-how-to-cross-dock-items.md).

## <a name="to-ship-items-with-a-sales-order"></a>Slik leverer du varer med en ordre

Fremgangsmåten nedenfor beskriver hvordan du leverer varer fra en ordre. Fremgangsmåten er lik for bestillingsreturer, serviceordrer og utgående overføringsordrer.  

1. Velg ikonet ![Lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Ordrer**, og velg deretter den relaterte koblingen.
2. Åpne en eksisterende ordre eller opprett en ny. Hvis du vil ha mer informasjon, kan du se [Selge produkter](sales-how-sell-products.md).
3. I feltet **Levere (antall)** angir du det leverte antallet.

    Verdien i feltet **Levert ant.** oppdateres. Hvis dette er en delvis levering, vil verdien være mindre enn verdien i feltet **Antall**.
4. Velg handlingen **Bokfør**.

> [!NOTE]
> Hvis organisasjonen ikke bruker ordrer, antar [!INCLUDE [prodshort](includes/prodshort.md)] at du har levert hele antallet når du bokfører salgsfakturaen. Hvis dette er i strid med hvordan organisasjonen arbeider, anbefaler vi at du bruker ordrer og registrerer leveringer som forklart i denne artikkelen.

## <a name="to-ship-items-with-a-warehouse-shipment"></a>Slik leverer du varer med en lagerlevering

Først oppretter du et leveringsdokument fra et forretningskildedokument. Deretter plukker du de angitte varene for leveringen.

### <a name="to-create-a-warehouse-shipment"></a>Slik oppretter du en lagerlevering

Vanligvis er det ansatte som er ansvarlige for leveringer, som oppretter en lagerlevering. Fremgangsmåten nedenfor viser hvordan du oppretter leveringen manuelt i standardversjonen av [!INCLUDE[prodshort](includes/prodshort.md)], men organisasjonen kan ha automatiserte deler av prosessen, for eksempel med bruk av håndholdte eller monterte skannere som støttes av eksterne leverandører.  

1. Velg ikonet ![Lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Lagerleveringer**, og velg deretter den relaterte koblingen.  
2. Velg handlingen **Ny**.  

    Fyll ut feltene på hurtigfanen **Generelt**. Når du mottar kildedokumentlinjer, kopieres noe av informasjonen til hver linje.  

    For lageroppsett med lagerstyring: Hvis lokasjonen har en standard sone og hylle for leveringer, fylles feltene **Sonekode** og **Hyllekode** ut automatisk, men du kan endre dem slik det passer.  

    > [!NOTE]  
    > Hvis du vil levere varer med andre lagerklassekoder enn lagerklassekoden til hyllen i feltet **Hyllekode** i dokumenthodet, må du slette innholdet i feltet **Hyllekode** før du henter kildedokumentlinjene for varene.  
3. Velg handlingen **Hent kildedokumenter**. Siden **Kildedokumenter** åpnes.

    Fra en ny eller åpen lagerlevering kan du bruke siden **Filtre for henting av kildedok** til å hente linjene i det frigitte kildedokument som definerer hvilke varer som skal leveres.

    1. Velg handlingen **Bruk filtre til å hente k.dok...**.  
    2. Hvis du vil definere et nytt filter, angir du en beskrivende kode i feltet **Kode** og velger deretter handlingen **Endre**.  
    3. Definer typen kildedokumentlinjer som du vil hente, ved å fylle ut de relevante filterfeltene.  
    4. Velg handlingen **Kjør**.  

    Alle frigitte kildedokumentlinjer som oppfyller filterkriteriene, settes nå inn på siden **Lagerlevering** der du aktiverte filterfunksjonen.  

    Filterkombinasjonene du definerer, lagres på siden **Filtre for henting av kildedok** til neste gang du trenger dem. Du kan opprette et ubegrenset antall filterkombinasjoner. Du kan når som helst endre kriteriene ved å velge handlingen **Endre**.

4. Velg kildedokumentene som du vil levere varer for, og velg deretter **OK**-knappen.  

Linjene i kildedokumentet vises på siden **Lagerlevering**. Feltet **Levere (antall)** er fylt ut med antall utestående for hver linje, men du kan endre antallet slik det er nødvendig. Hvis du sletter innholdet i feltet **Hyllekode** i hurtigfanen **Generelt** før du henter linjene, må du fylle ut riktig hyllekode på hver leveringslinje.  

> [!NOTE]  
> Du kan ikke levere flere varer enn det som er angitt i feltet **Restantall** på kildedokumentlinjen. Hvis du vil levere flere varer, må du hente et annet kildedokument som inneholder en linje for varen, ved å bruke filtreringsfunksjonen for å hente kildedokumenter med varen.  

Når du har de linjene du vil levere, kan du starte prosessen som sender linjene til lageransatte for plukking.

### <a name="to-pick-and-ship"></a>Slik plukker og leverer du

Vanligvis er det en lagermedarbeider som er ansvarlig for plukking, som oppretter et plukkdokument eller åpner et allerede opprettet plukkdokument.  

1. Velg ikonet ![Lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Lagerleveringer**, og velg deretter den relaterte koblingen.
2. Velg lagerlevringen som du vil plukke for, og velg deretter **Opprett plukk**-handlingen.
3. Fyll ut feltene på forespørselssiden, og velg deretter **OK**. Det angitte lagerplukkdokumentet opprettes.

    Du kan også åpne et eksisterende lagerplukk.
4. Velg ikonet ![Lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Plukking**, og velg deretter den relaterte koblingen. Velg plukkingen du vil arbeide med.

    Hvis lageret definert for bruk av hyller, så er plukklinjene konvertert til linjer for henting og plassering.

    Du kan sortere linjene, tilordne en ansatt til plukkingen, definere et anbrekksfilter (hvis du bruker lagerstyring), og plukke og skrive ut plukkinstruksjonene.

5. Utfør den faktiske plukkingen av varer, og plasser dem i den angitte leveringshyllen eller i leveringsområdet hvis du ikke har hyller.
6. Velg handlingen **Registrer plukk**.

    Feltet **Levere (antall)** og feltet **Dokumentstatus** i hodet for leveringsdokumentet oppdateres. Varene du har plukket, er ikke lenger tilgjengelige for plukking til andre leveringer eller for interne operasjoner.
7. Skriv ut leveringsdokumentene, forbered leveringspakkene og bokfør deretter leveringen.

Hvis du vil ha mer informasjon om hvordan du plukker for lagerlevering, kan du se [Plukke varer for lagerlevering](warehouse-how-to-pick-items-for-warehouse-shipment.md).

Du kan også bruke plukkforslaget til å gjøre flere plukkinstruksjoner om til én instruksjon (for flere leveringer), og derved forbedre effektiviteten for plukkingen i lageret. Hvis du vil ha mer informasjon, kan du se [Planlegge plukkinger i forslaget](warehouse-how-to-plan-picks-in-worksheets.md)

> [!NOTE]
> Hvis du venter på at en bestemt vare skal ankomme lageret og du bruker kryssoverføringsfunksjonalitet, så beregner [!INCLUDE[d365fin](includes/d365fin_md.md)], på hver følgeseddel- eller plukkforslagslinje, antallet for varen som er i kryssoverføringshyllen. Dette feltet oppdateres hver gang du går ut av eller åpner følgeseddelen eller forslaget. Hvis du vil ha mer informasjon, kan du se [Kryssoverføre varer](warehouse-how-to-cross-dock-items.md).

## <a name="see-also"></a>Se også

[Lagerstyring](warehouse-manage-warehouse.md)  
[Lager](inventory-manage-inventory.md)  
[Definere lagerstyring](warehouse-setup-warehouse.md)  
[Monteringsstyring](assembly-assemble-items.md)  
[Designdetaljer: Lagerstyring](design-details-warehouse-management.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
