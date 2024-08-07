---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problemi di velocità in  [!DNL Workfront Proof]
description: Questa pagina della guida consente di determinare se eventuali problemi di velocità che potrebbero verificarsi durante l'utilizzo di  [!DNL Workfront Proof]  sono correlati all'ISP o alla rete di distribuzione dei contenuti di  [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 20fcf4dd07c1058559533501f7e297d78c43a70b
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Problemi di velocità in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

Questa pagina della Guida consente di determinare se eventuali problemi di velocità che potrebbero verificarsi durante l&#39;utilizzo di [!DNL Workfront Proof] sono correlati all&#39;ISP o alla rete di distribuzione dei contenuti di [!DNL Workfront Proof].

I problemi di velocità sono in genere dovuti alla connessione ISP locale o alla configurazione dell&#39;accesso a Internet locale (ad esempio, dove viene utilizzato un server proxy) e pertanto non sono controllati da [!DNL Workfront Proof].

Detto questo, puoi adottare alcune misure per verificare la velocità della connessione, consentendo di determinare la causa principale dei problemi che stai riscontrando. Tutti questi passaggi sono ugualmente importanti per il processo di risoluzione dei problemi e vi invitiamo a prendere il tempo per raccogliere informazioni su tutti i passaggi elencati per garantire la diagnosi più accurata del problema.

Una volta raccolte tutte le informazioni, si consiglia di consultare il reparto IT locale per identificare eventuali problemi locali.

## Stabilire quale parte del sistema è lenta

Quando utilizzi [!DNL Workfront Proof], potresti lavorare con il dashboard, ad esempio gestendo il contenuto delle cartelle e gli utenti, oppure con il visualizzatore [!DNL Workfront Proof]: eseguendo una revisione della bozza, controllando i commenti già aggiunti e così via.

La determinazione della parte esatta del sistema lenta è il primo passo per la risoluzione dei problemi di velocità. Quando segnali che [!DNL Workfront Proof] è lento, assicurati di descrivere quanto segue:

* Si sta verificando lentezza in altre pagine Web?
* Il problema si verifica nel dashboard o nel visualizzatore [!DNL Workfront Proof]?
* Quale parte esatta del sistema è lenta? (ad esempio, elaborazione di una nuova bozza o apertura di un commento nel visualizzatore [!DNL Workfront Proof])

## Eseguire test di tracciamento e ping

Quando si verificano problemi di prestazioni, è importante eseguire il comando traceroute per verificare la connessione. A questo scopo, apri il prompt dei comandi nel sistema (Terminal in Mac/Linux) ed esegui i seguenti passaggi:

1. Digitare uno dei seguenti elementi, quindi attendere il completamento del trace:

   * Windows: **app tracert.probhq.com**
   * Mac/Linux: **app traceroute.proof.com**

1. (Solo per Windows) Digitare **ping app.proof.com**.
1. Al termine del ping, fare clic con il pulsante destro del mouse sul prompt dei comandi e scegliere Seleziona tutto.
1. Copia e incolla i risultati nella risposta all’e-mail.
Prima di inviare i risultati al team di supporto, assicurati di consentire il completamento delle operazioni di tracciamento e ping.

## Verifica la velocità di connessione tramite Speedtest.net

1. Apri un browser e passa a Speedtest.net.
1. Seguire le istruzioni della Knowledge Base di Speedtest per verificare la velocità della connessione Internet.
1. Copia e incolla i risultati in un messaggio e-mail inviato al team di supporto.

## Controlla la scheda di rete nella console del browser

La console web disponibile nei browser moderni raccoglie informazioni utili su eventuali latenze di rete, che si riveleranno utili per determinare la causa principale dei problemi di velocità che stai riscontrando.

Per controllare i tempi di caricamento di una pagina Web:

1. Apri la console del browser e la scheda Rete.
1. Ricarica la pagina.
1. Acquisisci screenshot o registra uno screencast dei risultati.
1. Condividi i risultati con il team di supporto.

Assicurati che la schermata mostri tutti i dati: puoi espandere la finestra della console quando acquisisci una schermata o scorrerla verso il basso in una schermata.

Per istruzioni più dettagliate, consulta anche la documentazione del browser in uso.

## Verificare la connessione in un&#39;altra rete e in un altro computer

Per la risoluzione dei problemi è fondamentale verificare se si verifica lo stesso problema con la velocità di connessione utilizzando un dispositivo o una rete diversi. Prova a passare a un altro computer o dispositivo mobile e prova a utilizzare una rete alternativa (ad esempio, dati mobili).

Confrontare la connessione in diverse combinazioni: utilizzando una macchina diversa sulla stessa rete, utilizzando la stessa macchina su una rete diversa e utilizzando sia una macchina alternativa che una rete, quindi condividere i risultati con il team di supporto.
