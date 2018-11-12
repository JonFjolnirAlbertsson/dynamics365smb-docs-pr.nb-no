---
title: Opprette hyller | Microsoft-dokumentasjon
description: "Den mest effektive metoden for å opprette hyllene i lageret, er å generere grupper av lignende hyller i hylleopprettingsforslaget, men du kan også opprette hyllene individuelt."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 7d5b2ce28f1eaebfca26c2db3801b44ff5278e78
ms.contentlocale: nb-no
ms.lasthandoff: 09/28/2018

---
# <a name="create-bins"></a>Opprette hyller
Den mest effektive metoden for å opprette hyllene i lageret, er å generere grupper av lignende hyller i hylleopprettingsforslaget, men du kan også opprette hyllene individuelt fra lokasjonskortet. Du kan også bruke en funksjon i vinduet **Hylleoppretting** til å opprette hyller automatisk.  

## <a name="to-create-a-bin-from-the-location-card"></a>Slik oppretter du en hylle fra lokasjonskortet  
1.  Velg ikonet ![lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre") ikonet, angi **Lokasjoner**, og velg den relaterte koblingen.  
2.  Velg lokasjonen der du vil opprette en hylle, og velg deretter **Hyller**-handlingen.  
3. Velg handlingen **Ny**.
4. Fyll ut feltene etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-create-bins-individually-in-the-bin-creation-worksheet"></a>Slik oppretter du hyller individuelt i hylleopprettingsforslaget  
1.  Velg ikonet ![lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Hylleopprettingsforslag**, og velg deretter den relaterte koblingen.  
2.  På hver linje fyller du ut de feltene som er nødvendig for å gi navn til og karakterisere hyllene du oppretter.  
3.  Velg handlingen **Opprett hyller**.  

## <a name="to-make-bins-automatically-in-the-bin-creation-worksheet"></a>Slik lager du hyller automatisk i hylleopprettingsforslaget  
Før du begynner å opprette hyller automatisk, bør du finne ut hvilken slags hylle som er viktig for dine operasjoner, og du bør finne den mest praktiske vareflyten gjennom strukturen i lageret.  

> [!NOTE]  
>  Når du bruker en hylle, kan du ikke slette den med mindre den er tom. Men hvis du noen gang ønsker å bruke et annet system for navngivning av hyller, kan du bruke reklassifiseringskladden til å flytte varene til et nytt hyllesystem. Denne prosessen er imidlertid manuell og tidkrevende, så det er best å sette opp hyllene riktig fra starten av.  

For å kunne arbeide i vinduet **Hylleoppretting** må du defineres som lageransatt på stedet der hyllene er. Hvis du vil ha mer informasjon, kan du se [Definere lageransatte](warehouse-how-to-set-up-warehouse-employees.md).    

1.  Velg ikonet ![lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Hylleopprettingsforslag**, og velg den relaterte koblingen.  
2.  Velg **Beregn hyller**-handlingen.
3. I vinduet **Beregn hyller** i feltet **Kode for hyllemal** velger du hyllemalen du vil bruke som modell for hyllene du bruker.
4.  Fyll ut en beskrivelse for hyllene du er i ferd med å opprette.  
5.  Opprett hyllekodene ved å fylle ut feltene **Fra nr.** og **Til nr.** i de tre kategoriene som vises i vinduet: **Reol**, **Seksjon** og **Nivå.** Hyllekoden kan inneholde opptil 20 tegn.  

    > [!NOTE]  
    >  Antall tegn du har angitt i de tre kategoriene for et hvilket som helst av feltene, for eksempel de tegnene du har angitt i de tre **Fra nr.** -feltene, pluss eventuelle feltskilletegn, må være 20 eller færre.  

     Du kan bruke bokstaver i koden som en identifiserende kombinasjon, men den bokstaven du bruker, må være den samme i **Fra nr.**- og og **Til nr.** -feltene. Du kan for eksempel definere Reol-delen av koden som **Fra nr. A01** og **Til nr. A10**. Programmet er ikke satt opp til å generere koder med bokstavsekvenser, for eksempel fra A01 til F05.  

6.  Hvis du ønsker å bruke et tegn, for eksempel en bindestrek, til å skille kategorifeltene du har definert som en del av hyllekoden, angir du dette tegnet i feltet **Feltseparator**.  
7.  Hvis du vil at programmet ikke skal opprette en linje for en hylle hvis den allerede finnes, velger du feltet **Kontroller eksisterende hylle**.  
8. Når du er ferdig med å fylle ut alle feltene, velger du **OK**.

    Programmet oppretter en linje for hver hylle i forslaget. Du kan nå slette noen av hyllene, for eksempel hvis du har en reol med en passasje gjennom de to første nivåene av et par seksjoner.  

9. Når du har slettet alle unødvendige hyller, velger du handlingen **Opprett hyller**. Programmet vil da opprette hyller for hver linje i forslaget.  

Gjenta prosessen for et annet sett av hyller til du har opprettet alle hyllene i lageret.  

## <a name="see-also"></a>Se også  
[Lagerstyring](warehouse-manage-warehouse.md)  
[Lager](inventory-manage-inventory.md)  
[Definere lagerstyring](warehouse-setup-warehouse.md)     
[Monteringsstyring](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyring](design-details-warehouse-management.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
