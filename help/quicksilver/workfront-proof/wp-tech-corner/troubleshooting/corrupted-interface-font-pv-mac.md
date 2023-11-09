---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Risoluzione dei problemi - font di interfaccia danneggiato nel visualizzatore di bozze su Mac
description: Risoluzione dei problemi relativi al font dell’interfaccia danneggiato nel visualizzatore di bozze su Mac
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# Risoluzione dei problemi - font di interfaccia danneggiato nel visualizzatore di bozze su Mac

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità del prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Bozza](../../../review-and-approve-work/proofing/proofing.md).

Se si nota che il visualizzatore di bozze non visualizza correttamente il carattere dell&#39;interfaccia, ciò potrebbe essere dovuto ad alcuni problemi con i caratteri sul computer Mac. Per risolvere il problema, provare le soluzioni seguenti:

## Rimuovi duplicati font

Verificare se nel sistema sono presenti caratteri duplicati.

1. Chiudere il browser in uso.
1. Aprire l&#39;applicazione Rubrica caratteri nella cartella Applicazioni.
1. Clic **[!UICONTROL Tutti i font]** (1)
1. Clic **[!UICONTROL Modifica]** > **[!UICONTROL Cerca duplicati abilitati]**.

1. Clic **[!UICONTROL Sì]** per risolvere i duplicati.
1. Se viene visualizzato un avviso relativo ai caratteri danneggiati, fare clic su **[!UICONTROL Sì]**.
1. Riavvia il computer.
1. Riprovare.

## Cancella la cache dei caratteri

A volte, le cache dei font in Mac OS X risultano danneggiate. Ad esempio, quando un carattere o una famiglia di caratteri viene reinstallato più volte o se un&#39;applicazione è stata aggiornata o reinstallata. A parte i file della cache dei caratteri del sistema operativo, alcune applicazioni possono disporre di una propria cache dei caratteri. L&#39;eliminazione di questi file di cache dei caratteri può risolvere il problema con il testo illeggibile.

Innanzitutto, è necessario avviare la Rubrica, selezionare il carattere o la famiglia con cui si hanno problemi e premere il pulsante Elimina sulla tastiera. Puoi anche fare clic con il pulsante destro del mouse e selezionare [!UICONTROL Rimuovi famiglia]. Se non si è sicuri del tipo di carattere o della famiglia che causa il problema, provare prima a rimuovere i duplicati come descritto in precedenza.

Il secondo passaggio consiste nel cancellare la cache dei caratteri e ci sono diversi modi per farlo.

Il primo consiste nel riavviare il sistema in modalità provvisoria tenendo premuto il tasto Maiusc immediatamente quando si sentono i segnali di avvio all&#39;avvio. Quando questa modalità viene caricata, dovrebbe essere visualizzata una barra di avanzamento, durante la quale il sistema eseguirà vari controlli e routine di manutenzione, uno dei quali è quello di cancellare la cache del font.

Il secondo approccio consiste nell’utilizzare il terminale, che può essere eseguito eseguendo il seguente comando dall’interno di un account amministrativo: *database sudo atsutil -remove*

>[!NOTE]
>
>Questo comando richiede l&#39;immissione della password, che non verrà visualizzata al momento della digitazione. È consigliabile consultare il reparto IT in quanto potrebbe essere necessario disporre di autorizzazioni di amministratore sul computer.

Un altro approccio consiste nell’utilizzare un’utility per la cache dei caratteri come ad esempio FontNuke e cancellare la cache con il relativo aiuto.

Molti studi di prestampa e artworking/design utilizzano anche il software Universal Type Server per gestire le licenze e la distribuzione dei font. A volte può verificarsi un problema con la cache dei caratteri del server di tipo universale, che può causare [!DNL Workfront Proof] annotazioni da eliminare.

Per risolvere il problema, cancellare la cache dei caratteri del server di tipo universale e riavviare il server di tipo universale.

## Correzione [!DNL Flash] conflitto di font

Potresti non avere accesso a questa funzionalità perché è supportata da [!DNL Flash], che è stato dichiarato obsoleto nella maggior parte degli ambienti.

Il visualizzatore di bozze legacy si basa su [!DNL Flash Player] e a volte, quando il testo non è presente nel visualizzatore di bozze, è possibile che vi sia un conflitto di font tra OS X e [!DNL Flash Player]. Provare a eseguire le operazioni seguenti:

1. Apri Finder e apri **[!UICONTROL Vai]** scheda.
1. Premere il tasto Opzione ( Alt) per aprire [!UICONTROL Libreria] nell’elenco a discesa.
1. Tenendo premuto il tasto Opzione, fare clic sul pulsante [!UICONTROL Libreria] cartella.
1. Dopo il [!UICONTROL Libreria] apertura cartella, vai a [!UICONTROL Font] cartella che si trova in.
1. Spostare tutti i tipi di carattere presenti nel [!UICONTROL Font] cartella in un&#39;altra cartella, ad esempio sul desktop (non creare un&#39;altra cartella all&#39;interno della cartella Fonts).
1. Questa azione consente di nascondere tutti i tipi di carattere personalizzati; è comunque necessario salvare i tipi di carattere di sistema standard in una posizione separata.
1. Esci e riavvia [!DNL Safari].
1. Riapri la bozza.

I tipi di carattere dovrebbero essere visualizzati adesso. Se non è necessario rimuovere i tipi di carattere dalla home directory, è possibile eliminarli in modo sicuro. In caso contrario, esaminali in batch, copiali nuovamente nella cartella Libreria/Tipi di carattere e individua la causa del problema.
