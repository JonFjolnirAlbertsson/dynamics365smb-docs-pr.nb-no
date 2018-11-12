---
title: "Bruke én mva-kode i kladder"
description: "I Norge kan du bruke funksjonen for én mva-kode i en kladd, slik at du kan bokføre mva ved hjelp av ett enkelt felt, **Mva-kode**."
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
ms.openlocfilehash: cf0aac90fbaaed02c9928f5a42d2db4926d7cd01
ms.contentlocale: nb-no
ms.lasthandoff: 09/28/2018

---
# <a name="use-one-vat-code-in-journals"></a>Bruke én mva-kode i kladder
I Norge kan du bruke funksjonen for én mva-kode i en kladd, slik at du kan bokføre mva ved hjelp av ett enkelt felt, **Mva-kode**. Når én mva-kode er konfigurert, er dette en rask måte å fylle ut mva-felt som brukes ofte.  

For å angi mva-koden for bestillinger og ordrer, må de tilsvarende mva-bokføringsgruppene for firma og mva-bokføringsgruppene for varer defineres.  

Mva-satsen beregnes fra kombinasjonen av mva-firmabokføringsgrupper, kjøperinformasjon og mva-varebokføringsgrupper.  

## <a name="to-create-a-vat-code"></a>Slik oppretter du en mva-kode:  

1.  Velg ikonet ![Søk etter side eller rapport](../../media/ui-search/search_small.png "Søk etter side eller rapport"), angi **VAT-koder**, og velg deretter den relaterte koblingen.  
2.  Velg handlingen **Ny**.  
3.  Angi opplysninger i feltet **Kode**, **Bokføringstype** og **Beskrivelse** for hver mva-kode.  
4.  Velg **OK**-knappen for å lukke vinduet **Mva-koder**.  

 Fremgangsmåten nedenfor beskriver mva-bokføringsoppsettet.  

## <a name="to-set-up-vat-posting"></a>Slik definerer du mva-bokføring:  

1.  Velg ikonet ![Søk etter side eller rapport](../../media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Mva-bokføringsoppsett**, og velg deretter den relaterte koblingen.  
2.  Velg handlingen **Ny**.  
3.  I kortet **Mva-bokføringsoppsett** må du fylle ut følgende felt:  

    - **Mva-bokføringsgruppe - firma**  
    - **Mva-bokføringsgruppe - vare**  
    - **Mva-type**  
    - **Mva-prosent**  
    - **Utgående mva-konto**  
    - **Inngående mva-konto**  

4.  I feltet **Mva-kode** velger du en kode fra listen.  

Nå når du bokfører et dokument i finanskladden og lukker det, brukes informasjonen som er angitt i **Mva-bokføringsoppsett**-kortet.  

For eksempel: mva-satsen som er bokført i kladden, defineres av oppsettet du har angitt i **Mva-bokføringsoppsett**-vinduet.  

> [!NOTE]  
>  Feltet **Mva-kode** og **Motkonto-mva. - kode** er lagt til i kladden. **Motkonto-mva. - kode** er mva-koden som brukes til å beregne motkontoen.  
>   
>  Det gjøres ingen endringer i bokføringen.  

## <a name="see-also"></a>Se også  
 [Norske mva-koder](norwegian-vat-codes.md)
