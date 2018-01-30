---
title: "Funzionalità multilingue e localizzazione | Microsoft Docs"
description: Informazioni su come lingua e impostazioni locali influenzano l'esperienza utente in Dynamics 365.
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: language, locale, localization, culture
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 94a7a3e1da9f2ac3145f18102f86386cfc980ea5
ms.contentlocale: it-it
ms.lasthandoff: 09/22/2017

---
# <a name="language-and-locale"></a>Lingua e impostazioni locali
[!INCLUDE[d365fin](includes/d365fin_md.md)] è supportato in vari mercati ed è disponibile nelle lingue che tali mercati richiedono. Ciò è il risultato del supporto per molteplici lingue al runtime in combinazione con il supporto per requisiti legali nei mercati supportati. Questo significa che è possibile utilizzare [!INCLUDE[d365fin](includes/d365fin_md.md)] in più lingue. È possibile modificare la lingua utilizzata per visualizzare testi e la modifica viene applicata dopo la prodecura di disconnessione e connessione automatica. L'impostazione è valida solo per l'utente corrente e non per gli altri utenti nella società.  

Ad esempio,per un utente canadese, è possibile visualizzare l'interfaccia utente in inglese e in francese, ma rimane una versione canadese di [!INCLUDE[d365fin](includes/d365fin_md.md)] in tutti gli altri aspetti. È quindi diversa, ad esempio, dalla versione di [!INCLUDE[d365fin](includes/d365fin_md.md)] per il Regno Unito.  

> [!NOTE]  
>  La modifica della lingua non è attualmente supportata in [!INCLUDE[d365fin](includes/d365fin_md.md)].

La modifica dei testi memorizzati come dati dell'applicazione non è invece supportata dalla funzionalità multilingue. Tale modifica rientra nell'ambito della progettazione dell'applicazione. Tra gli esempi di questo tipo di testi rientrano i nomi degli articoli in magazzino o i commenti relativi a un cliente. In altre parole, questi testi non vengono tradotti.  

> [!NOTE]  
>  [!INCLUDE[d365fin](includes/d365fin_md.md)] supporta solo un unico set di caratteri per i dati. Alcuni caratteri, pertanto, potrebbero non essere supportati nel tenant ed è possibile che si verifichino problemi durante il recupero di dati immessi utilizzando un set di caratteri diverso. Ad esempio, il tenant potrebbe supportare solo caratteri inglesi e russi e se si immettono i dati in una lingua diversa, potrebbero non essere archiviati correttamente. Per verificare di avere individuato correttamente le lingue supportate per [!INCLUDE[d365fin](includes/d365fin_md.md)], rivolgersi all'amministratore di sistema.  

## <a name="changing-the-locale"></a>Modifica delle impostazioni locali
Le impostazioni locali differiscono dalla lingua e dai requisiti legali nei mercati locali. Le impostazioni locali determinano la visualizzazione dei dati in termini di separatore, allineamento a sinistra o a destra ed alcune altre impostazioni. Le impostazioni locali determinano anche alcuni degli elementi di sistema nel browser, ad esempio l'azione per creare un nuovo elemento in un elenco.  

È possibile modificare le impostazioni locali nella scheda del browser utilizzato in [!INCLUDE[d365fin](includes/d365fin_md.md)]. La modifica è valida solo per l'utente corrente e non per gli altri utenti nella società.  

> [!IMPORTANT]  
>  Quando si modificano le impostazioni locali, viene visualizzato un lungo elenco di lingue e impostazioni locali. Tuttavia, solo le impostazioni locali selezionate sono utilizzate nella versione corrente di [!INCLUDE[d365fin](includes/d365fin_md.md)].  

Per modificare le impostazioni locali, passare alla finestra **Impostazioni personali**. Per ulteriori informazioni, vedere [Modifica delle impostazioni di base](ui-change-basic-settings.md).  

## <a name="see-also"></a>Vedi anche  
[Lingue della documentazione](about-languages.md)  
[Modifica delle impostazioni di base](ui-change-basic-settings.md)  
[Benvenuto in [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
