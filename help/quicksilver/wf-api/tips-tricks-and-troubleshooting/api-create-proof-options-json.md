---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Aggiungere opzioni di correzione avanzate con l’API di Adobe Workfront
description: Aggiungere opzioni di correzione avanzate con l’API di Adobe Workfront
author: Becky
feature: Workfront API, Workfront Proof
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 0%

---


# Aggiungi opzioni di correzione avanzate durante la creazione di una bozza tramite l’API di Adobe Workfront

Quando crei una bozza nell’API di Workfront, puoi aggiungere opzioni di correzione avanzate.

Utilizza uno dei seguenti flussi di lavoro per aggiungere opzioni di correzione a una bozza utilizzando l’API:

* (Consigliato) Crea una bozza semplice utilizzando l’API Workfront, quindi aggiungi opzioni di correzione avanzate alla bozza utilizzando l’API ProofHQ

* Creare una bozza con opzioni di correzione avanzate utilizzando JSON nell’API Workfront

## Crea una bozza utilizzando le API Workfront e ProofHQ (consigliato) {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

Questa sezione descrive come creare una bozza con opzioni di correzione avanzate tramite l’API Workfront, utilizzando una combinazione di API Workfront e ProofHQ.

L’API ProofHQ include una varietà di azioni non disponibili per le bozze nell’API Workfront. Utilizzando queste azioni, puoi modificare o configurare la bozza con una precisione maggiore di quella disponibile nell’API Workfront.

Per una panoramica dell’API ProofHQ, consulta la sezione [Panoramica di PoofHQ](../../proofhq-api/general/overview.md). Puoi inoltre fare riferimento alla sezione [Documentazione di ProofHQ](https://api.proofhq.com/home.html).

>[!NOTE]
>
>* L’API Workfront è un’API REST-ful. L’API ProofHQ è un’API SOAP.
>* Le bozze create nell’API ProofHQ non vengono collegate automaticamente a Workfront. Pertanto, consigliamo di creare bozze nell’API di Workfront prima di aggiornarle con l’API ProofHQ.
>


### Creare una bozza con opzioni di correzione avanzate

1. Crea una bozza utilizzando `Document createProof` nell’API di Workfront.

   >[!NOTE]
   Durante la creazione della bozza, non includere un valore per il parametro advancedProofingOptions .

1. Dopo aver creato la bozza, utilizza l’API ProofHQ per aggiungere eventuali opzioni avanzate.

### Esempi

Questa sezione mostra alcuni aggiornamenti di esempio che puoi eseguire con l’API ProofHQ.

**Esempi:**

* [Una bozza può essere scaricata, ha un messaggio e viene condivisa pubblicamente](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [Aggiornare una fase in modo che non sia privata, non obbligatoria e richieda una sola approvazione](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [Aggiungi due destinatari a una bozza senza processo decisionale principale](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**Una bozza può essere scaricata, ha un messaggio e viene condivisa pubblicamente**

La documentazione per questo endpoint si trova nella sezione [Aggiornamento API ProofHQ](https://api.proofhq.com/home/proofs/updateproof.html) pagina.

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateProof>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{file_id}}</FileID>
            <OwnerID>0</OwnerID>
            <Name>{{proof_name}}}</Name>
            <Subject>Email subject here</Subject>
            <Message>Email message here</Message>
            <EnableDownload>true</EnableDownload>
            <EnableTeamURL>true</EnableTeamURL>
        </soap:updateProof>
    </soapenv:Body>
</soapenv:Envelope>
```

**Aggiornare una fase in modo che non sia privata, non obbligatoria e richieda una sola approvazione**

La documentazione per questo endpoint si trova nella sezione [Aggiornamento API ProofHQworkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html) pagina.

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateWorkflowProofStage>
        <SessionID>{{session_id}}</SessionID>
        <FileID>{{proof_id}}</FileID>
        <Stage>
            <stage_id>{{stage_id}}</stage_id>
            <name>{{stage_name}}</name>
                <stage_one_decision_only>true</stage_one_decision_only>
                <stage_private>false</stage_private>
                <mandatory>false</mandatory>
            </Stage>
        </soap:updateWorkflowProofStage>
    </soapenv:Body>
</soapenv:Envelope>
```

**Aggiungi due destinatari a una bozza senza processo decisionale principale**

La documentazione per questo endpoint si trova nella sezione [API ProofHQ addWorkflowProofReviewers](https://api.proofhq.com/addworkflowproofreviewers.html) pagina.

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:addWorkflowProofReviewers>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{proof_id}}</FileID>
            <Recipients>
                <item>
                <email>{{recipient_email_1}}</email>
                <role>5</role>
                <name>{{recipient_name_1}}</name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
                <item>
                <email> {{recipient_email_2}} </email>
                <role>5</role>
                <name> {{recipient_name_2}} </name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
            </Recipients>
            <SuppressNewProofNotification></SuppressNewProofNotification>
        </soap:addWorkflowProofReviewers>
    </soapenv:Body>
</soapenv:Envelope>
```

## Creare una bozza utilizzando JSON nell’API Workfront

Questa sezione descrive come creare una bozza con opzioni di correzione avanzate tramite l’API Workfront, utilizzando JSON come valore di parametro nell’API Workfront

### Creare una bozza con opzioni di correzione avanzate

Puoi creare bozze tramite l’API di Workfront utilizzando l’ `Document createProof` azione. Questa azione accetta `advancedProofingOptions` , che ha il tipo di valore di `string`. Per includere opzioni di correzione avanzate nel `createProof` è necessario inserire le opzioni nella `advancedProofingOptions` in formato JSON.

>[!NOTE]
Può essere difficile prevedere i campi da includere nel JSON advancedProofingOptions. Potrebbe essere utile esaminare i dati di rete della tua organizzazione durante l’utilizzo della correzione avanzata in Workfront e basare il tuo JSON sui campi e i valori comunemente utilizzati dalla tua organizzazione.
Poiché questi campi possono essere difficili da prevedere, è consigliabile creare una bozza utilizzando l’API Workfront e aggiornarla utilizzando l’API ProofHQ. Per ulteriori informazioni, consulta [Crea una bozza utilizzando le API Workfront e ProofHQ (consigliato)](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended) nel presente articolo

### Esempio

Questo esempio mostra i campi e la formattazione utilizzabili per la creazione di JSON per `advancedProofingOptions` parametro . Le `advancedProofingOptions` Il file JSON può avere più o meno campi rispetto a quanto mostrato qui.

**Esempio:**

<!-- [Copy](javascript:void(0);) -->

```
{
    "stages": [
        {
            "name": "stage1",
            "lockOn": 1,
            "position": 1,
            "isPrivate": false,
            "activateOn": 1,
            "recipients": [
                {
                    "name": "",
                    "role": 5,
                    "email": "user1_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": null
                },
                {
                    "name": "",
                    "role": 5,
                    "email": "user2_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": false
                }
            ],
            "isMandatory": false,
            "deadlineDate": null,
            "deadlineTime": null,
            "isOneApproval": true,
            "activateOnDate": null,
            "parentPosition": null,
            "activateOnDecision": null,
            "deadlineCalculateOn": null,
            "deadlineBusinessDays": null
        }
    ],
    "message": "",
    "subject": "",
    "templates": [],
    "hasMessage": true,
    "canDownload": true,
    "customfields": [],
    "hasPublicSharing": true,
    "isAutomatedWorkflow": true,
    "stageBasedVisibility": 0
}
```
