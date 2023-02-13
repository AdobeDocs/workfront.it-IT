---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Crea un [!DNL Anaplan] voce di elenco da un [!DNL Adobe Workfront] richiesta di bilancio
description: Questo scenario di integrazione collega un [!DNL Adobe Workfront] progetto (campagna) con un [!DNL Anaplan] voce dell'elenco di budget. Questa operazione viene eseguita aggiungendo una richiesta di budget al [!DNL Workfront] progetto che deve ricevere finanziamenti. Questo scenario controlla le richieste di budget non elaborate, quindi esegue un processo per creare una voce di elenco budget vuota in [!DNL Anaplan] avviare i processi di allocazione del budget in Anaplan.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 1%

---

# Crea un [!DNL Anaplan] voce di elenco da un [!DNL Adobe Workfront] richiesta di bilancio

Questo scenario di integrazione collega un [!DNL Adobe Workfront] progetto (campagna) con un [!DNL Anaplan] voce dell&#39;elenco di budget. Questa operazione viene eseguita aggiungendo una richiesta di budget al [!DNL Workfront] progetto che deve ricevere finanziamenti. Questo scenario controlla le richieste di budget non elaborate, quindi esegue un processo per creare una voce di elenco budget vuota in [!DNL Anaplan] per avviare i processi di allocazione del budget in [!DNL Anaplan].

>[!IMPORTANT]
>
>&quot;Campaign&quot; in questo articolo fa riferimento al caso di utilizzo della campagna di marketing che questo scenario rappresenta e non è in alcun modo connesso al [!DNL Workfront Fusion] Connettore Adobe Campaign o al server obsoleto di recente [!UICONTROL Campaign] oggetto in [!DNL Workfront].

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader" [!DNL>Licenza Adobe Workfront Fusion**</td> 
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr>
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

&#42;&#42;Per informazioni su[!DNL  Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Evento di attivazione

L’esecuzione di questo scenario è pianificata ogni 15 minuti.

## Previsto [!DNL Workfront] Configurazione

Devi avere le seguenti caratteristiche in [!DNL Workfront] per utilizzare questo scenario:

* Un profilo utente in [!DNL Workfront] denominato *[!UICONTROL *[!DNL Anaplan] Integrazione]**, che dispone dei diritti di amministratore di sistema.

   Per informazioni sulla creazione di un utente in [!DNL Workfront], vedi [Aggiungi utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL Richiesta di budget]** modulo personalizzato allegato al [!UICONTROL Richiesta] oggetto.

   Per facilitare la mappatura dei dati a [!DNL Anaplan]:

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
     <td> <p>Menu a discesa [!UICONTROL]</p> <p>Opzioni:</p> 
      <ul> 
       <li> <p>[!UICONTROL Adeguamento al finanziamento]</p> </li> 
       <li> <p>[!UICONTROL Finanziamento Iniziale]</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Fondi per il lavoro richiesti]</td> 
     <td> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Fondi di spesa richiesti]</td> 
     <td> </td> 
    </tr> 
   </tbody> 
  </table>

   Per informazioni sulla creazione di moduli personalizzati, vedere [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* Modelli di progetto che rappresentano campagne e altri progetti che richiedono finanziamenti, configurati con un [!UICONTROL Richiesta di budget] argomento della coda. La [!UICONTROL Richiesta di budget] l’argomento della coda è assegnato per utilizzare [!UICONTROL Richiesta di budget] modulo personalizzato.
* A **[!UICONTROL Brief della campagna]** modulo per l&#39;oggetto di progetto.

   Il modulo deve contenere i campi seguenti:

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
     <td role="rowheader">[!UICONTROL In Data Di Inizio Mercato]</td> 
     <td>[!UICONTROL Date] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Data Di Fine Mercato]</td> 
     <td>[!UICONTROL Date]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Panoramica della campagna]</td> 
     <td>[!UICONTROL Campo RTF]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Messaggio chiave]</td> 
     <td>[!UICONTROL Campo RTF]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>Menu a discesa [!UICONTROL]</p> <p>Includi opzioni che corrispondono ai tuoi processi.</p> </td> 
    </tr> 
   </tbody> 
  </table>

   Per informazioni sulla creazione di moduli personalizzati, vedere [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Previsto [!DNL Anaplan] Configurazione

Devi avere le seguenti caratteristiche in [!DNL Anaplan] per utilizzare questo scenario:

* Un profilo utente in [!DNL Anaplan] denominato **[!UICONTROL [!DNL Workfront]Integrazione]** che dispone dei diritti di amministratore di sistema.
* La [!DNL Anaplan] Modello da utilizzare per lo scenario.
* Elenco all’interno della [!DNL Anaplan] Modello che acquisisce i budget delle campagne.

   Il modulo dell’elenco deve supportare la ricezione dei seguenti attributi:

   * [!UICONTROL GUID progetto Workfront]
   * [!UICONTROL Nome campagna]
   * [!UICONTROL Fondi per la manodopera richiesti]
   * [!UICONTROL Fondi di spesa richiesti]
   * [!UICONTROL Tipo di richiesta budget]
   * [!UICONTROL Motivo dell&#39;adeguamento al finanziamento]

   Questo elenco e questo modulo devono memorizzare ulteriori dettagli necessari per la normale funzionalità di [!DNL Anaplan], compresa la possibilità di impostare un budget e comunicare che la voce dell&#39;elenco di budget è pronta per essere sincronizzata di nuovo in [!DNL Workfront].

Per istruzioni su una di queste azioni, consulta la sezione [!DNL Anaplan] documentazione.

## Implementazione in [!DNL Workfront Fusion]

Completa i seguenti passaggi per distribuire questo scenario di integrazione al tuo [!DNL Fusion] conto. Questa operazione deve essere eseguita solo dopo il completamento del [!DNL Workfront] e [!DNL Anaplan] configurazione.

1. Passa a [!UICONTROL Modelli] menu in [!DNL Workfront Fusion] e fai clic su **[!UICONTROL Crea un [!DNL Anaplan] voce di elenco da una richiesta di budget Workfront]** modello di scenario.
1. Sostituisci i valori delle variabili seguenti [!DNL Anaplan] variabili:

   | Nome della variabile | Sostituisci il valore con |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] ID area di lavoro] | L’ID di un’area di lavoro dal tuo [!DNL Anaplan] conto. |
   | [!UICONTROL [!DNL Anaplan] ID modello] | L&#39;ID di un modello dal [!DNL Anaplan] e l&#39;area di lavoro selezionata. |
   | [!UICONTROL [!DNL Anaplan] Nome modulo] | Nome del modulo che descrive gli attributi della campagna nel [!DNL Anaplan] Elenco. |
   | [!UICONTROL Nome elenco campagne] | Nome dell&#39;elenco [!DNL Anaplan] e l&#39;area di lavoro e il modello selezionati. |

   {style=&quot;table-layout:auto&quot;}

   I dettagli sulla configurazione dei file e dei processi sono forniti nella sezione [!DNL Anaplan] documentazione di installazione.

1. Seleziona o aggiungi un [!DNL Anaplan] profilo di connessione.
1. Aggiorna tutti gli altri [!DNL Anaplan] moduli con un [!DNL Anaplan] quando richiesto.
1. Seleziona o aggiungi un [!DNL Workfront] profilo di connessione.

   Dopo aver distribuito il modello, questo è il modulo che verrà aggiornato per aggiungere o rimuovere i riferimenti di campo personalizzati dal valore della proprietà field se si desidera modificare i campi mappati predefiniti in [!DNL Anaplan].

1. Aggiorna tutti gli altri [!DNL Workfront] moduli con un [!DNL Workfront] quando richiesto.

## Altri modelli di scenario consigliati

Per completare il flusso di lavoro rappresentato da questo modello, devi anche distribuire il seguente modello aggiuntivo:

* [[!UICONTROL Applica un [!DNL Anaplan] assegnazione di bilancio a un [!DNL Adobe Workfront] progetto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Gli scenari aggiuntivi per l’ottimizzazione della spesa includono:

* [[!UICONTROL Invia [!DNL Adobe Workfront] aggiornamento del progetto a un [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Invia [!DNL Adobe Workfront] le ore effettive vengono aggiornate su un [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Invia [!DNL Adobe Workfront] spese per un [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
