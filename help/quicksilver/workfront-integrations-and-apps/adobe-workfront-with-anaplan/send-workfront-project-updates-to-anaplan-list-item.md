---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Invia [!DNL Adobe Workfront] aggiornamento del progetto a un [!DNL Anaplan] voce di elenco
description: Questo scenario di integrazione condivide i dettagli relativi all'avanzamento, allo stato e alla pianificazione chiave da un [!DNL Adobe Workfront] progetto con un [!DNL Anaplan] voce dell'elenco di budget. La condivisione di queste informazioni consente di sfruttare al meglio l'ottimizzazione della spesa e l'analisi finanziaria che [!DNL Anaplan] fornisce.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 2%

---

# Invia [!DNL Adobe Workfront] aggiornamento del progetto a un [!DNL Anaplan] voce di elenco

Questo scenario di integrazione condivide i dettagli relativi all&#39;avanzamento, allo stato e alla pianificazione chiave da un [!DNL Adobe Workfront] progetto con un [!DNL Anaplan] voce dell&#39;elenco di budget. La condivisione di queste informazioni consente di sfruttare al meglio l&#39;ottimizzazione della spesa e l&#39;analisi finanziaria che [!DNL Anaplan] fornisce.

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

* Un profilo utente in [!DNL Workfront] denominato **[!UICONTROL [!DNL Anaplan]Integrazione]** che dispone dei diritti di amministratore di sistema.

   Per informazioni sulla creazione di un utente in [!DNL Workfront], vedi [Aggiungi utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL Brief della campagna]** modulo personalizzato associato all’oggetto progetto per memorizzare i valori dei dati personalizzati che si sceglie di inviare ad Anaplan.

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
     <td role="rowheader">[!UICONTROL In Data Di Inizio Mercato]</td> 
     <td>[!UICONTROL Date] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Data Di Fine Mercato]</td> 
     <td>[!UICONTROL Date]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Panoramica della campagna]</td> 
     <td>[!UICONTROL Campo testo paragrafo]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Messaggio chiave]</td> 
     <td>[!UICONTROL Campo testo paragrafo]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>Menu a discesa [!UICONTROL]</p> <p>Includi opzioni che corrispondono ai tuoi processi.</p> </td> 
    </tr> 
   </tbody> 
  </table>

   Per informazioni sulla creazione di moduli personalizzati, vedere [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## Previsto [!DNL Anaplan] Configurazione

Devi avere le seguenti caratteristiche in [!DNL Anaplan] per utilizzare questo scenario:

* Un profilo utente in [!DNL Anaplan] denominato **[!UICONTROL [!DNL Workfront]Integrazione]** che dispone dei diritti di amministratore di sistema.
* La [!DNL Anaplan] Modello da utilizzare per lo scenario.
* Elenco all’interno della [!DNL Anaplan] Modello da utilizzare per lo scenario.
* A **[!UICONTROL Importazione aggiornamento progetto]** file che contiene le colonne seguenti, in questo ordine:

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront] GUID progetto]

3. [!UICONTROL Nome campagna]

4. [!UICONTROL Percentuale completato]

5. [!UICONTROL Data di inizio pianificata]

6. [!UICONTROL Data di completamento Pianificata]

7. [!UICONTROL Lavoro Necessario]

8. [!UICONTROL Costo Pianificato]

9. [!UICONTROL Costo spese pianificato]

10. [!UICONTROL Costo di Lavoro Reale]

11. [!UICONTROL Costo di Lavoro Pianificato]

12. [!UICONTROL Stato]

Per preparare il [!UICONTROL [!DNL Anaplan] Importazione spese pianificate] file:

1. Copia e incolla quanto segue in un editor di testo o [!DNL Excel]
1. Salvare il file in formato CSV
1. Carica il file in Anaplan.

   Per istruzioni, consulta la sezione [!DNL Anaplan] documentazione sull’importazione di dati in moduli da un file.

1. Prendi nota del nome che hai dato al file; viene utilizzato durante la distribuzione del [!UICONTROL Fusion] modello di scenario.

Esempio di contenuto CSV

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

1. [!UICONTROL Panoramica della campagna]

2. [!UICONTROL Messaggio chiave]

3. [!UICONTROL Data di inizio del mercato]

4. [!UICONTROL Data di fine del mercato]

5. [!UICONTROL Pubblico di Target]

Includi anche tutti gli altri campi che desideri impostare nella mappatura.

* A **[!UICONTROL Importazione aggiornamento progetto]** processo preparato per eseguire l’importazione dei dati consegnati in un caricamento di file.

Per istruzioni su una di queste azioni, consulta la sezione [!DNL Anaplan] documentazione.

## Implementazione in [!DNL Workfront Fusion]

Completa i seguenti passaggi per implementare questo scenario di integrazione nell&#39;account Fusion. Questa operazione deve essere eseguita solo dopo il completamento del [!DNL Workfront] e [!DNL Anaplan] configurazione.

1. Passa a [!UICONTROL Modelli] menu in [!DNL Workfront Fusion] e fai clic su **[!UICONTROL Invia aggiornamenti del progetto Workfront a [!DNL Anaplan] voce di elenco]** modello di scenario.
1. Sostituisci i valori delle variabili seguenti [!DNL Anaplan] variabili:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
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
      <td role="rowheader">[!UICONTROL Nome file: Importazione aggiornamento progetto]</td> 
      <td>Nome del file che riceverà i dati di aggiornamento del progetto.<p>(Esempio: WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome processo: Importazione aggiornamento progetto]</td> 
      <td> <p>Nome del processo che eseguirà l’importazione dei dati del progetto.</p> <p>(Esempio: WF Int - Aggiornamento dei dettagli della campagna)</p> </td> 
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

   Il filtro è configurato in modo da estrarre tutti i progetti collegati incompleti e quelli completati negli ultimi 29 minuti. Se si modifica la frequenza del [!DNL Fusion] scenario desiderato per aggiornare questo valore una volta distribuito il modello di scenario.

1. Sulla **[!UICONTROL Crea progetti con CSV aggiornato]** aggiungi una nuova struttura dati per mappare gli attributi del progetto su colonne CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Aggiorna tutti gli altri [!DNL Workfront] moduli con un [!DNL Workfront] quando richiesto.

## Altri modelli di scenario consigliati

Questo modello di scenario è completato dai seguenti modelli di scenario di ottimizzazione delle spese che possono essere distribuiti anche:

* [[!UICONTROL Invia [!DNL Adobe Workfront] le ore effettive vengono aggiornate su un [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Invia [!DNL Adobe Workfront] spese per un [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Scenari aggiuntivi per il collegamento di richieste di budget:

* [[!UICONTROL Crea un [!DNL Anaplan] voce di elenco da un [!DNL Adobe Workfront] richiesta di bilancio]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Applica un [!DNL Anaplan] assegnazione di bilancio a un [!DNL Adobe Workfront] progetto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Scenari aggiuntivi per il collegamento di richieste di campagne:

* [[!UICONTROL Crea un [!DNL Anaplan] voce di elenco da un [!DNL Adobe Workfront] richiesta campagna]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Applica un [!DNL Anaplan] assegnazione di bilancio a un [!DNL Adobe Workfront] richiesta di campagna o progetto della campagna]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
