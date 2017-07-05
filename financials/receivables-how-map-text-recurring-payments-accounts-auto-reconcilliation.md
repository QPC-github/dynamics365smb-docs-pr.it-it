---
title: 'Procedura: Mappare il testo nei pagamenti ricorrenti a conti per la riconciliazione automatica | Documenti Microsoft'
description: 'Procedura: Mappatura del testo nei pagamenti ricorrenti a conti per la riconciliazione automatica'
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account linking, direct payment posting, automatic payment processing, reconcile payment, recurring expense, recurring cash receipt
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 7c6f79959027625a33961d42abe26514bc94e81e
ms.contentlocale: it-it
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-map-text-on-recurring-payments-to-accounts-for-automatic-reconciliation"></a>Procedura: Mappatura del testo nei pagamenti ricorrenti a conti per la riconciliazione automatica
Nella finestra **Mappatura testo a conto** che si apre dalla finestra **Registrazione riconciliazione pagamenti**, è possibile impostare le mappature tra il testo sui pagamenti e specifici conti debiti, crediti e contropartita in modo da registrare questi pagamenti nei conti specificati durante la registrazione della riconciliazione pagamenti.

**Nota**: l'argomento si applica anche quando si utilizza la funzione **Mappa testo a conto** da un record del documento in entrata per agevolare la conversione dei documenti elettronici ricevuti dai servizi esterni in documenti in [!INCLUDE[d365fin](includes/d365fin_md.md)]. Per ulteriori informazioni, vedere [Procedura: Utilizzare OCR per convertire PDF e file di immagine in documenti elettronici](across-how-use-ocr-pdf-images-files.md).   

Una funzionalità simile esiste per riconciliare gli importi in eccesso nelle righe di riconciliazione pagamenti su base ad hoc. Per ulteriori informazioni, vedere [Procedura: Riconciliare i pagamenti che non possono essere collegati automaticamente](receivables-how-reconcile-payments-cannot-apply-auto.md).

I pagamenti registrati in base alla mappa testo a conto non vengono collegati ai movimenti aperti, ma vengono solo registrati nei conti specificati, oltre alla creazione dei movimenti contabili di conti correnti bancari. Di conseguenza, la mappa testo a conto è adatta a incassi e spese ricorrenti, ad esempio acquisti frequenti di combustibile per auto o interessi e oneri bancari, che vengono riportati regolarmente sul rendiconto bancario e non necessitano di un documento commerciale collegato. Per ulteriori informazioni, vedere la sezione “Esempio: mappatura testo a conto per la spesa di combustibile” in questo argomento.

**Nota**: i pagamenti nelle righe di registrazione riconciliazione vengono impostati per essere registrati solo in base alla mappatura testo a conto, se la funzione di collegamento automatico può fornire solo un'affidabilità di corrispondenza **Bassa** o **Media**. Se la funzione di collegamento automatico fornisce un'affidabilità di corrispondenza Alta, il pagamento viene automaticamente collegato a uno o più movimenti e non viene contabilizzato nei conti specificati nella finestra **Mappatura testo a conto**. In altre parole, un'affidabilità di corrispondenza di valore **Alto** oltrepassa una mappa testo a conto.

In una riga di registrazione riconciliazione pagamenti dove il pagamento è stato impostato per la registrazione in base alla mappatura testo a conto, il campo **Affidabilità corrispondenza** contiene **Alta - Mappatura testo a conto** e i campi **Tipo conto** e **Nr. conto** contengono i conti mappati.

## <a name="to-map-text-on-recurring-payments-to-accounts-for-automatic-reconciliation"></a>Mappare il testo nei pagamenti ricorrenti a conti per la riconciliazione automatica
1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Registrazioni riconciliazione pagamenti**, quindi scegliere il collegamento correlato.
2. Aprire una registrazione della riconciliazione di pagamento. Per ulteriori informazioni, vedere [Procedura: Riconciliare i pagamenti utilizzando il collegamento automatico](receivables-how-reconcile-payments-auto-application.md).
3. Scegliere l'azione **Mappa testo a conto**. Verrà aperta la finestra **Mappatura testo a conto**.
4. Nel campo **Mapping testo** immettere qualsiasi testo che appare nei pagamenti da registrare in specifici conti senza collegamento a un movimento aperto. È possibile immettere fino a 50 caratteri.

    **Nota**: se nessun altro pagamento o documento in entrata esiste con il testo di mappatura in questione, la mappatura da testo a conto si verifica anche quando solo una parte del testo nel pagamento o nel documento in entrata esiste come testo di mappatura.
5. Nel campo **Nr. fornitore** immettere il fornitore per cui vengono creati i documenti in entrata contenenti il testo di mappatura o vengono registrati i pagamenti. Per ulteriori informazioni, vedere [Procedura: Utilizzare OCR per convertire PDF e file di immagine in documenti elettronici](across-how-use-ocr-pdf-images-files.md).      
6. Nel campo **Nr. conto dare** immettere il conto nel quale verranno registrati i pagamenti che contengono la mappatura testo se sono pagamenti in entrata. Per i pagamenti in entrata, il segno del valore nel campo **Importo estratto conto** è positivo.
7. Nel campo **Nr. conto avere** immettere il conto nel quale verranno registrati i pagamenti che contengono la mappatura testo se sono pagamenti in uscita. Per i pagamenti in uscita, il segno del valore nel campo **Importo estratto conto** è negativo.
8. Nel campo **Tipo di origine saldo** specificare se il pagamento viene registrato in un conto di contabilità generale o in un conto relativo a un cliente o un fornitore.
9. Nel campo **Nr. origine saldo** specificare il conto in cui il pagamento viene registrato, a seconda della selezione del campo **Tipo di origine saldo** .
10. Ripetere i passaggi da 4 a 8 per tutto il testo presente nei pagamenti che si desidera mappare agli account per la registrazione diretta senza collegamento.

La volta successiva che si importa un file di rendiconto bancario o si sceglie l'azione **Collega automaticamente** nella finestra **Registrazioni riconciliazione pagamenti**, le righe di registrazione dei pagamenti che contengono il testo di mappatura specificato conterranno i conti mappati nei campi **Tipo conto** e **Nr. conto** . Il campo **Affidabilità corrispondenza** conterrà **Alta - Mappatura testo a conto**. Ciò a condizione che la funzione di collegamento automatico possa fornire solo un'affidabilità di corrispondenza di livello **Basso** o **Medio**.

## <a name="example-text-to-account-mapping-for-fuel-expense"></a>Esempio: mappatura testo a conto per la spesa di combustibile
Per registrare sempre le spese in combustibile effettuate presso i distributori Shell nella contabilità generale per la benzina (conto 8510), compilare una riga nella finestra **Mappatura testo a conto** come indicato di seguito.

| Mapping testo | Nr. conto dare | Nr. conto avere | Tipo di origine saldo | Tipo di origine saldo |
| --- | --- | --- | --- | --- |
| Shell |VUOTO |8510 |Conto C/G |VUOTO |

**Suggerimento**: per ulteriori informazioni sull'utilizzo dei campi e delle colonne, vedere [Utilizzo di [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md). Per ulteriori informazioni su come trovare pagine specifiche, vedere [Ricerca](ui-search.md).

## <a name="see-also"></a>Vedi anche
[Gestione della contabilità clienti](receivables-manage-receivables.md)  
[Vendite](sales-manage-sales.md)  
[Procedura: Impostare il servizio Feed bancari di Envestnet Yodlee](bank-how-setup-bank-statement-service.md)  
[Personalizzazione di [!INCLUDE[d365fin](includes/d365fin_md.md)] utilizzando le estensioni](ui-extensions.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
