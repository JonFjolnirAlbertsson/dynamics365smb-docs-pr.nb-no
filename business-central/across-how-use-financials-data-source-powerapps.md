---
title: "Bruk dataene til å lage en app | Microsoft-dokumenter"
description: "Du kan gjøre Financials-dataene tilgjengelige som en datakilde og angi en OData-URL-adresse til webtjenestene dine for å utvikle en forretningsapp ved hjelp av PowerApps."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Odata, Power App, SOAP
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 8db67d30ba18e9f7dba14b93ddf7b4de6e2b6444
ms.contentlocale: nb-no
ms.lasthandoff: 03/22/2018

---
# <a name="connecting-to-your-financials-data-to-build-a-business-app-using-powerapps"></a>Koble til Financials-dataene for å utvikle en forretningsapp ved hjelp av PowerApps
Du kan gjøre [!INCLUDE[d365fin](includes/d365fin_md.md)]-data tilgjengelige som en datakilde i PowerApps.  

> [!NOTE]  
>   Du må ha en gyldig konto med [!INCLUDE[d365fin](includes/d365fin_md.md)] og med PowerApps.  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-powerapps"></a>Legge til [!INCLUDE[d365fin](includes/d365fin_md.md)] som en datakilde i PowerApps
1. I leseren, kan du gå til [powerapps.microsoft.com](https://powerapps.microsoft.com/en-us/), og deretter logge på.
2. Velg **Ny app** i navigasjonsruten til venstre.
3. Velge redigeringsprogram, PowerApps Studio for Windows eller PowerApps Studio for Web.

   PowerApps Studio for Windows er et skrivebordsprogram som brukes til å opprette og publisere PowerApps. PowerApps Studio for Web er et nettløsningen som brukes til å opprette og publisere PowerApps.
4. Neste trinn for å opprette en PowerApp er å velge data. Velg pilikonet og deretter velge **Ny tilkobling** i øvre venstre side av siden.
5. I listen over tilgjengelige tilkoblinger velger du **Dynamics 365 Business Central**.
6. PowerApps vil vise en tilkoblingsside som ber deg om informasjonen som kreves for å koble til dine [!INCLUDE[d365fin](includes/d365fin_md.md)]-data. Hvis du vil koble til, må du angi en OData URL-adresse, brukernavn, passord og selskapsnavn.

   For *OData URL-adressen*, kan du kopiere OData V4 URL-adressen for web-tjenester som er oppført på siden **Web Services** i [!INCLUDE[d365fin](includes/d365fin_md.md)], som `https://mycompany.financials.dynamics.com:7048/MS/ODataV4/`.  

   For *Selskapsnavn*, bruk navnet som vises i **Navn**-feltet i vinduet **Selskapsopplysninger** i [!INCLUDE[d365fin](includes/d365fin_md.md)]. Hvis [!INCLUDE[d365fin](includes/d365fin_md.md)] inneholder flere selskaper, velger du det relevante selskapsnavnet fra listen i **Selskaper**-vinduet. I begge tilfeller må du kontrollere at navnet du angir i veiviseren for PowerApps tilsvarer teksten som vises i [!INCLUDE[d365fin](includes/d365fin_md.md)], som `My Company`.

   Om brukernavn og passord, kan du bruke navnet og web service hurtigtast som er angitt for kontoen i **Brukere**-vinduet i [!INCLUDE[d365fin](includes/d365fin_md.md)]. Ditt brukernavn er for eksempel *ADMIN*, og web service hurtigtast som fungerer som passordet ditt er *EgzeUFQ9Uv0o5O0lUMyqCzo1ueUW9yRF3SsLU =*.
7. Velg **Tilkobling**-knappen for å fortsette. PowerApps viser et standard datasett for [!INCLUDE[d365fin](includes/d365fin_md.md)]. Velg **Standard**-datasettet.

   PowerApps vil vise en liste over tabeller som er tilgjengelige fra [!INCLUDE[d365fin](includes/d365fin_md.md)]. Disse tabellene eller endepunktene, representerer alle web-tjenester som du har publisert fra [!INCLUDE[d365fin](includes/d365fin_md.md)].

   Alternativt, opprette en ny web service URL i [!INCLUDE[d365fin](includes/d365fin_md.md)] ved hjelp av **Opprett datasett** i siden **Web Services** ved hjelp av **Sett opp rapportering** assistert installasjonsveiledningen eller ved å velge **Rediger i Excel** i lister.
8. Velg tabellen som du vil bruke for din PowerApp, og velg deretter den **Koble til**-knappen.
9. Gjenta de forrige trinnene for å legge til flere [!INCLUDE[d365fin](includes/d365fin_md.md)]-data i Power BI-datamodellen.

   > [!NOTE]  
>    Når du har koblet til [!INCLUDE[d365fin](includes/d365fin_md.md)], blir du ikke bedt om OData-URL-adressen, brukernavnet eller passordet på nytt.

Nå har du koblet til Business Central-dataene og er klar til å begynne å bygge din PowerApp. Hvis du ønsker mer informasjon, se [PowerApps-dokumentasjonen](https://powerapps.microsoft.com/tutorials/getting-started/).

## <a name="see-also"></a>Se også
[Velkommen til [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Importere forretningsdata fra andre økonomisystemer](upload-data.md)  
[Konfigurere [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Finans](finance.md)  
