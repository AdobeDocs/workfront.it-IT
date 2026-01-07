---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 'Applica un''allocazione di budget di  [!DNL Anaplan]  a un progetto di  [!DNL Adobe Workfront] '
description: Questo scenario di integrazione sincronizza tutte le allocazioni di budget che sono state effettuate in [!DNL Anaplan] indietro a [!DNL Workfront]. Lo scenario richiama tutte le voci di budget della campagna collegate, quindi passa il valore preventivato al progetto Workfront collegato se il valore del budget è stato modificato.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 9b8add8f-1978-4ab4-87ac-f1159e7d6cbb
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 16%

---

# Applica un&#39;allocazione budget [!DNL Anaplan] a un progetto [!DNL Adobe Workfront]

Questo scenario di integrazione sincronizza tutte le allocazioni di budget effettuate in [!DNL Anaplan] in [!DNL Workfront]. Lo scenario richiama tutte le voci di budget della campagna collegate, quindi passa il valore preventivato al progetto [!DNL Workfront] collegato se il valore del budget è stato modificato.

>[!IMPORTANT]
>
>&quot;Campaign&quot; in questo articolo si riferisce al caso di utilizzo della campagna di marketing che questo scenario rappresenta e non è in alcun modo connesso al connettore Adobe Campaign [!DNL Workfront Fusion] o all&#39;oggetto [!UICONTROL Campaign] deprecato di recente in [!DNL Workfront].

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi pacchetto Workflow di Adobe Workfront, e qualsiasi pacchetto Automation and Integration di Adobe Workfront.</p><p>Workfront Ultimate</p><p>Pacchetti Workfront Prime e Select, con un ulteriore acquisto di Workfront Fusion.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Licenze Adobe Workfront</td> 
   <td> <p>Standard</p><p>Work o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront Fusion</td> 
   <td>
   <p>Basata sulle operazioni: nessun requisito di licenza Workfront Fusion</p>
   <p>Basata su connettore (precedente): Workfront Fusion for Work Automation and Integration </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Se la tua organizzazione dispone di un pacchetto Workfront Select o Prime che non include Workfront Automation and Integration, dovrà acquistare Adobe Workfront Fusion.</li></ul>
   </td> 
  </tr>
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Per informazioni sulle licenze di Adobe Workfront Fusion, consulta [Licenze di Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

+++

## Evento di attivazione

L’esecuzione di questo scenario è pianificata ogni 15 minuti.

## Configurazione [!DNL Workfront] prevista

Per utilizzare questo scenario, è necessario disporre dei seguenti elementi in [!DNL Workfront]:

* Un profilo utente in [!DNL Workfront] denominato **Integrazione Anaplan**, con diritti di amministratore di sistema.

  Per informazioni sulla creazione di un utente in [!DNL Workfront], vedere [Aggiungere utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configurazione [!DNL Anaplan] prevista

Per utilizzare questo scenario, è necessario disporre dei seguenti elementi in [!DNL Anaplan]:

* Un profilo utente in [!DNL Anaplan] denominato Integrazione **[!DNL Workfront]**, con diritti di amministratore di sistema.
* Modello [!DNL Anaplan] che si desidera utilizzare per questo scenario.
* Elenco all&#39;interno del modello [!DNL Anaplan] che acquisisce i budget delle campagne.

  Il modulo dell’elenco deve supportare la ricezione dei seguenti attributi:

   * [!UICONTROL GUID progetto Workfront]
   * [!UICONTROL Nome campagna]
   * [!UICONTROL Fondi manodopera richiesti]
   * [!UICONTROL Ricavo stimato]
   * [!UICONTROL Marchio]

  Questo elenco e modulo devono memorizzare ulteriori dettagli necessari per la normale funzionalità di [!DNL Anaplan], inclusa la possibilità di impostare un budget e comunicare che la voce dell&#39;elenco di budget è pronta per essere sincronizzata nuovamente in [!DNL Workfront].

* Una visualizzazione in [!DNL Anaplan] denominata **[!UICONTROL Campagne.Aggiorna campagne in Adobe Workfront]**.

  Questa vista deve contenere le seguenti colonne, nell’ordine indicato:

   1. [!UICONTROL Nome elemento]

   2. [!UICONTROL [!DNL Workfront] GUID progetto]

   3. [!UICONTROL Nome campagna]

   4. [!UICONTROL Budget]

   5. [!UICONTROL Ricavo stimato]

   6. [!UICONTROL Marchio]

  La visualizzazione deve essere filtrata in modo da visualizzare gli elementi con GUID [!UICONTROL [!DNL Workfront] del progetto ] e alcuni indicatori che indicano che le allocazioni budget devono essere trasmesse a [!DNL Workfront].

Per istruzioni su una di queste azioni, vedere la documentazione di [!DNL Anaplan].

## Distribuzione in [!DNL Workfront Fusion]

Per distribuire lo scenario di integrazione all&#39;account [!DNL Fusion], completare i passaggi seguenti. Questa operazione deve essere eseguita solo dopo aver completato la configurazione [!DNL Workfront] e [!DNL Anaplan] richieste.

1. Passa al menu [!UICONTROL Modelli] in [!DNL Workfront Fusion] e fai clic sul modello di scenario **[!UICONTROL Applica allocazioni budget [!DNL Anaplan] ai progetti Workfront]**.
1. Sostituire i valori delle variabili per le seguenti [!DNL Anaplan] variabili:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>Nome variabile</th> 
      <th>Sostituisci valore con</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID Workspace]</td> 
      <td>ID di un'area di lavoro dall'account [!DNL Anaplan].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID modello] </td> 
      <td>L'ID di un modello dall'account [!DNL Anaplan] e dall'area di lavoro selezionata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Nome Modulo]</td> 
      <td>Il nome del modulo che descrive gli attributi della campagna nell'elenco [!DNL Anaplan] selezionato.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome elenco campagne]</td> 
      <td>Il nome dell'elenco dall'account [!DNL Anaplan] e dall'area di lavoro e dal modello selezionati.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Nome visualizzazione]</td> 
      <td> <p>Nome della visualizzazione che contiene i budget delle campagne pronti da trasmettere a [!DNL Workfront].</p> <p>(Esempio: [!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   I dettagli sulla configurazione dei file e dei processi sono forniti nella documentazione di installazione di [!DNL Anaplan].

1. Selezionare o aggiungere un profilo di connessione [!DNL Anaplan].
1. Aggiorna tutti i moduli [!DNL Anaplan] rimanenti con una connessione [!DNL Anaplan], quando richiesto.
1. Nel modulo **[!UICONTROL Converti CSV in oggetto JSON]**, aggiungi una nuova struttura di dati per mappare le colonne CSV su un oggetto JSON utilizzabile.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. Quando richiesto, seleziona questa struttura dati per altri moduli in questa distribuzione di scenario.
1. Nel modulo **[!UICONTROL Controlla progetto collegato]**, selezionare o aggiungere un profilo di connessione [!DNL Workfront].
1. Aggiorna tutti i moduli [!DNL Workfront] rimanenti con una connessione [!DNL Workfront], quando richiesto.

## Altri modelli di scenario consigliati

Per completare il flusso di lavoro rappresentato da questo modello, è necessario distribuire anche il seguente modello aggiuntivo:

* [[!UICONTROL Crea una [!DNL Anaplan] voce di elenco da una [!DNL Adobe Workfront] richiesta budget]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)

Altri scenari per l’ottimizzazione della spesa includono:

* [[!UICONTROL Invia [!DNL Adobe Workfront] aggiornamenti di progetto a una [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Invia [!DNL Adobe Workfront] aggiornamenti ore effettive a una [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Invia [!DNL Adobe Workfront] spese a una [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
