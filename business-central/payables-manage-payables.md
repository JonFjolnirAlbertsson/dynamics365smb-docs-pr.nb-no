---
title: "Oversikt over oppgaver for å behandle leverandørgjeld | Microsoft-dokumentasjon"
description: "Gir en oversikt over oppgavene for å behandle leverandørgjeld, for eksempel betale kreditorer eller utligne utgående betalinger mot poster for å lukke fakturaer eller kreditnotaer."
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: vendor payment, creditor, debt, balance due, AP
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 5482579cb453b119be1b6eb5c24d5adc9441ea8b
ms.contentlocale: nb-no
ms.lasthandoff: 03/22/2018

---
# <a name="managing-payables"></a>Administrere skyldige beløp

En viktig del av håndtering av leverandørgjeld er å betale dine leverandører eller refundere de ansatte for utgifter. Du kan bruke funksjoner til å legge til betalingslinjer for forfalte kjøpsfakturaer i vinduet **Utbetalingskladd**. Du kan sende transaksjoner til banken din ved å eksportere flere betalingskladdelinjer til en fil og deretter laste opp filen til banken. Du kan også betale med sjekk, inkludert å overføre sjekker som elektroniske betalinger.

En annen vanlig oppgave er å utligne utgående betalinger mot deres relaterte leverandør- eller ansattposter for å kunne lukke de beslektede kjøpsfakturaene, kjøpskreditnotaene eller ansattkontoene som betalt. Du kan gjøre dette i vinduet **Betalingsavstemmingskladd** ved å importere en bankkontoutdragsfil for hurtig å registrere betalinger. Betaling brukes til å åpne leverandør-, kunde- eller ansattpostoppføringer ved å sammenligne betalingstekst for oppføringsinformasjon. Det finnes ulike måter å se gjennom og endre treff før du bokfører kladden. Du kan velge å lukke alle åpne bankposter relatert til de utlignede postene når du bokfører kladden. Bankkontoen avstemmes automatisk når alle betalinger er utlignet.

Du kan også bruke utgående betalinger manuelt i vinduet **Betalingskladd** eller fra de relaterte leverandør- eller ansattpostene.

Tabellen nedenfor beskriver en sekvens av oppgaver i leverandørgjeld, og har koblinger til emnene som beskriver dem.

| Hvis du vil | Se |
| --- | --- |
| Generer forfalte leverandørbetalinger eller ansattrefusjoner, forbered sjekkutbetalinger og eksporter betalinger til en bankfil ved bokføring. |[Utføre betalinger](payables-make-payments.md) |
| Utligne leverandørbetalinger automatisk på ubetalte kjøpsfakturaer ved å importere en bankkontoutdragsfil. |[Utligne betalinger automatisk og avstemme bankkonti](receivables-apply-payments-auto-reconcile-bank-accounts.md) |
| Utligne leverandørbetalinger på ubetalte fakturaer manuelt. |[Avstemme leverandørbetalinger manuelt](payables-how-apply-purchase-transactions-manually.md) |
|Sikre riktig lagerverdisetting ved å tilordne ekstra varekost, for eksempel frakt, fysisk håndtering, forsikring og transport, som du pådrar deg ved innkjøp.|[Bruke varegebyr til å gjøre rede for ekstra handelskostnader](payables-how-assign-item-charges.md)|

## <a name="see-also"></a>Se også
[Innkjøp](purchasing-manage-purchasing.md)  
[Håndtere fordringer](receivables-manage-receivables.md)  
[Bruke varegebyr til å gjøre rede for ekstra handelskostnader](payables-how-assign-item-charges.md)  
[Generelle forretningsfunksjoner](ui-across-business-areas.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
