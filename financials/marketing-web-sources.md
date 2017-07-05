---
title: "Impostazione di origini Web per le società contatto | Documenti Microsoft"
description: Viene descritto come utilizzare le origini Web per i contatti in Financials
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: internet
ms.date: 03/28/2017
ms.author: jswymer
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 8a452619aeeee907cf61fd5d1a8fce409ad2e42d
ms.contentlocale: it-it
ms.lasthandoff: 05/04/2017


---
# <a name="setting-up-web-sources-for-contact-companies"></a>Impostazione delle origini Web per le società contatto
È possibile utilizzare le origini Web con le società contatto per identificare, ad esempio, motori di ricerca e siti Web dove effettuare la ricerca di informazioni sui contatti. Quando si assegna un'origine Web, specificare il motore di ricerca e la parola di ricerca che saranno utilizzati per individuare le informazioni richieste.

L'utilizzo delle origini Web nei contatti è un processo a due passaggi. Innanzitutto, occorre definire il codice origine Web. Questo passaggio deve essere eseguito una sola volta per ogni origine Web. Dopo aver creato un codice origine Web, è possibile iniziare ad assegnarlo ai contatti.

## <a name="to-define-a-web-source-code"></a>Per definire un codice origine Web
1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Origini Web**, quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Nuovo**.
3. Compilare i campi **Codice**, **Descrizione** e **URL**.

    Nel campo **URL** immettere %1 per inserire un segnaposto per una parola di ricerca nell'URL. Quando si apre l'origine Web da un contatto, %1 verrà automaticamente sostituito con la parola da ricercare (ad esempio il nome della società) inserita nella finestra **Origini Web contatto**.

Ripetere tali passaggi per impostare altre origini Web.

## <a name="to-assign-web-sources-to-a-contact-company"></a>Per assegnare origini Web a una società contatto
Quando si assegna un'origine Web, specificare il motore di ricerca e la parola di ricerca che saranno utilizzati per individuare le informazioni richieste.

1. Aprire il contatto.
2. Scegliere l'azione **Società**, quindi l'azione **Origini Web**. Verrà visualizzata la finestra **Origine Web contatto**.
3. Nel campo **Codice origine Web** scegliere l'origine Web che si desidera assegnare.
4. Nel campo **Parola ricerca** inserire la parola ricerca che verrà utilizzata per individuare le informazioni.

Ripetere tali passaggi per assegnare altre origini Web.

È inoltre possibile assegnare l'origine Web dalla finestra **Lista contatti** seguendo la stessa procedura.

## <a name="see-also"></a>Vedi anche
[Creazione di società contatto](marketing-create-contact-companies.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
