---
title: 'Procedura: Monitorare lo stato di avanzamento e le prestazioni delle commesse | Documenti Microsoft'
description: Viene descritto come gestire il budget per le commesse.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, KPI, work in process, work in progress
ms.date: 03/28/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: fb38a02bbf2dd99ce003d23c4a5f88f0e3cd593a
ms.contentlocale: it-it
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-monitor-job-progress-and-performance"></a>Procedura: Monitorare lo stato di avanzamento e le prestazioni delle commesse
Durante lo svolgimento di una commessa, vengono consumati materiali, risorse ed effettuate altre spese che devono essere registrate nella commessa. La funzionalità WIP (Work in Process) consente di stimare il valore finanziario delle commesse nella contabilità generale nelle varie fasi di una commessa. In molti casi è possibile registrare le spese relative a una commessa prima di fatturarla. Se sono state registrate solo le spese, il rendiconto finanziario non sarà accurato. Per ulteriori informazioni, vedere [Metodi WIP](projects-understanding-wip.md).

Per tenere traccia del valore nella contabilità generale, è possibile calcolare il WIP e registrare il valore nella contabilità generale.

È possibile calcolare il WIP sulla base dei seguenti fattori:

* Valore costo
* Valore vendite
* Costo riconoscibile
* Percentuale di completamento
* Contratto completato

Se si desidera visualizzare il risultato utilizzando un metodo diverso, è possibile cambiare il metodo e ricalcolare il WIP. È possibile calcolare il WIP senza limitazioni. Il WIP viene solo calcolato ma non registrato nella contabilità generale. Dopo aver calcolato il WIP, è possibile effettuare la registrazione nella contabilità generale.

## <a name="to-create-a-job-wip-method"></a>Per creare un metodo WIP commessa
È possibile creare un metodo WIP commessa che corrisponda alle esigenze dell'organizzazione. Dopo averlo creato, è possibile impostarlo come metodo di default di calcolo del WIP commessa da utilizzare nella propria organizzazione.  

**Nota**. Dopo aver utilizzato il nuovo metodo per creare movimenti WIP, non è possibile eliminare il metodo o modificarlo.  

1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Metodi WIP commessa**, quindi scegliere il collegamento correlato.  
2. Scegliere l'azione **Nuovo** e compilare i campi necessari. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. Chiudere la finestra.   
4. Per impostare il nuovo metodo come default, nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Setup commesse**, quindi scegliere il collegamento correlato.  
5. Nel campo **Metodo WIP di default** , selezionare il metodo dall'elenco.

## <a name="to-define-a-wip-method-for-a-job"></a>Per definire un metodo WIP per una commessa
Quando si crea una nuova commessa, è necessario specificare il metodo WIP commessa da applicare. In alcuni casi, il metodo WIP commessa che è possibile utilizzare viene impostata automaticamente come default.

1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Commesse**, quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Nuovo**. Per ulteriori informazioni, vedere [Procedura: Creare commesse](projects-how-create-jobs.md).  
3. Nella finestra **Scheda commessa**, nel campo **Metodo WIP**, selezionare un metodo WIP dall'elenco. Se è stato definito un metodo di default, è possibile selezionare un'altra opzione, se necessario.  

## <a name="to-calculate-wip"></a>Per calcolare il WIP
È possibile determinare l'importo WIP che deve essere registrato per i conti patrimoniali per il reporting di fine periodo. A tale scopo, utilizzare il processo batch **Commessa - Calcola WIP**.  

1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Commessa - Calcola WIP**, quindi scegliere il collegamento correlato.  
2. Scegliere l'azione **Calcola WIP**.
3. Nella finestra **Commessa - Calcola WIP** compilare i campi in base alle esigenze.
4. Scegliere il pulsante **OK**.  

**Nota**: il processo batch consente di calcolare il WIP. ma non registrato nella contabilità generale. A tale scopo, è necessario eseguire il processo batch **Registra WIP in C/G** dopo avere calcolato il WIP. Per ulteriori informazioni, vedere la seguente procedura.

## <a name="to-post-wip"></a>Per registrare il WIP
Dopo avere calcolato il WIP, è possibile registrarlo nei conti patrimoniali per il reporting di fine periodo. A tale scopo, utilizzare il processo batch **Commessa - Registra WIP in C/G**.

1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Commessa - Registra WIP in C/G**, quindi scegliere il collegamento correlato.  
2. Nella finestra **Commessa - Registra WIP in C/G** compilare i campi in base alle esigenze.  
3. Scegliere il pulsante **OK**.

## <a name="to-view-job-usage-estimates-and-post-updates"></a>Per visualizzare le stime di utilizzo della commessa e gli aggiornamenti della registrazione
È possibile visualizzare l'utilizzo della commessa fino al completamento di un progetto in un unico passaggio. A questo scopo, utilizzare il processo batch **Commessa - Calc. utilizzo residuo** per tutti i task fino al termine della commessa incluso.  

In questo modo è possibile tenere traccia e confrontare le stime iniziali rispetto ai risultati effettivi ed apportare modifiche o creare nuovi movimenti in base alle esigenze. Ad esempio, è possibile che si sia stimato che una commessa richieda 10 ore e ad oggi siano state impiegate 15 ore. È possibile aggiungere le cinque ore in più nella riga di registrazione esistente o creare una nuova riga registrazioni per indicare le cinque ore come straordinario, ovvero un altro tipo di lavoro. Vengono calcolati il costo e il prezzo appropriati ed è quindi possibile contabilizzarli nella registrazione.  

**Nota**: i movimenti articoli creano movimenti contabili articoli e riducono la quantità di inventario. Il processo batch **Registra costo magazzino in C/GL** trasferisce il costo dal magazzino alla contabilità generale. I movimenti risorse creano movimenti contabili risorse.  

1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Reg. commesse**, quindi scegliere il collegamento correlato.  
2. Selezionare una registrazione commessa corrispondente, quindi scegliere l'azione **Calc. utilizzo residuo**.  
3. Nella finestra **Commessa - Calc. utilizzo residuo**, immettere il numero di documento e la data di registrazione che deve essere inserita nelle registrazioni, quindi scegliere **OK**.  
4. Aggiornare le registrazioni con tutte le necessarie modifiche.  
5. Scegliere **Registra**.

## <a name="to-view-job-ledger-entries"></a>Per visualizzare i movimenti contabili commesse
Tutti i movimenti correlati a una commessa vengono annotati nei registri commesse e numerati in sequenza a partire da 1. Dal registro commesse è possibile ottenere una panoramica di tutti i movimenti contabili della commessa.    

1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Registri commesse**, quindi scegliere il collegamento correlato.
2. Selezionare un registro appropriato quindi scegliere l'azione **Movimenti commesse**.

Nella finestra **Movimenti cont. commesse** è possibile esaminare le voci associate a qualsiasi commessa.  

## <a name="see-also"></a>Vedi anche
[Gestire progetti](projects-manage-projects.md)  
[Finanza](finance.md)  
[Acquisti](purchasing-manage-purchasing.md)         
[Vendite](sales-manage-sales.md)      
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
