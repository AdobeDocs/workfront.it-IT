---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: Imposta una bozza con un flusso di lavoro automatizzato in [!DNL Workfront Proof]
description: Questo ripete le informazioni presenti nella Configurazione delle bozze in Workfront. Consolidate qui o là. Forse meglio qui.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 605569df-8e63-476d-a0cd-e73802042011
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1637'
ht-degree: 0%

---

# Imposta una bozza con un flusso di lavoro automatizzato in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Flusso di lavoro automatizzato consente di gestire più facilmente la revisione e l’approvazione dei contenuti in caso di processi di revisione complessi o se si inviano regolarmente contenuti per la revisione agli stessi gruppi di persone.

Si crea la bozza, quindi si sposta da un passaggio all&#39;altro fino all&#39;approvazione finale. Gli utenti interessati vengono informati ogni volta che sono tenuti a rilasciare un&#39;approvazione.

![stage_diagramma.png](assets/stages-diagram-350x81.png)

Puoi aggiungere un flusso di lavoro automatizzato a una bozza durante il caricamento del documento o dopo il caricamento del documento.

## Creare una bozza con Flusso di lavoro automatizzato

1. Inizia a creare la bozza.
1. In **[!UICONTROL Condividi]** sezione, fai clic su **[!UICONTROL Utilizza flusso di lavoro automatizzato]**.

   Puoi deselezionare questa opzione per tornare a un flusso di lavoro standard.

1. (Facoltativo) Se desideri utilizzare un modello di flusso di lavoro automatizzato che [!DNL Workfront] amministratore configurato e condiviso con te, selezionalo nella **[!UICONTROL Selezionare un modello di flusso di lavoro]** menu a discesa.

   >[!NOTE]
   >
   >La possibilità di modificare il modello dipende dalle impostazioni del modello configurate dal [!DNL Workfront] amministratore. Se la possibilità di modificare il modello è disabilitata, solo il proprietario del modello può modificarlo.

1. Specifica le seguenti informazioni per configurare la prima fase del flusso di lavoro automatizzato:

   * **[!UICONTROL Nome]:** Il nome dell’area di visualizzazione viene visualizzato nel diagramma del flusso di lavoro e incluso nelle notifiche e-mail inviate ai revisori.
   * **[!UICONTROL Termine]:** La funzionalità di questo campo varia a seconda dell’opzione selezionata nel **[!UICONTROL Termine calcolato a partire da]** elenco a discesa.

   * **[!UICONTROL Dalla creazione di prove]:** Seleziona la data di scadenza della bozza.
   * **[!UICONTROL Dall’attivazione dell’area di visualizzazione]:** Seleziona il numero di giorni lavorativi che verranno aggiunti alla data di attivazione dell’area di visualizzazione per impostare automaticamente una scadenza sulla bozza.
   * **[!UICONTROL Attiva fase]:** Per ogni fase del flusso di lavoro, puoi decidere quando attivarlo. Per il primo passaggio sono disponibili le seguenti opzioni.

      * Creazione a prova di
      * In una data e un&#39;ora specifiche
      * Manualmente\

         Sono disponibili opzioni aggiuntive per le fasi successive. Queste opzioni richiedono uno stadio principale. Sono:
      * Dopo il raggiungimento della scadenza precedente
      * Tutte le decisioni vengono approvate o approvate con modifiche
      * Tutte le decisioni sono approvate
      * Tutte le decisioni sono prese
   * **[!UICONTROL Termine calcolato a partire da]:** L’opzione selezionata in questo elenco a discesa influisce sulle opzioni disponibili nel **[!UICONTROL Termine]** campo .

   * **[!UICONTROL Creazione di prove]:** In **[!UICONTROL Termine]** seleziona la data di scadenza della bozza.

   * **[!UICONTROL Attivazione fase]:** In **[!UICONTROL Termine]** seleziona il numero di giorni lavorativi che verranno aggiunti alla data di attivazione dell’area di visualizzazione per impostare automaticamente una scadenza sulla bozza.

   * **[!UICONTROL Blocca fase]:** Selezionare quando è possibile bloccare l&#39;area di visualizzazione.
   * **[!UICONTROL Decisore principale]:** Selezionare il processo decisionale principale sul palco. I responsabili decisionali sono disponibili nell’elenco a discesa solo dopo aver aggiunto i revisori all’area di visualizzazione.
   * **[!UICONTROL È necessaria una sola decisione]:** Selezionare questa opzione per completare la revisione dopo che uno dei responsabili decisionali avrà preso la sua decisione.\

      Questa opzione non è disponibile se hai designato un utente nel **[!UICONTROL Decisore principale]** menu a discesa.

   * **[!UICONTROL Stage privato]:** Quando questa opzione è selezionata, i commenti e le decisioni non sono visibili alle persone che non vengono aggiunte a questa fase o che non sono autorità di vigilanza, amministratori o amministratori di fatturazione nell’account


1. (Facoltativo) Aggiungi i revisori all’area di visualizzazione.
1. Quando aggiungi revisori, considera quanto segue:

   * Un revisore può essere aggiunto a una bozza una sola volta. (Non è possibile aggiungere la stessa persona a più di un passaggio della bozza.)
   * I revisori che vengono aggiunti a uno stadio privato possono vedere solo lo stadio a cui sono aggiunti sulle prove e i commenti fatti in quello stadio.
   * Per impostazione predefinita, l’aggiunta di un utente a un’area di visualizzazione consente all’utente di accedere alla bozza dal momento in cui viene creata.\

      L’amministratore di sistema può configurare il sistema di correzione per impedire agli utenti di accedere alla bozza finché il flusso di lavoro non entra nell’area in cui è stato aggiunto l’utente. Per ulteriori informazioni, consulta

1. (Facoltativo) Fai clic su **[!UICONTROL Nuovo stadio]**, quindi ripeti i passaggi 4 e 5 per aggiungere più fasi al flusso di lavoro automatizzato.
1. Continua a creare la bozza specificando le informazioni necessarie nel [!UICONTROL Organizza] e [!UICONTROL Altre impostazioni] sezioni [!UICONTROL Nuova bozza] come descritto in

## Diagrammi automatizzati dei flussi di lavoro

Durante l’impostazione del flusso di lavoro per la bozza, noterai un diagramma in fase di creazione. Ogni fase aggiunta alla bozza viene visualizzata nel diagramma, indicando chiaramente le dipendenze tra le fasi. Gli stadi privati sono contrassegnati da un’icona chiave.

Il diagramma è mobile, il che significa che rimarrà visibile anche se scorri la pagina verso il basso.

Se non è necessario visualizzare il diagramma, è possibile nasconderlo (1).

![Diagramma.png](assets/diagram-350x93.png)

## Aggiungi un passaggio

Puoi aggiungere un ulteriore passaggio a un flusso di lavoro che stai creando o modificando.

1. Se aggiungi un’area di visualizzazione a una bozza esistente, passa alla pagina dei dettagli Prova , come descritto in [Gestisci dettagli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. In **[!UICONTROL Flusso di lavoro]** sezione, fai clic su **[!UICONTROL Nuovo stadio]**.

1. Specificare le informazioni per lo stadio come al punto 4 della sezione [!UICONTROL Creazione di una bozza con un flusso di lavoro automatizzato] in questo articolo.
1. Fai clic su **[!UICONTROL Aggiungi fase]**, quindi fai clic su **[!UICONTROL Fine]**.

## Eliminare un’area di visualizzazione

1. Fai clic sull’icona del cestino disponibile nell’angolo in alto a destra dell’area di visualizzazione (1).\
   L’icona viene visualizzata quando passi il cursore del mouse sull’area di visualizzazione.\
   ![delete_a_stage.png](assets/deleting-a-stage-350x250.png)

## Impostazioni dello stage

* **[!UICONTROL Nome della fase]**: Appare nel diagramma del flusso di lavoro ed è incluso nelle notifiche e-mail inviate ai revisori.
* **[!UICONTROL Attiva fase]**: Per ogni fase del flusso di lavoro, puoi decidere quando attivarlo. Per il primo passaggio saranno disponibili le seguenti opzioni:

   * Creazione a prova di
   * In una data e un&#39;ora specifiche
   * Manualmente
   * Solo queste tre opzioni sono disponibili per il primo passaggio. Le altre opzioni saranno disponibili quando si aggiunge una seconda fase; richiedono la selezione di uno stadio padre.
   * Al raggiungimento della scadenza precedente (è necessario selezionare uno stadio padre)
   * Tutte le decisioni sono approvate o [!UICONTROL Approvato con modifiche] (richiede il prelievo di uno stadio padre)
   * Tutte le decisioni sono approvate (richiede la selezione di uno stadio padre)
   * Vengono prese tutte le decisioni (richiede la selezione di uno stadio padre)

* **[!UICONTROL Termine]:** Puoi decidere come calcolare la scadenza in ogni fase di un flusso di lavoro. Le opzioni sono:

   * Dalla creazione della bozza: In [!UICONTROL scadenza] (9) puoi selezionare la data di scadenza della bozza.
   * Dall’attivazione dell’area di visualizzazione: In [!UICONTROL scadenza] a discesa puoi selezionare il numero di giorni lavorativi che verranno aggiunti alla data di attivazione dell’area di visualizzazione per impostare automaticamente una scadenza sulla bozza.

* **[!UICONTROL Blocca]:** Esistono diverse opzioni che determinano quando un’area di visualizzazione può essere bloccata. Le opzioni includono:

   * Blocco manuale
   * Mai
   * Quando inizia la fase successiva
   * Quando tutte le decisioni sono prese

**[!UICONTROL Decisore principale]**: Imposta il modulo decisionale principale sul palco. I responsabili decisionali disponibili vengono visualizzati nell’elenco solo dopo aver aggiunto i revisori allo stadio.

>[!NOTE]
>
>Se scegli un decision maker primario, in questa fase non sarà più disponibile una sola opzione richiesta.

* **[!UICONTROL È necessaria una sola decisione]**: È possibile abilitare questa opzione su un&#39;area di visualizzazione. Ciò significa che la revisione sarà completata una volta che uno dei decisori prenderà la decisione.
* **[!UICONTROL Privacy]:** Ogni tappa può essere resa privata. Se un passaggio è privato, i commenti e le decisioni non saranno visibili alle persone che non vengono aggiunte a questo passaggio o che non sono autorità di vigilanza, amministratori o amministratori di fatturazione nell’account. Per ulteriori informazioni, consulta [Panoramica del flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md) .

## Aggiungere i revisori a un passaggio

1. Immetti un nome di contatto o un indirizzo e-mail nel campo in fondo a ogni passaggio.
1. Fai clic sull’icona verde a forma di più per aggiungerle.
1. Imposta il ruolo sulla bozza.
1. Imposta l’avviso e-mail.
1. Quando si imposta il primo passaggio, è anche possibile modificare il proprietario della bozza.

   >[!NOTE]
   >
   >* Un revisore può essere aggiunto a una bozza una sola volta. Non è possibile aggiungere la stessa persona a più di un passaggio della bozza.
   >* I revisori che non vengono aggiunti a uno stadio privato non possono vedere lo stadio della prova o dei commenti effettuati in tale fase.



## Convertire una bozza in un flusso di lavoro automatizzato

Puoi convertire una bozza di base in Flusso di lavoro automatizzato.

1. Fai clic su **[!UICONTROL Converti in flusso di lavoro automatizzato]** sulla [!UICONTROL Dettagli della bozza] pagina.
Dopo aver rielaborato la bozza in Flusso di lavoro automatizzato, tutte le fasi sono attive, pubbliche e [!UICONTROL Blocca fase] per impostazione predefinita, è impostata su Manuale . Tutte le fasi rimangono con gli utenti e le relative impostazioni.

   * L’area di attivazione è impostata su Attiva creazione di prove in ogni fase.
   * Il termine calcolato dall&#39;opzione è impostato su Creazione di prova in ogni fase.
   * Se sulla bozza di base è stata selezionata una sola opzione di decisione, questa è selezionata per tutte le fasi.
   * Se su prova di base [!UICONTROL Decisore principale] è stato selezionato quindi gli stadi con quel destinatario sono impostati su di loro e tutti gli altri hanno impostato su Nessuno.
   * Il nome dello stage rimane lo stesso.

## Aggiungi un modello aggiuntivo a un flusso di lavoro automatizzato esistente

Una volta convertita una bozza di base in Flusso di lavoro automatizzato, puoi aggiungere un modello aggiuntivo ad essa.

1. Nella sezione Flusso di lavoro della pagina Dettagli bozza fare clic su **[!UICONTROL Aggiungi modello].**

   * Le impostazioni del modello determinano cosa è possibile fare con una bozza a cui è stato aggiunto il modello. Ad esempio, se il modello ha la [!UICONTROL Aggiungi un passaggio e aggiungi le persone ai vari stadi] opzioni disattivate, pulsanti su [!UICONTROL aggiungi fase] e [!UICONTROL prova di condivisione] non sarà visibile.
   * Se [!UICONTROL Aggiungi un’opzione di stage] è disabilitato nel modello specificato, dopo averlo aggiunto il [!UICONTROL Aggiungi modello] non sono visibili.
   * Quando una persona viene aggiunta a una fase in un modello di flusso di lavoro automatizzato, ma è già presente nella bozza, se questo modello viene applicato, il sistema rimuove automaticamente questa persona dallo stadio. Se non viene aggiunto nessun altro a questa particolare fase, verrà visualizzato il seguente errore, in quanto il sistema non consentirà di aggiungere una fase vuota al flusso di lavoro.

      ![error_when_adding_template.png](assets/error-when-adding-template-350x66.png)
