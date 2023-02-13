---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problemi di velocità in [!DNL Workfront Proof]
description: Questa pagina di aiuto consente di determinare se si verificano problemi di velocità durante l'utilizzo [!DNL Workfront Proof] sono correlati al tuo ISP o [!DNL Workfront Proof]la rete di distribuzione dei contenuti.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 0%

---

# Problemi di velocità in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Questa pagina di aiuto consente di determinare se si verificano problemi di velocità durante l&#39;utilizzo [!DNL Workfront Proof] sono correlati al tuo ISP o [!DNL Workfront Proof]la rete di distribuzione dei contenuti.

I problemi di velocità sono generalmente dovuti alla connessione ISP locale o alla configurazione dell&#39;accesso a Internet locale (ad esempio, dove viene utilizzato un server proxy) e così via sono purtroppo al di fuori del controllo di [!DNL Workfront Proof].

Detto questo, ci sono alcuni passi che si possono fare per controllare la velocità di connessione che permetterà di determinare la causa principale dei problemi che si stanno verificando. Tutti questi passaggi sono ugualmente importanti per il processo di risoluzione dei problemi e vi invitiamo a prendere il tempo necessario per raccogliere informazioni su tutti i passaggi elencati per garantire la diagnosi più accurata del problema.

Una volta raccolti tutti i dettagli, ti consigliamo di consultare il tuo reparto IT locale per identificare eventuali problemi locali. Se hai bisogno di ulteriore aiuto, contatta il nostro [Team di supporto](https://support.workfront.com/hc/en-us/requests/new).

## Stabilire quale parte del sistema è lenta

Quando utilizzi [!DNL Workfront Proof], potresti lavorare con il dashboard, ad esempio gestire il contenuto della cartella e gli utenti o con il [!DNL Workfront Proof] Visualizzatore: effettuare una revisione delle prove, controllare le osservazioni già formulate e così via.

Determinare quale parte esatta del sistema è lenta è il primo passo nella risoluzione dei problemi di velocità. Quando viene generato un rapporto [!DNL Workfront Proof] a un livello di lentezza, assicurati di descrivere quanto segue:

* Stai vivendo una lentezza in altre pagine web?
* Il problema si verifica nel dashboard o [!DNL Workfront Proof] Visualizzatore?
* Quale parte esatta del sistema è lenta? (ad esempio, elaborazione di una nuova prova o apertura di un commento in [!DNL Workfront Proof] Visualizzatore)

## Eseguire test di tracciamento e ping

Quando si verificano problemi di prestazioni, è importante eseguire il comando traceroute per verificare la connessione. A questo scopo, apri il prompt dei comandi nel tuo sistema (Terminal in Mac/Linux) ed esegui i seguenti passaggi:

1. Digitare una delle seguenti opzioni, quindi attendere il completamento del tracciamento:

   * Windows: **tracert app.proofhq.com**
   * Mac/Linux: **traceroute app.proofhq.com**

1. (Solo Windows) Tipo **ping app.proofhq.com**.
1. Al termine del ping, fare clic con il pulsante destro del mouse nel prompt dei comandi e selezionare tutto.
1. Copia e incolla i risultati nella risposta all’e-mail.
Assicurati di consentire il completamento del tracciamento e del ping prima di inviare i risultati al team di supporto.

## Prova la velocità di connessione con Speedtest.net

1. Fai clic su [qui](http://www.speedtest.net/) per accedere a Speedtest.net.
1. Seguire le istruzioni riportate nella knowledge base Speedtest per verificare la velocità della connessione Internet.
1. Copia e incolla i risultati in un&#39;e-mail del nostro team di supporto.

## Controlla la scheda di rete nella console del browser

La console web disponibile nei browser moderni raccoglie informazioni utili su eventuali latenze di rete, che ci saranno utili per determinare la causa principale dei problemi di velocità che si verificano.

Per controllare i tempi di caricamento di una pagina web:

1. Apri la console del browser e la scheda Rete .
1. Ricarica la pagina.
1. Prendere screenshot o registrare uno screencast dei risultati.
1. Condividi i risultati con il team di supporto.

Assicurati che lo screenshot mostri tutti i dati: puoi espandere la finestra della console quando scegli una schermata o scorrere verso il basso in uno screencast.

Se non sai come aprire la console nel browser, vedi questi passaggi registrati:

* [Chrome](http://screencast.com/t/AgQU6JQQ)
* [Safari](http://screencast.com/t/f31GqQYm0w)
* [Firefox](http://screencast.com/t/Xg7SscmAi)
* [Bordo](http://www.screencast.com/t/epSwBiaD)
* [Internet Explorer](http://screencast.com/t/x5Q3eHczbc)

Puoi anche consultare la documentazione del browser per istruzioni più dettagliate.

## Controllare la connessione su una rete e un computer diversi

Controllare se si verifica lo stesso problema con la velocità di connessione utilizzando un dispositivo o una rete diversi è un passaggio fondamentale nel processo di risoluzione dei problemi. Prova a passare a un altro computer o a un dispositivo mobile e prova a utilizzare una rete alternativa (ad esempio dati mobili).

Confronta la connessione in diverse combinazioni: utilizzando un computer diverso sulla stessa rete, utilizzando lo stesso computer su una rete diversa e utilizzando sia la macchina alternativa che la rete, quindi condividere i risultati con il team di supporto.
