---
title: Få en oversikt over tilgjengelighet | Microsoft-dokumentasjon
description: Du kan få informasjon om tilgjengeligheten av varer eller beholdning på tvers av lokasjoner, per salg eller kjøpshendelser, etter en tidsperiode eller etter varens posisjon i en monterings- eller produksjonsstykkliste.
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: stock
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: a21bc82cc065f3d05863d3d3f9959dc4269a739a
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/09/2020
ms.locfileid: "3780038"
---
# <a name="view-the-availability-of-items"></a>Vise tilgjengeligheten av varer
Fra konteksten for en forretningsoppgave kan du få avansert informasjon om når og hvor en vare er tilgjengelig, for eksempel når du snakker med en kunde om en leveringsdato.

Du kan vise tilgjengeligheten for alle varer per lokasjon, og du kan vise tilgjengeligheten av hver vare etter hendelse, periode eller lokasjon. En hendelse er alle planlagte varetransaksjoner, for eksempel en følgeseddel eller mottak av inngående overføring.

> [!NOTE]  
>   Tilgjengelighetsvisninger etter lokasjon krever at du har beholdning på mer enn én lokasjon. Hvis du vil ha mer informasjon, kan du se [Definere lokasjoner](inventory-how-setup-locations.md).

Hvis du bruker lagerfunksjonalitet, varierer tilgjengelighet avhengig av tildelinger på hyllenivå når det oppstår lageraktiviteter som plukking og flytting, og når lagerreservasjonssystemet bruker begrensninger som må overholdes. En ganske komplisert algoritme bekrefter at alle betingelsene er oppfylt før tildeling av antall i plukk for utgående flyter. Hvis du vil ha mer informasjon, kan du se [Designdetaljer: Tilgjengelighet i lageret](design-details-availability-in-the-warehouse.md).

I [!INCLUDE[d365fin](includes/d365fin_md.md)] vises tilgjengelighetstallene vanligvis i to forskjellige felt, hver med en forskjellig definisjon:

* **Beholdning**-feltet, som kalles **Lager** enkelte steder, viser det faktiske antallet i dag i henhold til bokførte vareposter.
* Feltet **Beregnet disponibel beholdning** beregnes og viser antallet på lager pluss planlagte mottak minus bruttobehov. (I [!INCLUDE[d365fin](includes/d365fin_md.md)] inkluderer planlagte mottak antall bestillinger og inngående overføringsordrer. Bruttobehov inkluderer antall på salgsordrer og utgående overføringsordrer.)

> [!TIP]  
>   Beregnet disponibel saldo er spesielt relevant å vise på sidene **Varetilgjengelighet per periode** og **Varetilgjengelighet per hendelse** fordi de inneholder datodimensjonen.  

> [!NOTE]  
>   Fremgangsmåtene nedenfor viser hvordan du viser avansert informasjon om tilgjengelighet fra varelisten og varekortet. Du har også tilgang til informasjon fra salgsdokumentlinjer for varen på linjen. Hvis du vil ha mer informasjon, kan du se [Selge produkter](sales-how-sell-products.md).

## <a name="to-view-the-availability-of-an-item-according-to-when-it-will-be-received-or-shipped"></a>Slik viser du tilgjengeligheten for en vare i henhold til når den blir mottatt eller levert
Du viser tilgjengeligheten for en vare i henhold til planlagte varetransaksjoner på siden **Tilgjengelighet per hendelse**.

1. Velg ikonet ![Lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Varer**, og velg deretter den relaterte koblingen.
2. Åpne kortet for en vare som du vil vise varetilgjengelighet for.
3. Velg handlingen **Varetilgjengelighet per**, og velg deretter **Hendelse**-handlingen.

    Siden **Varetilgjengelighet per hendelse** viser hvordan lagerantall for varen vil utvikle seg over tid i henhold til planlagte hendelser for levering og mottak. Siden gir en konsentrert visning som viser én linje med akkumulert informasjon per tidsintervall hvor lagerantallet endres. Tidsintervaller som det ikke har oppstått noen hendelser i, vises ikke. Du kan utvide hver linje for å vise detaljer om hendelsen eller hendelsene som forårsaket det akkumulerte antallet på linjen.
4. Velg verdien i feltet **Beregnet disponibel beholdning** for å vise vareposter eller åpne dokumenter som utgjør verdien.

## <a name="to-view-the-availability-of-an-item-in-different-periods"></a>Slik viser du tilgjengeligheten for en vare i forskjellige perioder
Du viser tilgjengeligheten for en vare over tid for bestemte tidsperioder på siden **Varetilgjengelighet per periode**.

1. Velg ikonet ![lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Varer**, og velg deretter den relaterte koblingen.
2. Åpne kortet for en vare som du vil vise varetilgjengelighet for.
3. Velg handlingen **Varetilgjengelighet per**, og velg deretter **Periode**-handlingen.

    Siden **Varetilgjengelighet per periode** viser hvordan lagerantallet for varen vil utvikler seg over tid, vist for en periode som du velger, for eksempel dag, uke eller kvartal.
4. Velg verdien i feltet **Beregnet disponibel beholdning** for å vise vareposter eller åpne dokumenter som utgjør verdien.

## <a name="to-view-the-availability-of-an-item-at-the-locations-where-it-is-stored"></a>Slik viser du tilgjengeligheten for en vare på lokasjonene der den er lagret
Du viser tilgjengeligheten for en vare på de forskjellige lokasjonene der den er lagret, på siden **Varetilgjengelighet per lokasjon**.

1. Velg ikonet ![lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Varer**, og velg deretter den relaterte koblingen.
2. Åpne kortet for en vare som du vil vise varetilgjengelighet for.
3. Velg handlingen **Varetilgjengelighet per**, og velg deretter **Lokasjon**-handlingen.

    Siden **Varetilgjengelighet per lokasjon** viser hvordan lagerantallet for varen vil utvikle seg i fremtiden, vist for hver lokasjon der den er lagret.
4. Velg verdien i feltet **Disponibel beholdning** for å vise vareposter som utgjør verdien.
5. Velg verdien i feltet **Beregnet disponibel beholdning** for å vise vareposter eller åpne dokumenter som utgjør verdien.

## <a name="to-view-the-availability-of-all-items-by-the-location-where-they-are-stored"></a>Slik viser du tilgjengeligheten for alle varer på lokasjonen der de er lagret
Du kan vise tilgjengeligheten til alle varer på tvers av alle lokasjoner på siden **Varer per lokasjon**.

1. Velg ikonet ![lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Varer**, og velg deretter den relaterte koblingen.
2. Velg handlingen **Varer per lokasjon**.

    Siden **Varer per lokasjon** vises for alle varer hvor mange som er tilgjengelig på hver lokasjon.
3. Velg verdien i feltet **Disponibel beholdning** for å vise vareposter som utgjør verdien.

## <a name="to-view-the-availability-of-an-item-by-its-use-in-assembly-or-production-boms"></a>Vise tilgjengeligheten til en vare etter bruk i monterings- eller produksjonsstykklister
Hvis en vare er en del av monterings- eller produksjonsstykklister, enten som en overordnet vare eller som en komponent, kan du se hvor mange enheter av varen som er påkrevd på siden **Varetilgjengelighet per stykklistenivå**. Siden viser hvor mange enheter av en overordnet vare du kan lage basert på tilgjengeligheten av underordnede varer på underliggende linjer. Varene som har en monterings- eller produksjonsstykkliste, vises på siden som en linje som kan skjules. Du kan utvide denne linjen for å se de underliggende komponentene og delmonteringer på lavere nivå med sine egne stykklister.

Du kan for eksempel bruke siden for å bestemme om du kan oppfylle en ordre for en vare på en angitt dato. Du gjør dette ved å se på varens gjeldende tilgjengelighet og antallene som kan leveres av varens komponenter. Du kan også bruke siden til å identifisere flaskehalser i relaterte stykklister.

På hver linje på siden for både overordnede og underordnede varer angir følgende nøkkelfelt tilgjengelighetstall. Du kan bruke disse tallene for å bekrefte hvor mange enheter av en overordnet vare du kan levere hvis du starter den relaterte monteringsprosessen.

|Felt|Beskrivelse|
|------|-----------|
|**Kan lage overordnet**|Viser hvor mange enheter av en hvilken som helst delmontering i toppvaren du kan lage. Feltet angir hvor mange umiddelbare overordnede enheter du kan montere. Verdien er basert på tilgjengeligheten av varen på linjen.|
|**Kan lage toppvare**|Viser hvor mange enheter av toppvaren du kan lage. Feltet angir hvor mange enheter av stykklistevaren på øverste linje som du kan montere. Verdien er basert på tilgjengeligheten av varen på linjen.|

### <a name="to-view-the-availability-of-an-item-according-to-demand-for-its-parent"></a>Slik viser du tilgjengeligheten for en vare i henhold til behov for den overordnede
Siden **Varetilgjengelighet per stykklistenivå** viser informasjon for varen på kortet eller dokumentlinjen som siden er åpnet for. Varen vises alltid på øverste linje. Du kan vise informasjon for andre varer eller for alle varer ved å endre verdien i feltet **Varefilter**.

> [!NOTE]  
>   Som standard viser tilgjengelighetsfigurer på linjene den totale tilgjengeligheten for alle varene under den øverste varen. Disse tallene vises i feltet **Disponibelt antall**, og fokus er på toppvaren. Informasjon om hvor mange halvfabrikater du kan lage, kan imidlertid være skjevt. For å få en realistisk indikasjon om hvor mange av de viste delmonteringene du kan lage, må du fjerne merket for **Vis samlet tilgjengelighet** og deretter se tallet i feltet **Kan lage overordnet**.

Feltet **Flaskehals** angir hvilken vare i stykklistestrukturen som hindrer deg i å opprette et større antall enn antallet som vises i feltet **Kan lage toppvare**. Flaskehalsen kan for eksempel være en innkjøpt komponent med forventet mottaksdato som er for sen til å lage ekstra enheter av toppvaren etter datoen i feltet **Trengs innen dato**.

## <a name="to-view-the-availability-of-an-item-by-its-units-of-measure"></a>Slik viser du tilgjengeligheten for en vare ved hjelp av måleenheten
Siden **Varedisposisjon etter måleenhet** viser tilgjengeligheten av en vare i måleenheten som den er lagret i.

> [!NOTE]  
> Hvis du vil beholde denne informasjonen nøyaktig, må du konvertere måleenheten for varen. Hvis du for eksempel kjøper en vare i én enhet, for eksempel bokser, og du selger varer i en annen enhet, for eksempel stykker, må du bruke en varekladd til å konvertere enhetene, eller pakke ut varer. Du kan bruke en nedjusterings varekladdelinje til å redusere lageret i kjøpsenheten, for eksempel bokser og en oppjustering for å øke lager beholdningen i salgsenheten, for eksempel stykker. 

## <a name="assembly-availability-page"></a>Siden Montering – tilgjengelighet
Siden **Montering – tilgjengelighet** viser detaljerte tilgjengelighetsinformasjon for monteringsvaren. Det åpnes:

- Automatisk fra en ordrelinje i monter til ordre-scenarier når du angir et antall som forårsaker et problem med komponenttilgjengelighet.
- Automatisk fra et monteringsordrehode når du angir en verdi i Antall-feltet som forårsaker et problem med komponenttilgjengelighet.
- Manuelt når du åpner den fra en monteringsordre. I fanebladet Handlinger, under Funksjoner klikker du Vis tilgjengelighet.

Hurtigfanen **Detaljer** viser detaljert tilgjengelighetsinformasjon for monteringsvaren, inkludert hvor mange av antallet i monteringsordren som kan monteres innen forfallsdato basert på tilgjengeligheten av de nødvendige komponentene. Dette vises i feltet Kan montere på hurtigfanen Detaljer.

Verdien i **Kan montere**-feltet vises i rød skrift hvis antallet er lavere enn antallet i **Restantall**-feltet, noe som angir at det ikke er nok komponenter til å montere hele antallet.

Hurtigfanen **Linjer** viser detaljert informasjon om tilgjengelighet for monteringskomponentene.

Hvis én eller flere monteringskomponenter ikke er tilgjengelige, gjenspeiles dette i **Kan montere**-feltet på den aktuelle linjen som et lavere antall enn antallet i **Restantall**-feltet på hurtigfanen **Detaljer**.

## <a name="see-also"></a>Se også
[Håndtere lager](inventory-manage-inventory.md)  
[Monteringsstyring](assembly-assemble-items.md)  
[Arbeide med stykklister](inventory-how-work-BOMs.md)    
[Definer lokasjoner](inventory-how-setup-locations.md)  
[Overføre beholdning mellom lokasjoner](inventory-how-transfer-between-locations.md)  
[Selge produkter](sales-how-sell-products.md)      
[Arbeide med Business Central](ui-work-product.md)  
[Generelle forretningsfunksjoner](ui-across-business-areas.md)
