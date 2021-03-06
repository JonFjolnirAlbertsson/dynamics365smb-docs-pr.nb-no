---
title: Innføring i Business Central og Power BI | Microsoft Docs
description: Få innsikt, forretningsintelligens og KPI-er fra Business Central-dataene på en enkel måte med Business Central-apper for Power BI.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.reviewer: edupont
ms.date: 04/01/2020
ms.author: jswymer
ms.openlocfilehash: a1e2e8ceee41c2c6ed517d000fc7c3a4a6aa274c
ms.sourcegitcommit: aeaa0dc64e54432a70c4b0e1faf325cd17d01389
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/17/2020
ms.locfileid: "3697675"
---
# <a name="prodshort-and-power-bi"></a>[!INCLUDE[prodshort](includes/prodshort.md)] og Power BI

Det er enkelt å få innsikt i [!INCLUDE[prodshort](includes/prodshort.md)]-dataene med [Power BI](https://powerbi.microsoft.com) – et datavisualiseringssystem fra Microsoft. Power BI henter [!INCLUDE[prodshort](includes/prodshort.md)]-data, slik at du kan bygge instrumentbord og rapporter basert på disse dataene. Power BI gir deg et fleksibelt alternativ til rapporter som er bygget i [!INCLUDE[prodshort](includes/prodshort.md)], slik at du kan drille ned og tilpasse visualiseringen og til og med slå sammen data fra ulike selskaper i [!INCLUDE[prodshort](includes/prodshort.md)]. Noen Power BI-rapporter kan også bygges inn i Business Central og vises uten å forlate systemet. Mer komplekse instrumentbord er bedre å oppleve fra Power BI-nettstedet.

![Power BI og Business Central](media/power-bi-intro.png)


## <a name="what-you-can-do-with-power-bi-and-prodshort"></a>Det du kan gjøre med Power BI og [!INCLUDE[prodshort](includes/prodshort.md)]

Det finnes ulike funksjoner for å arbeide med [!INCLUDE[prodshort](includes/prodshort.md)] og Power BI. Du kan gjøre enkelte ting fra Power BI, mens andre ting gjør du fra [!INCLUDE[prodshort](includes/prodshort.md)]. I tillegg er noen funksjoner bare tilgjengelige i [!INCLUDE[prodshort](includes/prodshort.md)] Online, ikke i den lokale versjonen. Du får en oversikt i tabellen nedenfor.

|Funksjon|Beskrivelse|Online|Lokalt|Mer informasjon|
|-------|-----------|--------------|-----------|----------------|
|Vis [!INCLUDE[prodshort](includes/prodshort.md)] data i Power BI.|Du kan vise dataene fra [!INCLUDE[prodshort](includes/prodshort.md)] i rapporter i Power BI. [!INCLUDE[prodshort](includes/prodshort.md)] Online omfatter noen forhåndsdefinerte Power BI-rapporter. Det kan også hende at organisasjonen har gjort enkelte egendefinerte rapporter tilgjengelige for deg.|![avmerking](media/check.png)|![avmerking](media/check.png)|[Se ...](across-working-with-powerbi.md)|
|Vis Power BI-rapporter i [!INCLUDE[prodshort](includes/prodshort.md)]-klienten.| Power BI-rapporter som viser [!INCLUDE[prodshort](includes/prodshort.md)]-data, kan bygges inn direkte i deler på [!INCLUDE[prodshort](includes/prodshort.md)]-sider. Du kan bytte del for å vise enhver rapport som er gjort tilgjengelig for deg. |![avmerking](media/check.png)|![avmerking](media/check.png)<sup>[*](#onprem)</sup>|[Se ...](across-working-with-business-central-in-powerbi.md)|
|Opprett rapporter og instrumentbord i Power BI som viser [!INCLUDE[prodshort](includes/prodshort.md)]-dataene.|Bruk Power BI Desktop til å opprette egne rapporter og instrumentbord. Du kan publisere rapportene til din egen Power BI-tjeneste eller dele dem med andre i organisasjonen.|![avmerking](media/check.png)|![avmerking](media/check.png)|[Se ...](across-how-use-financials-data-source-powerbi.md)
|[!INCLUDE[prodshort](includes/prodshort.md)]-apper i Power BI| [!INCLUDE[prodshort](includes/prodshort.md)] publiserer tre apper for Power BI på Microsoft AppSource. Disse appene oppretter detaljerte rapporter og instrumentbord i Power BI-tjenesten for å vise [!INCLUDE[prodshort](includes/prodshort.md)]-data. Tilgjengelige apper omfatter følgende: <ul><li>[!INCLUDE [prodlong](includes/prodlong.md)] – CRM </li><li>[!INCLUDE [prodlong](includes/prodlong.md)] – Finance </li><li>[!INCLUDE [prodlong](includes/prodlong.md)] – Sales </li></ul>  |![avmerking](media/check.png)||[Se ...](across-powerbi-business-central-apps.md)

<a name="onprem"><sup>*</sup></a> Denne funksjonen krever et registrert program for Business Central i Microsoft Azure. Hvis du vil ha mer informasjon, kan du se [Registrere Business Central lokalt i Azure AD for integrering med andre tjenester](/dynamics365/business-central/dev-itpro/administration/register-app-azure).

## <a name="getting-ready-to-use-power-bi"></a>Gjøre klart til bruk av Power BI

Det er noen få oppgaver du må gjøre før du kan begynne å bruke Power BI med [!INCLUDE[prodshort](includes/prodshort.md)]. Noen av oppgavene gjøres vanligvis bare av administratorer eller superbrukere.

1. Hvis du bruker [!INCLUDE[prodshort](includes/prodshort.md)] lokalt, må du sørge for at distribusjonen oppfyller kravene som er beskrevet i [Konfigurere [!INCLUDE[prodshort](includes/prodshort.md)] lokalt for Power BI-integrering](admin-powerbi-setup.md#setup). Denne oppgaven er vanligvis en administrativ oppgave.

2. Publiser data som webtjenester.

    Kodeenheter, sider og spørringer du vil bruke som datakilden i Power BI-rapporter, må publiseres som webtjenester. Mange webtjenester er publisert som standard. Det er enkelt å finne webtjenestene ved å søke etter *webtjenester* i [!INCLUDE[prodshort](includes/prodshort.md)].
    
    Hvis du vil ha mer informasjon om publisering av webtjenester, kan du se [Publisere en webtjeneste](across-how-publish-web-service.md).

3. Få deg en Power BI-konto.

    Du må ha en Power BI-tjenestekonto for å kunne gjøre noe som helst med Power BI og [!INCLUDE[prodshort](includes/prodshort.md)], enten du er en administrator eller en forbruker. Du kan få deg en konto ved å gå til [https://powerbi.microsoft.com](https://powerbi.microsoft.com). Du registrerer deg for en konto ved å bruke e-postadressen og passordet for jobben din. Registreringen krever at du har en lisens, men i de fleste tilfeller skal du allerede ha en gratis lisens. Hvis du vil ha mer informasjon, kan du se [Power BI-lisensiering](admin-powerbi-setup.md#license).

4. Hvis du vil opprette dine egne Power BI-rapporter, går du til Power BI Desktop.

    Du kan laste ned [Power BI Desktop](https://powerbi.microsoft.com/desktop/). Hvis du vil ha mer informasjon, kan du se [Få Power BI Desktop](/power-bi/fundamentals/desktop-get-the-desktop).

## <a name="see-related-training-at-microsoft-learn"></a>Se relatert opplæring på [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>Se også

[Power BI for forbrukere](/power-bi/consumer/end-user-consumer)  
[Nytt utseende på Power BI-tjenesten](/power-bi/service-new-look)  
[Hurtigstart: Koble til data i Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  
[Power BI-dokumentasjon](/power-bi/)  
[Forretningsintelligens](bi.md)  
[Komme i gang](product-get-started.md)  
[Importere forretningsdata fra andre økonomisystemer](across-import-data-configuration-packages.md)  
[Konfigurere [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Bruke [!INCLUDE[d365fin](includes/d365fin_md.md)] som en Power BI-datakilde](across-how-use-financials-data-source-powerbi.md)  
[Bruke [!INCLUDE[d365fin](includes/d365fin_md.md)] som en Power Apps-datakilde](across-how-use-financials-data-source-powerapps.md)  
[Ved hjelp av [!INCLUDE[d365fin](includes/d365fin_md.md)] i Power Automate](across-how-use-financials-data-source-flow.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
