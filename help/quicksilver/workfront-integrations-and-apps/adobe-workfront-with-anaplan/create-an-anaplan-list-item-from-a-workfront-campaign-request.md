---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 'Crea un elemento di elenco  [!DNL Anaplan]  da una richiesta di campagna  [!DNL Adobe Workfront] '
description: Questo scenario di integrazione collega un  [!DNL Adobe Workfront] progetto con una [!DNL Anaplan] voce di elenco budget.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: daf6a18d-a3df-497d-a612-8a4645b1a8c9
source-git-commit: cb38223c4dd8048fd2ab105abce2c9a79b84c43f
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 2%

---

# Crea un elemento di elenco [!DNL Anaplan] da una richiesta di campagna [!DNL Adobe Workfront]

Questo scenario di integrazione collega un progetto [!DNL Adobe Workfront] con una voce di elenco budget [!DNL Anaplan].

Questo scenario verifica la presenza di nuove richieste di campagna aggiunte a una coda di richieste. Non appena viene registrata una richiesta di campagna, in [!DNL Anaplan] viene aggiunta una voce di budget per avviare il processo di finanziamento.

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
   <td role="rowheader">Piano [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>[!UICONTROL Pro] o versione successiva</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

&#42;&#42;Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

## Evento di attivazione

L’esecuzione di questo scenario è pianificata ogni 15 minuti.

## Configurazione [!DNL Workfront] prevista

Per utilizzare questo scenario, è necessario disporre dei seguenti elementi in [!DNL Workfront]:

* Un profilo utente in [!DNL Workfront] denominato Integrazione **[!UICONTROL [!DNL Anaplan]]**, con diritti di amministratore di sistema.

  Per informazioni sulla creazione di un utente in [!DNL Workfront], vedere [Aggiungere utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Modulo personalizzato **[!UICONTROL Brief campagna]** allegato all&#39;oggetto [!UICONTROL Request].

  I seguenti campi obbligatori devono essere inclusi nel modulo personalizzato per facilitare la mappatura dei dati ad Anaplan:

  | Nome Campo | Tipo di campo |
  |---|---|
  | [!UICONTROL Totale fondi richiesti] |   |
  | [!UICONTROL Fondi manodopera richiesti] |   |
  | [!UICONTROL Fondi spese richiesti] |   |
  | [!UICONTROL Inviato a [!DNL Anaplan]] | Casella di controllo |

  Nel modulo possono essere presenti i seguenti campi facoltativi. Questo scenario mappa solo i campi di cui sopra, ma è possibile mappare eventuali campi aggiuntivi nel resoconto della campagna.

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
     <td>Data </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Nella Data Di Fine Del Mercato]</td> 
     <td>Data</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Panoramica di [!UICONTROL Campaign]</td> 
     <td>Campo di testo paragrafo</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>Campo di testo paragrafo</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>A discesa</p> <p>Includi opzioni che si adattano ai tuoi processi.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Per informazioni sulla creazione di moduli personalizzati, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Un progetto configurato come coda di richieste per acquisire nuove richieste di campagne. Il modulo [!UICONTROL Brief campagna] deve essere allegato a queste richieste.

## Configurazione [!DNL Anaplan] prevista

Per utilizzare questo scenario, è necessario disporre dei seguenti elementi in [!DNL Anaplan]:

* Un profilo utente in [!DNL Anaplan] denominato Integrazione **[!UICONTROL [!DNL Workfront]]**, con diritti di amministratore di sistema.
* Modello [!DNL Anaplan] che si desidera utilizzare per questo scenario.
* Elenco all&#39;interno del modello [!DNL Anaplan] che acquisisce i budget delle campagne.

  Il modulo dell’elenco deve supportare la ricezione dei seguenti attributi:

   * [!UICONTROL [!DNL Workfront] GUID richiesta]
   * [!UICONTROL [!DNL Workfront] GUID progetto]
   * [!UICONTROL Nome campagna]
   * [!UICONTROL Fondi manodopera richiesti]
   * [!UICONTROL Fondi spese richiesti]
   * [!UICONTROL Tipo di richiesta budget]

  Questo elenco e modulo devono memorizzare ulteriori dettagli necessari per la normale funzionalità di [!DNL Anaplan], inclusa la possibilità di impostare un budget e comunicare che la voce dell&#39;elenco di budget è pronta per essere sincronizzata nuovamente in [!DNL Workfront].

Per istruzioni su una di queste azioni, vedere la documentazione di [!DNL Anaplan].

## Distribuzione in [!DNL Workfront Fusion]

Per distribuire lo scenario di integrazione all&#39;account [!DNL Fusion], completare i passaggi seguenti. Questa operazione deve essere eseguita solo dopo aver completato la configurazione [!DNL Workfront] e [!DNL Anaplan] richieste.

1. Passare al menu [!UICONTROL Modelli] in [!DNL Workfront Fusion] e fare clic sul modello di scenario **[!UICONTROL Crea un elemento di elenco [!DNL Anaplan] da una richiesta di Workfront Campaign]**.
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

* [[!UICONTROL Applica un [!DNL Anaplan] allocazione budget a una [!DNL Adobe Workfront] richiesta campagna o progetto campagna]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)

Altri scenari per l’ottimizzazione della spesa includono:

* [[!UICONTROL Invia [!DNL Adobe Workfront] aggiornamenti di progetto a una [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Invia [!DNL Adobe Workfront] aggiornamenti ore effettive a una [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Invia [!DNL Adobe Workfront] spese a una [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
