---
title: Crea campi
description: Ad Adobe, Maestro, puoi creare campi personalizzati per ogni tipo di record operativo o tassonomia. Puoi quindi associare il campo ai record Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7e2bb0ee-5f25-4307-9fec-876590c0ae1a
source-git-commit: 4946a65188391df62ad3e135a5b1dbba9a16dc89
workflow-type: tm+mt
source-wordcount: '3160'
ht-degree: 2%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!---
title: Formula fields
description: In Adobe Maestro, you can create custom fields for each kind of operational record type or taxonomy. You can then associate the field with Maestro records.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--Should the structure of this article be like this one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

# Crea campi

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono a Adobe Maestro, una nuova offerta di Adobe Workfront.
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti. Per utilizzare le funzionalità Maestro, devi essere un cliente Workfront.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

Ad Adobe, Maestro può creare campi personalizzati per tipi di record operativi o tassonomie. È quindi possibile associare i campi ai record Maestro per migliorare le informazioni sui record.

È necessario creare tipi di record prima di poter creare campi da associare. Per informazioni, consulta [Crea tipi di record](../architecture/create-record-types.md).

In Maestro puoi creare i campi nei seguenti modi:

* Da zero
* Collegando i tipi di record
* Importando i tipi di record utilizzando un file Excel e CSV
* Creazione di un tipo di record
* Creazione di un&#39;area di lavoro da un modello

Per ulteriori informazioni sui campi Maestro, consulta [Panoramica campo](../fields/fields-overview.md)

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> prodotto Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>La tua organizzazione deve essere iscritta al programma beta chiuso Adobe Maestro. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>piano Adobe Workfront</p></td>
   <td>
<p>Qualsiasi</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td>
   <td>
   <p>Qualsiasi</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Livello di accesso</td>
   <td> <p>Qualsiasi</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modello di layout</td>
   <td> <p>L’amministratore di sistema deve aggiungere l’area Maestro nel modello di layout. Per informazioni, consulta <a href="../access/grant-access.md">Concedere l’accesso a Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->



<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Crea campi da zero {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

1. Fai clic su **Menu principale** icona ![](assets/main-menu-workfront.png) nell&#39;angolo superiore destro di Workfront oppure **Menu principale** icona ![](assets/main-menu-shell.png)  nell’angolo superiore sinistro, se disponibile, fai clic su **Maestro** ![](assets/maestro-icon.png).

   Per impostazione predefinita, viene aperta l’ultima area di lavoro a cui si è effettuato l’accesso.

1. (Facoltativo) Espandere la freccia rivolta verso il basso a destra del nome di un&#39;area di lavoro esistente e selezionare l&#39;area di lavoro per la quale si desidera creare i tipi di record, quindi fare clic sul tipo di record.

   Tutti i record esistenti associati al tipo di record vengono visualizzati nelle righe della vista tabella.

   >[!TIP]
   >
   >    Se non viene visualizzato alcun record, è possibile che non siano ancora presenti record oppure che sia stato applicato un filtro che limita la visualizzazione sullo schermo.

   Tutti i campi esistenti associati al tipo di record vengono visualizzati nelle colonne della vista tabella. <!--caveat this for when we can hide the fields; mention that they can be hidden if they are not visible by default-->


1. Fai clic su **+** nell&#39;angolo superiore destro della vista tabella per aggiungere nuovi campi.
1. In **Nuovo campo** , selezionare uno dei seguenti tipi di campi:

   * [Testo a riga singola](#single-line-text)
   * [Paragrafo](#paragraph)
   * [Selezione multipla](#multi-select)
   * [Selezione singola](#single-select)
   * [Data](#date)
   * [Numero](#number)
   * [Percentuale](#percentage)
   * [Valuta](#currency)
   * [Casella di controllo](#checkbox)
   * [Persone](#people)
   * [Creato da](#created-by)
   * [Data di creazione](#created-date)
   * [Ultima modifica eseguita da](#last-modified-by)
   * [Data ultima modifica](#last-modified-date)

   >[!IMPORTANT]
   >
   >    Non è possibile modificare il tipo di campo dopo averlo salvato.

1. Continua ad aggiungere ogni campo, come descritto nelle sezioni seguenti.

### Testo a riga singola {#single-line-text}

I campi di testo a riga singola acquisiscono informazioni alfanumeriche limitate. Ad esempio, puoi acquisire le informazioni relative al Proprietario, alle parti interessate, al team o all’unità organizzativa in un campo di testo a riga singola. Il contenuto di un campo di testo a riga singola può contenere un massimo di 250 caratteri. <!-- asked Lilit if we can change this to "Single-line" since this can have numbers and text.-->

1. Inizia a creare un campo come descritto nella sezione [Crea campi da zero](#create-fields-from-scratch) in questo articolo, seleziona la **Testo su riga singola** tipo di campo.

   ![](assets/single-line-text-field-type.png)

1. Aggiungi le seguenti informazioni nella **Nuovo campo** scheda:
   * **Nome**: nome del tipo di campo che verrà visualizzato in una tabella o nella pagina Dettagli del record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrizione**: informazioni aggiuntive sul campo. La descrizione di un campo viene visualizzata quando si passa il cursore sull&#39;intestazione di colonna del campo in una tabella.
1. Fai clic su **Crea**.

   Il nuovo campo a riga singola viene aggiunto come colonna al tipo di record e i relativi valori possono essere associati ai record.


### Paragrafo {#paragraph}

I campi Paragrafo acquisiscono informazioni alfanumeriche aggiuntive su un record, simili al campo Descrizione.

>[!TIP]
>
>* Il contenuto di un campo paragrafo può contenere fino a 1.000 caratteri.
>
>* È possibile utilizzare la formattazione Rich Text per migliorare il contenuto dei campi paragrafo visualizzati nella visualizzazione Tabella o nella pagina Dettagli di un record.

1. Inizia a creare un campo come descritto nella sezione [Crea campi da zero](#create-fields-from-scratch) in questo articolo, seleziona la **Paragrafo** tipo di campo.

   ![](assets/paragraph-field-type.png)


1. Aggiungi le seguenti informazioni nella **Nuovo campo** scheda:
   * **Nome**: nome del tipo di campo che verrà visualizzato in una tabella o nella pagina Dettagli del record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrizione**: informazioni aggiuntive sul campo. La descrizione di un campo viene visualizzata quando si passa il cursore sulla colonna del campo in una tabella.
1. Fai clic su **Crea**.

   Il nuovo campo paragrafo viene aggiunto come colonna al tipo di record e i relativi valori possono essere associati ai record.


### Selezione multipla {#multi-select}

È possibile utilizzare un campo a selezione multipla per acquisire informazioni aggiuntive in qualsiasi formato selezionando più opzioni da un menu a discesa.

1. Inizia a creare un campo come descritto nella sezione [Crea campi da zero](#create-fields-from-scratch) in questo articolo, seleziona la **Selezione multipla** tipo di campo.

   ![](assets/multi-select-field-type.png)


1. Aggiungi le seguenti informazioni nella **Nuovo campo** scheda:
   * **Nome**: nome del tipo di campo che verrà visualizzato in una tabella o nella pagina Dettagli del record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrizione**: informazioni aggiuntive sul campo. La descrizione di un campo viene visualizzata quando si passa il cursore sulla colonna del campo in una tabella.
   * **Scelte**: le opzioni disponibili per la selezione dal menu a discesa dopo il salvataggio del campo. È possibile utilizzare sia numeri che lettere per il nome di ciascuna scelta.
1. Clic **Aggiungi scelta** per aggiungere tutte le scelte necessarie. Non esiste alcun limite al numero di scelte che è possibile aggiungere a un campo a selezione multipla.
1. (Facoltativo) Trascina e rilascia manualmente ciascuna scelta nell’ordine desiderato, oppure seleziona la
   **Ordina le scelte dalla A alla Z** opzione se si desidera che le scelte vengano elencate automaticamente in ordine alfabetico. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. Fai clic su **x** a destra di una scelta per rimuoverlo.
1. Fate clic sul campione di colore a sinistra di una scelta per espandere il selettore di colore e personalizzare il colore di ciascuna opzione.
1. Fai clic su **Crea**.

   Il nuovo campo a selezione multipla viene aggiunto come colonna al tipo di record e i relativi valori possono essere associati ai record.

### Selezione singola {#single-select}

I campi a selezione singola acquisiscono informazioni aggiuntive in qualsiasi formato selezionando un’opzione da un menu a discesa.

1. Inizia a creare un campo come descritto nella sezione [Crea campi da zero](#create-fields-from-scratch) in questo articolo, seleziona la **Selezione singola** tipo di campo.

   ![](assets/single-select-field-type.png)


1. Aggiungi le seguenti informazioni nella **Nuovo campo** scheda:
   * **Nome**: nome del tipo di campo che verrà visualizzato in una tabella o nella pagina Dettagli del record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrizione**: informazioni aggiuntive sul campo. La descrizione di un campo viene visualizzata quando si passa il cursore sulla colonna del campo in una tabella.
   * **Scelte**: le opzioni disponibili per la selezione dal menu a discesa dopo il salvataggio del campo. È possibile utilizzare sia numeri che lettere per il nome di ciascuna scelta.

1. Clic **Aggiungi scelta** per aggiungere tutte le scelte necessarie. Non esiste alcun limite al numero di scelte che è possibile aggiungere a un campo a selezione singola.
1. (Facoltativo) Trascina e rilascia manualmente ciascuna scelta nell’ordine desiderato, oppure seleziona la **Ordina le scelte dalla A alla Z** opzione se si desidera che le scelte vengano elencate automaticamente in ordine alfabetico. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. Fai clic su **x** a destra di una scelta per rimuoverlo.
1. Fate clic sul campione di colore a sinistra di una scelta per espandere il selettore di colore e personalizzare il colore di ciascuna opzione.
1. Fai clic su **Crea**.

   Il nuovo campo a selezione singola viene aggiunto come colonna al tipo di record e i relativi valori possono essere associati ai record.

### Data {#date}

È possibile utilizzare un campo data per acquisire informazioni aggiuntive in formato data e ora.

1. Inizia a creare un campo come descritto nella sezione [Crea campi da zero](#create-fields-from-scratch) in questo articolo, seleziona la **Data** tipo di campo.

   ![](assets/date-field-type.png)


1. Aggiungi le seguenti informazioni nella **Nuovo campo** scheda:
   * **Nome**: nome del tipo di campo che verrà visualizzato in una tabella o nella pagina Dettagli del record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrizione**: informazioni aggiuntive sul campo. La descrizione di un campo viene visualizzata quando si passa il cursore sulla colonna del campo in una tabella.
   * **Formato data**: tipo di formato della data che desideri visualizzare in questo campo. <!--update this casing - submitted bug for it-->

     Selezionare uno dei formati seguenti:
      * **Lingua**: corrisponde alle impostazioni locali del browser.
      * **Standard**: 05/16/2023
      * **Lungo**: 16 maggio 2023
      * **Europeo**: 16/05/2023
      * **ISO**: 2023-05-16
   * **Includi un campo ora**: seleziona questa opzione se desideri includere un timestamp. Questa opzione è deselezionata per impostazione predefinita. <!--update this setting name - submitted bug for it to be changed-->

     Selezionare una delle opzioni seguenti:

      * **24 ore**: ad esempio: 18:00
      * **12 ore**: ad esempio: 18:00

1. Fai clic su **Crea**.

   Il nuovo campo data viene aggiunto come colonna al tipo di record e i relativi valori possono essere associati ai record.

### Numero {#number}

I tipi di campo numerico acquisiscono informazioni in formato numerico.

1. Inizia a creare un campo come descritto nella sezione [Crea campi da zero](#create-fields-from-scratch) in questo articolo, seleziona la **Numero** tipo di campo.

   ![](assets/number-field-type.png)
1. Aggiungi le seguenti informazioni nella **Nuovo campo** scheda:

   * **Nome**: nome del tipo di campo che verrà visualizzato in una tabella o nella pagina Dettagli del record.
   * **Descrizione**: informazioni aggiuntive sul campo. La descrizione di un campo viene visualizzata quando si passa il cursore sulla colonna del campo in una tabella.
   * **Precisione**: numero di decimali da registrare per il campo. Puoi visualizzare fino a 6 decimali.
   * **Consenti numeri negativi**: seleziona questa opzione se desideri consentire l’utilizzo di numeri negativi in questo campo. Questa opzione è deselezionata per impostazione predefinita.

   >[!NOTE]
   >
   >    Se si seleziona Consenti numeri negativi e i valori negativi vengono memorizzati nei record a cui è associato il campo, non sarà più possibile deselezionare l&#39;impostazione in futuro.

1. Fai clic su **Crea**.

   Il nuovo campo numerico viene aggiunto come colonna al tipo di record e i relativi valori possono essere associati ai record.

### Percentuale {#percentage}

I tipi di campo Percentuale acquisiscono le informazioni in un formato numerico seguito da un segno di percentuale.

1. Inizia a creare un campo come descritto nella sezione [Crea campi da zero](#create-fields-from-scratch) in questo articolo, seleziona la **Percento** tipo di campo.

   ![](assets/percentage-field-type.png)

1. Aggiungi le seguenti informazioni nella **Nuovo campo** scheda:
   * **Nome**: nome del tipo di campo che verrà visualizzato in una tabella o nella pagina Dettagli del record.
   * **Descrizione**: informazioni aggiuntive sul campo. La descrizione di un campo viene visualizzata quando si passa il cursore sulla colonna del campo in una tabella.
   * **Precisione**: numero di decimali da registrare per il campo. Puoi visualizzare fino a 6 decimali.
   * **Consenti numeri negativi**: seleziona questa opzione se desideri consentire valori percentuali negativi in questo campo. Questa opzione è deselezionata per impostazione predefinita.

   >[!NOTE]
   >
   >    Se si seleziona Consenti numeri negativi e i valori negativi vengono memorizzati nei record a cui è associato il campo, non sarà più possibile deselezionare l&#39;impostazione in futuro.

1. Fai clic su **Crea**.

   Il nuovo campo percentuale viene aggiunto come colonna al tipo di record e i relativi valori possono essere associati ai record.

### Valuta {#currency}

I tipi di campo Valuta acquisiscono le informazioni in un formato numerico preceduto da un simbolo di valuta.

1. Inizia a creare un campo come descritto nella sezione [Crea campi da zero](#create-fields-from-scratch) in questo articolo, seleziona la **Valuta** tipo di campo.

   ![](assets/currency-field-type.png)

1. Aggiungi le seguenti informazioni nella **Nuovo campo** scheda:
   * **Nome**: nome del tipo di campo che verrà visualizzato in una tabella o nella pagina Dettagli del record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrizione**: informazioni aggiuntive sul campo. La descrizione di un campo viene visualizzata quando si passa il cursore sulla colonna del campo in una tabella.
   * **Valuta**: tipo di valuta da visualizzare in questo campo. Questa è una lista di valute secondo l&#39;Organizzazione Internazionale di Standardizzazione (ISO).
   * **Precisione**: numero di decimali da registrare per il campo. Puoi visualizzare fino a 6 decimali.
   * **Consenti numeri negativi**: seleziona questa opzione se desideri consentire valori di valuta negativi in questo campo. Questa opzione è deselezionata per impostazione predefinita.

   >[!NOTE]
   >
   >    Se si seleziona Consenti numeri negativi e i valori negativi vengono memorizzati nei record a cui è associato il campo, non sarà più possibile deselezionare l&#39;impostazione in futuro.

1. Fai clic su **Crea**.

   Il nuovo campo valuta viene aggiunto come colonna al tipo di record e i relativi valori possono essere associati ai record.

### Casella di controllo

È possibile utilizzare il tipo di campo Casella di controllo per aggiungere una singola opzione a un record. È possibile utilizzare questo campo per indicare un attributo o uno stato specifico per quel record specifico. È ad esempio possibile utilizzarlo come flag per tenere traccia di completamento, approvazione o qualsiasi altro attributo binario per ogni record.

1. Inizia a creare un campo come descritto nella sezione [Crea campi da zero](#create-fields-from-scratch) in questo articolo, seleziona la **Casella di controllo** tipo di campo.

   ![](assets/checkbox-field-type.png)

1. Aggiungi le seguenti informazioni nella **Nuovo campo** scheda:
   * **Nome**: nome del tipo di campo che verrà visualizzato in una tabella o nella pagina Dettagli del record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrizione**: informazioni aggiuntive sul campo. La descrizione di un campo viene visualizzata quando si passa il cursore sulla colonna del campo in una tabella.
1. Fai clic su **Crea**.

   Il nuovo campo casella di controllo viene aggiunto come colonna al tipo di record e i relativi valori possono essere associati ai record.

### Persone

È possibile utilizzare il tipo di campo Persone per aggiungere un utente <!--, job role, or team--> a un record. Questo è un campo di completamento automatico ed è possibile aggiungere solo utenti<!--, roles, or teams--> che esistono già in Workfront.

1. Inizia a creare un campo come descritto nella sezione [Crea campi da zero](#create-fields-from-scratch) in questo articolo, seleziona la **Persone** tipo di campo.

   ![](assets/people-field-type.png)

1. Aggiungi le seguenti informazioni nella **Nuovo campo** scheda:
   * **Nome**: nome del tipo di campo che verrà visualizzato in una tabella o nella pagina Dettagli del record.
   * **Descrizione**: informazioni aggiuntive sul campo. La descrizione di un campo viene visualizzata quando si passa il cursore sulla colonna del campo in una tabella.
   * **Consenti più valori**: seleziona questa opzione se desideri consentire agli utenti di aggiungere più di un utente in questo campo. Questa opzione è deselezionata per impostazione predefinita.

   >[!NOTE]
   >
   >    Se si seleziona Consenti più valori e più utenti vengono memorizzati nei record a cui è associato il campo, non sarà più possibile deselezionare l&#39;impostazione in futuro durante la modifica del campo.

1. Fai clic su **Crea**.

   Il nuovo campo Persone viene aggiunto come colonna al tipo di record e i relativi valori possono essere associati ai record.

### Creato da

È possibile utilizzare il tipo di campo Creato da per aggiungere l&#39;utente che ha creato il record a un record. Questo campo è di sola lettura e viene compilato automaticamente con il nome dell&#39;utente che ha eseguito l&#39;accesso al momento della creazione del record.

1. Inizia a creare un campo come descritto nella sezione [Crea campi da zero](#create-fields-from-scratch) in questo articolo, seleziona la **Creato da** tipo di campo.

   ![](assets/created-by-field-type.png)

1. Aggiungi le seguenti informazioni nella **Nuovo campo** scheda:

   * **Nome**: nome del tipo di campo che verrà visualizzato in una tabella o nella pagina Dettagli del record. <!--this might change and they might prepopulate it with "Created by"-->
   * **Descrizione**: informazioni aggiuntive sul campo. La descrizione di un campo viene visualizzata quando si passa il cursore sulla colonna del campo in una tabella.

1. Fai clic su **Crea**.

   Il nuovo campo Creato per tipo viene aggiunto come colonna al tipo di record e i relativi valori vengono precompilati con il nome dell’utente che ha creato ciascun record.


### Data di creazione

È possibile utilizzare il tipo di campo Data di creazione per aggiungere la data di creazione di un record a un record. Questo campo è di sola lettura e viene compilato automaticamente con la data (e facoltativamente con l’ora) di creazione del record.

1. Inizia a creare un campo come descritto nella sezione [Crea campi da zero](#create-fields-from-scratch) in questo articolo, seleziona la **Data di creazione** tipo di campo.

   ![](assets/created-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Aggiungi le seguenti informazioni nella **Nuovo campo** scheda:

   * **Nome**: nome del tipo di campo che verrà visualizzato in una tabella o nella pagina Dettagli del record. <!--this might change and they might prepopulate it with "Created date"-->
   * **Descrizione**: informazioni aggiuntive sul campo. La descrizione di un campo viene visualizzata quando si passa il cursore sulla colonna del campo in una tabella.
   * **Formato data**: seleziona uno dei seguenti formati:

      * **Lingua**: corrisponde alle impostazioni locali del browser.
      * **Standard**: 05/16/2023
      * **Lungo**: 16 maggio 2023
      * **Europeo**: 16/05/2023
      * **ISO**: 2023-05-16
   * **Includi un campo ora**: seleziona questa opzione se desideri includere un timestamp. Questa opzione è deselezionata per impostazione predefinita. <!--submitted a UI text change for this - check the UI-->

     Selezionare una delle opzioni seguenti:

      * **24 ore**: ad esempio: 18:00
      * **12 ore**: ad esempio: 18:00

1. Fai clic su **Crea**.

   Il nuovo campo Data creazione viene aggiunto come colonna al tipo di record e i relativi valori vengono precompilati con la data (o la data e l’ora) di creazione del record.


### Ultima modifica eseguita da

È possibile utilizzare il tipo di campo Ultima modifica per per aggiungere a un record l&#39;ultimo utente che ha modificato il record. Questo campo è di sola lettura e viene compilato automaticamente con il nome dell&#39;utente che ha eseguito l&#39;accesso l&#39;ultimo aggiornamento del record.

1. Inizia a creare un campo come descritto nella sezione [Crea campi da zero](#create-fields-from-scratch) in questo articolo, seleziona la **Ultima modifica eseguita da** tipo di campo.

   ![](assets/last-modified-by-field-type.png)

1. Aggiungi le seguenti informazioni nella **Nuovo campo** scheda:

   * **Nome**: nome del tipo di campo che verrà visualizzato in una tabella o nella pagina Dettagli del record. <!--this might change and they might prepopulate it with "Created by"-->
   * **Descrizione**: informazioni aggiuntive sul campo. La descrizione di un campo viene visualizzata quando si passa il cursore sulla colonna del campo in una tabella.

1. Fai clic su **Crea**.

   Il nuovo campo Ultima modifica per tipo viene aggiunto come colonna al tipo di record e i relativi valori vengono precompilati con il nome dell’ultimo utente che ha modificato ogni record.


### Data ultima modifica

È possibile utilizzare il tipo di campo Data ultima modifica per aggiungere la data dell&#39;ultima modifica di un record a un record. Questo campo è di sola lettura e viene compilato automaticamente con la data (e facoltativamente con l&#39;ora) dell&#39;ultima modifica del record.

1. Inizia a creare un campo come descritto nella sezione [Crea campi da zero](#create-fields-from-scratch) in questo articolo, seleziona la **Data di creazione** tipo di campo.

   ![](assets/last-modified-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Aggiungi le seguenti informazioni nella **Nuovo campo** scheda:

   * **Nome**: nome del tipo di campo che verrà visualizzato in una tabella o nella pagina Dettagli del record. <!--this might change and they might prepopulate it with "Created date"-->
   * **Descrizione**: informazioni aggiuntive sul campo. La descrizione di un campo viene visualizzata quando si passa il cursore sulla colonna del campo in una tabella.
   * **Formato data**: seleziona uno dei seguenti formati:

      * **Lingua**: corrisponde alle impostazioni locali del browser.
      * **Standard**: 05/16/2023
      * **Lungo**: 16 maggio 2023
      * **Europeo**: 16/05/2023
      * **ISO**: 2023-05-16
   * **Includi un campo ora**: seleziona questa opzione se desideri includere un timestamp. Questa opzione è deselezionata per impostazione predefinita. <!--submitted a UI text change for this - check the UI-->

     Selezionare una delle opzioni seguenti:

      * **24 ore**: ad esempio: 18:00
      * **12 ore**: ad esempio: 18:00

1. Fai clic su **Crea**.

   Il nuovo campo Ultima modifica del tipo di data viene aggiunto come colonna al tipo di record e i relativi valori vengono precompilati con la data (o data e ora) dell’ultima modifica apportata al record.

## Creare i campi collegando i tipi di record

È possibile creare campi record collegati quando si aggiunge una nuova connessione tra due tipi di record Maestro o un tipo di record e un tipo di oggetto di altre applicazioni.

Per informazioni sulla connessione dei tipi di record Maestro, vedere [Connetti tipi di record](../architecture/connect-record-types.md)

## Creare campi importando tipi di record tramite un file Excel e CSV

Per ulteriori informazioni, consulta [Crea tipi di record](../architecture/create-record-types.md).

## Creare campi creando un tipo di record

Quando si crea un tipo di record, per impostazione predefinita vengono creati anche diversi campi associati al nuovo tipo di record. Per ulteriori informazioni, consulta [Creare tipi di record operativi](../architecture/create-record-types.md).

## Creare campi creando un’area di lavoro da un modello

Maestro crea campi per tipi di record operativi e tassonomie quando crei un’area di lavoro da un modello.

Per informazioni, consulta [Creare aree di lavoro operative](../architecture/create-workspaces.md).