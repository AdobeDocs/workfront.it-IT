---
title: Gestire i record nella sezione Pianificazione degli oggetti di Adobe Workfront
description: È possibile visualizzare i record connessi agli oggetti di Adobe Workfront nella sezione Pianificazione di un oggetto di Workfront, nel pannello sinistro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 4d76ef1b34d484e3da2af94543a5fd660ad0a4ef
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 1%

---

<!--add this to the main TOC and the mini TOC-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--add also Group and Company when they are available-->


# Gestire i record nella sezione Pianificazione degli oggetti di Adobe Workfront

{{maestro-important-intro}}

È possibile visualizzare i record connessi agli oggetti di Adobe Workfront nella sezione Pianificazione di un oggetto di Workfront, nel pannello sinistro.

La sezione Pianificazione è disponibile per i seguenti oggetti Workfront:

* Progetto
* Portfolio
* Programma
<!--* Group
* Company-->

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Prodotto</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>La tua organizzazione deve essere iscritta al programma beta di Adobe Workfront Planning. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>piano Adobe Workfront</p></td>
   <td>
<p>Qualsiasi</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td>
   <td>
   <p>Nuovo: Standard</p>
   Oppure
   <p>Corrente: Piano</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td>
   <td> <p>Accesso di visualizzazione o superiore a progetti, programmi e Portfoli</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>In Workfront, puoi visualizzare o accedere ad altre autorizzazioni per un progetto, un portfolio o un programma</a> </p> 
   <p>In Workfront Planning, visualizzare o autorizzazioni superiori per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro di Workfront Planning, incluse quelle non create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L'amministratore del Workfront o del gruppo deve aggiungere al modello di layout l'area Pianificazione nel menu principale e la sezione Pianificazione nel pannello sinistro. Per informazioni, consulta <a href="../access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Per ulteriori informazioni, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Considerazioni sulla sezione Pianificazione degli oggetti di Workfront

* Innanzitutto, è necessario connettere i tipi di record ai tipi di oggetto Workfront e i record agli oggetti Workfront per visualizzarli in Workfront.

  Per informazioni, vedere i seguenti articoli:

   * [Connetti tipi di record](/help/quicksilver/maestro/architecture/connect-record-types.md)
   * [Connetti record](/help/quicksilver/maestro/records/connect-records.md)
* È possibile visualizzare la sezione Planning in un oggetto Workfront, anche quando non vi sono record associati all&#39;oggetto Workfront.
* È possibile collegare i record di Planning agli oggetti di Workfront da Workfront, nella sezione Planning.

## Gestire i record nella sezione Pianificazione

{{step1-to-maestro}}

Per impostazione predefinita, viene aperta l’ultima area di lavoro a cui si è effettuato l’accesso.

1. Fare clic sulla scheda di un tipo di record connesso a un progetto, portfolio o programma Workfront.
1. Scegliere una vista tabella dal menu **Visualizza** menu a discesa.
1. (Facoltativo) Vai al campo del record connesso nella tabella e aggiungi un oggetto Workfront, quindi fai clic sul nome dell’oggetto Workfront nel campo. Per informazioni, consulta [Collega record](/help/quicksilver/maestro/records/connect-records.md).
La pagina degli oggetti viene visualizzata in Workfront Planning.
1. Clic **Vai all&#39;origine**, nell&#39;angolo superiore destro dello schermo.

   La pagina dell&#39;oggetto si apre in Workfront.
1. Clic **Pianificazione** nel pannello a sinistra.

   >[!NOTE]
   >
   >   L&#39;amministratore del Workfront o del gruppo deve aggiungere la sezione Pianificazione al modello di layout prima che venga visualizzata per un progetto, portfolio o programma Workfront.

   Viene visualizzata la sezione Pianificazione con le seguenti informazioni:

   * I record collegati vengono visualizzati su singole schede contenenti le seguenti informazioni:
      * Nome del record
      * La miniatura del record
      * Nome del campo record connesso visualizzato in Workfront Planning.
   * I record vengono visualizzati nel rispettivo workspace.

   ![](assets/planning-section-on-project.png)

1. Fare clic su una scheda record per visualizzare ulteriori informazioni sul record. Viene visualizzata la casella di anteprima del record.
1. (Facoltativo) Inizia a modificare i campi nella casella di anteprima del record. Le modifiche vengono salvate automaticamente.
1. (Facoltativo) Fai clic su **Apri in una nuova scheda** icona ![](assets/open-details-in-a-new-tab-icon.png) nell&#39;angolo superiore destro della casella di anteprima per aprire la pagina dei dettagli del record.
1. Passa il puntatore del mouse su una scheda record, quindi fai clic sull&#39;icona Disconnetti record **-**, quindi fai clic su **Disconnetti**.
Si verificano le seguenti situazioni:
   * Il record non è più connesso all&#39;oggetto Workfront.
   * L&#39;oggetto Workfront viene inoltre rimosso dal campo connesso del record da Workfront Planning.
   * Vengono eliminati anche i valori dei campi Workfront connessi al record Planning.
1. Clic **Connetti** per collegare altri record.

   <!--checking with the team on the below note - not sure if if should stay Manage or Contribute - Lilit said Contribute??-->

   >[!NOTE]
   >
   >   Il pulsante Connetti viene visualizzato solo per le aree di lavoro per le quali si dispone delle autorizzazioni Contribute.

1. Fare clic sui record che si desidera connettere. Si verificano le seguenti situazioni:

   * I record vengono immediatamente collegati all&#39;oggetto Workfront e vengono visualizzati nella sezione Planning.
   * L&#39;oggetto Workfront viene aggiunto al campo connesso del record di Workfront Planning.
   * I valori dei campi Workfront connessi al record Planning vengono inseriti in Workfront Planning.

<!--add more steps here for what happens after clicking Connect-->

