---
title: "Come impostare più tassi d'interesse"
description: "È possibile calcolare gli addebiti di interessi con più tassi di interesse per un periodo specifico. Il calcolo degli interessi è simile per tutti gli addebiti di interessi, con la sola variazione del tasso di interesse in un periodo specifico."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 12/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 0af01fe46f6b7df1149825c35a9fc0cc19482403
ms.contentlocale: it-it
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-multiple-interest-rates"></a>Impostare più tassi d'interesse
Più tassi di interesse sono utilizzati in periodi differenti per pagamenti in ritardo nelle transazioni commerciali. Ad esempio, un governo specifica il tasso di interesse massimo da imporre ai consumatori. Questo tasso di interesse può essere modificato due volte all'anno, il 1° gennaio e il 1° luglio. Il tasso di interesse tra le aziende (B2B) è concordato tra le parti e non è soggetto ad alcun limite. Il tasso annunciato è in genere superiore del quattro per cento all'interesse bancario normale.

Quando si creano le condizioni di addebito degli interessi e i termini di sollecito, per la penalità di pagamento ritardato, è possibile specificare più tassi di interesse in modo che la penalità sia calcolata in base a tassi di interesse differenti in diversi periodi. Per ulteriori informazioni, vedere [Riscuotere i saldi inevasi](receivables-collect-outstanding-balances.md).

## <a name="to-set-up-multiple-interest-rates"></a>Per impostare più tassi d'interesse  
1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Condiz. interessi finanziari**, quindi scegliere il collegamento correlato.  
2.  Nella finestra **Condiz. interessi finanziari**, selezionare le condizioni di addebito, quindi scegliere l'azione **Tassi di interesse**.  
3.  Compilare i campi come necessario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  Scegliere il pulsante **OK**.  
5.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Termini di sollecito**, quindi scegliere il collegamento correlato.  
6.  Nella finestra **Termini di sollecito**, selezionare i termini di sollecito, quindi scegliere l'azione **Livelli**.  
7.  Nella finestra **Livelli di sollecito**, selezionare il campo **Interessi calcolati**.  

Quando si emette una nota di addebito interessi, la nota mostra gli addebiti di interessi con più tassi di interesse per un periodo di tempo specifico. La nota contiene anche dettagli relativi a contatti del cliente, società che ha emesso la nota, importo addizionale e importo totale. Il movimento di apertura nella nota è visualizzato in grassetto. Gli addebiti di interessi sono calcolati con più tassi di interesse per un periodo di tempo specifico e vengono stampati dopo il movimento di apertura della nota.  

## <a name="see-also"></a>Vedi anche  
[Riscuotere i saldi inevasi](receivables-collect-outstanding-balances.md)  
[Impostazione di dati finanziari](finance-setup-finance.md)
