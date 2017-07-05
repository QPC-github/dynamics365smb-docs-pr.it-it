---
title: Effettuare i pagamenti | Documenti Microsoft
description: Effettuare i pagamenti
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, vendor payment, creditor, debt, balance due, AP
ms.date: 03/28/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: f6721c0359b4499a597b349a280afb56818a1f28
ms.contentlocale: it-it
ms.lasthandoff: 05/04/2017


---
# <a name="make-payments"></a>Effettuare i pagamenti
Quando si eseguono i pagamenti ai fornitori, si registrano le relative righe di pagamento nella finestra **Registrazioni pagamenti**. Per individuare i pagamenti in scadenza, è possibile utilizzare la funzione **Sugg. pagamenti fornitore**. È inoltre possibile utilizzare il report **Fornitori - Scadenziario riepilogativo** per avere una panoramica dei pagamenti in scadenza.

Dalle registrazioni pagamenti è possibile stampare assegni automatici o registrare l'emissione degli assegni. Se si seleziona **Assegno automatico** nel campo **Tipo pagamento banca**, tutte le righe che rappresentano assegni devono essere stampate prima che le registrazioni pagamenti possano essere contabilizzate.

Quando si registrano i pagamenti, è possibile esportarli in un file della banca da caricare nella banca per l'elaborazione.

Una volta effettuati i pagamenti presso la banca, è necessario collegarli ai relativi movimenti contabili fornitori aperti. Questa operazione può essere eseguita manualmente o importando un file del rendiconto bancario e collegando i pagamenti automaticamente. Per ulteriori informazioni, vedere [Collegare i pagamenti automaticamente e Riconciliazione dei conti correnti bancari](receivables-apply-payments-auto-reconcile-bank-accounts.md).

Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.

| Per | Vedere |
| --- | --- |
| Utilizzare una funzione per suggerire i pagamenti fornitore in base ai criteri selezionati, ad esempio la data di scadenza, l'idoneità allo sconto e la liquidità. |[Procedura: Suggerire i pagamenti ai fornitori](payables-how-suggest-vendor-payments.md) |
| Emettere assegni per i pagamenti, come stampati o come assegni automatici. Annullare gli assegni prima o dopo la registrazione. |[Procedura: Utilizzare gli assegni](payables-how-work-checks.md) |
| Assicurarsi che la banca compensi solo gli assegni e gli importi convalidati inviandole un file che contenga informazioni sul fornitore, l'assegno e il pagamento. |[Procedura: Esportare un file Positive Pay](finance-how-positive-pay.md) |
|Esportare i pagamenti dalla finestra **Registrazioni pagamenti** a un file della banca che viene caricato nella banca per l'elaborazione, incluso l'EFT (trasferimento elettronico di fondi) nell'America del Nord. |[Procedura: Esportare pagamenti in un file della banca](payables-how-export-payments-bank-file.md)|  

## <a name="see-also"></a>Vedi anche
[Gestione della contabilità fornitori](payables-manage-payables.md)  
[Acquisti](purchasing-manage-purchasing.md)  
[Gestione della contabilità clienti](receivables-manage-receivables.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
