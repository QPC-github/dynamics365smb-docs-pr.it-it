---
title: 'Procedura: Utilizzare le distinte base | Documenti Microsoft'
description: "I DB di assemblaggio specificano quali componenti risorse sono obbligatori per assemblare l&quot;articolo di assemblaggio che rappresenta la DB di assemblaggio. Le DB assemblaggio in genere contengono articoli ma possono anche contenere una o più risorse che eseguono le attività di assemblaggio."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 05/06/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: ce75a9d292e12c58efc51c4db2fbc5a37b7553c7
ms.openlocfilehash: f55dcf4b391ae42ab46a22b729597a96645d9b71
ms.contentlocale: it-it
ms.lasthandoff: 05/05/2017


---
# <a name="how-to-work-with-bills-of-materials"></a>Procedura: Utilizzare le distinte base
**Nota**: la versione corrente di [!INCLUDE[d365fin](includes/d365fin_md.md)] contiene solo la prima parte della funzionalità di gestione assemblaggio. Per ora, è possibile creare solo le DB di assemblaggio e quindi gestire gli articoli padre correlati come articoli di inventario normali. In un aggiornamento futuro, è possibile gestire l'assemblaggio effettivo di articoli dai componenti, sia in flussi di assemblaggio per magazzino che di assemblaggio su ordine, quindi vendere i componenti come kit.

Utilizzare le distinte base (DB) per strutturare gli articoli padre da vendere come kit costituiti da componenti del padre o da assemblare su ordine o per magazzino.

In [!INCLUDE[d365fin](includes/d365fin_md.md)], una distinta base è detta "DB assemblaggio". La DB assemblaggio specifica i componenti contenuti in articoli padre. In questa documentazione, un articolo padre è detto "articolo di assemblaggio".

Le DB assemblaggio in genere contengono articoli ma possono anche contenere una o più risorse richieste per l'assemblaggio dell'articolo.

Le DB assemblaggio possono essere multilivello, cioè un componente della DB assemblaggio può essere un articolo di assemblaggio esso stesso. In tal caso, il campo **DB assemblaggio** nella riga della DB assemblaggio contiene il valore **Sì**.

Requisiti speciali si applicano agli articoli nelle DB assemblaggio correlati alla disponibilità. Per ulteriori informazioni, vedere la sezione "Per visualizzare la disponibilità di un articolo per l'utilizzo in DB di assemblaggio" in [Procedura: Ottenere una panoramica della disponibilità](inventory-how-availability-overview.md).

**Nota**: questa funzionalità richiede che l'esperienza sia impostata su ***** Suite *****. Per ulteriori informazioni, vedere [Personalizzazione dell'esperienza utente di Financials](ui-experiences.md).

## <a name="to-create-an-assembly-bom"></a>Per creare una DB assemblaggio
Per definire un articolo padre composto da altri articoli e potenzialmente da risorse richieste per l'assemblaggio, è necessario creare una DB assemblaggio.  

Esistono due passaggi per creare una DB assemblaggio:
- Impostazione di un nuovo articolo
- Definizione della struttura della distinta base dell'articolo di assemblaggio.

1. Impostare un nuovo articolo. Per ulteriori informazioni, vedere [Procedura: Registrare nuovi articoli](inventory-how-register-new-items.md).

    Continuare a inserire componenti o risorse nella distinta base assemblaggio.  
2. Nella finestra **Scheda articolo** per un articolo di assemblaggio, scegliere l'azione **Assembla** quindi l'azione **DB assemblaggio**.
3. Nella finestra **DB assemblaggio** compilare i campi secondo le proprie necessità. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-view-the-components-of-an-assembly-item-indented-according-to-the-bom-structure"></a>Per visualizzare i componenti di un articolo di assemblaggio con indentazione in base alla struttura DB
Nella finestra **DB assemblaggio**, è possibile aprire una finestra distinta in cui vengono visualizzati i componenti e tutte le risorse indentate in base alla posizione nella distinta base dell'articolo di assemblaggio.

1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), inserire **Articoli**, quindi scegliere il collegamento correlato.
2. Aprire la finestra della scheda per l'articolo di assemblaggio. (Il campo **DB assemblaggio** nella finestra **Articoli** contiene il valore **Sì**.)
3. Nella finestra **Scheda articolo** scegliere l'azione **Assembla** quindi l'azione **DB assemblaggio**.
4. Nella finestra **DB assemblaggio** selezionare l'azione **Mostra DB**.

## <a name="to-buy-sell-or-transfer-assembly-items"></a>Per acquistare, vendere o trasferire gli articoli di assemblaggio
Poiché la versione corrente di [!INCLUDE[d365fin](includes/d365fin_md.md)] contiene solo la funzionalità per definire e assegnare le DB di assemblaggio agli articoli, è possibile gestire gli articoli di assemblaggio nelle righe dei documenti solo come articoli normali.

**Avvertenza**: la quantità di magazzino dei componenti della DB non verrà rettificata se si esegue questa operazione.

## <a name="see-also"></a>Vedi anche
[Procedura: Registrare nuovi articoli](inventory-how-register-new-items.md)  
[Procedura: Ottenere una panoramica della disponibilità](inventory-how-availability-overview.md)     
[Magazzino](inventory-manage-inventory.md)  
[Utilizzo di [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](ui-work-product.md)
