---
title: Utveksle data | Microsoft-dokumentasjon
description: "Du kan utveksle data mellom Dynamics 365 og eksterne filer eller strømmer i forbindelse med vanlige forretningsoppgaver, for eksempel sending og mottak av elektroniske dokumenter og import og eksport av bankfiler."
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 11/17/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: aa56764b5f3210229ad21eae6891fb201462209c
ms.openlocfilehash: 41f42162499401693f30e37a736c4fe0afe24822
ms.contentlocale: nb-no
ms.lasthandoff: 12/14/2017

---
# <a name="exchanging-data"></a>Utveksle data
Du kan utveksle data mellom [!INCLUDE[d365fin](includes/d365fin_md.md)] og eksterne filer eller strømmer i forbindelse med vanlige forretningsoppgaver, for eksempel sending og mottak av elektroniske dokumenter og import og eksport av bankfiler.  

Før du kan sende og motta elektroniske dokumenter eller importere og eksportere bankfiler, må du definere rammeverket for datautveksling til å behandle datafiler eller -strømmer som er involvert. Du må i tillegg konfigurere relaterte områder. Disse omfatter hoveddata for kunder du sender elektroniske fakturaer til, og konverteringstjenesten for bankdata i tilfelle du distribuerer bankfilkonverteringer til en ekstern tjenesteleverandør. Hvis du vil ha mer informasjon, kan du se [Definere datautveksling](across-set-up-data-exchange.md).  

 Tabellen nedenfor beskriver en sekvens av oppgaver, og har koblinger til emnene som beskriver dem.  

|**Hvis du vil**|**Se**|  
|------------|-------------|  
|Konvertere salgsdokumentposter i [!INCLUDE[d365fin](includes/d365fin_md.md)] til et standardisert format og sende dem som elektroniske dokumenter som kundene kan motta til systemet.|[Sende elektroniske dokumenter](sales-how-to-send-electronic-documents.md)|  
|Send PDF-eller bildefiler til en leverandør av OCR-tjenester, og få dem tilbake som elektroniske dokumenter som kan konverteres til dokumentposter i [!INCLUDE[d365fin](includes/d365fin_md.md)].|[Bruke OCR til å konvertere PDF- og bildefiler til elektroniske dokumenter](across-how-use-ocr-pdf-images-files.md)|  
|Motta elektroniske dokumenter, enten fra OCR-tjenesten eller dokumentutvekslingstjenesten, i et standardisert format som du konverterer til de relevante dokumentpostene i [!INCLUDE[d365fin](includes/d365fin_md.md)].|[Motta og konvertere elektroniske dokumenter](purchasing-how-to-receive-and-convert-electronic-documents.md)|  
|Importer en bankkontoutdragsfil i vinduet **Betalingsavstemmingskladd** som det første trinnet i avstemming av betalinger eller i vinduet **Bankkontoavstemming** som det første trinnet i avstemming av bankkontoer.|[Konfigurere bankfeedservicen Envestnet Yodlee](bank-how-setup-bank-statement-service.md)|  
|Eksporter betalinger fra vinduet **Betalingskladd** til en bankfil du laster opp til nettbankkontoen for å få den behandlet.|[Fremgangsmåte: Eksportere betalinger til en bankfil](payables-how-export-payments-bank-file.md)|
|Utfør elektroniske betalinger i henhold til standarden for EU SEPA-kredittoverføring.|[Betale med tjenesten for bankdatakonvertering eller SEPA-kredittoverføring](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md)|  
|Instruere banken om å overføre betalingsbeløpet fra kundenes bankkonti til firmaets konto i henhold til oppsettet av SEPA direct debit.|[Opprette poster for SEPA Direct Debit-oppkreving og eksportere til en bankfil](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)|  
|Bruk en tjenesteleverandør for valutakurser for å oppdatere **Valutaer**-vinduet.|[Oppdatere valutakurser](finance-how-update-currencies.md)|  
|Vis hvilke filelementer som er tilordnet til felt i [!INCLUDE[d365fin](includes/d365fin_md.md)], når du importerer SEPA CAMT-bankkontoutdragsfiler.|[Felttilordning ved import av SEPA CAMT-filer](across-field-mapping-when-importing-sepa-camt-files.md)|  
|Vis hvilke felt i [!INCLUDE[d365fin](includes/d365fin_md.md)] som er tilordnet til filelementene, når du eksporterer betalingsfiler ved hjelp av konverteringstjenesten for bankdata.|[Felttilordning ved eksport av betalingsfiler ved hjelp av konverteringstjeneste for bankdata](across-field-mapping-when-exporting-payment-files-using-bank-data-conversion-service.md)|  

## <a name="see-also"></a>Se også  
[Definere datautveksling](across-set-up-data-exchange.md)  
[Utveksle data elektronisk](across-data-exchange.md)  
[Fakturere salg](sales-how-invoice-sales.md)   
[Registrere kjøp](purchasing-how-record-purchases.md)  
[Inngående dokumenter](across-income-documents.md)  
[Generelle forretningsfunksjoner](ui-across-business-areas.md)  
