---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Aggiungere opzioni di verifica avanzate con l’API di Adobe Workfront
description: Aggiungere opzioni di verifica avanzate con l’API di Adobe Workfront
author: Becky
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 0%

---


# Aggiungere opzioni di verifica avanzate durante la creazione di una bozza tramite l’API Adobe Workfront

Durante la creazione di una bozza nell’API di Workfront, puoi aggiungere opzioni di bozza avanzate.

Utilizza uno dei seguenti flussi di lavoro per aggiungere opzioni di correzione a una bozza utilizzando l’API:

* (Consigliato) Crea una bozza semplice utilizzando l’API Workfront, quindi aggiungi opzioni di bozza avanzate alla bozza utilizzando l’API ProofHQ

* Creare una bozza con opzioni di verifica avanzate utilizzando JSON nell’API di Workfront

## Creare una bozza utilizzando le API Workfront e ProofHQ (consigliato) {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

Questa sezione descrive come creare una bozza con opzioni di verifica avanzate tramite l’API Workfront, utilizzando una combinazione di API Workfront e ProofHQ.

L’API ProofHQ include diverse azioni non disponibili per le bozze nell’API Workfront. Utilizzando queste azioni, puoi modificare o configurare la bozza con maggiore precisione di quanto non sia disponibile nell’API di Workfront.

Per una panoramica dell’API ProofHQ, vedi [Panoramica di PoofHQ](../../proofhq-api/general/overview.md). È inoltre possibile fare riferimento al [Documentazione di ProofHQ](https://api.proofhq.com/home.html).

>[!NOTE]
>
>* L’API Workfront è un’API REST-ful. L’API ProofHQ è un’API SOAP.
>* Le bozze create nell’API ProofHQ non vengono collegate automaticamente a Workfront. Pertanto, consigliamo di creare bozze nell’API Workfront prima di aggiornarle con l’API ProofHQ.
>

### Creare una bozza con opzioni di verifica avanzate

1. Creare una bozza utilizzando `Document createProof` nell’API di Workfront.

   >[!NOTE]
   >
   Durante la creazione della bozza, imposta `{}` come valore per `advancedProofingOptions` parametro.

1. Dopo aver creato la bozza, utilizza l’API ProofHQ per aggiungere opzioni avanzate.

### Esempi

Questa sezione mostra alcuni aggiornamenti che è possibile apportare con l’API ProofHQ.

**Esempi:**

* [È possibile scaricare una bozza, averne un messaggio e condividerla pubblicamente](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [Aggiornare una fase in modo che non sia privata, non obbligatoria e richieda una sola approvazione](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [Aggiungere due destinatari a una bozza senza decision maker primario](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**È possibile scaricare una bozza, averne un messaggio e condividerla pubblicamente**

La documentazione di questo endpoint è disponibile sul sito [ProofHQ API updateProof](https://api.proofhq.com/home/proofs/updateproof.html) pagina.

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

La documentazione di questo endpoint è disponibile sul sito [Aggiornamento API ProofHQWorkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html) pagina.

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

**Aggiungere due destinatari a una bozza senza decision maker primario**

La documentazione di questo endpoint è disponibile sul sito [AddWorkflowProofReviewers API ProofHQ](https://api.proofhq.com/addworkflowproofreviewers.html) pagina.

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

## Creare una bozza utilizzando JSON nell’API di Workfront

Questa sezione descrive come creare una bozza con opzioni di verifica avanzate tramite l’API Workfront, utilizzando JSON come valore di parametro nell’API Workfront

### Creare una bozza con opzioni di verifica avanzate

Puoi creare bozze tramite l’API Workfront utilizzando `Document createProof` azione. Questa azione accetta `advancedProofingOptions` parametro, che ha il tipo di valore `string`. Per includere opzioni di verifica avanzate nel `createProof` , è necessario immettere le opzioni nella `advancedProofingOptions` parametro in formato JSON.

>[!NOTE]
>
Può essere difficile prevedere i campi da includere nel JSON advancedProofingOptions. Puoi esaminare i dati di rete della tua organizzazione durante l’utilizzo della verifica avanzata in Workfront e basare il tuo JSON sui campi e i valori comunemente utilizzati dalla tua organizzazione.
>
Poiché questi campi possono essere difficili da prevedere, si consiglia di creare una bozza utilizzando l’API Workfront e quindi di aggiornarla utilizzando l’API ProofHQ. Per ulteriori informazioni, consulta [Creare una bozza utilizzando le API Workfront e ProofHQ (consigliato)](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended) in questo articolo

### Esempio

Questo esempio mostra i campi e la formattazione che è possibile utilizzare durante la creazione del codice JSON per `advancedProofingOptions` parametro. Il tuo `advancedProofingOptions` Il file JSON può avere un numero di campi maggiore o minore di quello mostrato qui.

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
