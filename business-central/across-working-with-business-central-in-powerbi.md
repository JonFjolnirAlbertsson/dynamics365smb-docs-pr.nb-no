---
title: Arbeide med Business Central-data i Power BI | Microsoft Docs
description: Få innsikt, forretningsanalyse og KPI-er fra Business Central-dataene ved å bruke Power BI.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.date: 07/10/2020
ms.author: jswymer
ms.openlocfilehash: bdcbcb0fa82d799e29cfcdbb034e231635510656
ms.sourcegitcommit: aeaa0dc64e54432a70c4b0e1faf325cd17d01389
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/17/2020
ms.locfileid: "3697781"
---
# <a name="working-with-prodshort-data-in-power-bi"></a>Arbeide med [!INCLUDE [prodshort](includes/prodshort.md)]-data i Power BI

I denne artikkelen får du grunnleggende informasjon om å arbeide med rapporter og instrumentbord i Power BI som bruker [!INCLUDE [prodshort](includes/prodshort.md)] som datakilde. Artikkelen tar for seg noen aspekter som hjelper deg å komme i gang som [!INCLUDE[prodshort](includes/prodshort.md)]-bruker. Når det gjelder generelle retningslinjer og instruksjoner for hvordan du bruker Power BI, kan du se [Power BI-dokumentasjon for forbrukere](https://review.docs.microsoft.com/en-us/power-bi/consumer).

## <a name="get-ready"></a>Gjøre deg klar

Registrer deg for Power BI-tjenesten. Hvis du ikke allerede har registrert deg, går du til [https://powerbi.microsoft.com](https://powerbi.microsoft.com). Når du registrerer deg, bruker du en e-postadresse og et passord for jobben din.

## <a name="get-started"></a>Kom i gang

Når du har en Power BI-konto, kan du logge deg på på [https://powerbi.microsoft.com/](https://powerbi.microsoft.com/).

Power BI-tjenesten er vert for alle rapportene som er tilgjengelige for deg. Velg **Mitt arbeidsområde** > **Rapporter** for å vise rapporten. Deretter velger du bare rapporten du vil vise.

Med [!INCLUDE[prodshort](includes/prodshort.md)] Online får du automatisk et sett med standardrapporter på arbeidsområdet. Hvis du vil opprette egne rapporter, kan du bruke Power BI Desktop til å opprette dem og deretter publisere dem på arbeidsområdet ditt. Hvis du vil ha mer informasjon, kan du se [Komme i gang med å bygge rapporter i Power BI Desktop for å vise [!INCLUDE [prodlong](includes/prodlong.md)]-data](across-how-use-financials-data-source-powerbi.md).

Hvis du bruker [!INCLUDE[prodshort](includes/prodshort.md)] lokalt, må du starte fra grunnen av ved å bruke Power BI Desktop. Alternativt kan Power BI-rapporter distribueres som filer du kan laste opp.

## <a name="get-the-latest-data"></a>Få de nyeste dataene

Hver Power BI-rapport er basert på et datasett som henter data fra [!INCLUDE[prodshort](includes/prodshort.md)]-kildene. Du må sørge for at dataene i Power BI-rapportene er oppdatert med dataene i [!INCLUDE[prodshort](includes/prodshort.md)]. Dette begrepet omtales som *oppdatering*.  Det kan hende at oppdatering ikke skjer automatisk, avhengig av hvordan organisasjonen har konfigurert Power BI. Du kan oppdatere data på to måter: manuelt eller ved å planlegge en oppdatering. Manuell oppdatering utføres etter behov. Planlagt oppdatering lar deg oppdatere automatisk ved angitte tidsintervaller.

### <a name="refresh-manually"></a>Oppdatere manuelt

Velg **Flere alternativer (...)** ved siden av datasettet under **Datasett** i navigasjonsruten, og velg deretter **Oppdater nå**.

### <a name="schedule-a-refresh"></a>Planlegge en oppdatering

Velg Flere alternativer (...) ved siden av datasettet under Datasett i navigasjonsruten, og velg deretter **Planlegg oppdatering**. Fyll inn informasjonen under **Planlegg oppdatering**, og velg **Bruk**.

Hvis du vil ha mer informasjon, kan du se [Konfigurere planlagt oppdatering](/power-bi/connect-data/refresh-scheduled-refresh)

## <a name="upload-reports-from-files"></a><a name="upload"></a>Laste opp rapporter fra filer

Power BI-rapporter kan distribueres mellom brukere som PBIX-filer. Hvis du har en PBIX-fil, kan du laste opp filen til et arbeidsområde. Gjør følgende for å laste opp en rapport:

1. Velg **Hent data** i det nye arbeidsområdet.

2. Velg **Hent** i Filer-boksen.

3. Velg **Lokal fil**, gå til plasseringen der du lagret filen, og velg **Åpne**.

Hvis du vil ha mer informasjon, kan du se [Laste opp rapporten til tjenesten](/power-bi/paginated-reports/paginated-reports-quickstart-aw#upload-the-report-to-the-service).

> [!NOTE]
> Du må ha et arbeidsområdet i en [Premium-kapasitet](/power-bi/service-premium-what-is) for å kunne laste opp en rapport. Hvis du vil ha mer informasjon, kan du se [Administrere Premium-kapasiteter](/power-bi/admin/service-premium-capacity-manage). 

> [!TIP]
> Hvis du bruker [!INCLUDE[prodshort](includes/prodshort.md)] Online, kan du også laste opp en rapport fra [!INCLUDE[prodshort](includes/prodshort.md)]. Hvis du vil ha mer informasjon, kan du se [Arbeide med Power BI-rapporter i [!INCLUDE [prodshort](includes/prodshort.md)] – laste opp rapporter](across-working-with-powerbi.md#upload).

## <a name="share-reports-with-others"></a><a name="share"></a>Dele rapporter med andre

Når rapporten er i arbeidsområdet ditt, kan du dele den med andre i organisasjonen.

Hvis du vil dele en rapport, velger du **Del** i en liste over rapporter eller i en åpen rapport. I **Del rapport**-ruten angir du de fullstendige e-postadressene til enkeltpersonene eller distribusjonsgruppene du vil dele med. Følg instruksjonene på skjermen for å fullføre delingen. Hvis du vil ha mer informasjon, kan du se [Dele et instrumentbord eller en rapport](/power-bi/collaborate-share/service-share-dashboards#share-a-dashboard-or-report).

> [!NOTE]
> Du må ha [Power BI Pro-lisens](/power-bi/service-features-license-type), og det må også de du deler med. Innholdet må være i et arbeidsområde i en [Premium-kapasitet](/power-bi/service-premium-what-is). Hvis du vil ha mer informasjon, kan du se [Måter å dele arbeidet på i Power BI](/power-bi/service-how-to-collaborate-distribute-dashboards-reports).

## <a name="see-related-training-at-microsoft-learn"></a>Se relatert opplæring på [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>Se også

[Business Central og Power BI](admin-powerbi.md)  
[Bygge Power BI-rapporter for å vise [!INCLUDE [prodlong](includes/prodlong.md)]-data](across-how-use-financials-data-source-powerbi.md)  
[Oversikt over komponent og arkitektur for Power BI-integrering for [!INCLUDE[prodshort](includes/prodshort.md)]](admin-powerbi-overview.md)  
[Arbeide med Power BI-rapporter i [!INCLUDE [prodshort](includes/prodshort.md)]](across-working-with-powerbi.md)  
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
