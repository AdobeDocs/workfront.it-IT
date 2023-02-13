---
product-area: projects
navigation-topic: manage-issues
title: Visualizza problemi
description: È possibile visualizzare i problemi associati a un progetto, un'attività o un'iterazione.
author: Alina
feature: Work Management
exl-id: b6791c8f-b356-4235-8b0e-952e29a88952
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 0%

---

# Visualizza problemi

È possibile visualizzare i problemi associati a un progetto, un&#39;attività o un&#39;iterazione.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> <p>Rivedi o una licenza superiore per visualizzare i problemi nella sezione Problemi di un progetto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizza l'accesso ai problemi</p> <p>Visualizza o consente un accesso più elevato a progetti e attività</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni sull'accesso ai problemi relativi al livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concedere l’accesso ai problemi</a>. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza le autorizzazioni per il problema</p> <p> Per informazioni sulla concessione delle autorizzazioni per i problemi, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema </a></p> <p>Per informazioni sulla richiesta di autorizzazioni aggiuntive, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Visualizza i problemi in base allo stato

Per visualizzare i problemi relativi a un progetto, un&#39;attività o un&#39;iterazione:

1. Apri un progetto, un&#39;attività o un&#39;iterazione che contiene problemi, quindi fai clic su **Problemi** nel pannello a sinistra.

1. Per visualizzare tutti i problemi aperti o chiusi, fai clic su uno dei filtri elencati di seguito nella sezione **Filtro** menu a discesa.

>[!TIP]
>
>L’elenco dei filtri varia a seconda della selezione effettuata dall’amministratore di sistema o di gruppo per visualizzarli.

* **Apri:** Visualizza i problemi aperti.

   Sono inclusi quelli associati a un oggetto di risoluzione e quelli in uno stato di approvazione chiuso in sospeso.

   Per informazioni sulla risoluzione degli oggetti, vedere [Panoramica sulla risoluzione e risoluzione di oggetti](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

* **Completato:** Visualizza tutti i problemi che hanno una data di completamento effettiva.
* **Tutto** Visualizza tutti i problemi.

## Informazioni sui problemi

Puoi visualizzare informazioni su un problema quando accedi a esso.

Per accedere a un problema e visualizzare le relative informazioni:

1. Apri un progetto, un&#39;attività o un&#39;iterazione che contiene problemi, quindi fai clic su **Problemi** nel pannello a sinistra.
1. Da **Filtro** menu a discesa, seleziona il filtro per visualizzare i problemi che stai tentando di visualizzare.

   Seleziona una delle seguenti opzioni:

   * Aperto
   * Completato
   * Tutti

1. Fai clic sul nome di un problema.

   Quando si dispone delle autorizzazioni di gestione per il problema è possibile modificare qualsiasi campo modificabile del problema e aggiungere approvazioni, ore o documenti al problema.

1. Dal pannello a sinistra, fai clic su una delle seguenti opzioni per visualizzare ulteriori informazioni sul problema:

* **Aggiornamenti**: Puoi eseguire le seguenti azioni:

   * Commenta il problema o rispondi a un commento esistente.
   * Tempo di log.
   * Modifica lo stato del problema.

      Per ulteriori informazioni sull&#39;aggiornamento dei lavori in Workfront, vedi [Aggiorna lavoro](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* **Documenti**: Allega documenti al problema. Per ulteriori informazioni sull’aggiunta di documenti a Workfront, consulta [Aggiungere documenti ad Adobe Workfront dal file system](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

* **Dettagli del problema**: Espandi questo collegamento per visualizzare il **Panoramica** e **Forms personalizzato** aree.

   Se si dispone delle autorizzazioni di gestione per il problema e dei diritti di modifica nel modulo personalizzato, è possibile modificare alcune informazioni qui.

   Visualizza o modifica i campi seguenti nella sezione **Panoramica** area:

   * **Nome**
   * **Percorso**: il percorso in cui il problema è stato registrato nel progetto.

      Se un problema è stato inviato come richiesta in una coda di richiesta, i nomi del progetto, del gruppo di argomenti e dell&#39;argomento della coda sono elencati qui. Impossibile modificare il campo.

      Per ulteriori informazioni sull’invio delle richieste, vedi [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

   * **Descrizione**
   * **URL**: qualsiasi indirizzo web relativo al problema.
   * **Priorità**: un flag visivo che ti consente di assegnare priorità ai problemi.
   * **Gravità**: un flag visivo che indica la gravità del problema descritto nel problema.
   * **Contatto principale**: il contatto primario predefinito è l&#39;utente che ha creato il problema. È possibile modificare questo campo.
   * **Orari pianificati**: visualizza il tempo necessario a un utente per completare il problema. Il valore predefinito è 8 ore. È possibile modificare questo campo.
   * **Ore effettive**: visualizza il tempo necessario per completare il problema. Questo è il momento in cui qualcuno effettua il log per il problema.
   * **Data di inizio prevista**: la data in cui è pianificato l’inizio del problema. L’impostazione predefinita è la data e l’ora in cui è stato creato il problema.
   * **Data di inizio effettiva**: la data e l&#39;ora in cui lo stato del problema è stato modificato in In corso.
   * **Data completamento pianificata**: la data in cui è prevista la conclusione del problema.
   * **Data completamento effettivo**: la data in cui il problema è effettivamente completato. Questo campo viene compilato automaticamente quando lo stato del problema diventa Chiuso o Risolto oppure può essere modificato manualmente.
   * **Costo effettivo**: il costo in base alle ore effettive registrate sul problema. Questo campo non è modificabile. Il costo effettivo di un problema viene calcolato in base alla seguente formula, in cui il tasso di costo utente è il tasso di costo associato all&#39;utente che registra il tempo al problema:

      Costo effettivo problema = ore registrate * Tasso di costo utente

   * **Inserito da**: questo è l’utente che ha creato il problema. Questo campo non è modificabile.
   * **Ultimo aggiornamento di**: questo è l’utente che ha aggiornato qualsiasi campo del problema per ultimo. Questo campo non è modificabile.

      In **Forms personalizzato** area , visualizzazione della selezione di uno o più moduli personalizzati da associare al problema.

* **Ore**: Mostra un elenco di voci orarie sul problema.
* **Approvazioni:** Mostra i percorsi di approvazione associati al problema.

   Per ulteriori informazioni sull&#39;associazione delle approvazioni a un problema, consulta la [Associazione di un processo di approvazione a un elemento di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md#associating-the-approval-process-with-an-object) sezione [Creazione di un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Visualizzare quali progetti e attività presentano problemi

È possibile aggiungere icone nella visualizzazione di un progetto o di un rapporto di attività o di un elenco per indicare se i problemi sono associati. L’aggiunta di icone alla visualizzazione di un rapporto o di un elenco è simile per i progetti e le attività.

Per aggiungere icone che mostrano se un progetto presenta problemi in un rapporto di progetto:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.
1. Fai clic su **Reporting** > **Nuovo rapporto** > **Rapporto sul progetto**.
1. In **Mostra in questa colonna** campo, inizia a digitare **Icone di stato**, quindi selezionalo quando viene visualizzato nell’elenco.

1. Fai clic su **Salva e chiudi** .

   Le icone dei problemi vengono visualizzate nei progetti che presentano problemi nella **Icone di stato** colonna.

   ![project_list_with_issue_icon.png](assets/project-list-with-issue-icon-350x132.png)
