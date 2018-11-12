---
title: Definere salgssykluser for salgsmuligheter og syklusfaser | Microsoft-dokumentasjon
description: "Beskriver hvordan du definerer salgsfaser, fra første kontakt til avslutning, for å opprette en salgssyklus og tilordne den til salgsmuligheter i Business Central."
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 10/01/2018
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 34262b070ea19b5f109c9194d6a91ef048132e6b
ms.contentlocale: nb-no
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-opportunity-sales-cycles-and-cycle-stages"></a>Definere salgssykluser for salgsmuligheter og syklusfaser
Før du kan begynne å bruke salgsmuligheter, må du definere salgssykluser og salgssyklusfaser. En salgssyklus består av en serie med faser som går fra den første kontakten til avslutningen av et salg. Hver fase kan ha bestemte krav som må oppfylles, for eksempel at et tilbud er påkrevd, før en salgsmulighet kan gå til neste fase. Du kan også angi om en fase kan utelates. Du kan definere så mange salgssykluser du trenger, og du kan definere så mange salgssyklusfaser som nødvendig i en salgssyklus.

Implementering av salgssykluser for salgsmulighet innebærer å definere salgssyklusen, definere de ulike syklusfasene og deretter tilordne syklusen til salgsmuligheter. Det å tilordne den relevante aktiviteten eller de relevante oppgavene til salgsmuligheten kan også være en del av å definere en salgssyklus.

Dette emnet beskriver også hvordan du definerer oppgaver og aktiviteter, og hvordan du tilordner oppgaver til aktiviteter. Hvis du vil ha mer informasjon, kan du se delen «Definere aktiviteter med oppgaver».

## <a name="to-set-up-opportunity-sales-cycle-codes"></a>Definere salgssykluskoder for salgsmuligheter
1. Velg ikonet ![lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Salgssykluser**, og velg deretter den relaterte koblingen. Vinduet **Salgssykluser** åpnes, og det viser alle eksisterende salgssykluser.
2. Velg handlingen **Ny**, og fyll ut feltene etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

Gjenta disse trinnene for å konfigurere så mange salgssykluser som du vil. Etter at du har definert salgssykluser for salgsmuligheter, bør du definere ulike faser i hver enkelt syklus.

## <a name="to-define-opportunity-sales-cycle-stages"></a>Definere salgssyklusfaser for salgsmulighet
1. I vinduet **Salgssykluser** velger du salgssyklusen for salgsmuligheten du vil definere faser for, og deretter velger du handlingen **Faser**. Vinduet **Salgssyklusfaser** åpnes.
2. Velg handlingen **Ny** for å angi en ny fase i salgssyklusen.

Gjenta disse trinnene hvis du vil definere flere faser i salgssyklusen.

## <a name="to-assign-stage-cycles-to-opportunities"></a>Tilordne fasesykluser til salgsmuligheter
Når du legger til fasesyklusen for salgsmulighet, kan du begynne å legge til salgsmuligheter og deretter tilordne fasesyklusen til salgsmuligheter ved å bruke feltet **Salgssykluskode**. Hvis du vil ha mer informasjon, kan du se [Opprette salgsmuligheter](marketing-how-create-opportunities.md).

## <a name="to-set-up-activities-with-tasks"></a>Definere aktiviteter med oppgaver
Du kan kombinere flere oppgaver, for eksempel oppgaver som representerer et trinn, i aktiviteter. Aktivitetsoppgaver er knyttet til hverandre ved hjelp av en datoformel. Du kan tilordne aktiviteter til salgsmuligheter, selgere eller kontakter.

1. Velg ikonet ![lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Aktiviteter**, og velg deretter den relaterte koblingen.
2. Velg handlingen **Ny**, og fyll ut feltene etter behov.
3. I hurtigfanen **Linjer** fyller du ut feltene etter behov for å definere én eller flere oppgaver i aktiviteten.

## <a name="to-assign-tasks-or-activities-of-tasks-to-opportunities"></a>Tilordne oppgaver eller aktiviteter med oppgaver til salgsmuligheter
Når du har definert en oppgave, kan du tilordne den til en salgsmulighet og derved tilordne aktiviteten som oppgaven hører til i.

> [!NOTE]  
>   Denne fremgangsmåten beskriver hvordan du tilordner aktivitetsoppgaver til salgsmuligheter. Fremgangsmåten ligner den du bruker når du tilordner oppgaver til selgere og kontakter.

1. Velg ikonet ![lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Salgsmuligheter**, og velg deretter den relaterte koblingen.
2. Velg en salgsmulighet, og velg deretter handlingen **Oppgaver**.
3. I vinduet **Oppgaveliste** velger du handlingen **Opprett oppgave**.
4.  Fyll ut feltene etter behov i vinduet **Opprett oppgave**.

    Legg merke til at feltet **Salgsmulighet** tilordnes automatisk til den aktuelle salgsmuligheten.
5. Velg **OK**.
6. I vinduet **Oppgaveliste** velger du en ny oppgave, og deretter velger du handlingen **Tilordne aktiviteter**.
7. I vinduet **Tilordne aktivitet** fyller du ut feltene etter behov, og deretter velger du **OK**.

## <a name="see-also"></a>Se også
[Behandle salgsmuligheter](marketing-processing-sales-opportunities.md)  
[Salg](sales-manage-sales.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
