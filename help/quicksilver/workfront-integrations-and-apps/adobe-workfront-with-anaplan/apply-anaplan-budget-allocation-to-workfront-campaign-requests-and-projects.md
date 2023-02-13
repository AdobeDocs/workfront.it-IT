---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Applica un [!DNL Anaplan] assegnazione di bilancio a un [!DNL Adobe Workfront] richiesta di campagna o progetto della campagna
description: Questo scenario di integrazione sincronizza tutte le allocazioni di budget effettuate in [!DNL Anaplan] torna a [!DNL Workfront]. Lo scenario richiama tutte le voci di budget della campagna collegate, quindi passa il valore di budget al progetto Workfront collegato se il valore di budget è stato modificato.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 8ae28911-fa18-459a-aa50-cfb347e70e61
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Applica un [!DNL Anaplan] assegnazione di bilancio a un [!DNL Adobe Workfront] richiesta di campagna o progetto della campagna

Questo scenario di integrazione sincronizza tutte le allocazioni di budget effettuate in [!DNL Anaplan] torna a [!DNL Workfront]. Lo scenario richiama tutte le voci di budget della campagna collegate, quindi passa il valore di budget al collegato [!DNL Workfront] se il valore del budget è stato modificato.

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

* Un profilo utente in [!DNL Workfront] denominato **[!DNL Anaplan Integration]** che dispone dei diritti di amministratore di sistema.

   Per informazioni sulla creazione di un utente in [!DNL Workfront], vedi [Aggiungi utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Previsto [!DNL Anaplan] Configurazione

Devi avere le seguenti caratteristiche in [!DNL Anaplan] per utilizzare questo scenario:

* Un profilo utente in [!DNL Anaplan] denominato **[!UICONTROL [!DNL Workfront]Integrazione]** che dispone dei diritti di amministratore di sistema.
* La [!DNL Anaplan] Modello da utilizzare per lo scenario.
* Elenco all’interno della [!DNL Anaplan] Modello che acquisisce i budget delle campagne.

   Il modulo dell’elenco deve supportare la ricezione dei seguenti attributi:

   * [!UICONTROL [!DNL Workfront] GUID richiesta]
   * [!UICONTROL [!DNL Workfront] GUID progetto]
   * [!UICONTROL Nome campagna]
   * [!UICONTROL Fondi per la manodopera richiesti]
   * [!UICONTROL Ricavi stimati]
   * [!UICONTROL Brand]

   Questo elenco e questo modulo devono memorizzare ulteriori dettagli necessari per la normale funzionalità di [!DNL Anaplan], compresa la possibilità di impostare un budget e comunicare che la voce dell&#39;elenco di budget è pronta per essere sincronizzata di nuovo in [!DNL Workfront].

* Una visualizzazione in [!DNL Anaplan] chiamato **[!UICONTROL Campagne.Aggiorna campagne in Adobe Workfront]**.

   Questa visualizzazione deve contenere le colonne seguenti, in questo ordine:

   1. [!UICONTROL Nome elemento]

   2. [!UICONTROL [!DNL Workfront] GUID richiesta]

   3. [!UICONTROL [!DNL Workfront] GUID progetto]

   4. [!UICONTROL Nome campagna]

   5. [!UICONTROL Bdg]

   6. [!UICONTROL Ricavi stimati]

   7. [!UICONTROL Brand]
   La visualizzazione deve essere filtrata per visualizzare gli elementi con un [!UICONTROL [!DNL Workfront] GUID progetto] e alcuni indicatori che indicano che le allocazioni di bilancio devono essere trasmesse a Workfront.

Per istruzioni su una di queste azioni, consulta la sezione [!DNL Anaplan] documentazione.

## Distribuzione in Workfront Fusion

Completa i seguenti passaggi per implementare questo scenario di integrazione nell&#39;account Fusion. Questa operazione deve essere eseguita solo dopo il completamento del [!DNL Workfront] e [!DNL Anaplan] configurazione.

1. Passa a [!UICONTROL Modelli] menu in [!DNL Workfront Fusion] e fai clic su **[!UICONTROL Applica [!DNL Anaplan] allocazioni di budget per richieste e progetti di campagne Workfront]** modello di scenario.
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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Nome visualizzazione]</td> 
      <td> <p>Nome della visualizzazione contenente i budget delle campagne pronti per la trasmissione a [!DNL Workfront].</p> <p>(Esempio: [!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   I dettagli sulla configurazione dei file e dei processi sono forniti nella sezione [!DNL Anaplan] documentazione di installazione.

1. Seleziona o aggiungi un [!DNL Anaplan] profilo di connessione.
1. Aggiorna tutti gli altri [!DNL Anaplan] moduli con un [!DNL Anaplan] quando richiesto.
1. Sulla **[!UICONTROL Converti CSV in oggetto JSON]** , aggiungi una nuova struttura dati per mappare le colonne CSV su un oggetto JSON utilizzabile.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Quando richiesto, selezionare questa struttura dati per altri moduli in questa distribuzione di scenario.
1. Sulla **[!UICONTROL Controlla progetto collegato]** modulo, seleziona o aggiungi un [!DNL Workfront] profilo di connessione.
1. Aggiorna tutti gli altri [!DNL Workfront] moduli con un [!DNL Workfront] quando richiesto.

## Altri modelli di scenario consigliati

Per completare il flusso di lavoro rappresentato da questo modello, devi anche distribuire il seguente modello aggiuntivo:

* [[!UICONTROL Crea un [!DNL Anaplan] voce di elenco da un [!DNL Adobe Workfront] richiesta campagna]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)

Gli scenari aggiuntivi per l’ottimizzazione della spesa includono:

* [[!UICONTROL Invia [!DNL Adobe Workfront] aggiornamento del progetto a un [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Invia [!DNL Adobe Workfront] le ore effettive vengono aggiornate su un [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Invia [!DNL Adobe Workfront] spese per un [!DNL Anaplan] voce di elenco]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
