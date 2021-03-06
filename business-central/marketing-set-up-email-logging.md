---
title: Konfigurere loggføring av e-post| Microsoft Docs
description: Lær hvordan du kan gjøre om e-postinteraksjon mellom selgere og kunder til reelle salgsmuligheter.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect, opportunity, email
ms.date: 07/01/2020
ms.author: bholtorf
ms.openlocfilehash: 9ca381bfebcd6db8e67d8153d4d2bc17eeffad81
ms.sourcegitcommit: f9aec4a72172d9270e14e2938c5550d69508f1aa
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/02/2020
ms.locfileid: "3532672"
---
# <a name="track-email-message-exchanges-between-salespeople-and-contacts"></a>Spor utveksling av e-postmeldinger mellom selgere og kontakter

Få mer ut av kommunikasjonen mellom selgere og de eksisterende eller potensielle kundene ved å spore e-postutvekslinger og deretter gjøre dem om til salgsmuligheter. [!INCLUDE[d365fin](includes/d365fin_md.md)] fungerer med Exchange Online for å føre en logg over innkommende og utgående meldinger. Du kan vise og analysere innholdet i hver enkelt melding på siden **Samhandlingsposter**.

## <a name="set-up-public-folders-and-rules-for-email-logging-in-exchange-online"></a>Definere fellesmapper og regler for e-postpålogging i Exchange Online

[!INCLUDE[admin-setup-email-public-folder](includes/admin-setup-email-public-folder.md)]

Deretter kobler du [!INCLUDE[prodshort](includes/prodshort.md)] til Exchange Online.

## <a name="setting-up-d365fin-to-log-email-messages"></a>Konfigurere [!INCLUDE[d365fin](includes/d365fin_md.md)] for å logge e-postmeldinger

Kom i gang med e-postpålogging med to enkle trinn:

1. Koble [!INCLUDE[d365fin](includes/d365fin_md.md)] til Exchange Online for Office 365-abonnementet. Exchange Online behandler e-postmeldingene. Vi har gjort dette trinnet enkelt ved å tilby en veiledning for assistert oppsett. Du trenger bare administratorlegitimasjon for administratorkontoen i Office 365. Gå til **Assistert oppsett** og velg deretter **Konfigurer loggføring av e-post**.  

2. Kontroller at det er angitt gyldige e-postadresser i [!INCLUDE[d365fin](includes/d365fin_md.md)] for selgere og kontakter, avhengig av om de er potensielle eller eksisterende kunder. For hver kunde eller selger åpner du **Kontakt** eller **Selger/innkjøper**-kortet og ser i **E-post** -feltet.

> [!Tip]
> Når du har fullført trinnene i guiden, kan du kontrollere om tilkoblingen var vellykket. Søk etter **Markedsføringsoppsett**, velg **Behandle**, og velg deretter **Funksjoner** og deretter **Valider oppsett for loggføring av e-post**.

## <a name="viewing-email-message-exchanges-in-the-interaction-log"></a>Vise utvekslinger av e-postmeldinger i samhandlingsloggen

[!INCLUDE[d365fin](includes/d365fin_md.md)] oppretter en post på siden **Samhandlingslogg** hver gang en selger og en kontakt utveksler en e-postmelding. Hvis du vil vise samhandlingsloggen, åpner du **Kontakter** eller **Selger/innkjøper**-kortet for personen, og deretter velger du **Naviger**, **Logg** og deretter **Samhandlingsposter**. Det er et par ting vi kan gjøre med hver oppføring i loggen, for eksempel:

- Vis innholdet i e-postmeldingen som ble utvekslet, ved å klikke handlingen **Vis vedlegg**.
- Gjør en e-postutveksling om til en salgsmulighet – Hvis en oppføring ser lovende ut, kan du gjøre den om til en salgsmulighet og deretter håndtere fremdriften for den mot et salg. Velg oppføringen for å gjøre dette, og velg deretter handlingen **Opprett salgsmulighet**. Hvis du vil ha mer informasjon, kan du se [Håndtere salgsmuligheter](marketing-manage-sales-opportunities.md).

## <a name="see-also"></a>Se også
[Administrere forbindelser](marketing-relationship-management.md)

