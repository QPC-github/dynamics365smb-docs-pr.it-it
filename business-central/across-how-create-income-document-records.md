---
title: Creare i record di documenti in entrata
description: 'Utilizza diverse funzioni nella pagina Documenti in entrata per rivedere le ricevute delle spese, gestire i task OCR, convertire i file dei documenti in entrata e collegare file esterni.'
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice'
ms.date: 06/14/2022
ms.author: edupont
---
# <a name="create-incoming-document-records" />Creare i record di documenti in entrata

Nella pagina **Documenti in entrata** è possibile utilizzare diverse funzioni per esaminare le ricevute relative alle spese, gestire le attività OCR e convertire i file dei documenti in entrata, manualmente o automaticamente, nei relativi documenti o in righe di registrazione. I file esterni possono essere allegati in qualsiasi fase dell'elaborazione, ad esempio ai documenti registrati, nonché ai fornitori, clienti e movimenti di contabilità generale risultanti.

Per registrare un documento esterno in [!INCLUDE[prod_short](includes/prod_short.md)], prima crea o completa un record di documento in entrata. Questa operazione può essere eseguita manualmente oppure scattando una foto del documento per creare un record del documento in entrata con il file immagine allegato.

Per poter utilizzare la funzionalità **Documenti in entrata**, devi eseguire l'impostazione necessaria. Per ulteriori informazioni, vedere [Impostare documenti in entrata](across-how-setup-income-documents.md).

## <a name="approve-or-reject-an-incoming-document" />Per approvare o rifiutare un documento in entrata

Se hai impostato la funzione **Documenti in entrata** per richiedere l'approvazione per la creazione di documenti, gli utenti con i diritti appropriati devono approvare i record prima che vengano elaborati. Per ulteriori informazioni, vedi [Impostare i responsabili dell'approvazione dei record dei documenti in entrata](across-how-setup-income-documents.md#to-set-up-approvers-of-incoming-document-records).

1. Scegli la ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Dimmi cosa vuoi fare") immetti **Documenti in entrata**, quindi scegli il collegamento correlato.
2. Selezionare la riga con il documento che si desidera approvare o rifiutare quindi selezionare l'azione **Approva** o **Rifiuta**.

Se si approva il record del documento in entrata, la casella di controllo **Rilasciato** nella riga del documento in entrata è selezionata. L'utente incaricato di creare, ad esempio, le fatture di acquisto può procedere all'elaborazione del record.

## <a name="create-an-incoming-document-record-by-taking-a-photo" />Per creare un record di documento in entrata facendo una foto

> [!NOTE]  
> La seguente procedura si applica solo ai client di [!INCLUDE[prod_short](includes/prod_short.md)] per tablet e telefono.

1. In Gestione ruolo utente, scegli il riquadro **Crea documento in entrata da fotocamera** e vai al passaggio 4.
2. In alternativa, scegli l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni.](media/ui-search/search_small.png "Dimmi cosa vuoi fare") e immetti **Documenti in entrata**, quindi scegli il collegamento correlato.
3. Nella pagina **Documenti in entrata** scegli **Nuovo** e seleziona **Crea da fotocamera**. La fotocamera del tablet o del telefono è attivata.
4. Scatta la foto di un documento, ad esempio una ricevuta di acquisto, che vuoi elaborare come documento in entrata e fai clic sul pulsante **Usa**.

    Viene creato un nuovo record di documento in entrata con l'immagine allegata.

## <a name="attach-an-image-to-an-incoming-document-record-by-taking-a-photo" />Per allegare un'immagine a un record di documento in entrata facendo una foto

> [!NOTE]  
> La seguente procedura si applica solo ai client di [!INCLUDE[prod_short](includes/prod_short.md)] per tablet e telefono.

1. Scegli la ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Dimmi cosa vuoi fare") e immetti **Documenti in entrata**, quindi scegli il collegamento correlato.
2. Aprire la scheda di un record di documento in entrata esistente.
3. Nella pagina del record del documento scegli **Elabora** e seleziona **Allega immagine da fotocamera**. La fotocamera del tablet o del telefono è attivata.
4. Scatta la foto di un documento, ad esempio una ricevuta di acquisto, che vuoi elaborare come documento in entrata e fai clic sul pulsante **Usa**.

    L'immagine viene allegata al record di documento in entrata.

## <a name="create-an-incoming-document-record-manually" />Per creare manualmente il record di un documento in entrata

1. Scegli la ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") e immetti **Documenti in entrata**, quindi scegli il collegamento correlato.
2. Scegli **Nuovo**, e l'azione **Crea da file**.  
3. Nella pagina **Inserisci file** selezionare un file e scegliere **Apri**. Il file viene automaticamente allegato.
4. In alternativa, selezionare l'azione **Nuovo**.
5. Per allegare un file, seleziona **Elabora** e l'azione **Allega file**.
6. Nella pagina **Inserisci file** selezionare il file che rappresenta il documento in entrata in questione, quindi scegliere il pulsante **Apri**.
7. Nella pagina **Documento in entrata** compilare i campi secondo le proprie necessità. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="see-related-microsoft-trainingtrainingmodulesincoming-documents-dynamics-365-business-central" />Vedi il relativo [training Microsoft](/training/modules/incoming-documents-dynamics-365-business-central/)

## <a name="see-also" />Vedere anche

[Utilizzare OCR per convertire PDF e file di immagine in documenti elettronici](across-how-use-ocr-pdf-images-files.md)
[Creare i record di documenti in entrata direttamente da documenti e movimenti](across-how-connect-disconnect-income-document-records.md)
[Trovare documenti registrati senza record di documenti in entrata](across-how-find-posted-documents-without-income-document-records.md)
[Documenti in entrata](across-income-documents.md)  
[Acquisti](purchasing-manage-purchasing.md)  
[Utilizzare [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
