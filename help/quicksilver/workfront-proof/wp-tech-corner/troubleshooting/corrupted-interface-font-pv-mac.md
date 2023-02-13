---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Risoluzione dei problemi - font interfaccia danneggiato nel visualizzatore di correzione su Mac
description: Se noti che il visualizzatore di correzione non visualizza correttamente il font dell’interfaccia, ciò potrebbe essere dovuto ad alcuni problemi con i font sul computer Mac. Per risolvere il problema, prova le seguenti soluzioni - MODIFICA ME.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Risoluzione dei problemi - font interfaccia danneggiato nel visualizzatore di correzione su Mac

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Se noti che il visualizzatore di correzione non visualizza correttamente il font dell’interfaccia, ciò potrebbe essere dovuto ad alcuni problemi con i font sul computer Mac. Per risolvere il problema, prova le seguenti soluzioni:

## Rimuovi duplicati di font

Controlla se ci sono font duplicati nel sistema.

1. Chiudi il browser in uso.
1. Aprire l&#39;applicazione Font Book nella cartella Applicazioni.
1. Fai clic su **[!UICONTROL Tutti i font]** (1)
1. Fai clic su **[!UICONTROL Modifica]** > **[!UICONTROL Cerca duplicati abilitati]**.

1. Fai clic su **[!UICONTROL Sì]** per risolvere i duplicati.
1. Se viene visualizzato un avviso sui font danneggiati, fare clic su **[!UICONTROL Sì]**.
1. Riavvia il computer.
1. Riprova la bozza.

## Cancella la cache dei font

A volte, le cache dei font in Mac OS X diventano danneggiate. Ad esempio, quando un font o una famiglia di font viene reinstallato più volte o se un&#39;applicazione è stata aggiornata o reinstallata. Oltre ai file della cache dei font del sistema operativo, alcune applicazioni possono avere una propria cache dei font. L&#39;eliminazione di questi file della cache dei font può risolvere il problema con il testo illeggibile.

In primo luogo, sarà necessario avviare Font Book, selezionare il font o la famiglia con cui si verificano problemi e premere il pulsante Elimina sulla tastiera. Puoi anche fare clic con il pulsante destro del mouse e selezionare [!UICONTROL Rimuovi famiglia]. Se non sei sicuro del font o della famiglia che sta causando i problemi, puoi provare prima a rimuovere i duplicati come descritto sopra.

Il secondo passo sarebbe quello di cancellare la cache dei font e ci sono diversi modi per ottenere questo.

Il primo è semplicemente riavviare in modalità provvisoria tenendo premuto il tasto Maiusc immediatamente quando si sentono i tempi di avvio all&#39;avvio. Quando questa modalità viene caricata, deve essere visualizzata una barra di avanzamento durante la quale il sistema eseguirà vari controlli e routine di manutenzione, una delle quali consiste nel cancellare la cache dei font.

Il secondo approccio è quello di utilizzare il Terminal, che può essere fatto eseguendo il seguente comando dall&#39;interno di un account amministrativo: *sudo atsutil database -remove*

>[!NOTE]
>
>Questo comando richiede l&#39;immissione della password, che non verrà visualizzata quando digitato. Si consiglia di consultare il proprio reparto IT in quanto ciò potrebbe richiedere autorizzazioni di amministratore sul computer.

Un altro approccio consiste nell’utilizzare un’utilità per la cache dei font, ad esempio FontNuke, e cancellare la cache con il suo aiuto.

Molti studi di prestampa e artworking/design utilizzano anche il software Universal Type Server per gestire la licenza e la distribuzione dei font. A volte, può verificarsi un problema con la cache dei font del server del tipo universale, che può causare il [!DNL Workfront Proof] annotazioni da eliminare.

Per risolvere il problema, cancella la cache dei font del server del tipo universale e riavvia il server del tipo universale.

## Correzione [!DNL Flash] conflitto di font

È possibile che non si disponga dell&#39;accesso a questa funzionalità perché è supportata da [!DNL Flash], che è stato dichiarato obsoleto nella maggior parte degli ambienti.

Il visualizzatore di correzione legacy si basa su [!DNL Flash Player] e a volte, quando il testo è mancante nel visualizzatore di correzione, è possibile che ci sia un conflitto di font tra OS X e [!DNL Flash Player]. Prova quanto segue:

1. Apri Finder e apri le **[!UICONTROL Vai]** scheda .
1. Premi il tasto Opzione ( ⌥ Alt) per aprire la [!UICONTROL Libreria] nell’elenco a discesa.
1. Tenendo premuto il tasto Opzione, fai clic sul pulsante [!UICONTROL Libreria] cartella.
1. Dopo la [!UICONTROL Libreria] si apre, vai a [!UICONTROL Font] cartella all’interno di .
1. Sposta tutti i font presenti nella [!UICONTROL Font] in un&#39;altra cartella, ad esempio sul desktop (non creare un&#39;altra cartella all&#39;interno della cartella Font).
1. Questa azione nasconde tutti i font personalizzati; è comunque necessario salvare i font di sistema standard nella posizione separata.
1. Esci e riavvia [!DNL Safari].
1. Riapri la bozza.

Ora dovresti vedere i tuoi font. Se non hai bisogno dei font rimossi dalla directory principale, puoi eliminarli in tutta sicurezza. In caso contrario, eseguine l’analisi in batch, copiale nuovamente nella cartella Libreria/Font e scopri quale causa il problema.
