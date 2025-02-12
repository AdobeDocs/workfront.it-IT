---
product-area: projects
navigation-topic: manage-issues
title: Visualizza i problemi
description: È possibile visualizzare i problemi associati a un progetto, un'attività o un'iterazione.
author: Alina
feature: Work Management
exl-id: b6791c8f-b356-4235-8b0e-952e29a88952
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 0%

---

# Visualizza i problemi

È possibile visualizzare i problemi associati a un progetto, un&#39;attività o un&#39;iterazione.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiedi o superiore</p> <p>Rivedi o una licenza superiore per visualizzare i problemi nella sezione Problemi di un progetto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Visualizza l’accesso alle Issues</p> <p>Accesso di visualizzazione o superiore ai progetti e alle attività</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni sull'accesso ai problemi nel tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concedere l'accesso ai problemi</a>. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni per il problema</p> <p> Per informazioni sulla concessione delle autorizzazioni per i problemi, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema </a></p> <p>Per informazioni sulla richiesta di autorizzazioni aggiuntive, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Visualizza i problemi in base allo stato

Per visualizzare i problemi relativi a un progetto, un&#39;attività o un&#39;iterazione:

1. Apri un progetto, un&#39;attività o un&#39;iterazione che contiene problemi, quindi fai clic su **Problemi** nel pannello a sinistra.

1. Per visualizzare tutti i problemi, aperti o chiusi, fai clic su uno dei filtri elencati di seguito dal menu a discesa **Filtro**.

>[!TIP]
>
>L’elenco dei filtri varia a seconda dell’opzione selezionata dall’amministratore di sistema o di gruppo per visualizzarlo.

* **Apri:** visualizza i problemi aperti.

  Sono inclusi quelli associati a un oggetto risolutivo e quelli in stato Chiuso - In attesa di approvazione.

  Per informazioni sulla risoluzione di oggetti, vedere [Panoramica sulla risoluzione e la risoluzione di oggetti](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

* **Completato:** visualizza tutti i problemi con una data di completamento effettiva.
* **Tutti** visualizza tutti i problemi.

## Informazioni sui problemi

Quando si accede a un problema è possibile visualizzare le relative informazioni.

Per accedere a un problema e visualizzarne le informazioni:

1. Apri un progetto, un&#39;attività o un&#39;iterazione che contiene problemi, quindi fai clic su **Problemi** nel pannello a sinistra.
1. Dal menu a discesa **Filtro**, seleziona il filtro per visualizzare i problemi che stai tentando di visualizzare.

   Selezionare una delle opzioni seguenti:

   * Aperti
   * Completato
   * Tutti

1. Fai clic sul nome di un problema.

   Quando si dispone delle autorizzazioni di gestione per il problema, è possibile modificare qualsiasi campo modificabile del problema e aggiungere approvazioni, ore o documenti al problema.

1. Dal pannello a sinistra, fai clic su una delle seguenti opzioni per visualizzare ulteriori informazioni sul problema:

* **Aggiornamenti**: è possibile eseguire le azioni seguenti:

   * Commenta il problema o rispondi a un commento esistente.
   * Tempo di connessione.
   * Modifica lo stato del problema.

     Per ulteriori informazioni sull&#39;aggiornamento del lavoro in Workfront, vedere [Aggiorna lavoro](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* **Documenti**: allega documenti al problema. Per ulteriori informazioni sull&#39;aggiunta di documenti a Workfront, vedere [Aggiungere documenti ad Adobe Workfront dal file system](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

* **Dettagli problema**: espandi questo collegamento per visualizzare le aree **Panoramica** e **Forms** personalizzate.

  Se disponi di autorizzazioni di gestione per il problema e diritti di modifica sul modulo personalizzato, puoi modificare alcune informazioni qui.

  Visualizza o modifica i campi seguenti nell&#39;area **Panoramica**:

   * **Nome**
   * **Percorso**: il percorso attraverso il quale il problema è stato registrato nel progetto.

     Se un problema è stato inviato come richiesta in una coda di richieste, qui sono elencati i nomi del progetto, il Gruppo di argomenti e l’Argomento coda. Impossibile modificare questo campo.

     Per ulteriori informazioni sull&#39;invio di richieste, vedere [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

   * **Descrizione**
   * **URL**: qualsiasi indirizzo Web relativo al problema.
   * **Priorità**: un flag visivo che consente di assegnare la priorità ai problemi.
   * **Gravità**: un flag visivo che indica la gravità del problema descritto nel problema.
   * **Contatto principale**: il contatto principale predefinito è l&#39;utente che ha creato il problema. Questo campo può essere modificato.
   * **Ore pianificate**: visualizza la quantità di tempo che un utente impiegherà per completare il problema. Il valore predefinito è 8 ore. Questo campo può essere modificato.
   * **Ore effettive**: visualizza il tempo necessario per completare il problema. Questa è l&#39;ora effettiva in cui qualcuno registra il problema.
   * **Data inizio pianificata**: la data in cui è pianificato l&#39;inizio del problema. L’impostazione predefinita è la data e l’ora di creazione del problema.
   * **Data di inizio effettiva**: la data e l&#39;ora in cui lo stato del problema è stato modificato in In corso.
   * **Data di completamento pianificata**: la data in cui è pianificato il completamento del problema.
   * **Data di completamento effettiva**: la data in cui il problema è stato effettivamente completato. Questo campo viene compilato automaticamente quando lo stato del problema diventa Chiuso o Risolto, oppure può essere modificato manualmente.
   * **Costo effettivo**: il costo basato sulle ore effettive registrate sul problema. Campo non modificabile. Il costo effettivo di un problema viene calcolato in base alla formula seguente, in cui Tasso costo utente è la tariffa di costo associata all&#39;utente che registra il tempo al problema:

     Costo effettivo problema = Ore registrate * Tasso costo utente

   * **Inserito da**: l&#39;utente che ha creato il problema. Campo non modificabile.
   * **Ultimo aggiornamento eseguito da**: questo è l&#39;utente che ha aggiornato per ultimo qualsiasi campo del problema. Campo non modificabile.

     Nell&#39;area **Forms** personalizzato, visualizzazione di uno o più moduli personalizzati da associare al problema.

* **Ore**: mostra un elenco delle ore inserite nel problema.
* **Approvazioni:** mostra i percorsi di approvazione associati al problema.

  Per ulteriori informazioni sull&#39;associazione delle approvazioni a un problema, vedere la sezione [Associazione di un processo di approvazione a un elemento di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md#associating-the-approval-process-with-an-object) in [Creazione di un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Visualizza i progetti e le attività con problemi

È possibile aggiungere icone nella visualizzazione di un progetto, di un report attività o di un elenco per indicare se sono presenti problemi allegati. L&#39;aggiunta di icone alla visualizzazione di un report o di un elenco è simile per i progetti e le attività.

Per aggiungere icone che mostrano se un progetto presenta problemi in un report di progetto:

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront.
1. Fai clic su **Generazione rapporti** > **Nuovo rapporto** > **Rapporto progetto**.
1. Nel campo **Mostra in questa colonna**, inizia a digitare **Icone di stato**, quindi selezionala quando viene visualizzata nell&#39;elenco.

1. Fare clic su **Salva + Chiudi**.

   Le icone dei problemi vengono visualizzate nei progetti che presentano problemi nella colonna **Icone di stato**.

   ![elenco_progetti_con_icona_problema.png](assets/project-list-with-issue-icon-350x132.png)
