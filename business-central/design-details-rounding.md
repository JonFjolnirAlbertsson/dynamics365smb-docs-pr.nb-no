---
title: "Designdetaljer – Avrunding | Microsoft-dokumentasjon"
description: "Avrundingsoverskudd kan oppstå når du verdsetter kostnaden for en lagerreduksjon som måles i et annet antall enn den tilsvarende lagerøkningen. Avrundingsoverskudd beregnes for alle lagermetoder når du starter kjørselen **Juster kostverdi - vareposter**."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 231481ed9b8de81fb565e86e9b89c96434545cbf
ms.contentlocale: nb-no
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-rounding"></a>Designdetaljer: Avrunding
Avrundingsoverskudd kan oppstå når du verdsetter kostnaden for en lagerreduksjon som måles i et annet antall enn den tilsvarende lagerøkningen. Avrundingsoverskudd beregnes for alle lagermetoder når du starter kjørselen **Juster kostverdi - vareposter**.  

 Når du bruker lagermetoden Gjennomsnitt, beregnes og registreres avrundingsoverskuddet på en kumulativ basis (post etter post).  

 Når du bruker en annen lagermetode enn Gjennomsnitt, beregnes avrundingsoverskuddet når lagerøkningen er fullstendig utlignet, det vil si når restantallet for lagerøkningen er lik null. En separat oppføring opprettes deretter for avrundingsoverskudd, og bokføringsdatoen i avrundingsposten er bokføringsdatoen til den siste fakturerte verdiposten for lagerøkningen.  

## <a name="example"></a>Eksempel  
 Følgende eksempel illustrerer hvordan ulike avrundingsoverskudd håndteres henholdsvis for lagermetoden Gjennomsnitt og lagermetoden Ikke-gjennomsnitt. I begge tilfeller er kjørselen **Juster kostverdi - vareposter** kjørt.  

 Tabellen nedenfor viser varepostene som eksemplet er basert på.  

|Bokføringsdato|Antall|Løpenr.|  
|------------------|--------------|---------------|  
|01.01.20|3|1|  
|01.02.20|-1|2|  
|01.03.20|-1|3|  
|01.04.20|-1|4|  

 Avrundingsoverskuddet (1/300) beregnes med første reduksjon (løpenummer 2), og det overføres til postnummer 3 for en vare som bruker kostmetoden Gjennomsnitt. Løpenummeret 3 har derfor verdier –3.34.  

 Tabellen nedenfor viser de resulterende verdipostene.  

|Bokføringsdato|Antall|Kostbeløp (faktisk)|Varepostnr.|Løpenr.|  
|------------------|--------------|----------------------------|---------------------------|---------------|  
|01.01.20|3|10|1|1|  
|01.02.20|-1|-3,33|2|2|  
|01.03.20|-1|-3,34|3|3|  
|01.04.20|-1|-3,33|4|4|  

 Avrundingsoverskuddet (0,01) beregnes når restantallet for lagerøkningen er null for en vare som bruker en annen kostmetode enn Gjennomsnitt. Avrundingsoverskuddet har en egen post (nummer 5).  

 Tabellen nedenfor viser de resulterende verdipostene.  

|Bokføringsdato|Antall|Kostbeløp (faktisk)|Varepostnr.|Løpenr.|  
|------------------|--------------|----------------------------|---------------------------|---------------|  
|01.01.20|3|10|1|1|  
|01.02.20|-1|-3,33|2|2|  
|01.03.20|-1|-3,33|3|3|  
|01.04.20|-1|-3,33|4|4|  
|01.01.20|0|-0,01|1|5|  

## <a name="see-also"></a>Se også  
 [Designdetaljer: Kostberegning for beholdning](design-details-inventory-costing.md)   
 [Designdetaljer: Kostjustering](design-details-cost-adjustment.md)   
 [Designdetaljer: Kostmetoder](design-details-costing-methods.md) [Administrere lagerkostnader](finance-manage-inventory-costs.md)  
 [Finans](finance.md)  
 [Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
