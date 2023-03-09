---
title: Organizzare e visualizzare in anteprima un modulo con Progettazione moduli
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile organizzare un modulo personalizzato con Progettazione moduli.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 529de9d31be883325d425dceb286d750397c5d8e
workflow-type: tm+mt
source-wordcount: '1107'
ht-degree: 0%

---


# Organizzare e visualizzare in anteprima un modulo con il progettista del modulo

{{highlighted-preview-article-level}}

È possibile organizzare un modulo personalizzato con il progettista del modulo.

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
   <td>
   <p>Piano corrente: Standard</p>
   <p>oppure</p>
   <p>Piano legacy: piano</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni sulle modalità di concessione dell'accesso da parte degli amministratori di Workfront, vedere <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

## Aggiungere un’interruzione di sezione

È possibile raggruppare i campi personalizzati e i widget in un modulo personalizzato in sezioni con intestazioni. Ciò è utile per presentare un’esperienza organizzata agli utenti che compileranno il modulo. Inoltre, se devi limitare l’accesso a determinati campi personalizzati e widget a determinati utenti, puoi inserirli in una sezione e quindi concedere l’accesso alla sezione solo a tali utenti.

Ad esempio, se devi tenere traccia delle informazioni riservate che solo gli amministratori di sistema possono visualizzare o modificare, puoi creare un’interruzione di sezione con le autorizzazioni Solo amministratore e inserire i campi sensibili in tale sezione.

Le impostazioni di accesso selezionate per una sezione sono direttamente correlate alle autorizzazioni di cui dispongono gli utenti sull’oggetto Workfront a cui è allegato il modulo personalizzato. È possibile nascondere o visualizzare una sezione a seconda che l&#39;utente disponga dell&#39;accesso per visualizzare, contribuire o gestire l&#39;oggetto. In alternativa, è possibile impostare una sezione su Solo amministratore in modo che solo gli utenti con un livello di accesso amministratore di sistema possano accedervi.

Per informazioni sulle autorizzazioni per gli oggetti, vedi [Panoramica delle autorizzazioni di condivisione sugli oggetti](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Per informazioni sui campi personalizzati e i widget nei moduli personalizzati, vedi [Progettare un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Creare e configurare l’accesso per una sezione in un modulo personalizzato

1. Inizia a creare o modificare un modulo personalizzato e ad aggiungere campi, come descritto in [Progettare un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Clic **Interruzione di sezione** e trascinarlo nella posizione desiderata sull’area di lavoro.

1. Nel pannello a destra, configura le opzioni desiderate per la sezione:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra la sezione. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: evita di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Digita del testo per spiegare agli utenti a cosa serve la sezione. Questo viene visualizzato sotto l’etichetta della sezione nel modulo personalizzato.</td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Use display logic to specify whether the section should display on the form, based on selections users make in multi-choice custom fields when they fill out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> -->
     <tr> 
      <td role="rowheader"> <p>Concedi l’accesso</p> </td> 
      <td> <p> Per visualizzare questa sezione e modificare i valori dei campi, seleziona le autorizzazioni necessarie per un oggetto a cui è allegato il modulo personalizzato. 
       <p>Le seguenti autorizzazioni sono disponibili in <b>Gli utenti con questo accesso all’oggetto possono visualizzare i valori dei campi</b>:</p> 
         <ul>  
          <li><p><b>Modifica limitata</b>: (disponibile solo se l’oggetto è un progetto, un’attività, un problema o un utente):</p> 
          <p>Consente agli utenti di contribuire all'oggetto se si tratta di un progetto, attività o problema.</p>
          <p>Consente agli utenti di modificare il profilo o di disporre dell'autorizzazione di profilo per l'oggetto, se si tratta di un utente.</p></li> 
          <li><b>Modifica</b>: gestione delle autorizzazioni per l’oggetto </li> 
          <li><b>Solo amministratore</b>: livello di accesso Amministratore di sistema</li> 
         </ul> </li> 
        <p>Le seguenti autorizzazioni sono disponibili in <b>Gli utenti con questo accesso all’oggetto possono modificare i valori dei campi</b>: </p> 
         <ul> 
          <li> <p><b>Modifica limitata</b>: (disponibile solo se l’oggetto è un progetto, un’attività, un problema o un utente):</p> 
           <p>Se l'oggetto rappresenta un progetto, un'attività o un problema, questa autorizzazione consente agli utenti di contribuire all'oggetto</p>
          <p>Se l’oggetto è un utente, questa autorizzazione consente agli utenti di modificare il profilo o di essere proprietari dell’autorizzazione di profilo per l’oggetto.</p> 
          <li><b>Modifica</b>: gestione delle autorizzazioni per l’oggetto </li> 
          <li><b>Solo amministratore</b>: livello di accesso Amministratore di sistema</li> 
         </ul> </li> 
       </ul> 
       <p>Per informazioni sulle autorizzazioni per gli oggetti, vedi <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Panoramica delle autorizzazioni di condivisione sugli oggetti</a>.</p> 
       <p><b>NOTA</b>:  
       <ul> 
       <li> <p>Gli utenti senza le autorizzazioni specificate qui non possono visualizzare i campi personalizzati e i widget nella sezione. </p> <p>Questo vale anche se visualizzi i valori dei campi nei rapporti o li utilizzi nei campi calcolati nella generazione rapporti in modalità testo.</p> </li> 
       <li> <p>L'associazione di più tipi di oggetto al modulo può modificare le autorizzazioni di visualizzazione e modifica disponibili in questi passaggi. Per ulteriori informazioni, consulta <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Come più tipi di oggetto possono influenzare le autorizzazioni di interruzione di sezione in un modulo personalizzato</a> in questo articolo.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Trascina o aggiungi almeno un campo personalizzato o un widget nella nuova sezione. Questa operazione è necessaria prima di salvare la sezione.

1. Clic **Fine**.

   >[!TIP]
   >
   >Puoi fare clic su **Applica** in qualsiasi momento durante la creazione di un modulo personalizzato per salvare le modifiche e mantenere aperto il modulo.

### Come più tipi di oggetto possono influire sulle autorizzazioni dell’interruzione di sezione {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

L’autorizzazione Modifica limitata per le interruzioni di sezione del modulo personalizzato è disponibile solo per i tipi di oggetto Progetto, Attività, Problema e Utente.

In un modulo personalizzato con un&#39;interruzione di sezione configurata con l&#39;autorizzazione Modifica limitata, se si aggiunge uno degli altri tipi di oggetto al modulo (Portfolio, Programma, Documento, Società, Fatturazione, Iterazione, Spesa o Gruppo), verrà richiesto di passare all&#39;autorizzazione Modifica, che è compatibile sia con il tipo di oggetto sia con i tipi di oggetto esistenti nel modulo.

>[!INFO]
>
>**Esempio:** In un modulo personalizzato associato al tipo di oggetto Progetto, viene configurata un’interruzione di sezione con l’autorizzazione Modifica limitata.
>
>Aggiungendo al modulo il tipo di oggetto Portfolio, l&#39;opzione di autorizzazione Modifica limitata non sarà più disponibile per l&#39;interruzione di sezione nel modulo.
>
>In un messaggio sullo schermo viene richiesto di passare all&#39;autorizzazione Modifica, che è il livello di autorizzazioni minimo compatibile sia con il tipo di oggetto Progetto che con il tipo di oggetto Portfolio.


## Posizionare campi e widget personalizzati in un modulo personalizzato


1. Iniziare a creare o modificare un modulo personalizzato, come descritto in [Progettare un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Per posizionare campi personalizzati e widget sulla stessa riga, trascinare uno accanto all&#39;altro fino a visualizzare una linea tra di essi.

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* È possibile utilizzare **Anteprima** nell’angolo in alto a destra per avere un’idea di come verranno visualizzati nel modulo i campi personalizzati e i widget.
>* I campi personalizzati e i widget potrebbero non essere sempre visualizzati allo stesso modo nel modulo, a seconda dello spazio disponibile sullo schermo quando viene visualizzato da un utente. Ad esempio, il terzo campo di una riga di campi può essere disposto alla riga successiva di campi se lo spazio orizzontale è limitato.


1. (Facoltativo)Per posizionare un campo personalizzato o un widget sopra o sotto un altro campo, trascinarlo sopra o sotto fino a visualizzare una linea blu orizzontale tra gli elementi.

1. Per salvare le modifiche, fai clic su **Applica**

   oppure

   Clic **Salva e chiudi**.

## Visualizzare in anteprima un modulo personalizzato

1. Inizia a creare o modificare un modulo personalizzato e ad aggiungere campi, come descritto in [Progettare un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Clic **Anteprima** nell’angolo in alto a sinistra per vedere come si presenterà il modulo quando verrà utilizzato, quindi fai clic su **Fine anteprima** per tornare alla modifica del modulo.