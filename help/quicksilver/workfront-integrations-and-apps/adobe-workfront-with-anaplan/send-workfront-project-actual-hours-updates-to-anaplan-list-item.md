---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Invia [!DNL Adobe Workfront] le ore effettive vengono aggiornate su un [!DNL Anaplan] voce di elenco
description: Questo scenario di integrazione condivide i dettagli dell'orario effettivo acquisiti su un [!DNL Adobe Workfront] progetto con un [!DNL Anaplan] voce dell'elenco di budget. La condivisione di queste informazioni consente di sfruttare al meglio l'ottimizzazione della spesa e l'analisi finanziaria che [!DNL Anaplan] fornisce.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Invia [!DNL Adobe Workfront] le ore effettive vengono aggiornate su un [!DNL Anaplan] voce di elenco

Questo scenario di integrazione condivide i dettagli dell&#39;orario effettivo acquisiti su un [!DNL Adobe Workfront] progetto con un [!DNL Anaplan] voce dell&#39;elenco di budget. La condivisione di queste informazioni consente di sfruttare al meglio l&#39;ottimizzazione della spesa e l&#39;analisi finanziaria che [!DNL Anaplan] fornisce.

Questo modello di scenario fornisce un elenco di ore riepilogate per progetto, giorno e ruolo registrate nei progetti attivi negli ultimi 3 mesi.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> </td> 
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

* Un profilo utente in [!DNL Workfront] denominato **[!UICONTROL Integrazione Anaplan]** che dispone dei diritti di amministratore di sistema.

   Per informazioni sulla creazione di un utente in [!DNL Workfront], vedi [Aggiungi utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Previsto [!DNL Anaplan] Configurazione

Devi avere le seguenti caratteristiche in [!DNL Anaplan] per utilizzare questo scenario:

* Un profilo utente in [!DNL Anaplan] denominato **[!UICONTROL [!DNL Workfront ]Integrazione]** che dispone dei diritti di amministratore di sistema.
* La [!DNL Anaplan] Modello da utilizzare per lo scenario.
* Elenco all’interno della [!DNL Anaplan] Modello da utilizzare per lo scenario.
* Un file in [!DNL Anaplan] denominato **[!UICONTROL Importazione ore effettive Anaplan]** che contiene le colonne seguenti, in questo ordine:

   1. [!UICONTROL GUID progetto Workfront]

   2. [!UICONTROL Ore]

   3. [!UICONTROL Ore Costo stimato]

   4. [!UICONTROL Data inserimento]

   5. [!UICONTROL Nome del ruolo]

   6. [!UICONTROL Nome campagna]

   7. [!UICONTROL [!DNL Anaplan] ID voce elenco]
   Per preparare il [!DNL Anaplan] File della nota spese effettive:

   1. Copia e incolla quanto segue in un editor di testo o [!DNL Excel]
   1. Salvare il file in formato CSV
   1. Carica il file in [!DNL Anaplan].

      Per istruzioni, consulta la sezione [!DNL Anaplan] documentazione sull’importazione di dati in moduli da un file.

   1. Prendi nota del nome che hai dato al file; viene utilizzato durante la distribuzione del [!UICONTROL Fusion] modello di scenario.

   Esempio di contenuto CSV

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

* A **[!UICONTROL Importazione ore effettive del progetto]** processo preparato per eseguire l’importazione dei dati consegnati in un caricamento di file.

Per istruzioni su una di queste azioni, consulta la sezione [!DNL Anaplan] documentazione.

## Implementazione in [!DNL Workfront Fusion]

Completa i seguenti passaggi per distribuire questo scenario di integrazione al tuo [!DNL Fusion] conto. Questa operazione deve essere eseguita solo dopo il completamento del [!DNL Workfront] e [!DNL Anaplan] configurazione.

1. Passa a [!UICONTROL Modelli] menu in [!DNL Workfront Fusion] e fai clic su **[!UICONTROL Invia aggiornamenti effettivi di Workfront a [!DNL Anaplan] voce di elenco]** modello di scenario.
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
      <td>L’ID di un’area di lavoro dal tuo [!DNL Anaplan] conto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID modello] </td> 
      <td>L'ID di un modello dal [!DNL Anaplan] e l'area di lavoro selezionata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>Nome dell'elenco [!DNL Anaplan] e l'area di lavoro e il modello selezionati.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome file: Importazione ore effettive]</td> 
      <td> <p>Nome del file che riceverà i dati effettivi dell’orario del progetto.</p> <p> (Esempio: WorkfrontUpdateLinkedProjects_HoursRuoli.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome processo: Importazione ore effettive]</td> 
      <td> <p>Nome del processo che eseguirà l'importazione dei dati relativi alle ore del progetto.</p> <p>(Esempio: WF Int - Load Project Hours by Role (Orari del progetto per ruolo)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Sottodominio]</td> 
      <td>Il sottodominio del [!DNL Workfront] conto. Viene utilizzato per creare un collegamento al [!DNL Workfront] in una nota che può essere generata.</td> 
     </tr> 
    </tbody> 
   </table>

   I dettagli sulla configurazione dei file e dei processi sono forniti nella sezione [!DNL Anaplan] documentazione di installazione.

1. Seleziona o aggiungi un [!DNL Anaplan] profilo di connessione.
1. Aggiorna tutti gli altri [!DNL Anaplan] moduli con un [!DNL Anaplan] quando richiesto.
1. Seleziona o aggiungi un [!DNL Workfront] profilo di connessione.
1. Aggiorna tutti gli altri [!DNL Workfront] moduli con un [!DNL Workfront] quando richiesto.

## Altri modelli di scenario consigliati

Questo modello di scenario è completato dai seguenti modelli di scenario di ottimizzazione delle spese che possono essere distribuiti anche:

* [[!UICONTROL Invia [!DNL Adobe Workfront] aggiornamento del progetto a un [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Invia [!DNL Adobe Workfront] spese per un [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Scenari aggiuntivi per il collegamento di richieste di budget:

* [[!UICONTROL Crea un [!DNL Anaplan] voce di elenco da un [!DNL Adobe Workfront] richiesta di bilancio]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Applica un [!DNL Anaplan] assegnazione di bilancio a un [!DNL Adobe Workfront] progetto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Scenari aggiuntivi per il collegamento di richieste di campagne:

* [[!UICONTROL Crea un [!DNL Anaplan] voce di elenco da un [!DNL Adobe Workfront] richiesta campagna]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Applica un [!DNL Anaplan] assegnazione di bilancio a un [!DNL Adobe Workfront] richiesta di campagna o progetto della campagna]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
