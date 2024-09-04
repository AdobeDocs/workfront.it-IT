---
title: Gestire i record nella sezione Pianificazione degli oggetti di Adobe Workfront
description: È possibile visualizzare i record di Workfront Planning connessi agli oggetti di Adobe Workfront nella sezione Planning di un oggetto di Workfront, nel pannello sinistro.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 1%

---


<!--add also Group and Company when they are available-->

# Gestire i record nella sezione Pianificazione degli oggetti di Adobe Workfront

{{planning-important-intro}}

È possibile visualizzare i record di Workfront Planning connessi agli oggetti di Adobe Workfront nella sezione Planning di un oggetto di Workfront, nel pannello sinistro.

La sezione Pianificazione è disponibile per i seguenti oggetti Workfront:

* Progetto
* Portfolio
* Programma
<!--* Group
* Company-->

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per Workfront Planning.

Per accedere a Workfront Planning, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Prodotti</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td>
   <td>
<p>Uno dei seguenti piani di Workfront:</p>
<ul><li>Seleziona</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p>
   </td>

<tr>
   <td role="rowheader"><p>Piano di pianificazione Adobe Workfront*</p></td>
   <td>
<p>Qualsiasi</p>
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p>
   </td>

<tr>
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td>
   <td>
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p>
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata di Adobe per Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td>
   <td>
   <p>Standard</p>
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td>
   <td> <p>Accesso di visualizzazione o superiore a progetti, programmi e Portfoli</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td>
   <td>
   <p>In Workfront, visualizzare o autorizzazioni superiori per un progetto, portfolio o programma</a> </p> 
   <p>In Workfront Planning, Contribute o autorizzazioni superiori per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro di Workfront Planning, incluse quelle non create</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale e l'area Planning per i progetti, i portfolio e i programmi. </p> Per ulteriori informazioni, vedere <a href="/help/quicksilver/planning/access/access-overview.md">Panoramica dell'accesso</a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sulla sezione Pianificazione degli oggetti di Workfront

* I tipi di record di Workfront Planning devono essere connessi ai tipi di oggetto di Workfront.

  Per informazioni, vedere i seguenti articoli:

   * [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Connetti record](/help/quicksilver/planning/records/connect-records.md)
* È possibile visualizzare la sezione Planning in un oggetto Workfront, anche quando non vi sono record associati all&#39;oggetto Workfront.
* È possibile connettere i record di Planning con gli oggetti di Workfront da Workfront, nella sezione Planning quando è presente almeno un record connesso all&#39;oggetto di Workfront.

## Gestire i record nella sezione Pianificazione

{{step1-to-planning}}

1. Fai clic sulla scheda di un’area di lavoro.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic sulla scheda di un tipo di record connesso a un progetto, portfolio o programma Workfront.
1. Passare a un campo record connesso che presenta una connessione con un oggetto Workfront, nella visualizzazione tabella o dalla pagina dei dettagli di un record. Per informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).
1. Fare clic sul nome di un oggetto Workfront nel campo record connesso.
La pagina degli oggetti si apre in Workfront.

1. Fare clic su **Pianificazione** nel pannello sinistro.

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

1. (Facoltativo) Fare clic su **Mostra tutte le connessioni** per visualizzare tutti i tipi di record connessi, inclusi quelli senza record connessi. Per impostazione predefinita, i tipi di record senza record collegati non vengono visualizzati.
1. Fare clic su una scheda record per visualizzare ulteriori informazioni sul record. Viene visualizzata la casella di anteprima del record.
1. (Facoltativo) Inizia a modificare i campi nella casella di anteprima del record. Le modifiche vengono salvate automaticamente.
1. (Facoltativo) Fai clic sull&#39;icona ![](assets/open-details-in-a-new-tab-icon.png) di **Apri in una nuova scheda** nell&#39;angolo superiore destro della casella di anteprima per aprire la pagina dei dettagli del record. La pagina dei dettagli del record viene visualizzata in Workfront Planning.
1. Passa il puntatore del mouse su una scheda record, quindi fai clic sull&#39;icona Disconnetti record **-**, quindi fai clic su **Disconnetti**.
Si verificano le seguenti situazioni:
   * Il record non è più connesso all&#39;oggetto Workfront.
   * L&#39;oggetto Workfront viene inoltre rimosso dal campo connesso del record da Workfront Planning.
   * Vengono eliminati anche i valori dei campi di ricerca di Workfront connessi al record Planning.
1. Fai clic su **Connetti** per connettere altri record per i tipi di record connessi. Per ulteriori informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

   Si verificano le seguenti situazioni:

   * I record vengono immediatamente collegati all&#39;oggetto Workfront e vengono visualizzati nella sezione Planning.
   * L&#39;oggetto Workfront viene aggiunto al campo connesso del record di Workfront Planning.
   * I valori dei campi di ricerca di Workfront connessi al record Planning vengono inseriti in Workfront Planning.


