---
title: Importere og bokføre OCR-betalinger
description: Før du kan motta OCR-betalinger (optisk tegngjenkjenning), må du gjøre noen forberedelser.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/10/2020
ms.author: edupont
ms.openlocfilehash: ca7b03841eee93f829f965e510ce8e0b63b5f5cd
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/09/2020
ms.locfileid: "3779035"
---
# <a name="import-and-post-ocr-payments"></a>Importere og bokføre OCR-betalinger
Før du kan motta OCR-betalinger (optisk tegngjenkjenning), må du gjøre følgende forberedelser:  

- Opprette en innbetalingskladdemal for å balansere OCR-transaksjoner i henhold til bilagsnummeret i stedet for bilagstypen.  
- Lese inn og bokføre OCR-betalingsfiler i en innbetalingskladd.  

## <a name="to-import-ocr-payments"></a>Slik leser du inn OCR-betalinger  

1.  Velg ikonet ![Lyspære som åpner Fortell meg-funksjonen](../../media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Innbetalingskladder**, og velg deretter den relaterte koblingen.  
2.  Velg en kladd i feltet **Bunkenavn**.  

    > [!NOTE]  
    >  OCR-betalinger kan bare bokføres i en innbetalingskladd som ikke benytter en motkonto i feltet **Motkontonr.** på linjen Innbetalingskladd.  

3.  Velg handlingen **Importer betalinger**.  
4.  På siden **OCR-betaling - BBS** fyller du ut feltene som beskrevet i tabellen nedenfor.  

    |Felt|Beskrivelse|  
    |---------------------------------|---------------------------------------|  
    |**Filnavn**|Skriv inn hele banen til importfilen.|  

5.  Velg **OK** for å lese inn betalingsfilen i kladden.  

## <a name="to-post-ocr-payments"></a>Slik bokfører du OCR-betalinger  

1.  Velg ikonet ![Lyspære som åpner Fortell meg-funksjonen](../../media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Innbetalingskladder**, og velg deretter den relaterte koblingen.  
2.  Velg handlingen **Bokfør**.  

OCR-betalingsfilene bokføres i innbetalingskladden.  

## <a name="see-also"></a>Se også  
 [Elektroniske banktjenester i Norge](electronic-banking-in-norway.md)   
 [Opprette KID-numre på salgsdokumenter](how-to-set-up-kid-numbers-on-sales-documents.md)   
 [Opprette OCR-betalinger](how-to-set-up-ocr-payments.md)   
 [Arbeide med finanskladder](../../ui-work-general-journals.md)   
 [Skrive ut rapporten OCR-kladd - test](how-to-print-the-ocr-journal-test-report.md)
