---
title: Creare o modificare uno stato
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
description: In qualità di amministratore di Adobe Workfront, puoi creare stati personalizzati per progetti, attività e problemi.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 35c804b5-569d-4ba8-84b8-6129f0ffbc7f
source-git-commit: f3785c66b979cc95bf1d2d2ccacbdeefe0ef0967
workflow-type: tm+mt
source-wordcount: '974'
ht-degree: 2%

---

# Creare o modificare uno stato

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT SENSITIVE HELP LINKS.-->

In qualità di amministratore di Adobe Workfront, puoi creare stati personalizzati per progetti, attività e problemi. Possono essere per gli utenti di tutto il sistema Workfront o per gruppi o sottogruppi specifici. Per ulteriori informazioni sugli stati, consulta [Panoramica sugli stati](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

>[!NOTE]
>
>Gli amministratori dei gruppi possono anche creare i propri stati di gruppo, da utilizzare solo per i gruppi. Per ulteriori informazioni, consulta [Creare o modificare uno stato di gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Requisiti di accesso

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
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Creare o modificare uno stato personalizzato

Puoi aggiungere uno stato personalizzato da utilizzare per l’intera organizzazione o per un singolo gruppo.

Quando crei uno stato personalizzato per l’intera organizzazione, puoi configurarlo in modo che tutti i gruppi nel sistema possano usarlo senza modificarlo. Oppure puoi configurarlo in modo che gli amministratori dei gruppi possano modificarlo per i loro gruppi, come spiegato in [Creare o modificare uno stato di gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Preferenze del progetto** > **Stati**.

1. (Condizionale) Se crei o modifichi uno stato per l’utilizzo a livello di sistema, assicurati che **Stati del sistema** è selezionato nella casella nell&#39;angolo superiore destro.

   ![](assets/system-statuses-in-upper-rt-corner.jpg)

   Oppure

   Se lo stato è per un gruppo o sottogruppo, inizia a digitare il nome del gruppo nell’angolo in alto a destra, quindi selezionalo quando viene visualizzato.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Seleziona la scheda del tipo di oggetto (**Progetto**, **Attività** oppure **Problemi**) che si desidera associare allo stato.

1. Se stai creando un nuovo stato, fai clic su **Aggiungi un nuovo stato**.

   Oppure

   Se stai modificando uno stato esistente, passa il puntatore del mouse su di esso, quindi fai clic sul pulsante **Modifica** che viene visualizzata all’estrema destra.

   ![](assets/custom-status-edit.png)

1. Configura lo stato utilizzando le seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome stato</td> 
      <td> <p>Digitare un nome per lo stato. Questo è un campo obbligatorio.</p> <p>Quando crei un nome di stato, tieni presente che altri utenti del sistema possono creare uno stato con lo stesso nome. È consigliabile utilizzare un nome univoco per evitare confusione durante la selezione degli stati in Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>(Facoltativo) Immetti una descrizione dello stato. Questo comunica il suo scopo a coloro che lo utilizzano.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clr icn</td> 
      <td> <p>Per personalizzare il colore dello stato, fai clic sul campo del colore e seleziona un colore dal pannello Campione. È inoltre possibile immettere un numero esadecimale nel campo .</p> <p>Il colore di stato viene visualizzato nell’angolo superiore destro di Workfront quando un utente visualizza l’oggetto.</p> <img src="assets/status-color.png" style="width: 350;height: 211;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Equivale a</td> 
      <td> <p>Selezionare dall’elenco una delle opzioni che meglio descrive la funzione dello stato. Ad esempio, se il nome dello stato è Fine, l’opzione con cui viene equiparato dovrebbe essere Completa.</p> <p>Ogni stato deve corrispondere a una di queste opzioni, in quanto determina il funzionamento dello stato.</p> <p>Questa opzione non può essere modificata dopo la creazione dello stato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chiave</td> 
      <td> <p>Se si sta creando un nuovo stato, digitare un codice o un'abbreviazione per lo stato o utilizzare quello generato per te. Questa chiave deve essere univoca in Workfront perché può essere utilizzata a scopo di reporting. Se si tenta di specificare una chiave già in uso nel sistema, il campo diventa rosso.</p> <p>Potrebbe essere utile utilizzare un’abbreviazione riconoscibile da chi la utilizzerà.</p> <p>Questa opzione non può essere modificata dopo la creazione dello stato.</p> <p>Non è possibile modificare il codice chiave per gli stati Planning, Current e Complete. Questo è importante se si crea un rapporto in modalità testo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nascondi stato</td> 
      <td> <p>(Solo stati progetto e attività)</p> <p>Abilita questa opzione se desideri che lo stato sia nascosto agli utenti. Se è disabilitata (impostazione predefinita), tutti gli utenti del sistema possono utilizzare lo stato .</p> <p>Puoi nascondere lo stato di un problema disattivando tutti e 4 i tipi di problema (Segnalazione bug, Modifica ordine, Problema, Richiesta).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Blocca per tutti i gruppi</td> 
      <td>
       <p>Quando uno stato è bloccato, gli utenti di tutto il sistema possono visualizzarlo e utilizzarlo e gli amministratori di gruppo non possono personalizzarlo per i loro gruppi.</p> 
       <p>Quando uno stato viene sbloccato, gli amministratori di gruppo possono personalizzarlo per i singoli gruppi.</p>

   <div>
       <p>È possibile utilizzare sia lo stato bloccato che quello sbloccato in un processo di approvazione del sistema. Se si crea un processo di approvazione del sistema con uno stato di sistema sbloccato, gli utenti di tutto il sistema possono allegare il processo di approvazione a qualsiasi progetto, attività o problema nel sistema.</p>
       <p> Nei seguenti scenari, vengono visualizzati messaggi di avviso per consentire a te e agli utenti di comprendere i risultati dello sblocco di uno stato:</p>
       <ul>
       <li>Un amministratore sblocca lo stato a livello di sistema utilizzato in un processo di approvazione. Un messaggio avverte che potrebbe eliminare lo stato sbloccato per i gruppi, impedendo ai membri del gruppo di utilizzare correttamente il processo di approvazione per gli oggetti assegnati al gruppo.</li>
       <li>Un utente inizia a modificare un processo di approvazione che utilizza uno stato sbloccato. Un messaggio avvisa l’utente dello stato sbloccato in modo che possa valutare se sia opportuno bloccarlo nuovamente o sostituirlo.</li>
       <li>Un processo di approvazione a livello di sistema con stato sbloccato viene allegato a un oggetto e lo stato viene eliminato per il gruppo assegnato all'oggetto. Quando un membro del gruppo passa alla sezione Approvazioni per l'oggetto, un messaggio spiega che il processo di approvazione non può essere avviato per l'oggetto.</li>
       </ul>
       <p>Per ulteriori informazioni sul blocco degli stati, consulta <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md" class="MCXref xref">Stati bloccati e sbloccati a livello di sistema</a>.</p>
       </div>
      </td>
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

   Per istruzioni su come impostare questo stato come predefinito, consulta [Usa stati personalizzati come stati predefiniti](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

Per informazioni sul riordinamento degli stati dei gruppi, consulta [Riordinare gli stati a livello di sistema e di gruppo](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).
