---
title: Aggiungere società all'hub aziendale
description: Informazioni su come aggiungere società da altri ambienti Business Central all'hub aziendale in modo da poter gestire il lavoro in più ambienti.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: accountant, accounting, company hub
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 773731ecc860e7d1ea0d13bbf9e6896a746544be
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 10/01/2020
ms.locfileid: "3927696"
---
# <a name="add-companies-to-your-company-hub"></a>Aggiungere società all'hub aziendale

Con l'hub aziendale, è possibile accedere al lavoro da più società di più ambienti [!INCLUDE [prodshort](includes/prodshort.md)]. È possibile aggiungere ambienti e società manualmente, se le società non vengono visualizzate automaticamente nell'hub aziendale.  

Proprio nella pagina di destinazione dell'hub aziendale è disponibile il menu **Setup** da cui è possibile accedere alla pagina **Collegamenti ambiente**. Scegliere **Nuovo** e compilare i campi. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  

## <a name="environment-links"></a>Collegamenti ambiente

Un collegamento ambiente è una scheda in cui è possibile specificare l'ambiente [!INCLUDE [prodshort](includes/prodshort.md)] che ospita una o più società in cui si lavora. I dati della scheda per ciascun ambiente sono specificati dall'utente e possono essere modificati secondo le necessità. Tuttavia, il campo **Collegamento ambiente** è fondamentale, indica come è possibile accedere a [!INCLUDE [prodshort](includes/prodshort.md)] di ogni società. Utilizzare l'azione **Test della connessione** nella barra multifunzione per verificare che sia stato inserito il collegamento corretto. Il collegamento da inserire punta all'ambiente che ospita la società che si sta aggiungendo e deve includere l'ID Azure Active Directory (Azure AD) o il nome di dominio dell'organizzazione. Ad esempio, se è stato specificato un dominio come MyBusiness.com, il collegamento alla soluzione [!INCLUDE [prodshort](includes/prodshort.md)] sarà ```https://businesscentral.dynamics.com/mybusiness.com?redirectedfromsignup=1```. In caso contrario, sarà simile a questo: ```https://businesscentral.dynamics.com/1a23b456-789c-0123-45de-678910fg12h/production?redirectedfromsignup=1```  

Il collegamento viene utilizzato quando si sceglie la società nell'hub della società.  

:::image type="content" source="media/company-hub-company-list-actions.png" alt-text="Azioni per una società elencata nell'hub aziendale":::

> [!TIP]
> Se si sta lavorando nella versione di prova gratuita di [!INCLUDE [prodshort](includes/prodshort.md)], è facile aggiungere le società nel tenant. È possibile trovare il collegamento ambiente copiando l'ID Azure Active Directory dalla sezione **Risoluzione dei problemi** della pagina Guida e supporto. Il nome dell'ambiente è probabilmente il valore predefinito, PRODUZIONE. Aggiungere queste informazioni al campo **Collegamento ambiente**, ad esempio ```https://businesscentral.dynamics.com/1a23b456-789c-0123-45de-678910fg12h/production?redirectedfromsignup=1``` e quindi scegliere **Test della connessione**. La società di valutazione verrà aggiunta all'elenco.
>
> Se si passa alla società di prova di trenta giorni, My Company, è possibile aggiungerla all'elenco scegliendo l'azione **Ricarica/Ricarica tutte le società** nell'elenco.

## <a name="load-companies"></a>Caricare le società

Quando sono stati aggiunti gli ambienti, le società vengono visualizzate automaticamente. Tuttavia, se una nuova società è stata aggiunta a un ambiente, è possibile scegliere l'azione **Ricarica tutte le società** per aggiornare l'elenco. Usare la stessa azione per aggiornare i dati di tutte le società.  

> [!TIP]
> Per aggiornare i dati nell'hub aziendale, è necessario avere accesso ai dati nelle società da cui provengono i dati.

## <a name="see-also"></a>Vedere anche

[Gestire il lavoro tra più aziende nell'hub aziendale](company-hub.md)  
[Risorse per Guida e supporto](product-help-and-support.md)  