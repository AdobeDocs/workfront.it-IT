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
source-wordcount: '660'
ht-degree: 0%

---

# Risoluzione dei problemi - font di interfaccia danneggiato nel visualizzatore di bozze su Mac

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

Se si nota che il visualizzatore di bozze non visualizza correttamente il carattere dell&#39;interfaccia, ciò potrebbe essere dovuto ad alcuni problemi con i caratteri sul computer Mac. Per risolvere il problema, provare le soluzioni seguenti:

## Rimuovi duplicati font

Verificare se nel sistema sono presenti caratteri duplicati.

1. Chiudere il browser in uso.
1. Aprire l&#39;applicazione Rubrica caratteri nella cartella Applicazioni.
1. Fare clic su **[!UICONTROL Tutti i font]** (1).
1. Fai clic su **[!UICONTROL Modifica]** > **[!UICONTROL Cerca duplicati abilitati]**.

1. Fai clic su **[!UICONTROL Sì]** per risolvere i duplicati.
1. Se viene visualizzato un avviso relativo a tipi di carattere danneggiati, fare clic su **[!UICONTROL Sì]**.
1. Riavvia il computer.
1. Riprovare.

## Cancella la cache dei caratteri

A volte, le cache dei font in Mac OS X risultano danneggiate. Ad esempio, quando un carattere o una famiglia di caratteri viene reinstallato più volte o se un&#39;applicazione è stata aggiornata o reinstallata. A parte i file della cache dei caratteri del sistema operativo, alcune applicazioni possono disporre di una propria cache dei caratteri. L&#39;eliminazione di questi file di cache dei caratteri può risolvere il problema con il testo illeggibile.

Innanzitutto, è necessario avviare la Rubrica, selezionare il carattere o la famiglia con cui si hanno problemi e premere il pulsante Elimina sulla tastiera. È inoltre possibile fare clic con il pulsante destro del mouse e selezionare [!UICONTROL Rimuovi famiglia]. Se non si è sicuri del tipo di carattere o della famiglia che causa il problema, provare prima a rimuovere i duplicati come descritto in precedenza.

Il secondo passaggio consiste nel cancellare la cache dei caratteri e ci sono diversi modi per farlo.

Il primo consiste nel riavviare il sistema in modalità provvisoria tenendo premuto il tasto Maiusc immediatamente quando si sentono i segnali di avvio all&#39;avvio. Quando questa modalità viene caricata, dovrebbe essere visualizzata una barra di avanzamento, durante la quale il sistema eseguirà vari controlli e routine di manutenzione, uno dei quali è quello di cancellare la cache del font.

Il secondo approccio consiste nell&#39;utilizzare il Terminal, che può essere eseguito eseguendo il comando seguente dall&#39;interno di un account amministrativo: *sudo atsutil databases -remove*

>[!NOTE]
>
>Questo comando richiede l&#39;immissione della password, che non verrà visualizzata al momento della digitazione. È consigliabile consultare il reparto IT in quanto potrebbe essere necessario disporre di autorizzazioni di amministratore sul computer.

Un altro approccio consiste nell’utilizzare un’utility per la cache dei caratteri come ad esempio FontNuke e cancellare la cache con il relativo aiuto.

Molti studi di prestampa e artworking/design utilizzano anche il software Universal Type Server per gestire le licenze e la distribuzione dei font. A volte può verificarsi un problema con la cache dei caratteri del server di tipo universale, che può causare la scomparsa delle annotazioni [!DNL Workfront Proof].

Per risolvere il problema, cancellare la cache dei caratteri del server di tipo universale e riavviare il server di tipo universale.

## Correggi conflitto di font [!DNL Flash]

È possibile che non si disponga dell&#39;accesso a questa funzionalità perché è supportata da [!DNL Flash], che nella maggior parte degli ambienti è stata dichiarata obsoleta.

Il visualizzatore di bozze legacy è basato su [!DNL Flash Player] e talvolta, quando il testo non è presente nel visualizzatore di bozze, è possibile che si verifichi un conflitto di font tra OS X e [!DNL Flash Player]. Provare a eseguire le operazioni seguenti:

1. Apri il Finder e apri la scheda **[!UICONTROL Vai]**.
1. Premere il tasto Opzione ( Alt) per aprire la cartella [!UICONTROL Library] nell&#39;elenco a discesa.
1. Tenendo premuto il tasto Option, fare clic sulla cartella [!UICONTROL Library].
1. Una volta aperta la cartella [!UICONTROL Library], passa alla cartella [!UICONTROL Fonts] all&#39;interno di.
1. Spostare tutti i tipi di carattere presenti nella cartella [!UICONTROL Caratteri] in un&#39;altra cartella, ad esempio sul desktop. Non creare un&#39;altra cartella all&#39;interno della cartella Caratteri.
1. Questa azione consente di nascondere tutti i tipi di carattere personalizzati; è comunque necessario salvare i tipi di carattere di sistema standard in una posizione separata.
1. Chiudere e riavviare [!DNL Safari].
1. Riapri la bozza.

I tipi di carattere dovrebbero essere visualizzati adesso. Se non è necessario rimuovere i tipi di carattere dalla home directory, è possibile eliminarli in modo sicuro. In caso contrario, esaminali in batch, copiali nuovamente nella cartella Libreria/Tipi di carattere e individua la causa del problema.
