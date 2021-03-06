---
title: Bruke utvidelsen QuickBooks Payroll-filimport | Microsoft-dokumentasjon
description: Dette emnet beskriver hvordan du bruker utvidelsen til å importere lønn og lønnstransaksjoner fra QuickBooks.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, salary, wage
ms.date: 04/01/2020
ms.author: bholtorf
ms.openlocfilehash: 34fdb4fd63609e8a65f9bcc11a479a18ed76280f
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/01/2020
ms.locfileid: "3189702"
---
# <a name="the-quickbooks-payroll-file-import-extension"></a>Utvidelsen QuickBooks Payroll-filimport
Bruk QuickBooks Payroll-filimportutvidelsen til å importere lønnstransaksjoner fra QuickBooks til finanskonti i [!INCLUDE[d365fin](includes/d365fin_md.md)]. Dette er for eksempel nyttig når du går fra QuickBooks til [!INCLUDE[d365fin](includes/d365fin_md.md)], eller hvis outsourcer lønn, men også vil holde oversikt over den i [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="steps-to-import-payroll-data"></a>Trinn for å importere lønnsdata
Det første trinnet for deg, eller kanskje regnskapsføreren, er å bruke eksportfunksjonene i QuickBooks til å eksportere lønnsdata til en .IIF-fil. Det andre trinnet er å åpne siden **Finanskladder** i [!INCLUDE[d365fin](includes/d365fin_md.md)] og bruke **Importer lønnstransaksjoner**-handling til å importere filen. I løpet av importprosessen tilordner du finanskontiene fra QuickBooks til tilsvarende finanskonti i [!INCLUDE[d365fin](includes/d365fin_md.md)]. Det siste trinnet er å bokføre lønnstransaksjonene i [!INCLUDE[d365fin](includes/d365fin_md.md)] etter kontotilordningen. 

Hvis du vil ha mer informasjon, kan du se [Importere lønnstransaksjoner](finance-how-import-payroll-transactions.md).

## <a name="see-also"></a>Se også
[Tilpasse [!INCLUDE[d365fin](includes/d365fin_md.md)] ved hjelp av utvidelser](ui-extensions.md)    
[Finans](finance.md)    
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
