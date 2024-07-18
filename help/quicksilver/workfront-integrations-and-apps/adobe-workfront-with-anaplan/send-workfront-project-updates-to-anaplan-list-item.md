---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Invia aggiornamenti di  [!DNL Adobe Workfront] progetto a una [!DNL Anaplan] voce di elenco
description: Questo scenario di integrazione condivide i dettagli relativi all'avanzamento, allo stato e alla pianificazione chiave di un progetto  [!DNL Adobe Workfront]  con una voce di elenco del budget  [!DNL Anaplan] . La condivisione di queste informazioni ti consente di sfruttare al meglio l'ottimizzazione della spesa e l'analisi finanziaria fornite da  [!DNL Anaplan] .
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 0%

---

# Invia aggiornamenti del progetto [!DNL Adobe Workfront] a una voce di elenco [!DNL Anaplan]

Questo scenario di integrazione condivide i dettagli relativi all&#39;avanzamento, allo stato e alla pianificazione chiave di un progetto [!DNL Adobe Workfront] con una voce dell&#39;elenco di budget [!DNL Anaplan]. La condivisione di queste informazioni consente di sfruttare al meglio l&#39;ottimizzazione delle spese e l&#39;analisi finanziaria fornite da [!DNL Anaplan].

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

* Un profilo utente in [!DNL Workfront] denominato Integrazione **[!UICONTROL [!DNL Anaplan]]**, con diritti di amministratore di sistema.

  Per informazioni sulla creazione di un utente in [!DNL Workfront], vedere [Aggiungere utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Modulo personalizzato **[!UICONTROL Brief campagna]** allegato all&#39;oggetto del progetto per memorizzare i valori dei dati personalizzati che si sceglie di inviare ad Anaplan.

  I campi seguenti rappresentano esempi di campi che possono essere inclusi nel modulo personalizzato per facilitare la mappatura dei dati su Anaplan, ma non sono necessari per questo scenario di integrazione:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Nome Campo</th> 
     <th>Tipo di campo</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL Nella Data Di Inizio Del Mercato]</td> 
     <td>[!UICONTROL Date] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Nella Data Di Fine Del Mercato]</td> 
     <td>[!UICONTROL Date]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Panoramica di [!UICONTROL Campaign]</td> 
     <td>[!UICONTROL Paragrafo Campo Di Testo]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>[!UICONTROL Paragrafo Campo Di Testo]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>Elenco a discesa [!UICONTROL]</p> <p>Includi opzioni che si adattano ai tuoi processi.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Per informazioni sulla creazione di moduli personalizzati, vedere [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## Configurazione [!DNL Anaplan] prevista

Per utilizzare questo scenario, è necessario disporre dei seguenti elementi in [!DNL Anaplan]:

* Un profilo utente in [!DNL Anaplan] denominato Integrazione **[!UICONTROL [!DNL Workfront]]**, con diritti di amministratore di sistema.
* Modello [!DNL Anaplan] che si desidera utilizzare per questo scenario.
* Elenco all&#39;interno del modello [!DNL Anaplan] che si desidera utilizzare per questo scenario.
* Un file **[!UICONTROL Importazione aggiornamento progetto]** contenente le colonne seguenti, nell&#39;ordine seguente:

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront] GUID progetto]

3. [!UICONTROL Nome campagna]

4. [!UICONTROL Percentuale completato]

5. [!UICONTROL Data inizio pianificata]

6. [!UICONTROL Data di completamento Pianificata]

7. [!UICONTROL Ore pianificate]

8. [!UICONTROL Costo Pianificato]

9. [!UICONTROL Costo Spesa Pianificato]

10. [!UICONTROL Costo effettivo manodopera]

11. [!UICONTROL Costo di Lavoro Pianificato]

12. [!UICONTROL Stato]

Per preparare il file [!UICONTROL [!DNL Anaplan] Importazione spese pianificata]:

1. Copiare e incollare quanto segue in un editor di testo o [!DNL Excel]
1. Salva il file in formato CSV
1. Carica il file in Anaplan.

   Per istruzioni, vedere la documentazione di [!DNL Anaplan] sull&#39;importazione di dati nei moduli da un file.

1. Prendere nota del nome assegnato al file, che verrà utilizzato durante la distribuzione del modello di scenario [!UICONTROL Fusion].

Esempio di contenuto CSV

<!-- [Copy](javascript:void(0);) -->
<pre><code>"itemID","Workfront Project GUID","Campaign Name","Percent Complete","Planned Start Date","Planned Completion Date","Planned Hours","Planned Cost","Planned Expense Cost","Actual Labor Cost","Planned Labor Cost","Status","Campaign Overview","Key Message","In Market Start Date","In Market End Date","Target Audience"<br>"202000001019","6182bc1f0025e184b2c00d9205e22c49","Launch Be U APAC Styles Catalog","0","2022-03-31","2022-05-31","88.25","0","0","0","0","Planning","","","","",""</code></pre>Le colonne facoltative possono includere:

1. [!UICONTROL Panoramica campagna]

2. [!UICONTROL Messaggio chiave]

3. [!UICONTROL Data di inizio del mercato]

4. [!UICONTROL In data di fine mercato]

5. [!UICONTROL Pubblico di destinazione]

Includi anche eventuali altri campi che desideri impostare nella mappatura.

* Un processo **[!UICONTROL Importazione aggiornamento progetto]** preparato per eseguire l&#39;importazione dei dati consegnati in un caricamento di file.

Per istruzioni su una di queste azioni, vedere la documentazione di [!DNL Anaplan].

## Distribuzione in [!DNL Workfront Fusion]

Per distribuire questo scenario di integrazione nell’account Fusion, completa i passaggi seguenti. Questa operazione deve essere eseguita solo dopo aver completato la configurazione [!DNL Workfront] e [!DNL Anaplan] richieste.

1. Passare al menu [!UICONTROL Modelli] in [!DNL Workfront Fusion] e fare clic sul modello di scenario **[!UICONTROL Invia aggiornamenti progetto Workfront a [!DNL Anaplan] elemento di elenco]**.
1. Sostituire i valori delle variabili per le seguenti [!DNL Anaplan] variabili:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
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
      <td role="rowheader">[!UICONTROL Nome File: Importazione Aggiornamento Progetto]</td> 
      <td>Nome del file che riceverà i dati di aggiornamento del progetto.<p>(Esempio: WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome processo: importazione aggiornamento progetto]</td> 
      <td> <p>Nome del processo che eseguirà l'importazione dei dati del progetto.</p> <p>(Esempio: WF Int - Aggiorna dettagli campagna)</p> </td> 
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

   Il filtro è configurato per richiamare tutti i progetti collegati incompleti e quelli completati negli ultimi 29 minuti. Se si modifica la frequenza dello scenario [!DNL Fusion], si desidera aggiornare questo valore una volta distribuito il modello di scenario.

1. Nel modulo **[!UICONTROL Aggiorna CSV]** dei progetti di compilazione, aggiungi una nuova struttura di dati per mappare gli attributi del progetto alle colonne CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "itemID": 1000001,<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Percent Complete": 10.01,<br>        "Planned Start Date":"2022-02-22",<br>        "Planned Completion Date":"2022-02-22",<br>        "Planned Hours": 12.5,<br>        "Planned Cost": 123.45,<br>        "Planned Expense Cost": 123.45,<br>        "Planned Labor Cost": 123.45,<br>        "Status": "CUR",<br>        "Campaign Overview":"text",<br>        "Key Message":"text",<br>        "In Market Start Date":"2022-02-22",<br>        "In Market End Date":"2022-02-22",<br>        "Target Audience":"text"<br>    }<br>]<br></code></pre>

1. Aggiorna tutti i moduli [!DNL Workfront] rimanenti con una connessione [!DNL Workfront], quando richiesto.

## Altri modelli di scenario consigliati

Questo modello di scenario è completato dai seguenti modelli di scenario di ottimizzazione spesa che possono anche essere distribuiti:

* [[!UICONTROL Invia [!DNL Adobe Workfront] aggiornamenti ore effettive a una [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Invia [!DNL Adobe Workfront] spese a una [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Scenari aggiuntivi per il collegamento delle richieste di budget:

* [[!UICONTROL Crea una [!DNL Anaplan] voce di elenco da una [!DNL Adobe Workfront] richiesta budget]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Applica un [!DNL Anaplan] allocazione budget a un [!DNL Adobe Workfront] progetto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Scenari aggiuntivi per il collegamento delle richieste di campagne:

* [[!UICONTROL Crea un [!DNL Anaplan] elemento di elenco da una [!DNL Adobe Workfront] richiesta campagna]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Applica un [!DNL Anaplan] allocazione budget a una [!DNL Adobe Workfront] richiesta campagna o progetto campagna]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
