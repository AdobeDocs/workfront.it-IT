---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Invia [!DNL Adobe Workfront] spese a una [!DNL Anaplan] voce di elenco
description: Questo scenario di integrazione condivide i dettagli relativi alle spese di un progetto  [!DNL Adobe Workfront]  con una voce di elenco  [!DNL Anaplan]  di budget. La condivisione di queste informazioni ti consente di sfruttare al meglio l'ottimizzazione della spesa e l'analisi finanziaria fornite da  [!DNL Anaplan] .
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 0%

---

# Invia [!DNL Adobe Workfront] spese a una voce di elenco [!DNL Anaplan]

Questo scenario di integrazione condivide i dettagli relativi alle spese di un progetto [!DNL Adobe Workfront] con una voce di elenco budget [!DNL Anaplan]. La condivisione di queste informazioni consente di sfruttare al meglio l&#39;ottimizzazione delle spese e l&#39;analisi finanziaria fornite da [!DNL Anaplan].

>[!IMPORTANT]
>
>&quot;Campaign&quot; in questo articolo si riferisce al caso di utilizzo della campagna di marketing che questo scenario rappresenta e non è in alcun modo connesso al connettore Adobe Campaign [!DNL Workfront Fusion] o all&#39;oggetto [!UICONTROL Campaign] deprecato di recente in [!DNL Workfront].

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o versione successiva</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>Workfront Fusion per l'automazione e l'integrazione del lavoro </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

&#42;&#42;Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Evento di attivazione

L’esecuzione di questo scenario è pianificata ogni 15 minuti.

## Configurazione [!DNL Workfront] prevista

Per utilizzare questo scenario, è necessario disporre dei seguenti elementi in [!DNL Workfront]:

* Un profilo utente in [!DNL Workfront] denominato *[!UICONTROL *[!DNL Anaplan] Integration]**, con diritti di amministratore di sistema.

  Per informazioni sulla creazione di un utente in [!DNL Workfront], vedere [Aggiungere utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Modulo personalizzato **[!UICONTROL Brief campagna]** allegato all&#39;oggetto del progetto per memorizzare i valori dei dati personalizzati che si desidera inviare a [!DNL Anaplan].

  Il modulo deve contenere i seguenti campi:

  | Nome Campo | Tipo di campo |
  |---|---|
  | [!UICONTROL Data ultima trasmissione] | Data |
  | [!UICONTROL Note di integrazione] | Campo di testo paragrafo |

  Per informazioni sulla creazione di moduli personalizzati, vedere [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Configurazione [!DNL Anaplan] prevista

Per utilizzare questo scenario, è necessario disporre dei seguenti elementi in [!DNL Anaplan]:

* Un profilo utente in [!DNL Anaplan] denominato Integrazione **[!UICONTROL [!DNL Workfront]]**, con diritti di amministratore di sistema.
* Modello [!DNL Anaplan] che si desidera utilizzare per questo scenario.
* Elenco all&#39;interno del modello [!DNL Anaplan] che si desidera acquisire i budget delle campagne.
* Un file **[!UICONTROL Importazione spese effettive Anaplan]** contenente le colonne seguenti, nell&#39;ordine seguente:

   1. [!UICONTROL [!DNL Workfront] GUID spesa]

   2. [!UICONTROL [!DNL Workfront] GUID progetto]

   3. [!UICONTROL Importo effettivo]

   4. [!UICONTROL Descrizione]

   5. [!UICONTROL Tipo Spesa]

   6. [!UICONTROL Data di validità]

   7. [!UICONTROL Nome campagna]

   8. [!UICONTROL [!DNL Anaplan] ID elemento elenco]

  Per preparare il file [!UICONTROL [!DNL Anaplan] Importazione spese effettive]:

   1. Copiare e incollare quanto segue in un editor di testo o in [!DNL Excel].
   1. Salva il file in formato CSV.
   1. Carica il file in [!DNL Anaplan].

      Per istruzioni, vedere la documentazione di [!DNL Anaplan] sull&#39;importazione di dati nei moduli da un file.

   1. Prendere nota del nome assegnato al file, che verrà utilizzato durante la distribuzione del modello di scenario [!UICONTROL Fusion].

  Esempio di contenuto CSV

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Actual Amount","Description","Expense Type","Effective Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","2345","Expense 1","","2022-03-09","New Project 6","202000001030"</code></pre>

* Un file **[!UICONTROL [!DNL Anaplan]di Importazione spese pianificata]** contenente le colonne seguenti, nell&#39;ordine seguente:

   1. [!UICONTROL [!DNL Workfront] GUID spesa]

   2. [!UICONTROL [!DNL Workfront] GUID progetto]

   3. [!UICONTROL Importo effettivo]

   4. [!UICONTROL Descrizione]

   5. [!UICONTROL Tipo Spesa]

   6. [!UICONTROL Data di validità]

   7. [!UICONTROL Nome campagna]

   8. [!UICONTROL [!DNL Anaplan] ID elemento elenco]

  Per preparare il file [!UICONTROL [!DNL Anaplan] Importazione spese pianificata]:

   1. Copiare e incollare quanto segue in un editor di testo o [!DNL Excel]
   1. Salva il file in formato CSV
   1. Carica il file in Anaplan.

      Per istruzioni, vedere la documentazione di [!DNL Anaplan] sull&#39;importazione di dati nei moduli da un file.

   1. Prendere nota del nome assegnato al file, che verrà utilizzato durante la distribuzione del modello di scenario [!UICONTROL Fusion].

  Esempio di contenuto CSV

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Planned Amount","Description","Expense Type","Planned Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","1234","Expense 1","Entertainment","2022-03-08","New Project 6","202000001030"</code></pre>


* Un processo **[!UICONTROL Importazione aggiornamento progetto]** preparato per eseguire l&#39;importazione dei dati consegnati in un caricamento di file.

>[!NOTE]
>
>Esistono file di importazione separati per le spese pianificate ed effettive in modo che possano essere riportate in modo indipendente rispettivamente nelle date pianificate ed effettive.

Per istruzioni su una di queste azioni, vedere la documentazione di [!DNL Anaplan].

## Distribuzione in [!DNL Fusion]

Per distribuire lo scenario di integrazione all&#39;account [!DNL Fusion], completare i passaggi seguenti. Questa operazione deve essere eseguita solo dopo aver completato la configurazione [!DNL Workfront] e [!DNL Anaplan] richieste.

1. Passa al menu [!UICONTROL Modelli] in [!DNL Workfront Fusion] e fai clic sul **[!UICONTROL Invia aggiornamenti delle spese di Workfront al modello di scenario [!DNL Anaplan] elemento di elenco]**.
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
      <td>ID dell'area di lavoro dall'account [!DNL Anaplan] che si desidera utilizzare per questo scenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID modello] </td> 
      <td>ID del modello dall'account [!DNL Anaplan] e dall'area di lavoro selezionata che si desidera utilizzare per questo scenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome elenco campagne]</td> 
      <td>Il nome dell'elenco dall'account [!DNL Anaplan], dall'area di lavoro selezionata e dal modello che si desidera utilizzare per questo scenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome File: Importazione Spese Effettive]</td> 
      <td> <p>Nome del file che riceverà i dati relativi alle spese effettive del progetto.</p> <p> (Esempio: WorkfrontUpdateLinkedProjects_ActExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome File: Importazione Spesa Pianificata]</td> 
      <td> <p>Nome del file che riceverà i dati delle spese pianificate del progetto.</p> <p> (Esempio: WorkfrontUpdateLinkedProjects_PlannedExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome processo: importazione aggiornamento progetto]</td> 
      <td> <p>Nome del processo che eseguirà l'importazione dei dati di spesa del progetto.</p> <p>(Esempio: Intero WF - Carica spese progetto)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   I dettagli sulla configurazione dei file e dei processi sono forniti nella documentazione di installazione di [!DNL Anaplan].

1. Selezionare o aggiungere un profilo di connessione [!DNL Anaplan].
1. Aggiorna tutti i moduli [!DNL Anaplan] rimanenti con una connessione [!DNL Anaplan], quando richiesto.
1. Selezionare o aggiungere un profilo di connessione [!DNL Workfront].
1. Aggiorna tutti i moduli [!DNL Workfront] rimanenti con una connessione [!DNL Workfront], quando richiesto.
1. Nel modulo **[!UICONTROL Genera CSV spese effettive]**, aggiungi una nuova struttura di dati per mappare gli attributi del progetto alle colonne CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Actual Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Effective Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

1. Nel modulo **[!UICONTROL Genera CSV]** delle spese pianificate, aggiungi una nuova struttura di dati per mappare gli attributi del progetto alle colonne CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Planned Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Planned Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

## Altri modelli di scenario consigliati

Questo modello di scenario è completato dai seguenti modelli di scenario di ottimizzazione spesa che possono anche essere distribuiti:

* [[!UICONTROL Invia [!DNL Adobe Workfront] aggiornamenti di progetto a una [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Invia [!DNL Adobe Workfront] aggiornamenti ore effettive a una [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

Scenari aggiuntivi per il collegamento delle richieste di budget:

* [[!UICONTROL Crea una [!DNL Anaplan] voce di elenco da una [!DNL Adobe Workfront] richiesta budget]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Applica un [!DNL Anaplan] allocazione budget a un [!DNL Adobe Workfront] progetto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Scenari aggiuntivi per il collegamento delle richieste di campagne:

* [[!UICONTROL Crea un [!DNL Anaplan] elemento di elenco da una [!DNL Adobe Workfront] richiesta campagna]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Applica un [!DNL Anaplan] allocazione budget a una [!DNL Adobe Workfront] richiesta campagna o progetto campagna]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
