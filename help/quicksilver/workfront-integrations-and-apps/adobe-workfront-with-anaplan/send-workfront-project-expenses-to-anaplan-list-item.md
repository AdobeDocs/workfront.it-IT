---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Invia [!DNL Adobe Workfront] spese per un [!DNL Anaplan] voce di elenco
description: Questo scenario di integrazione condivide i dettagli relativi alle spese da un [!DNL Adobe Workfront] progetto con un [!DNL Anaplan] voce dell'elenco di budget. La condivisione di queste informazioni consente di sfruttare al meglio l'ottimizzazione della spesa e l'analisi finanziaria che [!DNL Anaplan] fornisce.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 2%

---

# Invia [!DNL Adobe Workfront] spese per un [!DNL Anaplan] voce di elenco

Questo scenario di integrazione condivide i dettagli relativi alle spese da un [!DNL Adobe Workfront] progetto con un [!DNL Anaplan] voce dell&#39;elenco di budget. La condivisione di queste informazioni consente di sfruttare al meglio l&#39;ottimizzazione della spesa e l&#39;analisi finanziaria che [!DNL Anaplan] fornisce.

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>Workfront Fusion per automazione e integrazione del lavoro </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

&#42;&#42;Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Evento di attivazione

L’esecuzione di questo scenario è pianificata ogni 15 minuti.

## Previsto [!DNL Workfront] Configurazione

Devi avere le seguenti caratteristiche in [!DNL Workfront] per utilizzare questo scenario:

* Un profilo utente in [!DNL Workfront] denominato *[!UICONTROL *[!DNL Anaplan] Integrazione]**, che dispone dei diritti di amministratore di sistema.

   Per informazioni sulla creazione di un utente in [!DNL Workfront], vedi [Aggiungi utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL Brief della campagna]** modulo personalizzato associato all’oggetto progetto per memorizzare i valori dei dati personalizzati che si sceglie di inviare a [!DNL Anaplan].

   Il modulo deve contenere i campi seguenti:

   | Nome Campo | Tipo di campo |
   |---|---|
   | [!UICONTROL Data ultima trasmissione] | Data |
   | [!UICONTROL Note sull’integrazione] | Campo di testo paragrafo |

   Per informazioni sulla creazione di moduli personalizzati, vedere [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Previsto [!DNL Anaplan] Configurazione

Devi avere le seguenti caratteristiche in [!DNL Anaplan] per utilizzare questo scenario:

* Un profilo utente in [!DNL Anaplan] denominato **[!UICONTROL [!DNL Workfront ]Integrazione]** che dispone dei diritti di amministratore di sistema.
* La [!DNL Anaplan] Modello da utilizzare per lo scenario.
* Elenco all’interno della [!DNL Anaplan] Modello che desideri acquisire i budget delle campagne.
* Un **[!UICONTROL Importazione spese effettive Anaplan]** file che contiene le colonne seguenti, in questo ordine:

   1. [!UICONTROL [!DNL Workfront] GUID spesa]

   2. [!UICONTROL [!DNL Workfront] GUID progetto]

   3. [!UICONTROL Somma Reale]

   4. [!UICONTROL Descrizione]

   5. [!UICONTROL Tipo di Spesa]

   6. [!UICONTROL Data di validità]

   7. [!UICONTROL Nome campagna]

   8. [!UICONTROL [!DNL Anaplan] ID voce elenco]
   Per preparare il [!UICONTROL [!DNL Anaplan] Importazione spese effettive] file:

   1. Copia e incolla quanto segue in un editor di testo o [!DNL Excel].
   1. Salva il file in formato CSV.
   1. Carica il file in [!DNL Anaplan].

      Per istruzioni, consulta la sezione [!DNL Anaplan] documentazione sull’importazione di dati in moduli da un file.

   1. Prendi nota del nome che hai dato al file; viene utilizzato durante la distribuzione del [!UICONTROL Fusion] modello di scenario.

   Esempio di contenuto CSV

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

* Un **[!UICONTROL [!DNL Anaplan]Importazione spese pianificate]** file che contiene le colonne seguenti, in questo ordine:

   1. [!UICONTROL [!DNL Workfront] GUID spesa]

   2. [!UICONTROL [!DNL Workfront] GUID progetto]

   3. [!UICONTROL Somma Reale]

   4. [!UICONTROL Descrizione]

   5. [!UICONTROL Tipo di Spesa]

   6. [!UICONTROL Data di validità]

   7. [!UICONTROL Nome campagna]

   8. [!UICONTROL [!DNL Anaplan] ID voce elenco]
   Per preparare il [!UICONTROL [!DNL Anaplan] Importazione spese pianificate] file:

   1. Copia e incolla quanto segue in un editor di testo o [!DNL Excel]
   1. Salvare il file in formato CSV
   1. Carica il file in Anaplan.

      Per istruzioni, consulta la sezione [!DNL Anaplan] documentazione sull’importazione di dati in moduli da un file.

   1. Prendi nota del nome che hai dato al file; viene utilizzato durante la distribuzione del [!UICONTROL Fusion] modello di scenario.

   Esempio di contenuto CSV

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>


* A **[!UICONTROL Importazione aggiornamento progetto]** processo preparato per eseguire l’importazione dei dati consegnati in un caricamento di file.

>[!NOTE]
>
>Esistono file di importazione separati per le spese pianificate ed effettive, in modo che possano essere segnalati in modo indipendente nelle rispettive date previste ed effettive rispettivamente.

Per istruzioni su una di queste azioni, consulta la sezione [!DNL Anaplan] documentazione.

## Implementazione in [!DNL Fusion]

Completa i seguenti passaggi per distribuire questo scenario di integrazione al tuo [!DNL Fusion] conto. Questa operazione deve essere eseguita solo dopo il completamento del [!DNL Workfront] e [!DNL Anaplan] configurazione.

1. Passa a [!UICONTROL Modelli] menu in [!DNL Workfront Fusion] e fai clic su **[!UICONTROL Invia aggiornamenti spese Workfront a [!DNL Anaplan] voce di elenco]** modello di scenario.
1. Sostituisci i valori delle variabili seguenti [!DNL Anaplan] variabili:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>Nome della variabile</th> 
      <th>Sostituisci il valore con</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID area di lavoro</td> 
      <td>ID dell’area di lavoro dal [!DNL Anaplan] account da utilizzare per questo scenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID modello] </td> 
      <td>ID del modello dal [!DNL Anaplan] account e l'area di lavoro selezionata che si desidera utilizzare per questo scenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>Nome dell'elenco [!DNL Anaplan] e l'area di lavoro e il modello selezionati che si desidera utilizzare per questo scenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome file: Importazione spese effettive]</td> 
      <td> <p>Nome del file che riceverà i dati di spesa effettivi del progetto.</p> <p> (Esempio: WorkfrontUpdateLinkedProjects_ActExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome file: Importazione spese pianificate]</td> 
      <td> <p>Nome del file che riceverà i dati di spesa pianificati del progetto.</p> <p> (Esempio: WorkfrontUpdateLinkedProjects_PlannedExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome processo: Importazione aggiornamento progetto]</td> 
      <td> <p>Nome del processo che eseguirà l'importazione dei dati di spesa del progetto.</p> <p>(Esempio: Costi del progetto di caricamento del file (WF)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   I dettagli sulla configurazione dei file e dei processi sono forniti nella sezione [!DNL Anaplan] documentazione di installazione.

1. Seleziona o aggiungi un [!DNL Anaplan] profilo di connessione.
1. Aggiorna tutti gli altri [!DNL Anaplan] moduli con un [!DNL Anaplan] quando richiesto.
1. Seleziona o aggiungi un [!DNL Workfront] profilo di connessione.
1. Aggiorna tutti gli altri [!DNL Workfront] moduli con un [!DNL Workfront] quando richiesto.
1. Sulla **[!UICONTROL Crea CSV spese effettive]** aggiungi una nuova struttura dati per mappare gli attributi del progetto su colonne CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Sulla **[!UICONTROL Crea CSV delle spese pianificate]** aggiungi una nuova struttura dati per mappare gli attributi del progetto su colonne CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

## Altri modelli di scenario consigliati

Questo modello di scenario è completato dai seguenti modelli di scenario di ottimizzazione delle spese che possono essere distribuiti anche:

* [[!UICONTROL Invia [!DNL Adobe Workfront] aggiornamento del progetto a un [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Invia [!DNL Adobe Workfront] le ore effettive vengono aggiornate su un [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

Scenari aggiuntivi per il collegamento di richieste di budget:

* [[!UICONTROL Crea un [!DNL Anaplan] voce di elenco da un [!DNL Adobe Workfront] richiesta di bilancio]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Applica un [!DNL Anaplan] assegnazione di bilancio a un [!DNL Adobe Workfront] progetto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Scenari aggiuntivi per il collegamento di richieste di campagne:

* [[!UICONTROL Crea un [!DNL Anaplan] voce di elenco da un [!DNL Adobe Workfront] richiesta campagna]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Applica un [!DNL Anaplan] assegnazione di bilancio a un [!DNL Adobe Workfront] richiesta di campagna o progetto della campagna]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
