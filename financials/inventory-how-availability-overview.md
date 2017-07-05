---
title: "Procedura: Ottenere una panoramica della disponibilità | Documenti Microsoft"
description: "Viene descritto come visualizzare la disponibilità di articoli tra le ubicazioni, per eventi di vendita o di acquisto, in base a un periodo di tempo o alla posizione dell&quot;articolo su una DB assemblaggio."
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: stock
ms.date: 03/28/2017
ms.author: SorenGP
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 47071e5e325de8a31663b8d5a59d1ce93e5d0111
ms.contentlocale: it-it
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-get-an-availability-overview"></a>Procedura: Ottenere una panoramica della disponibilità
Dal contesto di un task di business, è possibile ottenere informazioni avanzate relative al momento e all'ubicazione in cui un articolo è disponibile, ad esempio quando si parla con un cliente per proporre una data di consegna.

È possibile visualizzare la disponibilità di tutti gli articoli per ubicazione ed è possibile visualizzare la disponibilità di ciascun articolo per evento, periodo o ubicazione. Per evento si intende qualsiasi transazione articolo pianificata, ad esempio una spedizione o un carico di trasferimento in entrata.

**Nota**: le visualizzazioni di disponibilità per ubicazione richiedono che si disponga di un magazzino presso più di un'ubicazione. Per ulteriori informazioni, vedere [Procedura: Impostare le ubicazioni](inventory-how-setup-locations.md).

In [[!INCLUDE[d365fin](includes/d365fin_md.md)] i dati relativi alla disponibilità vengono visualizzati in due campi diversi, ognuno con una diversa definizione:

* Il campo **Giacenza** mostra l'effettiva quantità in base ai movimenti contabili articoli registrati.
* Nel campo **Disponibilità calcolata** viene calcolato e viene visualizzata la giacenza più i carichi programmati e meno il fabbisogno lordo. In [[!INCLUDE[d365fin](includes/d365fin_md.md)] i carichi programmati includono le quantità degli ordini di acquisto e degli ordini di trasferimento in entrata. Il fabbisogno lordo include le quantità degli ordini di vendita e degli ordini di trasferimento in uscita.

**Suggerimento**: la disponibilità calcolata è particolarmente importante per visualizzare le finestra **Disponibilità art. per periodi** e **Disponibilità articolo per evento** dal momento che contengono le dimensioni per data.  

**Nota**: di seguito viene descritto come visualizzare le informazioni avanzate sulla disponibilità per articolo dall'elenco articoli e dalla scheda articolo. È inoltre possibile accedere alle informazioni contenute nelle righe dei documenti di vendita, per l'articolo nella riga. Per ulteriori informazioni, vedere [Procedura: Vendere prodotti](sales-how-sell-products.md).

## <a name="to-view-the-availability-of-an-item-according-to-when-it-will-be-received-or-shipped"></a>Per visualizzare la disponibilità di un articolo secondo quando verrà ricevuto o spedito
Si visualizza la disponibilità di un articolo secondo le transazioni pianificate dell'articolo nella finestra **Disponibilità articolo per evento**.

1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Articoli**, quindi scegliere il collegamento correlato.
2. Aprire la scheda di un articolo per cui si desidera visualizzare la disponibilità.
3. Scegliere l'azione **Disponibilità articolo per** quindi scegliere l'azione **Evento**.

    La finestra **Disponibilità articolo per evento** mostra come le quantità di magazzino dell'articolo si svilupperanno nel tempo in base agli eventi programmati per carico e spedizione. La finestra fornisce una visualizzazione ridotta che mostra una riga di informazioni accumulate per intervallo di tempo in cui le quantità di magazzino cambiano. Gli intervalli di tempo in cui non si è verificato alcun evento non sono visualizzati. È possibile espandere ogni riga per mostrare i dettagli sull'evento o gli eventi che hanno generato la quantità accumulata sulla riga.
4. Selezionare il valore nel campo **Disponibilità calcolata** per visualizzare i movimenti articoli o documenti aperti che compongono il valore.

## <a name="to-view-the-availability-of-an-item-in-different-periods"></a>Per visualizzare la disponibilità di un articolo in diversi periodi di tempo
È possibile visualizzare la disponibilità di un articolo nel tempo per periodi specificati nella finestra **Disponibilità art. per periodi**.

1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Articoli**, quindi scegliere il collegamento correlato.
2. Aprire la scheda di un articolo per cui si desidera visualizzare la disponibilità.
3. Scegliere l'azione **Disponibilità articolo per** quindi scegliere l'azione **Periodo**.

    La finestra **Disponibilità articolo per periodo** mostra come le quantità di magazzino dell'articolo si svilupperanno nel tempo in base al periodo selezionato, ad esempio giorno, settimana oppure trimestre.
4. Selezionare il valore nel campo **Disponibilità calcolata** per visualizzare i movimenti articoli o documenti aperti che compongono il valore.

## <a name="to-view-the-availability-of-an-item-at-the-locations-where-it-is-stored"></a>Per visualizzare la disponibilità di un articolo nelle ubicazioni dove è immagazzinato
È possibile visualizzare la disponibilità di un articolo presso i luoghi diversi dove viene immagazzinato nella finestra **Disp. art. per ubicazione**.

1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Articoli**, quindi scegliere il collegamento correlato.
2. Aprire la scheda di un articolo per cui si desidera visualizzare la disponibilità.
3. Scegliere l'azione **Disponibilità articolo per** quindi scegliere l'azione **Ubicazione**.

    La finestra **Disponibilità articolo per ubicazione** mostra come le quantità di magazzino dell'articolo si svilupperanno nel futuro in ogni ubicazione in cui è immagazzinato.
4. Selezionare il valore nel campo **Giacenza disponibile** per visualizzare i movimenti articoli che compongono il valore.
5. Selezionare il valore nel campo **Disponibilità calcolata** per visualizzare i movimenti articoli o documenti aperti che compongono il valore.

## <a name="to-view-the-availability-of-all-items-by-the-location-where-they-are-stored"></a>Per visualizzare la disponibilità di tutti gli articoli in base all'ubicazione in cui sono immagazzinati
È possibile visualizzare la disponibilità di tutti gli articoli in tutte le ubicazioni nella finestra **Articoli per ubicazione**.

1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Articoli**, quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Articoli per ubicazione**.

    La finestra **Articoli per ubicazione** mostra per tutti gli articoli le quantità disponibili in ogni ubicazione.
3. Selezionare il valore nel campo **Giacenza disponibile** per visualizzare i movimenti articoli che compongono il valore.

## <a name="to-view-the-availability-of-an-item-by-its-use-in-assembly-boms"></a>Per visualizzare la disponibilità di un articolo in base al relativo utilizzo nella DB assemblaggi
Se un articolo esiste in DB assemblaggi, come articolo principale o come componente, è possibile visualizzare il numero di unità che sono necessarie nella finestra **Disponibilità articolo per livello DB**. Nella finestra viene visualizzato il numero delle unità di un articolo padre che è possibile effettuare in base alla disponibilità di articoli figlio nelle righe sottostanti. Ogni articolo che ha una DB assemblaggio è visibile nella finestra come riga comprimibile. È possibile espandere la riga per visualizzare i componenti sottostanti i sottoassemblaggi di livello inferiore con le proprie DB.

È possibile utilizzare la finestra per verificare se è possibile soddisfare un ordine di vendita per un articolo nella data stabilita osservando la disponibilità corrente e le quantità che possono essere fornite dai componenti. È inoltre possibile utilizzare la finestra per identificare i colli di bottiglia nelle DB assemblaggio correlate.

In ogni riga della finestra per gli articoli padre e gli articoli figlio, i seguenti campi chiave specificano le cifre sulla disponibilità. È possibile utilizzare tali cifre per promettere il numero di unità di un articolo padre che è possibile fornire se si inizia il processo assemblaggio correlato.

|Campo|Descrizione|
|------|-----------|
|**Produzione possibile - Padre**|Mostra quante unità di un sottoassemblaggio nell'articolo principale è possibile preparare. Questo campo specifica quante unità dell'articolo padre immediate possono essere assemblate. Il valore è basato sulla disponibilità dell'articolo nella riga.|
|**Produzione possibile - Articolo principale**|Mostra quante unità dell'articolo principale è possibile preparare. Questo campo specifica quante unità dell'articolo DB nella prima riga possono essere assemblate. Il valore è basato sulla disponibilità dell'articolo nella riga.|

Nella finestra **Disponibilità articolo per livello DB** vengono visualizzate le informazioni relative all'articolo sulla scheda o la riga del documento per il quale viene viene aperta la finestra. L'articolo viene indicato sempre nella prima riga. È possibile visualizzare informazioni per altri articoli o per tutti gli articoli modificando il valore nel campo **Filtro articolo**.

**Nota**: per default, le cifre sulla disponibilità nelle righe mostrano la disponibilità totale di tutti gli articoli sotto l'articolo principale. Le cifre vengono visualizzate nel campo **Quantità disponibile** e lo stato attivo è sull'articolo principale. Tuttavia, le informazioni relative al numero di sottoassemblaggi che è possibile preparare potrebbero essere distorte. Per ottenere un'indicazione vera di quanti dei sottoassemblaggi mostrati è possibile preparare, è necessario cancellare il campo **Mostra disponibilità totale**, quindi visualizzare la cifra nel campo **Produzione possibile - Padre**.

Il campo **Collo di bottiglia** specifica quale articolo nella struttura di DB limita la possibilità di produrre una quantità maggiore di quella indicata nel campo **Produzione possibile - Articolo principale**. Ad esempio, l'articolo collo di bottiglia può essere un componente acquistato con una data di carico prevista troppo in ritardo per creare unità aggiuntive dell'articolo principale entro la data presente nel campo **Disponibile entro**.

## <a name="see-also"></a>Vedi anche
[Gestire i costi del magazzino](inventory-manage-inventory.md)  
[Procedura: Utilizzare le distinte base](inventory-how-work-BOMs.md)    
[Procedura: Impostare le ubicazioni](inventory-how-setup-locations.md)  
[Procedura: Trasferire il magazzino tra le ubicazioni](inventory-how-transfer-between-locations.md)  
[Procedura: Vendere prodotti](sales-how-sell-products.md)      
[Catena di approvvigionamento](madeira-supply-chain.md)  
[Utilizzo di dati finanziari](ui-work-product.md)  
[Funzionalità aziendali generali](ui-across-business-areas.md)
