---
title: Report di contabilità fornitori e analisi
description: Vedi quali report e analisi sono disponibili nella versione standard di Business Central in modo da poter tenere traccia della contabilità fornitori.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: reporting
ms.date: 07/13/2021
ms.author: edupont
ms.openlocfilehash: 774fd24bc15cb4cefb56991289d9c72c0909a319
ms.sourcegitcommit: a486aa1760519c380b8cdc8fdf614bed306b65ea
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/13/2021
ms.locfileid: "6543356"
---
# <a name="accounts-payable-reports-and-analytics-in-business-central"></a>Report di contabilità fornitori e analisi in Business Central

Per aiutarti a gestire la contabilità fornitori in [!INCLUDE [prod_short](includes/prod_short.md)], report standard e analisi sono integrati. Va oltre i tradizionali vincoli di creazione di report per consentire di progettare in modo efficiente vari tipi di report.  

## <a name="reports"></a>Report

La tabella seguente descrive alcuni dei report di contabilità fornitori.

| Report | ID oggetto | Descrizione |
|--|--|--|
| **Scadenziario fornitori** | 322|Mostra i saldi scaduti per i fornitori negli intervalli di tempo scaduti. Gli importi scaduti possono essere visualizzati per data di scadenza, data di registrazione o per data del documento, se necessario. Puoi scegliere di mostrare gli importi in valuta locale (VL) e stampare i dettagli dei documenti scaduti. Gli intervalli di tempo possono avere intestazioni con date o con numero di date scadute, relative allo scadenzario specificato per tipo.<br>Questo report è il report principale per la riconciliazione della contabilità fornitori con la contabilità generale. Supponendo che non sia stata consentita la registrazione diretta nei conti utilizzati nel conto debiti delle categorie di registrazione fornitori, questo report è una specifica degli importi presenti nella contabilità generale.|
| **Fornitore - Saldo alla data** | 321 | Mostra il saldo del fornitore alla data di fine dell'intervallo di date specificato. Puoi scegliere di visualizzare il saldo del fornitore nella tua valuta locale (VL). Seleziona il campo **Includi movimenti scollegati** per mostrare i movimenti che sono stati chiusi entro la data di fine ma non sono stati applicati (aperti) in una data successiva. Seleziona il campo **Mostra movimenti con saldo zero** per mostrare i fornitori con un saldo pari a zero entro la data di fine del filtro data. Il filtro data si applica ai movimenti contabili fornitori dettagliati per i movimenti nel report. Se hai pagamenti successivi alla data di fine che sono stati applicati alle fatture entro l'intervallo di date, le fatture verranno visualizzate nel report in quanto non sono state chiuse entro la data di fine. |
| **Fornitori - Bilancio verifica** | 329 | Mostra i saldi periodi per i fornitori per il periodo specificato nel filtro data, nonché il saldo periodo da inizio anno per l'anno fiscale corrispondente al periodo selezionato. Il report è raggruppato per categorie di registrazione fornitori e fornirà una vista diversa della contabilità fornitori rispetto al report **Scadenziario fornitori**. **Nota**: Se non è stato impostato alcun periodo contabile, il sistema non saprà quale anno fiscale utilizzare e mostrerà l'anno in corso dall'ultimo anno fiscale definito o selezionerà semplicemente il periodo, che può essere o meno dall'inizio di un anno.|
| **Fornitori - Dett. bil. verif.** | 304 | Mostra tutti i movimenti contabili fornitori all'interno del filtro data specificato. Il report mostra i saldi iniziali del fornitore relativi al filtro data. |
| **Statistiche acquisti** |312 |[!INCLUDE [reports-purchase-statistics](includes/reports-purchase-statistics.md)]<br>Questo report può essere utilizzato anche nella contabilità fornitori poiché è più semplice eseguire una rapida ricerca di pagamenti registrati, sconti e altre transazioni per un determinato fornitore.|
|**Fornitori - Scadenzario riepilogativo**|305| Report legacy per lo scadenziario fornitori. Ti consigliamo di utilizzare il report **Scadenziario fornitori**. Puoi scegliere una durata del periodo e una data da utilizzare come data *di scadenza*.|
|**Pagamenti in sospeso**|319|Mostra i movimenti contabili fornitori in cui il campo **In sospeso** non è vuoto.|
|**Registrazioni pagamenti anticipati fornitori**|317|Mostra le registrazioni dei pagamenti con le informazioni sullo sconto di pagamento e sulla tolleranza. Il report può essere utilizzato per controllare i pagamenti prima di creare file di pagamento e registrare il giornale. **Nota**: il report mostrerà gli sconti di pagamento in modo errato quando sono utilizzate più note di credito in un'applicazione. In questo caso, lo sconto di pagamento per le note di credito aggiuntive verrà mostrato come importo non applicato.|
|**Lista fornitori**|301|Mostra varie informazioni di base sui fornitori, quali categorie di registrazione fornitori, sconti e informazioni sui pagamenti, livello di priorità, valuta di default e saldo corrente in VL. Il report può essere utilizzato ad esempio per mantenere le informazioni nella tabella Fornitori.|

## <a name="see-also"></a>Vedere anche

[Analisi dei rendiconti finanziari in Microsoft Excel](finance-analyze-excel.md)  
[Utilizzo delle dimensioni](finance-dimensions.md)  
[Gestione dei cespiti](fa-manage.md)  
[Panoramica delle funzionalità locali](about-localization.md)  
[Esperienze di contabile in [!INCLUDE[prod_long](includes/prod_long.md)]](finance-accounting.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]