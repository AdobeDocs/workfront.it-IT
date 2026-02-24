---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Crea Forms di assegnazione progetto
description: È possibile utilizzare i moduli di assegnazione dei progetti per semplificare la creazione di progetti in Workfront
author: Becky
feature: Work Management, Requests
role: User, Admin
hide: true
hidefromtoc: true
source-git-commit: 5ff71313c550d949079e7426b657a0a4e19a656c
workflow-type: tm+mt
source-wordcount: '1329'
ht-degree: 4%

---

# Crea moduli di assegnazione progetto

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

I moduli di assegnazione progetti sono un tipo di modulo di richiesta che consente agli utenti di richiedere progetti. I progetti vengono creati dal modulo, senza la necessità di creare un progetto a partire da un problema inviato.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

Per eseguire i passaggi descritti in questo articolo, devi disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
   <p>Nuova licenza: Standard </p>
   Oppure
   <p>Licenza corrente: Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Per creare i moduli di assegnazione dei progetti è necessario essere un amministratore di Workfront. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Altri prodotti</td> 
   <td> <p>L'organizzazione deve aver acquistato Workfront Planning per utilizzare le funzioni di Planning, ad esempio le automazioni.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Funzionalità e limitazioni di Project Intake Forms

### Funzionalità

Le forme di assunzione dei progetti includono le seguenti funzionalità:

#### Automazioni di Workfront Planning

I moduli di assegnazione dei progetti Workfront supportano Workfront Planning Automations per configurare le proprietà specifiche del progetto creato.

Per ulteriori informazioni sulle automazioni Planning, vedere [Configurare le automazioni Adobe Workfront Planning](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

### Configurazione approvazione

I moduli di assegnazione dei progetti includono la possibilità di configurare gli approvatori per le richieste inviate.

### Limitazioni

#### Tipi di campo supportati

Project Intake Forms può includere campi di qualsiasi modulo personalizzato con il tipo di oggetto Project.

I seguenti tipi di campo non sono attualmente supportati in Project Intake Forms:

* Sezione
* Formula
* Rollup
* Rollup su riga singola
* Pianificare una connessione
* Riferimenti ai campi nativi che fanno riferimento a campi nativi del progetto, di sola lettura (ad esempio, `workRequiredExpression`)

#### Richiesta esperienza

I moduli di accettazione del progetto possono essere utilizzati solo con la nuova esperienza di richiesta.

Per informazioni sulla nuova esperienza di richiesta, consulta [Creare e inviare richieste](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

#### Condivisione

I moduli di assegnazione dei progetti non supportano la condivisione pubblica. Le opzioni di condivisione includono:

* **Chiunque**: chiunque nel sistema può utilizzare il modulo per inviare una richiesta di progetto.
* **Utenti specificati**: è possibile selezionare gli utenti specifici che hanno accesso al modulo di richiesta del progetto.

## Creare un modulo di assegnazione progetto

{{step1-to-requests}}

1. Abilita **Passa a una nuova esperienza** nell&#39;angolo superiore destro dello schermo.
1. Fai clic su **Moduli di richiesta** nell&#39;angolo superiore destro della schermata.

   >[!NOTE]
   >
   >Poiché solo gli amministratori di Workfront possono creare moduli di acquisizione, il pulsante Richiedi moduli è visibile solo agli amministratori.

   Viene visualizzato un elenco dei moduli di richiesta attualmente disponibili. Sono inclusi i moduli di richiesta di Workfront Planning.

1. Fai clic su **Nuovo modulo di richiesta** nell&#39;angolo superiore destro della schermata.
1. Immettere un nome per il modulo di richiesta. Per impostazione predefinita, il nome del modulo è **Modulo senza titolo**.
1. Selezionare il tipo di oggetto **Progetto** nella parte superiore dell&#39;elenco a discesa. Attualmente, questo è l’unico tipo di progetto Workfront disponibile. Gli altri elementi dell&#39;elenco appartengono a Workfront Planning.
1. (Facoltativo) Aggiungi una **Descrizione** per il modulo di richiesta.
1. Fai clic su **Crea**. Il modulo di richiesta per il tipo di record selezionato viene aperto nella scheda Modulo.

   Il generatore di moduli di assegnazione del progetto si apre sulla scheda Modulo.

   Per impostazione predefinita, il modulo di assegnazione contiene le seguenti informazioni:

   * **Sezione predefinita**: questa è l&#39;interruzione di sezione predefinita che Workfront applica al modulo di richiesta. Tutti i campi record vengono visualizzati nell&#39;area **Sezione predefinita**.
   * Campo **Oggetto**: campo che identificherà la richiesta in Workfront. Impossibile modificare la configurazione e il valore del campo Oggetto.
   * Tutti i campi associati ai progetti.

     I campi contenuti nel modulo di richiesta saranno visibili a tutti coloro che inviano una richiesta di progetto.

1. Per aggiungere campi al modulo, fai clic sul tipo di campo nel menu di navigazione a sinistra, quindi seleziona il campo.
1. (Facoltativo) Per rimuovere un campo, passa il cursore del mouse sul campo del modulo che desideri rimuovere, quindi fai clic sull&#39;icona **x** per rimuoverlo.
1. (Facoltativo) Per rimuovere la **sezione predefinita** dal modulo, eseguire le operazioni seguenti:

   1. Rimuovi tutti i campi dalla sezione predefinita.
   1. Fai clic sulla scheda **Elementi di contenuto** e aggiungi una nuova sezione, quindi aggiungi un nome per la sezione.
   1. Aggiungi campi alla nuova sezione.
   1. Fai clic sull&#39;icona **x** per rimuovere la **sezione predefinita**.
1. Fare clic su un campo qualsiasi, quindi utilizzare i controlli nel pannello destro del modulo per definirne le dimensioni o una delle seguenti informazioni:

   * **Etichetta**: questo è il nome del campo che verrà visualizzato nel modulo di richiesta. Questo non modifica il nome del campo record.
   * **Istruzioni**: aggiungere ulteriori informazioni sul campo.
   * **Imposta un campo obbligatorio**: se selezionata, il campo deve avere un valore. In caso contrario, il modulo non può essere inviato.
   * **Aggiungi logica**: definisci quali condizioni devono essere soddisfatte affinché il campo venga visualizzato o nascosto.

   >[!TIP]
   >
   >   Il tipo di campo di ciascun campo viene visualizzato nella parte superiore del pannello di destra, dopo aver selezionato il campo nel modulo.
   >     

1. (Facoltativo) Fai clic sulla scheda **Elementi di contenuto** sul lato sinistro del modulo e aggiungi i seguenti elementi:

   * **Testo descrittivo**
   * **Interruzione di sezione**

   Per ulteriori informazioni sulla creazione di un modulo personalizzato, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Fare clic sulla scheda **Automazioni** sul lato sinistro del modulo, quindi eseguire una delle operazioni seguenti:

   * Seleziona un modello di progetto
   * Allega eventuali moduli personalizzati
   * Impostare il proprietario di un progetto
   * Aggiungere il progetto a un portfolio o programma

   Tutte le selezioni effettuate qui verranno applicate ai progetti creati da questo modulo di assegnazione.

1. (Facoltativo) Fare clic su **Anteprima** per visualizzare la modalità di visualizzazione del modulo per gli altri utenti che lo utilizzeranno per inviare un nuovo record.

1. (Facoltativo) Fai clic sulla scheda **Configurazione**, quindi aggiungi almeno un utente o un team&lt; al campo **Approvatori** per approvare nuove richieste per questo modulo di assegnazione.

   * Quando si associa un modulo di assegnazione agli approvatori, prima di generare un progetto è necessario che tutte le nuove richieste vengano approvate dagli approvatori.
   * È possibile aggiungere uno o più approvatori a un modulo di assegnazione.
   * Se almeno un approvatore rifiuta la richiesta, la richiesta viene rifiutata e il progetto non viene creato.
   * Tutti gli approvatori devono prendere una decisione prima che un progetto venga approvato o rifiutato.
   * Se un team è impostato come approvatore, è necessaria una sola decisione del team.

     Per ulteriori informazioni sull&#39;aggiunta di approvazioni ai moduli di richiesta, vedere [Aggiungere approvazione a un modulo di richiesta](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Facoltativo) Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del modulo nell&#39;intestazione, quindi fai clic su **Modifica** per aggiornare il nome del modulo.

1. Fai clic su **Pubblica** per pubblicare il modulo e ottenere un collegamento univoco.

   Si verificano le seguenti situazioni:

   * Il pulsante **Pubblica** è stato rimosso.
   * Il pulsante **Annulla pubblicazione** è stato aggiunto al modulo. Facendo clic su di esso, il modulo non sarà accessibile.
   * Un pulsante **Condividi** è stato aggiunto al modulo.
   * Il modulo diventa disponibile nell’area Richieste del menu Principale in Workfront.

1. Fai clic su **Condividi** per condividere il modulo con altri.
1. Fare clic sulla freccia rivolta a sinistra a sinistra del nome della maschera nell&#39;intestazione per chiudere la maschera.

   Viene aperta la vista tabella **Moduli di richiesta** alla quale viene aggiunto il modulo.

1. (Facoltativo) Passa il puntatore del mouse sul nome di un modulo di richiesta nella visualizzazione tabella, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del modulo e fai clic su una delle seguenti opzioni:

   * **Modifica modulo**: fare clic qui per modificare ulteriormente le informazioni nel modulo.
   * **Annulla pubblicazione**: fare clic qui per annullare la pubblicazione del modulo che lo rimuove dall&#39;area Richieste di Workfront.
   * **Condividi**: fare clic qui per modificare gli utenti che hanno accesso al modulo.
   * **Copia collegamento**: fare clic qui per copiare rapidamente il collegamento del modulo di richiesta senza aprire il modulo.
   * **Elimina**: fare clic qui per eliminare il modulo. Tutte le richieste e i record aggiunti utilizzando il modulo non vengono eliminati. Impossibile recuperare il modulo.

   >[!NOTE]
   >
   >È possibile identificare le maschere di assegnazione del progetto nella vista tabella perché visualizzano &quot;Progetto&quot; nella colonna Tipo oggetto.

1. Fare clic sulla freccia rivolta a sinistra a sinistra di **Moduli di richiesta** nell&#39;intestazione per chiudere la tabella dei moduli di richiesta.

