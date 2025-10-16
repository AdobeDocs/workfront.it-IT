---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 'Invia  [!DNL Adobe Workfront] aggiornamenti ore effettive a una voce di elenco  [!DNL Anaplan] '
description: Questo scenario di integrazione condivide i dettagli relativi alle ore effettive acquisiti in un progetto  [!DNL Adobe Workfront]  con una voce di elenco  [!DNL Anaplan]  di budget. La condivisione di queste informazioni ti consente di sfruttare al meglio l'ottimizzazione della spesa e l'analisi finanziaria fornite da  [!DNL Anaplan] .
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: d3f234313677d916318c181c91cb951948454006
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 0%

---

# Invia aggiornamenti di [!DNL Adobe Workfront] ore effettive a una voce di elenco [!DNL Anaplan]

Questo scenario di integrazione condivide i dettagli delle ore effettive acquisiti in un progetto [!DNL Adobe Workfront] con una voce di elenco budget [!DNL Anaplan]. La condivisione di queste informazioni consente di sfruttare al meglio l&#39;ottimizzazione delle spese e l&#39;analisi finanziaria fornite da [!DNL Anaplan].

Questo modello di scenario fornisce un elenco delle ore riepilogate per progetto, giorno e ruolo registrate nei progetti attivi negli ultimi 3 mesi.

>[!IMPORTANT]
>
>&quot;Campaign&quot; in questo articolo si riferisce al caso di utilizzo della campagna di marketing che questo scenario rappresenta e non è in alcun modo connesso al connettore Adobe Campaign [!DNL Workfront Fusion] o all&#39;oggetto [!UICONTROL Campaign] deprecato di recente in [!DNL Workfront].

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi pacchetto di flusso di lavoro Adobe Workfront e qualsiasi pacchetto di automazione e integrazione Adobe Workfront</p><p>Workfront Ultimate</p><p>Pacchetti Workfront Prime e Select, con un ulteriore acquisto di Workfront Fusion.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Licenze Adobe Workfront</td> 
   <td> <p>Standard</p><p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront Fusion</td> 
   <td>
   <p>Basato su operazioni: nessun requisito di licenza Workfront Fusion</p>
   <p>Basato su connettore (legacy): Workfront Fusion for Work Automation and Integration </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Se la tua organizzazione dispone di un pacchetto Select o Prime Workfront che non include l’automazione e l’integrazione di Workfront, deve acquistare Adobe Workfront Fusion.</li></ul>
   </td> 
  </tr>
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Per informazioni sulle licenze di Adobe Workfront Fusion, vedere [Licenze di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

## Evento di attivazione

L’esecuzione di questo scenario è pianificata ogni 15 minuti.

## Configurazione [!DNL Workfront] prevista

Per utilizzare questo scenario, è necessario disporre dei seguenti elementi in [!DNL Workfront]:

* Un profilo utente in [!DNL Workfront] denominato **[!UICONTROL Integrazione Anaplan]**, con diritti di amministratore di sistema.

  Per informazioni sulla creazione di un utente in [!DNL Workfront], vedere [Aggiungere utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configurazione [!DNL Anaplan] prevista

Per utilizzare questo scenario, è necessario disporre dei seguenti elementi in [!DNL Anaplan]:

* Un profilo utente in [!DNL Anaplan] denominato Integrazione **[!UICONTROL [!DNL Workfront]]**, con diritti di amministratore di sistema.
* Modello [!DNL Anaplan] che si desidera utilizzare per questo scenario.
* Elenco all&#39;interno del modello [!DNL Anaplan] che si desidera utilizzare per questo scenario.
* File in [!DNL Anaplan] denominato **[!UICONTROL Importazione ore effettive Anaplan]** contenente le colonne seguenti, nell&#39;ordine seguente:

   1. [!UICONTROL GUID progetto Workfront]

   2. [!UICONTROL Ore]

   3. [!UICONTROL Ore Costo Stimato]

   4. [!UICONTROL Data di ingresso]

   5. [!UICONTROL Nome ruolo]

   6. [!UICONTROL Nome campagna]

   7. [!UICONTROL [!DNL Anaplan] ID elemento elenco]

  Per preparare il file della nota spese effettiva [!DNL Anaplan]:

   1. Copiare e incollare quanto segue in un editor di testo o [!DNL Excel]
   1. Salva il file in formato CSV
   1. Carica il file in [!DNL Anaplan].

      Per istruzioni, vedere la documentazione di [!DNL Anaplan] sull&#39;importazione di dati nei moduli da un file.

   1. Prendere nota del nome assegnato al file, che verrà utilizzato durante la distribuzione del modello di scenario [!UICONTROL Fusion].

  Esempio di contenuto CSV

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>[!DNL Workfront] Project GUID,Hours,Hours Estimated Cost,Entry Date,Role Name,Workfront Project Name,Item ID<br>6218062a000d0442903fcfa21e11f556,2,0,3/7/22,Designer,New Project 6,202000001030</code></pre>

* Un processo di **[!UICONTROL Importazione ore effettive progetto]** preparato per eseguire l&#39;importazione dei dati consegnati in un caricamento di file.

Per istruzioni su una di queste azioni, vedere la documentazione di [!DNL Anaplan].

## Distribuzione in [!DNL Workfront Fusion]

Per distribuire lo scenario di integrazione all&#39;account [!DNL Fusion], completare i passaggi seguenti. Questa operazione deve essere eseguita solo dopo aver completato la configurazione [!DNL Workfront] e [!DNL Anaplan] richieste.

1. Passa al menu [!UICONTROL Modelli] in [!DNL Workfront Fusion] e fai clic sul modello di scenario **[!UICONTROL Invia aggiornamenti delle ore effettive di Workfront a [!DNL Anaplan] elemento di elenco]**.
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
      <td role="rowheader">[!UICONTROL Nome elenco campagne]</td> 
      <td>Il nome dell'elenco dall'account [!DNL Anaplan] e dall'area di lavoro e dal modello selezionati.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome File: Importazione Ore Effettive]</td> 
      <td> <p>Nome del file che riceverà i dati relativi alle ore effettive del progetto.</p> <p> (Esempio: WorkfrontUpdateLinkedProjects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome processo: Importazione ore effettive]</td> 
      <td> <p>Il nome del processo che eseguirà l’importazione dei dati delle ore del progetto.</p> <p>(Esempio: Intero WF - Carica ore progetto per ruolo)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Sottodominio]</td> 
      <td>Il sottodominio dell'account [!DNL Workfront]. Viene utilizzato per creare un collegamento al progetto [!DNL Workfront] in una nota che potrebbe essere generata.</td> 
     </tr> 
    </tbody> 
   </table>

   I dettagli sulla configurazione dei file e dei processi sono forniti nella documentazione di installazione di [!DNL Anaplan].

1. Selezionare o aggiungere un profilo di connessione [!DNL Anaplan].
1. Aggiorna tutti i moduli [!DNL Anaplan] rimanenti con una connessione [!DNL Anaplan], quando richiesto.
1. Selezionare o aggiungere un profilo di connessione [!DNL Workfront].
1. Aggiorna tutti i moduli [!DNL Workfront] rimanenti con una connessione [!DNL Workfront], quando richiesto.

## Altri modelli di scenario consigliati

Questo modello di scenario è completato dai seguenti modelli di scenario di ottimizzazione spesa che possono anche essere distribuiti:

* [[!UICONTROL Invia [!DNL Adobe Workfront] aggiornamenti di progetto a una [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Invia [!DNL Adobe Workfront] spese a una [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Scenari aggiuntivi per il collegamento delle richieste di budget:

* [[!UICONTROL Crea una [!DNL Anaplan] voce di elenco da una [!DNL Adobe Workfront] richiesta budget]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Applica un [!DNL Anaplan] allocazione budget a un [!DNL Adobe Workfront] progetto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Scenari aggiuntivi per il collegamento delle richieste di campagne:

* [[!UICONTROL Crea un [!DNL Anaplan] elemento di elenco da una [!DNL Adobe Workfront] richiesta campagna]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Applica un [!DNL Anaplan] allocazione budget a una [!DNL Adobe Workfront] richiesta campagna o progetto campagna]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
