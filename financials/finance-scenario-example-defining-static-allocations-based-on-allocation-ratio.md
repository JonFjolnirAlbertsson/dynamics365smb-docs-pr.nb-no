---
title: "Definere statiske fordelinger basert på fordelingsgrad | Microsoft-dokumentasjon"
description: "Statisk fordelingsmetode er basert på en bestemt verdi, for eksempel kvadratmeteren som brukes, eller et fastsatt fordelingsforhold, for eksempel 5:2:4."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: b48d7f73b640b98d0cdab6e2e7e7486a3bdb39db
ms.contentlocale: nb-no
ms.lasthandoff: 09/22/2017

---
# <a name="scenario-example-defining-static-allocations-based-on-allocation-ratio"></a>Eksempelscenario: Definere statiske fordelinger basert på fordelingsgrad
Statisk fordelingsmetode er basert på en bestemt verdi, for eksempel kvadratmeteren som brukes, eller et fastsatt fordelingsforhold, for eksempel 5:2:4.  

Dette emnet beskriver hvordan du definerer tre nye kostobjekter for fordelingsmål for PROD-kostsenteret for fordelingskilden ved hjelp av det fastsatte fordelingsforholdet på 5:2:4. De tre målkostobjektene er TILBEHØR, MALING og ARMATUR.  

> [!NOTE]  
>  I eksempelet brukes demodataene i [!INCLUDE[d365fin](includes/d365fin_md.md)].  

## <a name="to-define-the-allocation-source-prod-cost-center-on-the-general-fasttab"></a>Slik definerer du PROD-kostsenteret for fordelingskilden i hurtigfanen Generelt:  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Ikonet Søk etter side eller rapport"), angi **Kostfordeling**, og velg deretter den relaterte koblingen.  
2.  I vinduet **Kostfordeling** velger du **Ny**.  
3.  Trykk på Enter eller angi en ID i **ID**-feltet.  
4.  I feltet **Grad** angir du **1**.  
5.  I feltene **Gyldig fra** og **Gyldig til** angir du datoene du vil bruke.  
6.  Angi **PROD** i feltet **Kostsenterkode**-feltet.  
7.  I feltet **Krediter til kosttype** skriver du inn kosttypen **9903**.  

## <a name="to-define-the-allocation-target-cost-objects-on-the-lines-fasttab"></a>Slik definerer du kostobjekter for fordelingsmålene i hurtigfanen Linjer:  

1.  På den første fakturalinjen i feltet **Målkosttype** angir du **9903**.  
2.  På den første fakturalinjen i feltet **Målkostobjekt** angir du **TILBEHØR**.  
3.  På den første linjen, i feltet **Fordelingsmåltype**, velger du **All kost** for å definere hvordan alle påløpte kostnader fordeles.  
4.  På den første linjen i **Grunnlag**-feltet velger du **Statisk** for å bruke den statiske fordelingsmetoden.  
5.  På den første linjen, i feltet **Del**, angir du fordelingsforholdet **5**.  
6.  På den andre fakturalinjen i feltet **Målkosttype** angir du **9903**.  
7.  På den andre fakturalinjen i feltet **Målkostobjekt** angir du **MALING**.  
8.  På den andre linjen, i feltet **Fordelingsmåltype**, velger du **All kost** for å definere hvordan alle påløpte kostnader fordeles.  
9. På den andre linjen i **Grunnlag**-feltet velger du **Statisk** for å bruke den statiske fordelingsmetoden.  
10. På den andre linjen, i feltet **Del**, angir du fordelingsforholdet **2**.  
11. På den tredje fakturalinjen i feltet **Målkosttype** angir du **9903**.  
12. På den tredje fakturalinjen i feltet **Målkostobjekt** angir du **ARMATUR**.  
13. På den tredje linjen, i feltet **Fordelingsmåltype**, velger du **All kost** for å definere hvordan alle påløpte kostnader fordeles.  
14. På den tredje linjen i **Grunnlag**-feltet velger du **Statisk** for å bruke den statiske fordelingsmetoden.  
15. På den tredje linjen, i feltet **Del**, angir du fordelingsforholdet **4**.  

> [!IMPORTANT]  
>  [!INCLUDE[d365fin](includes/d365fin_md.md)] beregner automatisk **Prosent**-feltet ved å bruke en prosentsats som er avhengige av alle de tre fordelingsforholdene som er angitt i **Del**-feltet for alle de tre linjene.  

## <a name="see-also"></a>Se også  
[Definere fordelingskilde og -mål](finance-how-to-set-up-allocation-source-and-targets.md)   
[Definere og fordele kostnader](finance-define-and-allocate-costs.md)   
[Eksempelscenario: Definere dynamiske fordelinger basert på solgte varer](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md)   
[Definere og fordele kostnader](finance-define-and-allocate-costs.md)
