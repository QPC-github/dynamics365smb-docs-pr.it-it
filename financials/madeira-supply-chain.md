---
title: Catena di approvvigionamento | Documenti Microsoft
description: Informazioni sui concetti e i processi principali della catena di approvvigionamento
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: product overview, ERP
ms.date: 03/28/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 4ed8437f5d1b7628f256bb435de8ba13bd64a8f9
ms.contentlocale: it-it
ms.lasthandoff: 05/04/2017


---
# <a name="supply-chain"></a>Catena di approvvigionamento
[!INCLUDE[d365fin](includes/d365fin_md.md)] supporta i comuni processi della catena di approvvigionamento, sebbene limitati alle esigenze delle aziende di distribuzione e vendita all'ingrosso senza gestione warehouse.

Oltre ai documenti di fatture di vendita è possibile gestire l'evasione ordini con ordini di vendita e la spedizione di parti di quantità di un ordine, ad esempio nel caso in cui non sia ancora disponibile la quantità completa. È possibile gestire spedizioni dirette da un fornitore a un cliente collegando l'ordine di vendita al relativo ordine di acquisto.

Le quantità di magazzino vengono aggiornate in modo dinamico contestualmente ad acquisti e vendite degli articoli e le informazioni o gli avvisi sulla disponibilità vengono visualizzate per i venditori in diversi modi. È possibile modificare manualmente le quantità di magazzino registrandole direttamente nei movimenti contabili articoli, ad esempio, dopo un conteggio fisico. È possibile offrire e vendere articoli ai clienti senza gestire un magazzino correlato. Se si desidera includere questi articoli non in stock nel processo della catena di approvvigionamento, si deve semplicemente convertirli in normali articoli.

Oltre ai documenti fattura di acquisto, è possibile gestire il lato dell'approvvigionamento con gli ordini di acquisto con la possibilità di registrare carichi parziali di una quantità dell'ordine. Una funzione semplice di pianificazione degli approvvigionamenti consente di avviare un acquisto direttamente dalla fattura di vendita che richiede gli articoli.

Entrambi i documenti di vendita e acquisto possono essere registrati solo come spediti o ricevuti oppure come spediti o ricevuti e fatturati, con la possibilità di suddividere le responsabilità tra gestori ordini e ruoli contabili.

Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.

| Per | Vedere |
| --- | --- |
| Registrare i nuovi clienti, apportare le offerte di vendita, vendere i prodotti in ordini o fatture, ad esempio come spedizioni dirette, e gestire i resi di vendita. |[Vendite](sales-manage-sales.md) |
| Registrare nuovi fornitori, prodotti del fornitore in ordini o fatture, ad esempio con avvio da una fattura di vendita, e gestire i resi acquisto. |[Acquisti](purchasing-manage-purchasing.md) |
| Registrare nuovi prodotti fisici o di assistenza, rettificare le quantità di magazzino e gestire il valore di magazzino registrando i costi rettificati nella contabilità generale. |[Magazzino](inventory-manage-inventory.md) |

## <a name="see-also"></a>Vedi anche
[Setup Vendite](sales-setup-sales.md)  
[Gestione della contabilità clienti](receivables-manage-receivables.md)     
[Impostazioni acquisti](purchasing-setup-purchasing.md)  
[Gestione della contabilità fornitori](payables-manage-payables.md)    
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Funzionalità aziendali generali](ui-across-business-areas.md)
