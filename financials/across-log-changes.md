---
title: Registrazioni di modifiche in Dynamics 365 for Financials | Documenti di Microsoft
description: Registrare le modifiche apportate dagli utenti.
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: user log, user activity, tracking
ms.date: 03/04/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 470931febc303ace8fa1e8015453c20b587762b0
ms.contentlocale: it-it
ms.lasthandoff: 05/04/2017


---
# <a name="logging-changes-in-dynamics-365-for-financials"></a>Registrazione di modifiche in Dynamics 365 for Financials
È possibile abilitare il log modifiche in [!INCLUDE[d365fin](includes/d365fin_md.md)] in modo da disporre di uno storico delle attività. Il registro si basa sulle modifiche eseguite ai dati nelle tabelle di cui si tiene traccia. Nel log modifiche, i movimenti vengono ordinati cronologicamente e mostrano le modifiche apportate nei campi delle tabelle specificate. Il log modifiche raccoglie tutte le modifiche apportate alla tabella.  

## <a name="working-with-the-change-log"></a>Utilizzo del log modifiche
Un problema comune in diversi sistemi finanziari è individuare l'origine degli errori e delle modifiche dei dati. Potrebbe trattarsi di un numero di telefono errato del cliente o di una registrazione errata nella contabilità generale. Il log modifiche consente di tenere traccia di tutte le modifiche dirette apportate da un utente ai dati nel database. È necessario specificare cosa si desidera venga registrato per ciascuna tabella e campo, quindi attivare il log modifiche.  

Il log modifiche viene attivato e disattivato nella finestra **Setup log modifiche**. Quando si attiva o disattiva il log modifiche, questa attività viene registrata, in modo da poter visualizzare sempre quale utente ha disattivato o riattivato il log modifiche. Non è possibile disattivare tale funzione.  

Nella finestra **Setup log modifiche**, scegliendo l'azione **Tabelle**, è possibile specificare le tabelle di cui si desidera tenere traccia delle modifiche e le modifiche di cui tenere traccia. [!INCLUDE[d365fin](includes/d365fin_md.md)] traccia anche una serie di tabelle del sistema.

Dopo avere impostato e attivato il log modifiche e apportato una modifica ai dati, è possibile visualizzare e filtrare le modifiche nella finestra **Movimenti log modifiche**. Se si desidera rimuovere i movimenti, è possibile farlo nella finestra **Elimina mov. log modifiche**, in cui è possibile impostare filtri in base alle date e all'ora.  

## <a name="see-also"></a>Vedi anche
[Modifica delle impostazioni di base](ui-change-basic-settings.md)  
[Ordinamento](ui-sorting.md)  
[Utilizzo della funzionalità Cerca pagina o report](ui-search.md)  
[Procedura: Gestire gli utenti e le autorizzazioni](ui-how-users-permissions.md)    
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
