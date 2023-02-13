---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Test delle connessioni Webhook
description: Test delle connessioni Webhook
author: John
feature: Workfront API
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: a62ae524f922326811423cd17d0656920b7cc9d3
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---


# Test delle connessioni Webhook

Per verificare che l&#39;implementazione del webhook del documento funzioni correttamente, esegui i test manuali in questa sezione. Questi passaggi passano attraverso l’interfaccia web di Adobe Workfront e indirettamente raggiungono gli endpoint per l’implementazione del webhook.

## Prerequisiti

Per eseguire i test sono necessari i seguenti prerequisiti:

* Un account Workfront con Advanced Document Management (ADM) abilitato

* Un utente Workfront per questo account con diritti di amministratore di sistema

* Un&#39;istanza Document Webhook con endpoint HTTP accessibili a Workfront

Questi test presuppongono anche che l&#39;istanza Document Webhook sia registrata. (Puoi registrare la tua istanza in Workfront in Configurazione > Documenti > Integrazioni personalizzate.)

**Prova 1: Provisioning del servizio Document Webhook per un utente**

Verifica l’URL di autenticazione e l’URL dell’endpoint dei token per i provider di Webhook basati su OAuth.

1. In Workfront, vai alla pagina Documenti principale facendo clic sul collegamento Documenti nella barra di navigazione superiore.
1. Fare clic sul menu a discesa Aggiungi documenti e selezionare il servizio Document Webhook in Aggiungi servizio.
1. (Solo servizi OAuth) Dopo aver completato il passaggio precedente, vedrai il caricamento della pagina di autenticazione OAuth2 del servizio in una finestra a comparsa. (Nota: potrebbe essere richiesto di accedere prima al servizio). Dalla pagina di autenticazione, concedere l&#39;accesso Workfront all&#39;account dell&#39;utente facendo clic sul pulsante Trust o Allow.
1. Verifica che il servizio sia stato aggiunto al menu a discesa Aggiungi documenti . Se non lo vedi inizialmente, prova ad aggiornare il browser.

**Prova 2: Collega un documento ai test Workfront per i seguenti endpoint: /files, /metadata**

1. In Workfront, vai alla pagina Documenti principale facendo clic sul collegamento Documenti nella barra di navigazione superiore.
1. Selezionare il servizio Document Webhook in Aggiungi documenti.
1. Dal modale, passa alla struttura della cartella.
1. Verifica di essere in grado di navigare nella struttura della cartella.
1. Selezionare e collegare un documento in Workfront

**Prova 3: Passare a un documento nel sistema di gestione dei contenuti**

Verifica i seguenti endpoint: /metadata (in particolare viewLink)

1. Collegamento di un documento in Workfront
1. Selezionare il documento e fare clic sul collegamento Apri.
1. Verifica che il documento si apra in una nuova scheda.

**Prova 4: Passa a un documento nel sistema di gestione dei contenuti (con accesso)**

Verifica i seguenti endpoint: /metadata (in particolare viewLink)

1. Assicurati di essere disconnesso dal sistema di gestione dei contenuti.
1. Collega un documento in Workfront.
1. Selezionare il documento e fare clic sul collegamento Apri.
1. Verifica che la schermata di accesso del sistema di gestione dei contenuti venga caricata in una nuova scheda.
1. Accedi e verifica di essere stato portato al documento

**Prova 5: Scarica il documento dal sistema di gestione dei contenuti**

Verifica i seguenti endpoint (in particolare il collegamento per il download): /metadata 

1. Collega un documento in Workfront.
1. Seleziona il documento e fai clic sul collegamento Scarica .
1. Verifica che il download inizi.

**Prova 6: Cercare contenuti**

Verifica i seguenti endpoint: /search

1. In Workfront, vai alla pagina Documenti principale facendo clic sul collegamento Documenti nella barra di navigazione superiore.
1. Selezionare il servizio Document Webhook in Aggiungi documenti.
1. Dal modale, esegui una ricerca.
1. Verifica che i risultati della ricerca siano corretti.

**Prova 7: Invio di documenti da Workfront al sistema di gestione dei contenuti**

Verifica i seguenti endpoint: /files, /uploadInit, /upload

1. In Workfront, vai alla pagina Documenti principale facendo clic sul collegamento Documenti nella barra di navigazione superiore.
1. Caricare un documento in Workfront dal computer
1. Vai alla pagina dei dettagli del documento
1. Dal menu a discesa Azioni documento, seleziona il servizio Webhook documento in Invia a...
1. Passa alla cartella di destinazione desiderata e fai clic sul pulsante Salva .
1. Verifica che il documento sia caricato nella posizione corretta nel sistema di gestione dei contenuti.

**Prova 8: Visualizzare le miniature in Workfront**

Verifica i seguenti endpoint: /thumbnail

1. Collega un documento in Workfront.
1. Selezionare il documento nell&#39;elenco.
1. Verifica che la miniatura sia visualizzata nel pannello di destra.

**Prova 9: Ottenere i byte di contenuto**

Verifica i seguenti endpoint: /download

1. Collega un documento in Workfront.
1. Passare alla pagina dei dettagli del documento.
1. Invia il documento a Workfront selezionando Azioni documento > Invia a... > Workfront. Verrà creata una nuova versione del documento in Workfront.
1. Scarica il documento da Workfront facendo clic sul collegamento Scarica .

**Prova 10: Aggiorna il token di accesso (solo provider di Webhook OAuth2)**

Verifica i seguenti endpoint: URL endpoint token

1. Provisioning di un servizio Document Webhook per un utente
1. Annulla la validità del token di accesso dell’utente con 1 in attesa del timeout o con 2) in attesa dell’annullamento manuale della validità nel sistema esterno.
1. Aggiorna il token di accesso in Workfront. Per farlo, ad esempio, è possibile collegare un documento a Workfront. Il token di accesso è stato aggiornato se è stato possibile accedere a un documento e collegarlo.

>[!NOTE]
>
>Attualmente, l&#39;opzione Invia a non è disponibile per i documenti collegati. Questo verrà aggiunto da Workfront. Puoi testare l’endpoint /download colpendo manualmente l’endpoint utilizzando un client REST, come Postman. In alternativa, è possibile testare l’endpoint /download generando una bozza digitale. Per abilitare la correzione digitale, contattare Workfront.
