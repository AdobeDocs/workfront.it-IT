---
title: Gestire i record nella sezione Pianificazione degli oggetti di Adobe Workfront
description: È possibile visualizzare i record di Workfront Planning connessi agli oggetti di Adobe Workfront nella sezione Planning di un oggetto di Workfront, nel pannello sinistro.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '1433'
ht-degree: 1%

---


<!--add also Group and Company when they are available-->

# Gestire le connessioni record dagli oggetti Workfront

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

In Workfront è possibile visualizzare i record di Workfront Planning e i rispettivi record connessi agli oggetti di Adobe Workfront nelle seguenti aree:

* Sezione Planning di un oggetto Workfront: visualizza tutti i tipi di record connessi a un oggetto e i rispettivi record connessi.
* Un campo personalizzato della connessione Planning: visualizza un tipo di record e i relativi record collegati.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per Workfront Planning.

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
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning*</p></td>
   <td>
<p>Qualsiasi</p>
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p>
   </td>

<tr>
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td>
   <td>
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p>
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p>
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
   <p>In Workfront Planning, visualizzare le autorizzazioni di un'area di lavoro per visualizzare tutti i record connessi o le autorizzazioni Contribute o superiori a un'area di lavoro per connettere o disconnettere i record</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro di Workfront Planning, incluse quelle non create</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>Per visualizzare l'area Planning o la sezione Planning per un oggetto Workfront, a tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale e l'area Planning per i progetti, i portfolio e i programmi. </p> Per ulteriori informazioni, vedere <a href="/help/quicksilver/planning/access/access-overview.md">Panoramica dell'accesso di Adobe Planning</a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gestire i record nella sezione Pianificazione

È possibile utilizzare la sezione Planning di un oggetto Workfront per visualizzare tutti i tipi di record e i rispettivi record connessi all&#39;oggetto Workfront.
La sezione Pianificazione è disponibile per i seguenti oggetti Workfront:

* Progetto
* Portfolio
* Programma
<!--* Group
* Company-->

### Considerazioni sulla sezione Pianificazione degli oggetti di Workfront

Quando si visualizzano i record di Workfront Planning dalla sezione Planning di un oggetto Workfront, tenere presente quanto segue:

* I tipi di record di Workfront Planning devono prima essere connessi ai tipi di oggetto di Workfront.

  Per informazioni, vedere i seguenti articoli:

   * [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Connetti record](/help/quicksilver/planning/records/connect-records.md)
* È possibile visualizzare la sezione Planning da un oggetto Workfront, anche quando non vi sono record associati all&#39;oggetto Workfront.

### Gestire le connessioni ai record dalla sezione Planning

{{step1-to-planning}}

1. Fai clic sulla scheda di un’area di lavoro.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic sulla scheda di un tipo di record connesso a un progetto, portfolio o programma Workfront.
1. Passare a un campo record connesso che presenta una connessione con un oggetto Workfront, nella visualizzazione tabella o dalla pagina dei dettagli di un record. Per informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).
1. Fare clic sul nome di un oggetto Workfront nel campo record connesso.
La pagina dell&#39;oggetto si apre in Workfront.

   >[!NOTE]
   >
   >  Se si conosce un oggetto Workfront già connesso a un record di Planning, è possibile passare alla sezione Planning dall&#39;oggetto Workfront.

1. Fare clic su **Pianificazione** nel pannello sinistro.

   >[!NOTE]
   >
   >   L&#39;amministratore del Workfront o del gruppo deve aggiungere la sezione Pianificazione al modello di layout prima che venga visualizzata per un progetto, un portfolio o un programma Workfront.

   Viene visualizzata la sezione Pianificazione con le seguenti informazioni:

   * I record collegati vengono visualizzati su singole schede contenenti le seguenti informazioni:
      * Nome del record
      * La miniatura del record
      * Nome del campo record connesso visualizzato in Workfront Planning.
   * I record vengono visualizzati nel rispettivo workspace e tipo di record.

   ![](assets/planning-section-on-project.png)

1. (Facoltativo) Fare clic su **Mostra tutte le connessioni** per visualizzare tutti i tipi di record connessi, inclusi quelli senza record connessi. Per impostazione predefinita, i tipi di record senza record collegati non vengono visualizzati.
1. Fare clic su una scheda record per visualizzare ulteriori informazioni sul record. Viene visualizzata la casella di anteprima del record.
1. (Facoltativo) Inizia a modificare i campi nella casella di anteprima del record. Le modifiche vengono salvate automaticamente.
1. (Facoltativo) Fai clic sull&#39;icona ![](assets/open-details-in-a-new-tab-icon.png) di **Apri in una nuova scheda** nell&#39;angolo superiore destro della casella di anteprima per aprire la pagina dei dettagli del record. La pagina dei dettagli del record viene visualizzata in Workfront Planning.
1. (Facoltativo) Passa il puntatore del mouse su una scheda record, quindi fai clic sull&#39;icona Disconnetti record **-**, quindi fai clic su **Disconnetti**.
Si verificano le seguenti situazioni:
   * Il record non è più connesso all&#39;oggetto Workfront.
   * L&#39;oggetto Workfront viene inoltre rimosso dal campo connesso del record da Workfront Planning.
   * Vengono eliminati anche i valori dei campi di ricerca di Workfront connessi al record Planning.
1. Fai clic su **Connetti** per connettere altri record per i tipi di record connessi. Per ulteriori informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

   Si verificano le seguenti situazioni:

   * I record vengono immediatamente collegati all&#39;oggetto Workfront e vengono visualizzati nella sezione Planning.
   * L&#39;oggetto Workfront viene aggiunto al campo connesso del record di Workfront Planning.
   * I valori dei campi di ricerca di Workfront connessi al record Planning vengono inseriti in Workfront Planning.

## Gestire i record nel tipo di campo Connessione Planning

È possibile utilizzare un campo personalizzato della connessione Planning su un oggetto Workfront per visualizzare un tipo di record e i relativi record collegati all&#39;oggetto Workfront.

È possibile controllare i tipi di record di Planning visualizzati per l&#39;oggetto Workfront quando si creano i campi personalizzati della connessione di Planning.

* Nel campo Connessione Planning vengono visualizzati i record di Planning dopo che è stata stabilita una connessione e quando il campo viene associato ai moduli per i seguenti oggetti di Workfront:

   * Progetto
   * Portfolio
   * Programma
   * Gruppo
   * Azienda

Per ulteriori informazioni, vedere [Creare un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Considerazioni sul tipo di campo Connessione Planning

Quando si visualizzano i record di Workfront Planning da un campo di connessione di Planning di un oggetto Workfront, tenere presente quanto segue:

* È possibile associare un solo tipo di record a un campo di connessione Planning.
* Se si dispone dell&#39;accesso corretto, è necessario allegare un modulo personalizzato con un campo personalizzato della connessione Planning a un oggetto Workfront che può essere connesso da Workfront Planning.
* I tipi di record di Workfront Planning devono prima essere connessi ai tipi di oggetto di Workfront. Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).
* È possibile connettere o disconnettere record dal campo di connessione Planning di un oggetto Workfront solo per gli oggetti che possono disporre di connessioni Workfront Planning.
* È necessario disporre delle autorizzazioni Contribute per un&#39;area di lavoro in Workfront Planning per poter connettere o disconnettere i record dal campo di connessione Planning di un oggetto Workfront.
* Non è possibile modificare un campo di connessione di Planning quando si modificano in blocco oggetti di Workfront.

### Gestire le connessioni record dal tipo di campo Connessione Planning

1. Passare a uno dei tipi di oggetto seguenti che è stato connesso a un tipo di record di Workfront Planning:

   * Progetto
   * Portfolio
   * Programma
   * Azienda
   * Gruppo

1. Fare clic su **&lt; Oggetto > Dettagli** nel pannello a sinistra.
1. (Condizionale) Aggiungi un modulo personalizzato con almeno un campo di connessione Planning per l’oggetto selezionato, se non ne è presente uno.

   >[!NOTE]
   >
   >Prima di poter aggiungere il modulo a un oggetto, è necessario che l&#39;amministratore del Workfront o del gruppo crei il modulo e aggiunga un campo di connessione Planning.


1. Fare clic all&#39;interno del campo per aggiungere record collegati, quindi fare clic sulla freccia rivolta verso il basso all&#39;interno del campo per selezionare i record dall&#39;elenco.

   ![](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >Non è possibile aggiungere record ai campi di connessione di Planning associati a oggetti di Workfront diversi dall&#39;oggetto selezionato al momento della configurazione del campo.
   >
   >Non è possibile, ad esempio, aggiungere record a un campo di connessione di Planning creato per una connessione di Portfolio dal modulo personalizzato di un progetto.
   >
   >L&#39;oggetto del campo e l&#39;oggetto selezionato non corrispondono.
   >
   >![](assets/warning-unsupported-object-planning-connection-field-on-form.png)

1. Fare clic all&#39;esterno dell&#39;elenco per chiuderlo.

   Si verificano le seguenti situazioni:

   * I record vengono immediatamente connessi all&#39;oggetto Workfront e vengono visualizzati nel campo di connessione Planning e nella sezione Planning dell&#39;oggetto Workfront.
   * L&#39;oggetto Workfront viene aggiunto al campo connesso del record di Workfront Planning.
   * I valori dei campi di ricerca di Workfront connessi al record Planning vengono inseriti in Workfront Planning.
1. (Facoltativo) Fare clic sul nome di un record nel campo Connessione Planning per aprirlo in Workfront Planning.
In Workfront Planning viene visualizzata la scheda Dettagli record.
È possibile esaminare le informazioni sul record oppure passare alla pagina del tipo di record.

1. (Facoltativo) Dal modulo personalizzato in Workfront, fare clic sull&#39;icona ![](assets/remove-icon.png) **Rimuovi** su un record per rimuoverlo dal campo di connessione di Planning e disconnetterlo dall&#39;oggetto Workfront.
L&#39;oggetto Workfront viene disconnesso dal record Planning e tutte le informazioni di ricerca provenienti da Workfront vengono rimosse dal record.