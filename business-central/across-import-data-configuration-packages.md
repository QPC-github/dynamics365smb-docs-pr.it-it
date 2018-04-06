---
title: Utilizzare Excel per importare dati in Financials| Documenti Microsoft
description: Utilizzare il pacchetto di configurazione di default per aggiungere i dati del cliente in Excel e importare nuovamente i dati in Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: migration, Excel
ms.date: 03/07/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 4526e8b11c9cbae36c7db58259499fbfa1b0c243
ms.contentlocale: it-it
ms.lasthandoff: 03/22/2018

---
# <a name="importing-data-from-legacy-accounting-software-using-a-configuration-package"></a>Importazione di dati del software di contabilizzazione legacy utilizzando un pacchetto di configurazione
È possibile importare dati master e alcuni dati transazionali da altri sistemi finanziari in base al pacchetto di configurazione standard disponibile in [!INCLUDE[d365fin](includes/d365fin_md.md)]. Nella finestra **Pacchetti di configurazione** è possibile utilizzare il pacchetto per importare e convalidare i dati prima di applicare il pacchetto.  

> [!NOTE]  
> I pacchetti di configurazione fanno parte di RapidStart Services per [!INCLUDE[d365fin](includes/d365fin_md.md)], un toolkit completo per la configurazione di nuove soluzioni basate sui requisiti aziendali dei clienti e sui dati di setup. RapidStart Services offre anche la funzionalità per l'importazione di dati legacy. Per ulteriori informazioni, vedere [Impostare una società con RapidStart Services](admin-set-up-a-company-with-rapidstart.md).

> [!TIP]  
>   In alternativa, usare le procedure guidate di migrazione dati per importare i dati da QuickBooks o Dynamics GP. Per ulteriori informazioni, vedere [Migrazione dei dati di QuickBooks](ui-extensions-quickbooks-data-migration.md) o [Migrazione dei dati di Dynamics GP](ui-extensions-dynamicsgp-data-migration.md).  

## <a name="working-with-data-in-excel"></a>Utilizzo di dati in Excel
Quando si esporta il pacchetto di configurazione di default in Excel, la cartella di lavoro generata contiene un prospetto per ogni tabella del pacchetto. Per semplificare i task, è possibile avvantaggiarsi degli strumenti di modifica XML incorporati in Excel. È inoltre possibile utilizzare le funzioni incorporate di Excel per agevolare la formattazione dei dati e inserire i dati nella cella appropriata. Ad esempio, aggiungere un prospetto vuoto e copiarvi i dati legacy. Creare quindi una formula Excel per mappare i dati nel prospetto di trasformazione tra i campi del prospetto esportato e i dati legacy del cliente. Dopo aver eseguito la mappatura di tutti i dati, copiare l'intervallo dei dati nel prospetto della tabella.  

> [!IMPORTANT]  
>  Non modificare le colonne nei prospetti. Se vengono spostate, modificate o eliminate, il prospetto non può essere importato in [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="tables-in-the-default-configuration-package"></a>Tabelle nel pacchetto di configurazione di default
Il pacchetto di configurazione di default supporta le seguenti tabelle:

-   Condizioni pagamento
-   Gruppo prezzi cliente
-   Metodo di spedizione
-   Agenti/Addetti acq.
-   Località
-   Conto C/G
-   Cliente
-   Fornitore
-   Articolo
-   Testate vendita
-   Righe vendite
-   Testate acquisti
-   Righe Acquisto
-   Righe registrazioni COGE
-   Righe reg. magazzino
-   Cat. reg. cliente
-   Cat. reg. fornitore
-   Cat. reg. magazzino
-   Unità di misura
-   Cat. reg. business
-   Cat. reg. articoli/servizi
-   Setup registrazioni COGE
-   Regioni
-   Categorie articolo
-   Prezzo vendita
-   Prezzo acquisto

## <a name="importing-customer-data"></a>Importazione di dati dei clienti
Dopo che i dati dei clienti sono stati importati in Excel, vengono importati in [!INCLUDE[d365fin](includes/d365fin_md.md)]. Nella finestra **Pacchetti di configurazione** importare i dati del file Excel. È possibile verificare che i dati siano coerenti con [!INCLUDE[d365fin](includes/d365fin_md.md)] prima di applicare il pacchetto.

## <a name="see-also"></a>Vedi anche
[Importazione dei dati aziendali da altri sistemi contabili](upload-data.md)  
[Impostare una società con RapidStart Services](admin-set-up-a-company-with-rapidstart.md)  
[Migrazione dei dati QuickBooks](ui-extensions-quickbooks-data-migration.md)  
[Migrazione dei dati Dynamics GP](ui-extensions-dynamicsgp-data-migration.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
## [!INCLUDE[d365fin](includes/training_link_md.md)]
