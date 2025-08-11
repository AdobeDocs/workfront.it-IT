---
title: Compilazione automatica di una richiesta da dati precedenti
content-type: reference
description: Puoi utilizzare l’intelligenza artificiale per compilare automaticamente i campi della richiesta utilizzando i dati di richieste precedenti.
author: Becky
feature: Get Started with Workfront
source-git-commit: cf2ae77ed27b1dd30144f6de31bec474f53f1efb
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---

# Compilazione automatica di una richiesta da dati precedenti

>[!NOTE]
>
>* Questa funzionalità sarà disponibile come versione open beta con la seguente pianificazione:
>
>   * Versione mensile: 11 settembre 2025
>   * Versione trimestrale: 16 ottobre 2025

L’intelligenza artificiale può aiutarti a compilare automaticamente i campi della richiesta in base alle richieste precedenti. Puoi approvare o rifiutare questi suggerimenti prima di inviare la richiesta.

La funzione di riempimento automatico non sovrascrive i campi già compilati.

Gli utenti non ricevono suggerimenti di dati a cui non hanno altrimenti accesso.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Nuovo: Collaboratore o versione successiva</p>
   Oppure
   <p>Corrente: richiesta o successiva</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Issues</p>  </td> 
  </tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td><p>Accesso per aggiungere richieste a una coda di richieste</p> <p>Visualizza o autorizzazioni superiori per la richiesta esistente</p> <p>Per informazioni sulla configurazione di una coda richieste, vedere <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda richieste</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Ottieni suggerimenti durante la compilazione del modulo

La compilazione automatica può suggerire i valori dei campi durante la compilazione del modulo. Quando si immettono valori nei campi della richiesta, Workfront li confronta con le richieste precedenti. Se il valore immesso è strettamente correlato con altri valori di campo in contesti simili in richieste precedenti, Workfront consiglia tali valori.

Ad esempio, se una clinica utilizza sempre lo stesso codice di fatturazione, Workfront suggerisce che il codice di fatturazione venga inserito nel campo appropriato quando viene inserito il nome della clinica.

Per utilizzare i suggerimenti basati sulle richieste precedenti:

1. Inizia a creare una richiesta.

   Per istruzioni, vedere [Creare e inviare richieste](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Inizia a compilare i campi.

   Durante la compilazione dei campi, è possibile che in altri campi vengano visualizzati suggerimenti.

1. Per ogni suggerimento di campo, selezionare **Accetta** o **Rifiuta** per il campo.

   ![Accetta o rifiuta suggerimento](assets/accept-reject-suggestion.png)

   Oppure

   Selezionare **Accetta tutti** o **Rifiuta tutti** nella parte superiore della pagina per accettare o rifiutare tutti i suggerimenti.

   >[!NOTE]
   >
   >Eventuali suggerimenti non rivisti verranno accettati automaticamente quando invii la richiesta.
