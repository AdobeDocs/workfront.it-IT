---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Verificare le connessioni del webhook
description: Verificare le connessioni del webhook
author: Becky
feature: Workfront API
role: Developer
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---


# Verificare le connessioni del webhook

Per verificare il corretto funzionamento dell’implementazione del webhook del documento, esegui i test manuali descritti in questa sezione. Questi passaggi passano attraverso l’interfaccia web di Adobe Workfront e indirettamente raggiungono gli endpoint per l’implementazione del webhook.

## Prerequisiti

Per eseguire i test sono necessari i seguenti prerequisiti:

* Un account Workfront con Advanced Document Management (ADM) abilitato

* Un utente Workfront per questo account con diritti di amministratore di sistema

* Un&#39;istanza del webhook del documento con endpoint HTTP accessibili a Workfront

Questi test presuppongono inoltre che l’istanza del webhook del documento sia registrata. (Puoi registrare la tua istanza in Workfront in Configurazione > Documenti > Integrazioni personalizzate).

**Test 1: provisioning del servizio Document Webhook per un utente**

Verifica l’URL di autenticazione e l’URL dell’endpoint del token per i provider Webhook basati su OAuth.

1. In Workfront, passare alla pagina principale Documenti facendo clic sul collegamento Documenti nella barra di navigazione superiore.
1. Fai clic sul menu a discesa Aggiungi documenti e seleziona il servizio Document Webhook in Aggiungi servizio.
1. (Solo per i servizi OAuth) Dopo aver completato il passaggio precedente, visualizzerai la pagina di autenticazione OAuth2 del servizio in una finestra a comparsa. (Nota: potrebbe essere richiesto di accedere prima al servizio.) Dalla pagina di autenticazione, concedi a Workfront l’accesso all’account dell’utente facendo clic sul pulsante Considera attendibili o Consenti.
1. Verifica che il servizio sia stato aggiunto al menu a discesa Aggiungi documenti. Se inizialmente non è visibile, prova ad aggiornare il browser.

**Test 2: collegare un documento in Workfront Test i seguenti endpoint: /files, /metadata**

1. In Workfront, passare alla pagina principale Documenti facendo clic sul collegamento Documenti nella barra di navigazione superiore.
1. Selezionare il servizio Web Document in Aggiungi documenti.
1. Dalla finestra modale, passa alla struttura delle cartelle.
1. Verifica di essere in grado di navigare nella struttura di cartelle.
1. Selezionare un documento e collegarlo a Workfront

**Prova 3: passare a un documento nel sistema di gestione dei contenuti**

Verifica i seguenti endpoint: /metadata (in particolare viewLink)

1. Collegare un documento a Workfront
1. Selezionare il documento e fare clic sul collegamento Apri.
1. Verificate che il documento venga aperto in una nuova scheda.

**Prova 4: passare a un documento nel sistema di gestione dei contenuti (con accesso)**

Verifica i seguenti endpoint: /metadata (in particolare viewLink)

1. Assicurarsi di essere disconnessi dal sistema di gestione dei contenuti.
1. Collegare un documento a Workfront.
1. Selezionare il documento e fare clic sul collegamento Apri.
1. Verificare che la schermata di accesso del sistema di gestione dei contenuti venga caricata in una nuova scheda.
1. Accedi e verifica di essere reindirizzato al documento

**Test 5: scaricare il documento dal sistema di gestione dei contenuti**

Verifica i seguenti endpoint (in particolare il collegamento di download): /metadata 

1. Collegare un documento a Workfront.
1. Selezionare il documento e fare clic sul collegamento Scarica.
1. Verifica l’inizio del download.

**Prova 6: ricerca contenuto**

Verifica i seguenti endpoint: /search

1. In Workfront, passare alla pagina principale Documenti facendo clic sul collegamento Documenti nella barra di navigazione superiore.
1. Selezionare il servizio Web Document in Aggiungi documenti.
1. Dal modale, esegui una ricerca.
1. Verifica che i risultati della ricerca siano corretti.

**Prova 7: invia documento da Workfront a Content Management System**

Verifica i seguenti endpoint: /files, /uploadInit, /upload

1. In Workfront, passare alla pagina principale Documenti facendo clic sul collegamento Documenti nella barra di navigazione superiore.
1. Carica un documento in Workfront dal computer
1. Vai alla pagina dei dettagli del documento
1. Dal menu a discesa Azioni documento, selezionare il servizio Web Document in Invia a...
1. Vai alla cartella di destinazione desiderata e fai clic sul pulsante Salva.
1. Verificare che il documento sia caricato nella posizione corretta nel sistema di gestione dei contenuti.

**Test 8: visualizzazione miniature in Workfront**

Verifica i seguenti endpoint: /thumbnail

1. Collegare un documento a Workfront.
1. Seleziona il documento nell’elenco.
1. Verifica che la miniatura venga visualizzata nel pannello di destra.

**Prova 9: ottieni i byte di contenuto**

Verifica i seguenti endpoint: /download

1. Collegare un documento a Workfront.
1. Passare alla pagina dei dettagli del documento.
1. Inviare il documento a Workfront selezionando Azioni documento > Invia a... > Workfront. Verrà creata una nuova versione del documento in Workfront.
1. Scaricare il documento da Workfront facendo clic sul collegamento Scarica.

**Prova 10: aggiorna token di accesso (solo provider del webhook OAuth2)**

Verifica i seguenti endpoint: URL endpoint token

1. Eseguire il provisioning di un servizio Web Document per un utente
1. Annulla la validità del token di accesso dell’utente 1 )in attesa del timeout oppure 2) annullandolo manualmente nel sistema esterno.
1. Aggiorna il token di accesso in Workfront. A tale scopo, ad esempio, è possibile collegare un documento in Workfront. Se sei riuscito a passare a un documento e a collegarlo, saprai che il token di accesso è stato aggiornato correttamente.

>[!NOTE]
>
>Al momento, l&#39;opzione Invia a non è disponibile per i documenti collegati. Questo verrà aggiunto da Workfront. Puoi testare l’endpoint /download premendo manualmente l’endpoint utilizzando un client REST, ad esempio Postman. In alternativa, è possibile testare l’endpoint /download generando una bozza digitale. Per attivare la verifica digitale, contattare Workfront.
