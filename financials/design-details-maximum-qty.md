---
title: "Designdetaljer – Maks.ant. | Microsoft-dokumentasjon"
description: "Maksimumsantall-prinsippet er en måte å opprettholde beholdningen på ved hjelp av et gjenbestillingspunkt."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 26bed0b8832d5b12ce5d697df8ec6194ac7ae9b2
ms.contentlocale: nb-no
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-maximum-qty"></a>Designdetaljer: Maks.ant.
Maksimumsantall-prinsippet er en måte å opprettholde beholdningen på ved hjelp av et gjenbestillingspunkt.  
  
 Alt for prinsippet Fast gjenbest.ant. gjelder også for dette prinsippet. Den eneste forskjellen er antallet i forsyningen som foreslås. Når du bruker prinsippet om maksimumsantall, defineres gjenbestillingsantallet dynamisk basert på det beregnede beholdningsnivået og varierer derfor vanligvis fra bestilling til bestilling.  
  
## <a name="calculated-per-time-bucket"></a>Beregnet per tidsperiode  
 Gjenbestillingsantallet fastsettes på tidspunktet (slutten av en tidsperiode) der planleggingssystemet oppdager at gjenbestillingspunktet er overskredet. Systemet måler nå avstanden fra gjeldende beregnede beholdningsnivået opp til angitt maksimal lagerbeholdning. Dette utgjør antallet som må bestilles. Systemet kontrollerer deretter om forsyning allerede er bestilt et annet sted og kommer til å mottas innen leveringstiden, og i så fall reduseres antallet i den nye forsyningsordren med antallet som allerede er bestilt.  
  
 Systemet sikrer at den beregnede beholdningen minst når gjenbestillingspunktet, i tilfelle brukeren har glemt å angi en maksimumsbeholdning.  
  
## <a name="combines-with-order-modifiers"></a>Kombineres med ordremodifikatorer  
 Avhengig av oppsettet kan det være best å kombinere prinsippet for maksimumsantall med ordremodifikatorer for å sikre et minimumsordreantall, runde det opp til et heltall innkjøpsenheter, eller dele den inn i flere partier som er definert av maksimumsordreantallet.  
  
## <a name="combines-with-calendars"></a>Kombinerer med kalendere  
 Før det blir foreslått en ny forsyningsordre for å oppfylle et gjenbestillingspunkt, kontrollerer systemet om ordren er planlagt for en fridag, i henhold til kalendere som er definert i feltet **Hovedkalenderkode** i vinduene **Selskapsopplysninger** og **Lokasjonskort**.  
  
 Hvis den planlagte datoen er en fridag, flytter planleggingssystemet ordren fremover til nærmeste arbeidsdato. Dette kan resultere i en ordre som oppfyller et gjenbestillingspunkt, men som ikke oppfyller enkelte spesifikke behov. For slike ubalanserte behov oppretter planleggingssystemet en ekstra forsyning.  
  
## <a name="see-also"></a>Se også  
 [Designdetaljer: Gjenbestillingsprinsipper](design-details-reordering-policies.md)   
 [Designdetaljer: Planleggingsparametere](design-details-planning-parameters.md)   
 [Designdetaljer: Håndtere gjenbestillingsprinsipper](design-details-handling-reordering-policies.md)   
 [Designdetaljer: Forsyningsplanlegging](design-details-supply-planning.md)