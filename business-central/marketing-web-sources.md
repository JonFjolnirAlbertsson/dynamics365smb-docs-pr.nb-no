---
title: Definere webkilder for kontaktselskaper | Microsoft-dokumentasjon
description: "Du kan definere Internett-kilder eller webkilder og tilordne dem til et kontaktselskap for å bidra til å identifisere hvor du vil søke etter informasjon om kontaktene."
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: internet
ms.date: 10/01/2018
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: b8c59f24eae07efe8f2c4ca1e4e22d05fd4f1b1c
ms.contentlocale: nb-no
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-web-sources-for-contact-companies"></a>Definere webkilder for kontaktselskaper
Du kan for eksempel bruke webkilder med kontaktselskaper for å identifisere søkemotorer og webområder på Internett, som du vil bruke til å søke etter informasjon om kontaktene. Når du tilordner webkilder, angir du hvilken søkemotor og søkeord programmet skal bruke for å finne de forespurte opplysningene.

Bruk av webkilder på kontakter er en totrinnsprosess. Først må du definere koden for webkilden. Du trenger bare utføre dette trinnet én gang for hver webkilde. Når du har en kode for webkilde, kan du begynne å tilordne koden til kontaktpersoner.

## <a name="to-define-a-web-source-code"></a>Slik definerer du en kode for webkilde
1. Velg ikonet ![lyspære som åpner Fortell meg-funksjonen](media/ui-search/search_small.png "Fortell hva du vil gjøre"), angi **Webkilder**, og velg deretter den relaterte koblingen.
2. Velg handlingen **Ny**.
3. Fyll ut feltene **Kode**, **Beskrivelse** og **URL**.

    Skriv inn %1 i feltet **Nettadresse** for å sette inn en plassholder for et søkeord i nettadressen. Når du starter webkilden fra et kontaktkort, erstattes %1 med søkeordet (for eksempel navnet på selskapet) som du angav i vinduet **Kontaktens webkilder**.

Gjenta disse trinnene hvis du vil definere flere webkilder.

## <a name="to-assign-web-sources-to-a-contact-company"></a>Slik tilordner du webkilder til et kontaktselskap
Når du tilordner webkilder, angir du hvilken søkemotor og søkeord som programmet skal bruke for å finne de forespurte opplysningene.

1. Åpne kontakten.
2. Velg handlingen **Selskap**, og velg deretter handlingen **Webkilder**. Vinduet **Kontaktens webkilder** åpnes.
3. Velg webkilden du vil tilordne i feltet **Webkilde - kode**.
4. I feltet **Søkeord** angir du et søkeord som du vil bruke for å finne opplysningene.

Gjenta disse trinnene hvis du vil tilordne flere webkilder.

Ved å følge samme fremgangsmåte kan du også tilordne webkilder fra vinduet **Kontaktoversikt**.

## <a name="see-also"></a>Se også
[Opprette kontaktselskaper](marketing-create-contact-companies.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
