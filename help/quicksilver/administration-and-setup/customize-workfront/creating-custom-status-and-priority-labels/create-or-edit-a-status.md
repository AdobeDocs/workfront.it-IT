---
title: Creare o modificare uno stato
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
description: In qualità di amministratore di Adobe Workfront, puoi creare stati personalizzati per progetti, attività e problemi.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 35c804b5-569d-4ba8-84b8-6129f0ffbc7f
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 2%

---

# Creare o modificare uno stato

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT SENSITIVE HELP LINKS.-->

In qualità di amministratore di Adobe Workfront, puoi creare stati personalizzati per progetti, attività e problemi. Possono essere destinati agli utenti di tutto il sistema Workfront o a gruppi o sottogruppi specifici. Per ulteriori informazioni sugli stati, vedere [Panoramica sugli stati](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

>[!NOTE]
>
>Gli amministratori di gruppi possono anche creare i propri stati di gruppo, utilizzabili solo dai loro gruppi. Per ulteriori informazioni, vedere [Creare o modificare lo stato di un gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
     <p>Nuovo: Standard</p>
     <p>oppure</p>
     <p>Corrente: Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare o modificare uno stato personalizzato

Puoi aggiungere uno stato personalizzato da utilizzare per l’intera organizzazione o per un singolo gruppo.

Quando crei uno stato personalizzato per l’intera organizzazione, puoi configurarlo in modo che tutti i gruppi del sistema possano utilizzarlo senza modificarlo. Oppure puoi configurarlo in modo che gli amministratori dei gruppi possano modificarlo per i loro gruppi, come spiegato in [Creare o modificare lo stato di un gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Preferenze progetto** > **Stati**.

1. (Condizionale) Se stai creando o modificando uno stato per l&#39;uso a livello di sistema, assicurati che **Stati di sistema** sia selezionato nella casella in alto a destra.

   ![Stati di sistema](assets/system-statuses-in-upper-rt-corner-new.jpg)

   Oppure

   Se lo stato è per un gruppo o un sottogruppo, iniziare a digitare il nome del gruppo nell&#39;angolo superiore destro, quindi selezionarlo quando viene visualizzato.

   ![Stati di sistema per il gruppo](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Selezionare la scheda del tipo di oggetto (**Progetto**, **Attività** o **Problemi**) che si desidera associare allo stato.

1. Se stai creando un nuovo stato, fai clic su **Aggiungi nuovo stato**.

   Oppure

   Se stai modificando uno stato esistente, passa il puntatore del mouse su di esso, quindi fai clic sull&#39;icona **Modifica** visualizzata all&#39;estrema destra.

   ![Modifica stato personalizzato](assets/custom-status-edit.png)

1. Configura lo stato utilizzando le seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome stato</td> 
      <td> <p>Digita un nome per lo stato. Questo è un campo obbligatorio.</p> <p>Quando crei un nome di stato, tieni presente che altri utenti nel sistema possono creare uno stato con lo stesso nome. È consigliabile utilizzare un nome univoco per evitare confusione durante la selezione degli stati in Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>(Facoltativo) Digita una descrizione dello stato. Questo comunica il suo scopo a coloro che lo usano.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Colore</td> 
      <td> <p>Personalizzate il colore dello stato facendo clic sul campo del colore e selezionando un colore dal pannello Campione. Puoi anche immettere un numero esadecimale nel campo.</p> <p>Il colore dello stato viene visualizzato nell’angolo superiore destro di Workfront quando un utente visualizza l’oggetto.</p> <img src="assets/status-color.png" style="width: 350;height: 211;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Equivale a</td> 
      <td> <p>Seleziona una delle opzioni dall’elenco che descrive meglio la funzione dello stato. Ad esempio, se il nome dello stato è Fatto (Done), l'opzione corrispondente deve essere Completa.</p> <p>Ogni stato deve corrispondere a una di queste opzioni, in quanto determina il funzionamento dello stato.</p> <p>Questa opzione non può essere modificata dopo la creazione dello stato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chiave</td> 
      <td> <p>Se si sta creando un nuovo stato, digitare un codice o un'abbreviazione per lo stato oppure utilizzare quello generato automaticamente. Questa chiave deve essere univoca in Workfront perché può essere utilizzata a scopo di reporting. Se si tenta di specificare una chiave già in uso nel sistema, il campo diventa rosso.</p> <p>Potrebbe essere utile utilizzare un’abbreviazione riconoscibile da coloro che la utilizzeranno.</p> <p>Questa opzione non può essere modificata dopo la creazione dello stato.</p> <p>Non è possibile modificare il codice chiave per gli stati Pianificazione, Corrente e Completo. Questo è importante se stai creando un rapporto in modalità testo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nascondi stato</td> 
      <td> <p>(Solo stati Progetto e Attività)</p> <p>Abilita questa opzione se desideri che lo stato sia nascosto agli utenti. Quando questa opzione è disattivata (impostazione predefinita), tutti gli utenti del sistema possono utilizzare lo stato.</p> <p>È possibile nascondere lo stato di un problema disabilitando questa opzione per tutti e 4 i tipi di problemi (Rapporto bug, Ordine di modifica, Problema, Richiesta).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Blocca per tutti i gruppi</td> 
      <td>
       <p>Quando uno stato è bloccato, gli utenti di tutto il sistema possono visualizzarlo e utilizzarlo e gli amministratori dei gruppi non possono personalizzarlo per i loro gruppi.</p> 
       <p>Quando uno stato viene sbloccato, gli amministratori dei gruppi possono personalizzarlo per i singoli gruppi.</p>

   <div>
       <p>In un processo di approvazione di sistema è possibile utilizzare sia gli stati bloccato che quello sbloccato. Se si crea un processo di approvazione del sistema con uno stato di sistema sbloccato, gli utenti di tutto il sistema possono allegare il processo di approvazione a qualsiasi progetto, attività o problema del sistema.</p>
       <p> Negli scenari seguenti, vengono visualizzati messaggi di avviso per aiutare te e i tuoi utenti a comprendere i risultati dello sblocco di uno stato:</p>
       <ul>
       <li>Un amministratore sblocca uno stato a livello di sistema utilizzato in un processo di approvazione. Viene visualizzato un messaggio di avviso che indica che lo stato sbloccato per i gruppi potrebbe essere eliminato, impedendo così ai membri del gruppo di utilizzare correttamente il processo di approvazione per gli oggetti assegnati al gruppo.</li>
       <li>Un utente inizia a modificare un processo di approvazione che utilizza uno stato sbloccato. Un messaggio avvisa l’utente dello stato sbloccato, in modo che possa valutare se è consigliabile bloccarlo di nuovo o sostituirlo.</li>
       <li>Un processo di approvazione a livello di sistema con uno stato sbloccato viene associato a un oggetto e lo stato è stato eliminato per il gruppo assegnato all'oggetto. Quando un membro del gruppo accede alla sezione Approvazioni per l'oggetto, un messaggio spiega che il processo di approvazione non può essere avviato per l'oggetto.</li>
       </ul>
       <p>Per ulteriori informazioni sugli stati di blocco, vedere <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md" class="MCXref xref">Stati di sistema bloccati e sbloccati</a>.</p>
       </div>
      </td>
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

   Per istruzioni su come impostare questo stato come predefinito, vedere [Utilizzare gli stati personalizzati come predefiniti](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

Per informazioni sul riordinamento degli stati dei gruppi, vedere [Riordinare gli stati a livello di sistema e di gruppo](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).
