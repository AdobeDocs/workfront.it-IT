---
title: Aggiungere o modificare un’immagine o un altro widget di risorse in un modulo personalizzato con il generatore di moduli legacy
description: Puoi aggiungere o modificare le proprietà di uno qualsiasi dei seguenti widget di risorse, come immagini, video, file PDF e file Adobe XD, in un modulo personalizzato. Questa funzione ti consente di includere contenuti visivi, come immagini di branding, un video istruttivo o un prototipo interattivo per un’app che stai progettando.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 62a2f9a1-80de-40e7-9d8b-46ed9df083c1
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '1344'
ht-degree: 1%

---

# Aggiungere o modificare un’immagine o un altro widget di risorse in un modulo personalizzato con il generatore di moduli legacy

Puoi aggiungere o modificare le proprietà di uno qualsiasi dei seguenti widget di risorse in un modulo personalizzato:

* Immagine
* Video
* file PDF
* File Adobe XD

Questa funzione ti consente di includere contenuti visivi, come immagini di branding, un video istruttivo o un prototipo interattivo per un’app che stai progettando.

Quando a un oggetto viene allegato un modulo personalizzato contenente un widget, gli utenti che utilizzano l&#39;oggetto possono visualizzarlo nelle seguenti aree:

* L’area Dettagli dell’oggetto (ad esempio, per un progetto, l’area Dettagli progetto)
* La casella Modifica dell’oggetto, se presenta il nuovo aspetto dell’esperienza Adobe Workfront (ad esempio le caselle Modifica progetto e Modifica attività)

Attualmente, gli utenti non possono visualizzare il widget nelle seguenti aree:&#x200B;

* Elenchi e rapporti
* Home e Riepilogo
* La casella Modifica dell’oggetto, se non ha il nuovo aspetto dell’esperienza Adobe Workfront (ad esempio, la casella Modifica spesa)
* L’app mobile di Workfront


## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni sulle modalità di concessione dell'accesso da parte degli amministratori di Workfront, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Per informazioni sulle configurazioni di piano, tipo di licenza o livello di accesso disponibili, contattare l&#39;amministratore Workfront.

## Aggiungere o modificare un widget di risorse in un modulo personalizzato

1. Iniziare a lavorare su un modulo personalizzato, come descritto in [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Con il **Aggiungi un campo** apri la scheda, effettua una delle seguenti operazioni:

   * Se state aggiungendo un nuovo widget, selezionate **Immagine**, **PDF**, o **Video** per aggiungerlo nella parte inferiore del modulo o trascinarlo nella posizione desiderata all&#39;interno del modulo.

      ![](assets/add-widget.png)


   * Se desideri aggiungere un widget già aggiunto a un altro modulo personalizzato, fai clic su **Libreria campi**, quindi fare clic sul nome del widget nell&#39;elenco visualizzato. Per ulteriori informazioni, consulta [Riutilizzare un campo personalizzato o un widget in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   * Se stai modificando un widget già aggiunto al modulo personalizzato, selezionalo.

1. Digitate o modificate una delle seguenti proprietà per il widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il widget. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: evita di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il widget.</p> <p>Quando configuri il widget per la prima volta e digiti l’etichetta, il campo Nome si popola automaticamente in modo che corrisponda a esso. Tuttavia, i campi Etichetta e Nome non sono sincronizzati. In questo modo è possibile modificare l'etichetta visualizzata dagli utenti senza dover cambiare il nome visualizzato dal sistema.</p> <p><b>IMPORTANTE</b>: anche se è possibile farlo, ti consigliamo di non modificare questo nome dopo che tu o altri utenti iniziate a utilizzare il modulo personalizzato in widget. In questo caso, il sistema non riconoscerà più il widget a cui potrebbe ora fare riferimento in altre aree di Workfront. </p> <p>Ogni nome di widget deve essere univoco nell’istanza Workfront della tua organizzazione. In questo modo, è possibile riutilizzare un modulo già creato per un altro modulo personalizzato. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obbligatorio) Digita o incolla l’URL del widget in cui è memorizzato su Internet.</p> 
       <p><strong>Importante</strong>: l’URL di deve essere un URL pubblico. </p>
      <p>Se stai aggiungendo un widget video, al momento puoi farlo aggiungendo quanto segue nella casella URL:</p> 
      <ul> 
      <li> <p>Collegamento YouTube o Vimeo</p> </li> 
      <li> <p>Collegamento video Google Drive</p> </li> 
      <li> <p>Collegamento a video con estensione MP4 e MOV</p> </li> 
      <li> <p>Collegamento a un video già caricato nell’area Documenti della tua istanza di Workfront. Per istruzioni, consulta <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Aggiungere un widget video a un modulo personalizzato dall’area Documenti</a> in questo articolo.</p> 
      </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Digita eventuali informazioni aggiuntive sul widget. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dimensione</td> 
      <td>Modifica le dimensioni di visualizzazione del widget in base alle esigenze.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Applica**.
1. Se si desidera continuare a creare il modulo personalizzato in altri modi, passare a uno dei seguenti articoli:

   * [Posizionare campi e widget personalizzati in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Riutilizzare un campo personalizzato o un widget in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Aggiungere logica di visualizzazione e logica di salto a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Anteprima e completamento di un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)


## Aggiungere un file XD a un modulo personalizzato

1. Iniziare a lavorare su un modulo personalizzato, come descritto in [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Con il **Aggiungi un campo** apri la scheda, seleziona **Adobe XD**.
1. Digitate o modificate una delle seguenti proprietà per il widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il widget. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: evita di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il widget.</p> <p>Quando configuri il widget per la prima volta e digiti l’etichetta, il campo Nome si popola automaticamente in modo che corrisponda a esso. Tuttavia, i campi Etichetta e Nome non sono sincronizzati. In questo modo è possibile modificare l'etichetta visualizzata dagli utenti senza dover cambiare il nome visualizzato dal sistema.</p> <p><b>IMPORTANTE</b>: anche se è possibile farlo, ti consigliamo di non modificare questo nome dopo che tu o altri utenti iniziate a utilizzare il modulo personalizzato in widget. In questo caso, il sistema non riconoscerà più il widget a cui potrebbe ora fare riferimento in altre aree di Workfront. </p> <p>Ogni nome di widget deve essere univoco nell’istanza Workfront della tua organizzazione. In questo modo, è possibile riutilizzare un modulo già creato per un altro modulo personalizzato. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obbligatorio) Digita o incolla un collegamento valido per il prototipo XD.</p> 
      <p>Nota: l’impostazione Accesso link nella scheda Condividi di Adobe XD deve essere impostata su Chiunque abbia il link. In caso contrario, gli utenti non potranno visualizzare il prototipo. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>(Facoltativo) Digita eventuali informazioni aggiuntive sul widget. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dimensione</td> 
      <td>(Facoltativo) Modifica la dimensione di visualizzazione del widget in base alle esigenze.</td> 
     </tr> 
    </tbody> 
   </table>

1. Se si desidera continuare a creare il modulo personalizzato in altri modi, passare a uno dei seguenti articoli:

   * [Posizionare campi e widget personalizzati in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Riutilizzare un campo personalizzato o un widget in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Aggiungere logica di visualizzazione e logica di salto a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Anteprima e completamento di un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## Aggiungere un widget video a un modulo personalizzato dall’area Documenti {#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Quando si aggiunge un video a un modulo personalizzato in questo modo, al video vengono applicate solo le autorizzazioni impostate per il modulo personalizzato quando gli utenti accedono al modulo su un oggetto, non le autorizzazioni impostate per il video nell&#39;area Documenti.

1. Vai al video nell’area Documenti e genera una bozza per esso, come descritto in [Creare una bozza interattiva per un sito web o altro contenuto web](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Apri la bozza.
1. Fai clic con il pulsante destro del mouse in un punto qualsiasi del video, quindi seleziona **Copia indirizzo video**.
1. Nel modulo personalizzato in cui stai aggiungendo il widget video, incolla l’indirizzo copiato nel **URL** casella.
