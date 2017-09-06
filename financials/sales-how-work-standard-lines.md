---
title: "Definere og bruke standardlinjer for gjentakende salg og kjøp | Microsoft-dokumentasjon"
description: "Du kan definere salgslinjer og kjøpslinjer du ofte lager, og deretter sette dem inn i salgs- og kjøpsdokumenter for å fylle ut linjene raskt med standardinformasjon."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade, sell, replenishment
ms.date: 07/02/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 85d15de13739e944ff8817b402b37ae1c7e1b144
ms.openlocfilehash: 980a0646317c2b5c02c0eadcde9ba984c11580c4
ms.contentlocale: nb-no
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-create-recurring-sales-and-purchase-lines"></a>Opprette gjentakende salgs- og kjøpslinjer
Hvis du ofte må opprette salgs- og kjøpslinjer med lignende informasjon, kan du definere standardlinjer du deretter kan sette inn på gjentakende salgs- og kjøpsdokumenter, for eksempel for gjentakende etterfyllingsordrer.  

Fremgangsmåten nedenfor viser hvordan du arbeider med standardlinjer. Det fungerer på en lignende måte som for standard kjøpslinjer.  

## <a name="to-set-up-standard-sales-lines"></a>Definere standard salgslinjer  
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Ikonet Søk etter side eller rapport"), angi **Standard salgskoder**, og velg deretter den relaterte koblingen.  
2. I vinduet **Standard salgslinjer** velger du handlingen **Ny**.  
3. Fyll ut feltene i hurtigfanen **Generelt** etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. I hurtigfanen **Linjer** angir du informasjon i feltene for å klargjøre salgslinjer som gjenspeiler standardlinjene du forventer å bruke som gjentakende linjer i salgsdokumenter.  

## <a name="to-insert-standard-sales-lines-on-a-sales-invoice"></a>Sette inn standard salgslinjer på en salgsfaktura
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Ikonet Søk etter side eller rapport"), angi **Fakturaer**, og velg deretter den relaterte koblingen.
2. Åpne salgsfakturaen du vil sette inn én eller flere standard salgslinjer på.
3. Velg handlingen **Hent gjentakende salgslinjer**.
4. I vinduet **Gjentakende salgslinjer** velger du oppslagsknappen i **Kode**-feltet, og deretter velger du et sett med standard salgslinjer.
5. Velg **OK** for å sette inn de standard salgslinjene på fakturaen, der du kan bruke informasjonen på nytt som den er eller redigere den.

## <a name="to-create-multiple-sales-invoices-based-on-standard-sales-lines"></a>Opprette flere salgsfakturaer basert på standard salgslinjer
Du kan bruke kjørselen **Opprett gjentak. salgsfakt.** til å opprette salgsfakturaer i henhold til standard salgslinjer som er tilordnet til kundene, og med bokføringsdatoer innenfor datoene for gjelder fra og til, som du angir for standard salgskode.

I vinduet **Gjentakende salgslinjer** kan du også angi en Direct Debit-betalingsmåte og en Direct Debit-belastningsfullmakt. Salgsfakturaene som er opprettet med kjørselen **Opprett gjentak. salgsfakt.**, inneholder deretter informasjon som kreves for å kreve inn betaling for salgsfakturaer med SEPA direct debit. Hvis du vil ha mer informasjon, kan du se Innkreve betalinger med SEPA Direct Debit.

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Ikonet Søk etter side eller rapport"), angi **Opprett gjentakende salgsfakturaer**, og velg deretter den relaterte koblingen.
2. I vinduet **Opprett gjentak. salgsfakt.** fyller du ut feltene etter behov.
3. I vinduet **Kode** angir du koden for standard salgslinjer som er tilordnet en kunde du vil opprette salgsfakturaer for.
4. Velg **OK**.

Salgsfakturaer blir opprettet for kunder med angitt standard kundesalgskode og eventuell angitt avtalegiroinformasjon, for bokføring på den angitte datoen.

## <a name="see-also"></a>Se også  
[Salg](sales-manage-sales.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
