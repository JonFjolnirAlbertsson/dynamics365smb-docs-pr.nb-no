---
title: Bruke vareserier i produksjon | Microsoft-dokumentasjon
description: "Hovedoppgaven med å tilpasse en hovedkalender for selskapet, eller selskapets forretningspartner, er å angi eventuelle endringer i statusen for arbeids- eller fridager."
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
ms.openlocfilehash: 4e89cee3fb8b3c079cebf0665a1e068ac1f46fae
ms.contentlocale: nb-no
ms.lasthandoff: 09/28/2018

---
# <a name="work-with-production-families"></a>Arbeide med produksjonsfamilier
En produksjonsfamilie er en gruppe individuelle varer der forbindelsen er basert på likheten i produksjonsprosessen. Ved hjelp av produksjonsfamilier kan noen varer produseres to eller flere ganger i én produksjon, noe som optimaliserer materialforbruket.

I **Antall**-feltet i **Familie**-vinduet angir du antallet som skal produseres når hele familien er produsert én gang.

## <a name="example"></a>Eksempel
I utstansingsprosesser kan fire enheter av samme vare produseres fra ett ark, samtidig med 10 enheter av en annen, forskjellig vare. Utstansingsmaskinen utstanser alle de 14 enhetene i én operasjon.

Når du definerer produksjonsfamilier, reduseres vrakantallet, fordi det som vanligvis ville blitt overflødig vrak ved produksjon av store enheter, i stedet brukes til å produsere små varer.

## <a name="to-set-up-a-production-family"></a>Slik konfigurerer du produksjonsfamilier
1. Velg ikonet ![lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Familier**, og velg deretter den relaterte koblingen.
2. Fyll ut feltene etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-produce-based-on-a-production-familily"></a>Produsere basert på en produksjonsfamilie
1. Velg ikonet ![lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Fast planlagte prod.ordrer**, og velg deretter den relaterte koblingen.
2. Opprett en ny produksjonsordre. Hvis du vil ha mer informasjon, kan du se [Opprette produksjonsordrer](production-how-to-create-production-orders.md).
3. Velg **Familie** i **Kildetype**-feltet.  
4. Velg den aktuelle produksjonsfamilien i **Kildenr.**-feltet.

## <a name="see-also"></a>Se også
[Opprette produksjonsstykklister](production-how-to-create-production-boms.md)  
[Definere produksjon](production-configure-production-processes.md)  
[Produksjon](production-manage-manufacturing.md)    
[Planlegging](production-planning.md)   
[Lager](inventory-manage-inventory.md)  
[Innkjøp](purchasing-manage-purchasing.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
