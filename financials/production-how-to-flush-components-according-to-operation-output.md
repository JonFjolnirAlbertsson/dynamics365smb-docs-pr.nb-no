---
title: Lagertrekke komponenter i henhold til operasjonsavgang | Microsoft-dokumentasjon
description: "For varer som er definert med trekkmetoden Bakover, er standard virkemåte å beregne og bokføre komponentforbruk når du endrer statusen for en frigitt produksjonsordre til **Ferdig**. Hvis du vil ha mer informasjon, kan du se Trekkmetode."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: b58e897768848b50232b360f3822846d6dd316df
ms.contentlocale: nb-no
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-flush-components-according-to-operation-output"></a>Lagertrekke komponenter i henhold til operasjonsavgang
For varer som er definert med trekkmetoden Bakover, er standard virkemåte å beregne og bokføre komponentforbruk når du endrer statusen for en frigitt produksjonsordre til **Ferdig**.  

Hvis du også definerer rutekoblingskoder, skjer beregning og bokføring når hver operasjon er fullført, og antallet som faktisk ble forbrukt i operasjonen, bokføres. Hvis du vil ha mer informasjon, kan du se [Opprette ruter](production-how-to-create-routings.md).  

Hvis en produksjonsordre om å produsere 800 meter for eksempel krever 8 kg av en komponent, bokføres 2 kg automatisk som forbruk når du bokfører 200 meter som avgang.  

Denne funksjonaliteten er nyttig av følgende årsaker:  

-   **Lagerverdisetting** -Verdipostene for avgang og forbruk opprettes parallelt ettersom produksjonsordren går fremover. Uten rutekoblingskoder vil lagerverdien øke etter hvert som avgangen bokføres og deretter reduseres på et senere tidspunkt når verdien for komponentforbruk bokføres sammen med den ferdige produksjonsordren.  
-   **Lagertilgjengelighet** - Med gradvis forbruksbokføring er komponentvarenes tilgjengelighet mer oppdatert, noe som er viktig for å opprettholde den interne balansen mellom behov og forsyning. Uten rutekoblingskoder kan andre behov for komponenten tro at den er tilgjengelig så lenge den venter på en forsinket forbruksbokføring.  
-   **Til rett tid**  – Med evnen til å tilpasse produktene til kundens ønsker kan du minimere svinn ved å kontrollere at arbeids- og systemendringer bare forekommer når det er nødvendig.  

Følgende fremgangsmåte viser hvordan du kombinerer lagertrekk bakover og rutekoblingskoder slik at lagertrekksantallet for hver operasjon er proporsjonalt med den faktiske avgangen for den fullførte operasjonen.  

## <a name="to-flush-components-according-to-operation-output"></a>Slik utfører du lagertrekk i henhold til operasjonsavgang:  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Ikonet Søk etter side eller rapport"), angi **Varer**, og velg deretter den relaterte koblingen.  
2.  Velg handlingen **Rediger**.  
3.  På hurtigfanen **Etterfylling**, i **Trekkmetode**- feltet, velger du **Fremover**.  

    > [!NOTE]  
    >  Velg **Plukk + Fremover** hvis komponenten er brukt på en lokasjon som er konfigurert for lagerstyring.  

4.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Ikonet Søk etter side eller rapport"), angi **Ruter**, og velg deretter den relaterte koblingen.  
5.  Definer rutekoblingskoder for hver operasjon som forbruker komponenten. Hvis du vil ha mer informasjon, kan du se [Opprette ruter](production-how-to-create-routings.md).  
6.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Ikonet Søk etter side eller rapport"), angi **Produksjonsstykkliste**, og velg deretter den relaterte koblingen.  
7.  Definer rutekoblingskoder fra hver forekomst av komponenten til operasjonen der den er brukt.

    > [!IMPORTANT]  
    >  Komponenten må ha en rutekobling til den siste operasjonen i ruten.  

## <a name="see-also"></a>Se også  
[Opprette produksjonsstykklister](production-how-to-create-production-boms.md)  
[Definere produksjon](production-configure-production-processes.md)  
[Produksjon](production-manage-manufacturing.md)    
[Planlegging](production-planning.md)   
[Lager](inventory-manage-inventory.md)  
[Innkjøp](purchasing-manage-purchasing.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
