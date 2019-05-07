---
title: Kontrollere sider i Business Central
description: Bruk funksjonen for sideinspeksjon til å zoome inn detaljer om sideutformingen og datakilden. Sideinspeksjonsfunksjonen er ideell for feilsøking av problemer med dataene.
ms.custom: na
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.service: dynamics365-business-central
author: jswymer
ms.date: 04/01/2019
ms.openlocfilehash: eb9d4ec76c0dbbd59763f7622ca51137c9563a91
ms.sourcegitcommit: addfb47612cc2e4e98dfd7e338b6f41cde405d5c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/16/2019
ms.locfileid: "969881"
---
# <a name="inspecting-pages-in-business-central"></a>Kontrollere sider i Business Central

Sideinspeksjonsfunksjonen gjør det mulig å få opplysninger om en side ved å gi innsikt i sideutformingen, de ulike elementene som utgjør siden, og kilden bak dataene som vises. Sideninspeksjon er spesielt utviklet for administratorer, avanserte brukere, støttepersonell og utviklere. Den er ideell for å lære datamodellen bak en side og feilsøking. Hvis du har et problem på en side, kan du bruke sideninspeksjon til å få informasjon som kan videresendes til systemansvarlig eller servicepersonell.

## <a name="working-with-page-inspection"></a>Arbeide med sideinspeksjon

Hvis du vil kontrollere en side i øvre høyre hjørne, kan du velge ![Innstillinger-ikonet](media/ui-experience/settings_icon_small.png) og deretter velge **Inspiser**. Du kan også bruke hurtigtasten **Ctrl+Alt+F1**.

Ruten **Sideninspeksjon** åpnes på siden. Følgende figur viser ruten **Sideninspeksjon** på siden **Ordre**.

![Sideinspeksjon](media/page-inspection-example.png)

Når ruten **Sideinspeksjon** åpnes for første gang, vises informasjon som gjelder hovedobjektet på siden.

Du kan tastaturet eller pekeenheten til å flytte fokus til forskjellige elementer på siden. Når du velger en faktaboks eller en del på hovedsiden, markeres rammeområdet med en kant, og **Sidenspeksjon**-ruten viser informasjon om det valgte elementet. Den forrige figuren viser opplysninger om listedelen på siden **Ordre**. Når du går til andre sider i programmet, vil ruten **Sideinspeksjon** automatisk oppdateres med sideinformasjon når du flytter.

Hvis du vil ha mer informasjon om hva som vises i sideinspeksjonen, kan du se [Inspisere og feilsøke sider](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-inspecting-pages) i hjelpen for utviklere og IT-eksperter for Business Central.

Hvis du ikke ser opplysningene du forventer å se i ruten **Sideinspeksjon**, har du trolig ikke den nødvengige tillatelsen, som beskrevet i neste del.

## <a name="controlling-access-to-page-inspection-details"></a>Kontrollere tilgang til sideinspeksjonsinformasjon

Som administrator kan du kontrollere tilgang til alle opplysninger som vises i ruten **Sideinspeksjon**, ved å konfigurere brukernes tillatelser. For å gi en brukertillatelse til alle opplysninger, kan du gi brukere **Kjør**-tilgang for **System**-objekt **5330**. Du kan gi tillatelse ved hjelp av et tillatelsessett (som for eksempel **D365-feilsøking**) eller en brukergruppe (som for eksempel **D365-feilsøking**). Hvis du vil ha mer informasjon om tillatelser, kan du se [Administrere brukere og tillatelser](ui-how-users-permissions.md).

Brukere som ikke har tilgang til **Systemobjekt 5330**, har fremdeles tilgang til **Sideinspeksjon**-ruten, men de ser bare **Side**- og **Tabell**-feltene, som viser grunnleggende informasjon som kan de kan sende videre til støttegruppen.

## <a name="see-also"></a>Se også

[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  