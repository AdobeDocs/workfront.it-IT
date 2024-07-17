---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Crea una voce di elenco  [!DNL Anaplan]  da una richiesta budget  [!DNL Adobe Workfront]
description: Questo scenario di integrazione collega un  [!DNL Adobe Workfront] progetto (campagna) con una [!DNL Anaplan] voce di elenco budget. A tale scopo, aggiungere una richiesta di budget al progetto  [!DNL Workfront]  che deve ricevere finanziamenti. Questo scenario controlla le richieste di budget non elaborate, quindi esegue un processo per creare una voce di elenco budget vuota in [!DNL Anaplan] per avviare i processi di allocazione budget in Anaplan.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---

# Crea una voce di elenco [!DNL Anaplan] da una richiesta budget [!DNL Adobe Workfront]

Questo scenario di integrazione collega un progetto [!DNL Adobe Workfront] (campagna) con una voce dell&#39;elenco di budget [!DNL Anaplan]. A tale scopo, aggiungere una richiesta di budget al progetto [!DNL Workfront] che deve ricevere fondi. Questo scenario controlla le richieste di budget non elaborate, quindi esegue un processo per creare una voce di elenco budget vuota in [!DNL Anaplan] per avviare i processi di allocazione budget in [!DNL Anaplan].

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
   <td role="rowheader" [!DNL>Licenza Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL Workfront Fusion per l'automazione e l'integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr>
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

&#42;&#42;Per informazioni sulle [!DNL  Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Evento di attivazione

L’esecuzione di questo scenario è pianificata ogni 15 minuti.

## Configurazione [!DNL Workfront] prevista

Per utilizzare questo scenario, è necessario disporre dei seguenti elementi in [!DNL Workfront]:

* Un profilo utente in [!DNL Workfront] denominato *[!UICONTROL *[!DNL Anaplan] Integration]**, con diritti di amministratore di sistema.

  Per informazioni sulla creazione di un utente in [!DNL Workfront], vedere [Aggiungere utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Modulo personalizzato **[!UICONTROL Richiesta budget]** allegato all&#39;oggetto [!UICONTROL Richiesta].

  I seguenti campi obbligatori devono essere inclusi nel modulo personalizzato per facilitare la mappatura dei dati a [!DNL Anaplan]:

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <thead> 
    <tr> 
     <th>Nome Campo</th> 
     <th>Tipo di campo</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL Tipo di richiesta budget]</td> 
     <td> <p>Elenco a discesa [!UICONTROL]</p> <p>Opzioni:</p> 
      <ul> 
       <li> <p>[!UICONTROL Adeguamento al finanziamento]</p> </li> 
       <li> <p>[!UICONTROL - Finanziamento iniziale]</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL fondi manodopera richiesti]</td> 
     <td> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL - Fondi spese richiesti]</td> 
     <td> </td> 
    </tr> 
   </tbody> 
  </table>

  Per informazioni sulla creazione di moduli personalizzati, vedere [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* Modelli di progetto che rappresentano campagne e altri progetti che richiedono finanziamenti, configurati con un argomento coda [!UICONTROL Richiesta budget]. L&#39;argomento della coda [!UICONTROL Richiesta budget] è assegnato per l&#39;utilizzo del modulo personalizzato [!UICONTROL Richiesta budget].
* Modulo **[!UICONTROL Brief campagna]** per l&#39;oggetto progetto.

  Questo modulo deve contenere i seguenti campi:

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
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
     <td>[!UICONTROL Campo Rich Text]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>[!UICONTROL Campo Rich Text]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>Elenco a discesa [!UICONTROL]</p> <p>Includi opzioni che si adattano ai tuoi processi.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Per informazioni sulla creazione di moduli personalizzati, vedere [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Configurazione [!DNL Anaplan] prevista

Per utilizzare questo scenario, è necessario disporre dei seguenti elementi in [!DNL Anaplan]:

* Un profilo utente in [!DNL Anaplan] denominato Integrazione **[!UICONTROL [!DNL Workfront]]**, con diritti di amministratore di sistema.
* Modello [!DNL Anaplan] che si desidera utilizzare per questo scenario.
* Elenco all&#39;interno del modello [!DNL Anaplan] che acquisisce i budget delle campagne.

  Il modulo dell’elenco deve supportare la ricezione dei seguenti attributi:

   * [!UICONTROL GUID progetto Workfront]
   * [!UICONTROL Nome campagna]
   * [!UICONTROL Fondi manodopera richiesti]
   * [!UICONTROL Fondi spese richiesti]
   * [!UICONTROL Tipo di richiesta budget]
   * [!UICONTROL Motivo dell&#39;adeguamento del finanziamento]

  Questo elenco e modulo devono memorizzare ulteriori dettagli necessari per la normale funzionalità di [!DNL Anaplan], inclusa la possibilità di impostare un budget e comunicare che la voce dell&#39;elenco di budget è pronta per essere sincronizzata nuovamente in [!DNL Workfront].

Per istruzioni su una di queste azioni, vedere la documentazione di [!DNL Anaplan].

## Distribuzione in [!DNL Workfront Fusion]

Per distribuire lo scenario di integrazione all&#39;account [!DNL Fusion], completare i passaggi seguenti. Questa operazione deve essere eseguita solo dopo aver completato la configurazione [!DNL Workfront] e [!DNL Anaplan] richieste.

1. Passare al menu [!UICONTROL Modelli] in [!DNL Workfront Fusion] e fare clic sul modello di scenario **[!UICONTROL Crea una voce di elenco [!DNL Anaplan] da una richiesta budget Workfront]**.
1. Sostituire i valori delle variabili per le seguenti [!DNL Anaplan] variabili:

   | Nome variabile | Sostituisci valore con |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] ID Workspace] | ID di un&#39;area di lavoro dall&#39;account [!DNL Anaplan]. |
   | ID modello [!UICONTROL [!DNL Anaplan]] | L&#39;ID di un modello dall&#39;account [!DNL Anaplan] e dall&#39;area di lavoro selezionata. |
   | Nome modulo [!UICONTROL [!DNL Anaplan]] | Il nome del modulo che descrive gli attributi della campagna nell&#39;elenco [!DNL Anaplan] selezionato. |
   | [!UICONTROL Nome elenco campagne] | Il nome dell&#39;elenco dall&#39;account [!DNL Anaplan] e dall&#39;area di lavoro e dal modello selezionati. |

   {style="table-layout:auto"}

   I dettagli sulla configurazione dei file e dei processi sono forniti nella documentazione di installazione di [!DNL Anaplan].

1. Selezionare o aggiungere un profilo di connessione [!DNL Anaplan].
1. Aggiorna tutti i moduli [!DNL Anaplan] rimanenti con una connessione [!DNL Anaplan], quando richiesto.
1. Selezionare o aggiungere un profilo di connessione [!DNL Workfront].

   Dopo aver distribuito il modello, questo è il modulo che verrà aggiornato per aggiungere o rimuovere i riferimenti ai campi personalizzati dal valore della proprietà fields se si desidera modificare i campi mappati predefiniti in [!DNL Anaplan].

1. Aggiorna tutti i moduli [!DNL Workfront] rimanenti con una connessione [!DNL Workfront], quando richiesto.

## Altri modelli di scenario consigliati

Per completare il flusso di lavoro rappresentato da questo modello, è necessario distribuire anche il seguente modello aggiuntivo:

* [[!UICONTROL Applica un [!DNL Anaplan] allocazione budget a un [!DNL Adobe Workfront] progetto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Altri scenari per l’ottimizzazione della spesa includono:

* [[!UICONTROL Invia [!DNL Adobe Workfront] aggiornamenti di progetto a una [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Invia [!DNL Adobe Workfront] aggiornamenti ore effettive a una [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Invia [!DNL Adobe Workfront] spese a una [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
