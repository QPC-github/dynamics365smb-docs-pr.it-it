---
title: Informazioni sui tipi di articolo | Documenti Microsoft
description: "È possibile modificare la valutazione di magazzino di un articolo mediante i metodi di costing Media o FIFO, ad esempio, quando i costi degli articoli cambiano per i motivi diversi dalle transazioni."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 11/18/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 2240840e977bcd1186c74972ce0457deb03058a0
ms.contentlocale: it-it
ms.lasthandoff: 11/26/2018

---
# <a name="about-item-types"></a>Informazioni sui tipi di articolo
Nel campo **Tipo** nella pagina **Scheda articolo** è possibile selezionare l'articolo utilizzato nella propria azienda e quindi come viene gestito nel sistema. Sono disponibili tre opzioni:

|Opzione|Scopo tipico|
|------|-----------|
|Inventario|Un'unità fisica, come una bicicletta, per un pieno supporto commerciale.|
|Non in inventario|Un'unità fisica, ad esempio un bullone, per un supporto aziendale limitato, ad esempio perché l'articolo viene utilizzato solo internamente e ha un costo ridotto.|
|Assistenza|Un'unità di misura del tempo della manodopera, ad esempio un'ora di consulenza, per un supporto aziendale limitato.|

Il tipo **Inventario** prevede il monitoraggio completo della quantità e del valore di inventario. Di conseguenza, tutti i tipi di transazione dell'articolo sono supportati e gli articoli di tipo Inventario possono essere utilizzati con tutte le funzionalità di gestione degli articoli.

I tipi **Assistenza** e **Non in inventario** non prevedono il tracciamento della quantità e del valore dell'inventario. Di conseguenza, sono supportati solo i tipi e le funzionalità delle transazioni dell'articolo selezionato.

I tre tipi dell'articolo supportano rispettivamente le seguenti funzionalità.

|Tipo di articolo|Vendite|Acquisti|Consumo per la commessa|Consumo di assistenza|Consumo assemblaggio|Consumo produzione|Output assemblaggio|Output produzione|Trasferimento ubicazione|Conteggio fisico|Rivalutazione del magazzino|Costing di magazzino|Tracciabilità articolo|Impegni|Gestione della warehouse|Pianificazione|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|Magazzino|Sì|Sì|Sì|Sì|Sì|Sì|Sì|Sì|Sì|Sì|Sì|Sì|Sì|Sì|Sì|Sì|
|Non in inventario|Sì|Sì|Sì|Sì|Sì|Sì|No|No|No|No|No|No|No|No|No|No|
|Servizio|Sì|Sì|Sì|No|No|No|No|No|No|No|No|No|No|No|No|No|

> [!NOTE]
> Gli articoli offerti ai clienti che non si desidera gestire nel sistema fino a quando non si inizia a venderli possono essere impostati come articoli di catalogo. Gli articoli di catalogo non devono essere confusi con articoli normali di tipo Non in inventario. Per ulteriori informazioni, vedere [Utilizzare gli articoli di catalogo](inventory-how-work-nonstock-items.md).

> [!NOTE]
> Gli articoli dei clienti per cui si esegue il servizio di assistenza, come una stampante, sono denominati articoli in assistenza. Gli articoli in assistenza non hanno nulla a che fare con articoli normali o di catalogo. Tuttavia, i componenti di assistenza possono essere articoli regolari. Per ulteriori informazioni, vedere [Impostare gli articoli in assistenza e i componenti degli articoli in assistenza](service-how-setup-service-items.md).

## <a name="see-also"></a>Vedi anche
[Registrare nuovi articoli](inventory-how-register-new-items.md)  
[Impostazione del magazzino](inventory-setup-inventory.md)  
[Gestione dei costi di magazzino](finance-manage-inventory-costs.md)  
[Magazzino](inventory-manage-inventory.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
