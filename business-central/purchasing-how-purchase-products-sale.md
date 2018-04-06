---
title: "Kjøpe varer som er på salg ved å opprette kjøpsfakturaer | Microsoft dokumenter"
description: "Du kan opprette en faktura for en leverandør fra en salgsfaktura for å kjøpe produkter."
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supply planning, sales demand, replenish
ms.date: 01/25/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 82447508b12c4f158cb3fc5e257576e14ef284b4
ms.contentlocale: nb-no
ms.lasthandoff: 03/22/2018

---
# <a name="purchase-items-for-a-sale"></a>Kjøpe varer for salg
I ordrer og på salgsfakturaer kan du bruke funksjoner til raskt å opprette kjøpsdokumenter for manglende vareantall som kreves av salget. Du kan bruke to ulike funksjoner, avhengig av dokumenttypen.
|Funksjon|Beskrivelse|
|--------|-----------|
|**Opprett bestillinger**|I en ordre oppretter denne funksjonen en bestilling for hver enkelt leverandør av varene i ordren. Du kan redigere kjøpsantallet før du oppretter bestillingene. Det er bare utilgjengelige salgsantall som foreslås.
|**Opprett kjøpsfaktura**|I en ordre og på en salgsfaktura oppretter denne funksjonen en kjøpsfaktura for en valgt leverandør for alle linjene eller valgte linjer i salgsdokumentet. Hele salgsantallet foreslås.|

## <a name="to-create-one-or-more-purchase-orders-from-a-sales-order"></a>Opprette én eller flere bestillinger fra en ordre
Hvis du vil opprette en bestilling for hvert utilgjengelige vareantall i ordren, bruker du funksjonen **Opprett bestillinger**.

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ordrer**, og velg deretter den relaterte koblingen.
2. Åpne en ordre du vil kjøpe varer for.
3. Velg handlingen **Opprett bestillinger**.

    Vinduet **Opprett bestillinger** åpnes med en linje for hver unike vare i ordren. Som standard vises linjer for både helt tilgjengelige salgsantall og utilgjengelige salgsantall (nedtonet). Du kan velge handlingen **Vis utilgjengelige** hvis du bare vil se linjer for utilgjengelige salgsantall.

    Feltet **Antall å kjøpe** inneholder som standard det utilgjengelige salgsantallet.
4. Hvis du vil kjøpe et annet antall enn det utilgjengelige salgsantallet, endrer du verdien i feltet **Antall å kjøpe**.

    > [!NOTE]  
    >   Du kan også endre feltet **Antall å kjøpe** på nedtonede linjer selv om de representerer helt tilgjengelige salgsantall.
5. Velg **OK**.

    En bestilling opprettes for hver enkelt leverandør av varene i ordren, inkludert eventuelle antallsendringer du har foretatt i vinduet **Opprett bestillinger**.
7. Fortsett behandlingen av for eksempel bestillingen eller bestillingene ved å redigere eller legge til bestillingslinjer. Hvis du vil ha mer informasjon, kan du se [Registrere kjøp](purchasing-how-record-purchases.md).


## <a name="to-create-a-purchase-invoice-from-a-sales-order-or-sales-invoice"></a>Opprette en kjøpsfaktura fra en ordre eller salgsfaktura
Hvis du vil opprette én kjøpsfaktura for én eller flere linjer i et salgsdokument ved først å velge leverandøren du vil kjøpe fra, bruker du funksjonen **Opprett kjøpsfaktura**.

> [!NOTE]  
>   Denne funksjonen oppretter en kjøpsfaktura for det nøyaktige vareantallet i det valgte salgsdokumentet. Hvis du vil endre kjøpsantallet, må du redigere kjøpsfakturaen etter at den er opprettet.  

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ordrer**, og velg deretter den relaterte koblingen.
2. Åpne en salgsfaktura du vil kjøpe varer for.
3. Velg én eller flere salgsfakturalinjer du vil bruke på kjøpsfakturaen. Hvis du vil bruke alle salgsfakturalinjene, merker du dem alle eller ingen av dem.
4. Velg handlingen **Opprett kjøpsfaktura**.
5. Velg **Alle linjer** eller **Valgte linjer**, og velg deretter **OK**-knappen.  
6. I listen over leverandører som vises, velger du leverandøren du vil kjøpe alle varene fra, og deretter velger du **OK**.

    Det opprettes en kjøpsfaktura som inneholder én, flere eller alle linjene på salgsfakturaen.
7. Fortsette med å behandle kjøpsfakturaen, for eksempel ved å redigere eller legge til kjøpsfakturalinjene. Hvis du vil ha mer informasjon, kan du se [Registrere kjøp](purchasing-how-record-purchases.md).

## <a name="see-also"></a>Se også
[Innkjøp](purchasing-manage-purchasing.md)  
[Registrere kjøp](purchasing-how-record-purchases.md)  
[Fakturere salg](sales-how-invoice-sales.md)  
[Registrere nye leverandører](purchasing-how-register-new-vendors.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
