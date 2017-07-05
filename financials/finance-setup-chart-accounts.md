---
title: Impostazione del piano dei conti | Documenti Microsoft
description: "Viene descritto come è modificare il piano dei conti."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: COA, cha of acc
ms.date: 03/28/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 48202a9e9a763dcb22bed9975aa9c4a39d2dc4ae
ms.contentlocale: it-it
ms.lasthandoff: 05/04/2017


---
# <a name="setting-up-or-changing-the-chart-of-accounts"></a>Impostazione o modifica del piano dei conti
Il piano dei conti mostra i conti di contabilità che memorizzano i dati finanziari. [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)] include un piano dei conti standard pronto per supportare l'azienda.
Tuttavia, è possibile modificare i conti predefinti ed è possibile aggiungere nuovi conti.  

## <a name="adding-or-changing-accounts"></a>Aggiungere o modificare i conti
Nel piano dei conti, è possibile aprire ogni conto C/G e aggiungere o modificare le impostazioni.

**Nota**: è possibile eliminare un conto di contabilità generale. Tuttavia, prima che venga eliminato, è necessario soddisfare le seguenti condizioni:  

* Il saldo nel conto deve essere pari a zero.  
* Nel campo **Consenti Eliminaz. Conti C/G Anteriori a** della finestra **Setup Contabilità Generale** deve essere impostata una data ed è necessario che il conto non includa movimenti contabili in tale data o dopo tale data.  
* Se il campo **Verifica Uso Conti C/G** della finestra **Setup Contabilità Generale** è selezionato, il conto non deve essere utilizzato in tutte le categorie di registrazione o impostazioni delle registrazioni.  

[!INCLUDE[d365fin](includes/d365fin_md.md)] impedirà di eliminare un conto di contabilità generale che memorizza i dati necessari per il piano dei conti.  

## <a name="see-also"></a>Vedi anche
[Contabilità generale e piano dei conti](finance-general-ledger.md)  
[Gestione di conti correnti bancari](bank-manage-bank-accounts.md)  
[Dimensioni](finance-dimensions.md)  
[Importazione dei dati da altri sistemi contabili](upload-data.md)  
[Procedura: Utilizzare i codici GIFI in Canada](ca-finance-work-gifi-codes.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]