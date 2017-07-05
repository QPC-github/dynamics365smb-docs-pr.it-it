---
title: Impostazioni delle relazioni d&quot;affari per i contatti | Documenti Microsoft
description: Descrive le relazioni d&quot;affari per i contatti in Financials
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: marketing, prospect, contact, client, customer
ms.date: 03/28/2017
ms.author: jswymer
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: f6719ac45f298d6c952427c871eaf818cb7480c3
ms.contentlocale: it-it
ms.lasthandoff: 05/04/2017


---
# <a name="setting-up-business-relations-on-contact-companies"></a>Impostazione delle relazioni d'affari nelle società contatto
È possibile utilizzare le relazioni d'affari vengono utilizzate per indicare il tipo di relazione commerciale che intercorre con i contatti, ad esempio potenziale cliente, banca, consulente e fornitore di servizi e così via.

L'utilizzo delle relazioni d'affari nei contatti è un processo a due passaggi. Innanzitutto, occorre definire il codice relazioni d'affari. Questo passaggio deve essere eseguito una sola volta per ogni relazione d'affari. Dopo aver creato un codice di relazione d'affari, è possibile iniziare ad assegnarlo alle società.

**Nota**: se si prede di sincronizzare i contatti con fornitori, clienti o conti correnti bancari in altre sezioni dell'applicazione, è consigliabile impostare una relazione d'affari.

## <a name="to-define-a-business-relation-code"></a>Per definire un codice relazioni d'affari
Il codice relazione d'affari definisce una categoria o un tipo della relazione d'affari, ad esempio BANCA o Legge. È possibile impostare più codici di relazione d'affari. Per definire la relazione d'affari, utilizzare la finestra **Relazioni d'affari**.

1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Relazioni d'affari**, quindi scegliere il collegamento correlato.
2. Selezionare l'azione **Nuovo** e immettere un codice e una descrizione. Il codice può avere un massimo di 11 caratteri e può essere qualsiasi combinazione di numeri o lettere.

## <a name="AssignBusRelContact"></a> Per assegnare relazioni d'affari a un contatto
Non è possibile assegnare relazioni d'affari a un contatto, ma solo alle società.

1. Aprire il contatto.
2. Scegliere l'azione **Società**, quindi l'azione **Relazioni d'affari**.

    Verrà aperta la finestra **Relazioni d'affari contatto**.
3. Nel campo **Codice relazione d'affari** selezionare la relazione d'affari da assegnare.

Ripetere questi passaggi per assegnare altre relazioni d'affari. È inoltre possibile assegnare altre relazioni d'affari dalla lista Contatti seguendo la stessa procedura.

Il numero di relazioni d'affari assegnate al contatto viene visualizzato nel campo **Nr. relazione d'affari** nella sezione **Segmentazione** nella finestra **Contatto**.

Una volta assegnate le relazioni d'affari ai contatti, è possibile utilizzare queste informazioni per selezionare i contatti per i segmenti. Per ulteriori informazioni, vedere [Procedura: aggiungere contatti ai segmenti](marketing-add-contact-segment.md).

## <a name="see-also"></a>Vedi anche
[Creazione di società contatto](marketing-create-contact-companies.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
