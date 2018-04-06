---
title: Acquistare articoli per una vendita creando fatture di acquisto | Documenti Microsoft
description: "Da una fattura di vendita, per acquistare prodotti, è possibile creare una fattura di acquisto per un fornitore."
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supply planning, sales demand, replenish
ms.date: 01/25/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 82447508b12c4f158cb3fc5e257576e14ef284b4
ms.contentlocale: it-it
ms.lasthandoff: 03/22/2018

---
# <a name="purchase-items-for-a-sale"></a>Acquistare articoli per una vendita
Dagli ordini di vendita e dalle fatture di vendita, è possibile utilizzare funzioni per creare rapidamente i documenti di acquisto relativi alle quantità mancanti di articoli che sono necessari per la vendita. È possibile utilizzare due funzioni diverse che variano a seconda del tipo documento.
|Funzione|Description|
|--------|-----------|
|**Crea ordini di acquisto**|Da un ordine di vendita, questa funzione crea un ordine di acquisto per ciascun fornitore di articoli nell'ordine di vendita. È possibile modificare la quantità di acquisto prima di creare gli ordini di acquisto. Vengono suggerite solo le quantità di vendita non disponibili.
|**Crea fattura di acquisto**|Da un ordine di vendita e da una fattura di vendita, questa funzione crea una fattura di acquisto per un fornitore selezionato per tutte le righe o per le righe selezionate nel documento di vendita. Viene suggerita la quantità di vendita completa.|

## <a name="to-create-one-or-more-purchase-orders-from-a-sales-order"></a>Per creare uno o più ordini di acquisto da un ordine di vendita
Per creare un ordine di acquisto per ogni quantità articolo non disponibile nell'ordine di vendita, è possibile utilizzare la funzione **Crea ordini di acquisto**.

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Ordini di vendita**, quindi scegliere il collegamento correlato.
2. Aprire un ordine di vendita per cui si desidera acquistare degli articoli.
3. Scegliere l'azione **Crea ordini di acquisto**.

    Viene visualizzata la finestra **Crea ordini di acquisto** in cui viene mostrata una riga per ogni articolo differente nell'ordine di vendita. Vengono visualizzate per impostazione predefinita le righe per entrambe le quantità di vendita disponibili e non disponibili (in grigio). È possibile scegliere l'azione **Mostra non disponibili** per visualizzare solo le righe relative alle quantità di vendita non disponibili.

    Il campo **Quantità da acquistare** contiene la quantità di vendita non disponibile per impostazione predefinita.
4. Per effettuare un acquisto di una quantità diversa dalla quantità di vendita non disponibile, modificare il valore nel campo **Quantità da acquistare**.

    > [!NOTE]  
    >   È possibile modificare anche il campo **Quantità da acquistare** nelle righe inattive anche se rappresentano le quantità di vendita completamente disponibili.
5. Scegliere il pulsante **OK**.

    Un ordine di acquisto viene creato per ciascun fornitore di articoli nell'ordine di vendita, inclusa qualsiasi modifica delle quantità effettuata nella finestra **Crea ordini di acquisto**.
7. Continuare a elaborare l'ordine o gli ordini di acquisto, ad esempio, modificando o aggiungendo altre righe all'ordine di acquisto. Per ulteriori informazioni, vedere [Registrare gli acquisti](purchasing-how-record-purchases.md).


## <a name="to-create-a-purchase-invoice-from-a-sales-order-or-sales-invoice"></a>Per creare una fattura di acquisto da un ordine o una fattura di vendita
Per creare un'unica fattura di acquisto per una o più righe di un documento di vendita selezionando prima il fornitore da cui effettuare l'acquisto, utilizzare la funzione **Crea fattura di acquisto**.

> [!NOTE]  
>   Questa funzione crea una fattura di acquisto per la quantità articolo esatta nel documento di vendita selezionato. Per modificare la quantità di acquisto, è necessario modificare la fattura di acquisto dopo che è stata creata.  

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Ordini di vendita**, quindi scegliere il collegamento correlato.
2. Aprire una fattura di vendita per cui si desidera acquistare degli articoli.
3. Selezionare una o più righe della fattura di vendita da utilizzare nella fattura di acquisto. Per utilizzare tutte le righe della fattura di vendita, selezionarle tutte o non selezionarne alcuna.
4. Scegliere l'azione **Crea fattura di acquisto**.
5. Selezionare **Tutte le righe** o **Righe selezionate**, quindi scegliere **OK**.  
6. Nell'elenco di fornitori che viene visualizzato, selezionare il fornitore da cui si desidera acquistare tutti gli articoli e scegliere **OK**.

    Viene creata una fattura d'acquisto che contiene una, più o tutte le righe nella fattura di vendita.
7. Continuare a elaborare la fattura di acquisto, ad esempio, modificando o aggiungendo altre righe alla fattura di acquisto. Per ulteriori informazioni, vedere [Registrare gli acquisti](purchasing-how-record-purchases.md).

## <a name="see-also"></a>Vedi anche
[Acquisti](purchasing-manage-purchasing.md)  
[Registrare gli acquisti](purchasing-how-record-purchases.md)  
[Fatturare le vendite](sales-how-invoice-sales.md)  
[Registrare nuovi fornitori](purchasing-how-register-new-vendors.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
