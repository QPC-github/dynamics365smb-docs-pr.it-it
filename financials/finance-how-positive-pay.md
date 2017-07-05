---
title: 'Procedura: Esportare file Positive Pay | Documenti Microsoft'
description: Descrive come assicurarsi che la banca compensi solo gli assegni e gli importi convalidati tramite l&quot;esportazione di file Positive Pay che contengano informazioni sul fornitore e pagamento.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: check, clearing
ms.date: 03/24/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: ee93f8eb889ae1d635bca22ff133e1523fd1b825
ms.contentlocale: it-it
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-export-a-positive-pay-file"></a>Procedura: Esportare un file Positive Pay
Per assicurarsi che la banca compensi solo gli assegni e gli importi convalidati, è possibile esportare un file Positive Pay con informazioni su fornitore, numero di assegno e importo del pagamento da inviare alla banca per riferimento quando si elaborano i pagamenti.

[!INCLUDE[d365fin](includes/d365fin_md.md)] è preconfigurato per supportare i file Positive Pay per Bank of America e City Bank.

## <a name="to-set-up-a-bank-account-for-positive-pay"></a>Per impostare un conto bancario per i file Positive Pay
1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Conti Correnti Bancari**, quindi scegliere il collegamento correlato.
2. Aprire la scheda della banca per cui si desidera utilizzare il Positive Pay.
3. Nel campo **Codice esportazione Positive Pay** immettere POSPAYBANK.
4. Chiudere la finestra.

## <a name="to-export-a-positive-pay-file"></a>Per esportare un file Positive Pay
1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Conti Correnti Bancari**, quindi scegliere il collegamento correlato.
2. Selezionare il conto bancario per cui si desidera esportare un file Positive Pay.
3. Scegliere l'opzione **Esportazione Positive Pay**.

    Verrà visualizzata la finestra **Esportazione Positive Pay** che mostra i pagamenti che sono stati effettuati per il conto bancario dalla data dell'ultimo caricamento, come mostrato nei campi **Data ultimo caricamento** e **Data ultimo caricamento**.
4. Nel campo **Data limite caricamento** specificare una data prima della quale i pagamenti non sono inclusi nel file esportato.
5. Scegliere l'azione **Esporta**.
6. Nella finestra **Esporta file** scegliere il pulsante **Salva**, quindi salvare il file in un percorso appropriato.
7. Caricare il file nel sito elettronico della banca.
8. Annotare o copiare il numero di conferma visualizzato quando il file viene caricato.

Per visualizzare i record Positive Pay esportati

1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Conti Correnti Bancari**, quindi scegliere il collegamento correlato.
2. Selezionare il conto bancario per cui si desidera visualizzare i record di esportazione Positive Pay.
3. Scegliere l'azione **Movimenti Positive Pay**.

    Nella finestra **Movimenti Positive Pay** è possibile visualizzare tutti i record di esportazione Positive Pay per il conto corrente bancario.
4. Nel campo **Numero di conferma** immettere per ogni record esportare il numero di conferma che si riceve quando il caricamento del file alla banca è riuscito.
5. Per visualizzare le righe di pagamento, scegliere l'azione **Dettagli movimenti Positive Pay**.

Per riesportare file Positive Pay

1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Conti Correnti Bancari**, quindi scegliere il collegamento correlato.
2. Selezionare il conto bancario per cui si desidera riesportare i file Positive Pay.
3. Scegliere l'azione **Movimenti Positive Pay**.
4. Selezionare la riga per il file di esportazione Positive Pay da riesportare.
5. Nella finestra **Movimenti Positive Pay** selezionare l'azione **Riesporta Positive Pay su file**.

## <a name="see-also"></a>Vedi anche
[Finanza](finance.md)  
[Impostazione di dati finanziari](finance-setup-finance.md)  
[Procedura: Utilizzare le registrazioni di contabilità generale](ui-work-general-journals.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
