---
title: Gestire i record nella sezione Pianificazione degli oggetti di Adobe Workfront
description: È possibile visualizzare i record di Workfront Planning connessi agli oggetti di Adobe Workfront nella sezione Planning di un oggetto di Workfront, nel pannello sinistro.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '1847'
ht-degree: 1%

---


<!--add also Group and Company when they are available-->

# Gestire le connessioni record dagli oggetti Workfront

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedi [Abilitare o disabilitare le versioni rapide per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

È possibile visualizzare i record di Workfront Planning in Workfront nelle seguenti aree degli oggetti ad essi collegati:

* Sezione Planning di un oggetto Workfront: visualizza tutti i tipi di record connessi a un oggetto e i rispettivi record connessi.
* Un campo personalizzato della connessione Planning: visualizza un tipo di record, i rispettivi record connessi e fino a 7 campi di ricerca dei record connessi.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

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
   <td> <p>Visualizzare o accedere più facilmente a progetti, programmi e portafogli</p>  
   <p>Nessuna configurazione del livello di accesso per Workfront Planning. </p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td>
   <td>
   <p>In Workfront, visualizzare o autorizzazioni superiori per un progetto, portfolio o programma</a> </p> 
   <p>In Workfront Planning:
   <ul><li>
   Visualizza le autorizzazioni per un'area di lavoro <span class="preview"> e il tipo di record</span> per visualizzare tutti i record connessi </li>
   oppure
   <li> Autorizzazioni Contribute o superiori per un'area di lavoro <span class="preview"> e un tipo di record</span> per connettere o disconnettere record</a></li></ul> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro di Workfront Planning, incluse quelle non create</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> <p>Nell'ambiente di produzione, tutti gli utenti, inclusi gli amministratori di sistema, devono essere assegnati a un modello di layout che includa Planning.</p>
<p><span class="preview">Nell'ambiente di anteprima, per impostazione predefinita, Planning è abilitato per utenti standard e amministratori di sistema.</span></p>  </p>  
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

   ![Sezione Pianificazione sul progetto](assets/planning-section-on-project.png)

1. (Facoltativo) Fare clic su **Mostra tutte le connessioni** per visualizzare tutti i tipi di record connessi, inclusi quelli senza record connessi. Per impostazione predefinita, i tipi di record senza record collegati non vengono visualizzati.
1. Fare clic su una scheda record per visualizzare ulteriori informazioni sul record. Viene visualizzata la casella di anteprima del record.
1. (Facoltativo) Inizia a modificare i campi nella casella di anteprima del record. Le modifiche vengono salvate automaticamente.
1. (Facoltativo) Fai clic sull&#39;icona **Apri in una nuova scheda** ![Apri i dettagli in una nuova scheda](assets/open-details-in-a-new-tab-icon.png) nell&#39;angolo superiore destro della casella di anteprima per aprire la pagina dei dettagli del record. La pagina dei dettagli del record viene visualizzata in Workfront Planning.
1. (Facoltativo) Passa il puntatore del mouse su una scheda record, quindi fai clic sull&#39;icona Disconnetti record **-**, quindi fai clic su **Disconnetti**.
Si verificano le seguenti situazioni:
   * Il record non è più connesso all&#39;oggetto Workfront.
   * L&#39;oggetto Workfront viene inoltre rimosso dal campo connesso del record da Workfront Planning.
   * Vengono eliminati anche i valori dei campi di ricerca di Workfront connessi al record Planning.
1. Fai clic su **Connetti** per connettere altri record per i tipi di record connessi.

   Per ulteriori informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).
1. (Facoltativo) Se non riesci a trovare un record da connettere e vuoi aggiungerlo, fai clic su **+ Aggiungi** per aggiungere un nuovo record. Per ulteriori informazioni, vedere la sezione &quot;Creare record durante la connessione da altri record&quot; nell&#39;articolo [Creare record](/help/quicksilver/planning/records/create-records.md).

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

* Un campo di connessione Planning viene visualizzato nei modi seguenti nel modulo personalizzato di un oggetto Workfront, dopo che i record Planning sono connessi all&#39;oggetto Workfront:

   * Se è selezionato solo il campo principale del record connesso, il campo Connessione Planning viene visualizzato come campo con più valori, se la connessione consente il collegamento di più record. Per informazioni, vedere [Panoramica sui tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types-overview.md).
   * Se l&#39;amministratore del Workfront o del gruppo ha aggiunto campi di ricerca aggiuntivi dal record connesso nella maschera personalizzata, il campo di connessione di Planning viene visualizzato come tabella. È possibile selezionare fino a 7 campi per il campo di connessione Planning. La vista tabella è di sola lettura.

* È possibile associare un solo tipo di record a un campo di connessione Planning. Non esiste alcun limite al numero di campi di connessione di Planning presenti in un modulo.
* Per allegare un modulo personalizzato con un campo personalizzato della connessione Planning a un oggetto Workfront, è necessario disporre dell&#39;accesso e delle autorizzazioni corretti per l&#39;oggetto, il record e Workfront Planning.
* Per poter connettere o disconnettere record dal campo di connessione Planning di un oggetto Workfront, è necessario disporre delle autorizzazioni Contribute per un&#39;area di lavoro in Workfront Planning.
* I tipi di record di Workfront Planning devono prima essere connessi ai tipi di oggetto di Workfront. Per informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).In questo modo i record di Workfront Planning sono accessibili da Workfront.
* È possibile connettere o disconnettere record dal campo di connessione Planning di un oggetto Workfront solo per gli oggetti che possono disporre di connessioni Workfront Planning.

  È possibile, ad esempio, allegare ai task un modulo personalizzato con un campo di connessione Planning, ma non collegare oggetti di Workfront Planning ai task.
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

   ![Campo di connessione Planning nel progetto con elenco record aperto](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >Non è possibile aggiungere record ai campi di connessione di Planning associati a oggetti di Workfront diversi dall&#39;oggetto selezionato al momento della configurazione del campo.
   >
   >Non è ad esempio possibile aggiungere record a un campo di connessione di Planning creato per una connessione di Portfolio dal modulo personalizzato di un progetto.
   >
   >L&#39;oggetto del campo e l&#39;oggetto selezionato non corrispondono.
   >
   >![Avviso oggetto non supportato Campo di connessione Planning nel modulo](assets/warning-unsupported-object-planning-connection-field-on-form.png)

1. Fare clic all&#39;esterno dell&#39;elenco per chiuderlo.

   Si verificano le seguenti situazioni:

   * I record vengono immediatamente connessi all&#39;oggetto Workfront e vengono visualizzati nel campo di connessione Planning e nella sezione Planning dell&#39;oggetto Workfront.
   * L&#39;oggetto Workfront viene aggiunto al campo connesso del record di Workfront Planning.
   * I valori dei campi di ricerca di Workfront connessi al record Planning vengono inseriti in Workfront Planning.
   * Se l&#39;amministratore del Workfront o del gruppo ha aggiunto campi di ricerca dei record al momento della creazione della maschera personalizzata, i campi di ricerca del record vengono compilati automaticamente in una visualizzazione per tabella. La vista tabella nel campo della connessione Planning è di sola lettura.

     ![Campo di connessione Planning con tabella nel modulo personalizzato Dettagli progetto](assets/planning-connection-field-with-table-on-project-details-custom-form.png)

     >[!NOTE]
     >
     >La vista tabella viene visualizzata solo quando i campi di ricerca sono stati aggiunti al campo Connessioni di Planning nella maschera personalizzata.


1. (Facoltativo) Fare clic sul nome di un record o passare il puntatore del mouse sul nome del record nella tabella, quindi fare clic sull&#39;icona **Apri record** ![Apri record sul modulo personalizzato di connessione Planning](assets/open-record-icon-on-planning-connection-custom-form.png) nel campo di connessione Planning per aprirlo in Workfront Planning.
Viene visualizzata la casella di anteprima dei dettagli dei record di Workfront Planning.
1. Rivedi o modifica le informazioni sul record oppure fai clic sull&#39;icona **Apri in una nuova scheda** ![Apri record in una nuova scheda](assets/open-details-in-a-new-tab-icon.png) per aprire la pagina dei dettagli del record.

1. (Facoltativo) Dal modulo personalizzato in Workfront, fare clic sull&#39;icona **Rimuovi** ![Rimuovi icona](assets/remove-icon.png) su un record per rimuoverlo dal campo di connessione di Planning e disconnetterlo dall&#39;oggetto Workfront.
L&#39;oggetto Workfront viene disconnesso dal record Planning e tutte le informazioni di ricerca provenienti da Workfront vengono rimosse dal record.

1. Fai clic su **Salva modifiche** per salvare il modulo personalizzato e tutte le altre modifiche apportate all&#39;oggetto Workfront.
