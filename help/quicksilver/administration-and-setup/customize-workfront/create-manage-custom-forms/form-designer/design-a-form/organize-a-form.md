---
title: Organizzazione e visualizzazione in anteprima di un modulo con Form Designer
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile organizzare un modulo personalizzato con Progettazione moduli.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '1107'
ht-degree: 0%

---


# Organizzazione e visualizzazione in anteprima di un modulo con la struttura del modulo

È possibile organizzare un modulo personalizzato con la struttura del modulo.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>
   <p>Piano attuale: Standard</p>
   <p>oppure</p>
   <p>Piano legacy: Pianificare</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni su come gli amministratori di Workfront concedono questo accesso, consulta <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

## Aggiungi un’interruzione di sezione

È possibile raggruppare i campi e i widget personalizzati in un modulo personalizzato in sezioni con intestazioni. Questa funzione è utile per presentare un’esperienza organizzata agli utenti che compileranno il modulo. Inoltre, se devi limitare l’accesso a determinati campi e widget personalizzati a determinati utenti, puoi inserirli in una sezione e quindi concedere l’accesso alla sezione solo a tali utenti.

Ad esempio, se devi tenere traccia di informazioni sensibili che solo gli amministratori di sistema devono poter visualizzare o modificare, puoi creare un’interruzione di sezione con autorizzazioni di sola amministrazione e inserire i campi sensibili in quella sezione.

Le impostazioni di accesso selezionate per una sezione sono direttamente legate alle autorizzazioni di cui dispone l’utente sull’oggetto Workfront in cui è allegato il modulo personalizzato. È possibile nascondere o mostrare una sezione in base al fatto che l’utente abbia accesso a visualizzare, contribuire o gestire l’oggetto. Oppure puoi impostare una sezione su Solo amministratore in modo che solo gli utenti con un livello di accesso amministratore di sistema possano accedervi.

Per informazioni sulle autorizzazioni per gli oggetti, vedere [Panoramica della condivisione delle autorizzazioni sugli oggetti](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Per informazioni sui campi e i widget personalizzati nei moduli personalizzati, consultare [Progettazione di un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Creazione e configurazione dell’accesso per una sezione di un modulo personalizzato

1. Inizia a creare o modificare un modulo personalizzato e aggiungi campi, come descritto in [Progettazione di un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Fai clic su **Interruzione di sezione** e trascinarlo nella posizione desiderata sull&#39;area di lavoro.

1. Nel pannello di destra, configura le opzioni desiderate per la sezione:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Immetti un’etichetta descrittiva da visualizzare sopra la sezione . Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: Evita di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Digita del testo per spiegare agli utenti a cosa si riferisce la sezione. Viene visualizzato sotto l’etichetta della sezione nel modulo personalizzato.</td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Use display logic to specify whether the section should display on the form, based on selections users make in multi-choice custom fields when they fill out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> -->
     <tr> 
      <td role="rowheader"> <p>Concedi l’accesso</p> </td> 
      <td> <p> Per visualizzare questa sezione e modificarne i valori dei campi, selezionare le autorizzazioni necessarie agli utenti per un oggetto a cui è allegato il modulo personalizzato. 
       <p>Le seguenti autorizzazioni sono disponibili in <b>Gli utenti con questo accesso all’oggetto possono visualizzare i valori dei campi</b>:</p> 
         <ul>  
          <li><p><b>Modifica limitata</b>: (Disponibile solo se l’oggetto è un progetto, un’attività, un problema o un utente):</p> 
          <p>Consente agli utenti di contribuire all’oggetto se si tratta di un progetto, un’attività o un problema.</p>
          <p>Consente agli utenti di modificare il profilo o di possedere l’autorizzazione di profilo per l’oggetto, se si tratta di un utente.</p></li> 
          <li><b>Modifica</b>: Gestire le autorizzazioni per l’oggetto </li> 
          <li><b>Solo amministratore</b>: Livello di accesso amministratore di sistema</li> 
         </ul> </li> 
        <p>Le seguenti autorizzazioni sono disponibili in <b>Gli utenti con questo accesso all’oggetto possono modificare i valori dei campi</b>: </p> 
         <ul> 
          <li> <p><b>Modifica limitata</b>: (Disponibile solo se l’oggetto è un progetto, un’attività, un problema o un utente):</p> 
           <p>Se l’oggetto è un progetto, un’attività o un problema, questa autorizzazione consente agli utenti di contribuire all’oggetto</p>
          <p>Se l’oggetto è un utente, questa autorizzazione consente agli utenti di modificare il profilo o di disporre dell’autorizzazione di profilo per l’oggetto.</p> 
          <li><b>Modifica</b>: Gestire le autorizzazioni per l’oggetto </li> 
          <li><b>Solo amministratore</b>: Livello di accesso amministratore di sistema</li> 
         </ul> </li> 
       </ul> 
       <p>Per informazioni sulle autorizzazioni per gli oggetti, vedere <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Panoramica della condivisione delle autorizzazioni sugli oggetti</a>.</p> 
       <p><b>NOTA</b>:  
       <ul> 
       <li> <p>Gli utenti senza le autorizzazioni specificate in questo campo non possono visualizzare i campi e i widget personalizzati nella sezione . </p> <p>Questo vale anche se i valori dei campi vengono visualizzati nei rapporti o utilizzati nei campi calcolati nel reporting in modalità testo.</p> </li> 
       <li> <p>L’associazione di più tipi di oggetto al modulo può modificare le autorizzazioni di visualizzazione e modifica disponibili in questi passaggi. Per ulteriori informazioni, consulta <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Effetti di più tipi di oggetti sulle autorizzazioni di interruzione di sezione in un modulo personalizzato</a> in questo articolo.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Trascina o aggiungi almeno un campo o widget personalizzato alla nuova sezione. Questa operazione è necessaria prima di salvare la sezione.

1. Fai clic su **Fine**.

   >[!TIP]
   >
   >Puoi fare clic su **Applica** in qualsiasi momento durante la creazione di un modulo personalizzato per salvare le modifiche e mantenere il modulo aperto.

### Effetti di più tipi di oggetti sulle autorizzazioni delle interruzioni di sezione {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

L’autorizzazione Modifica limitata per le interruzioni di sezione del modulo personalizzato è disponibile solo per i tipi di oggetto Progetto, Attività, Problema e Utente.

In un modulo personalizzato con un’interruzione di sezione configurata con l’autorizzazione Modifica limitata, se si aggiunge al modulo uno degli altri tipi di oggetto (Portfolio, programma, documento, società, record di fatturazione, iterazione, spesa o gruppo), verrà richiesto di passare all’autorizzazione Modifica, compatibile sia con quel tipo di oggetto che con i tipi di oggetto esistenti nel modulo.

>[!INFO]
>
>**Esempio:** In un modulo personalizzato associato al tipo di oggetto Progetto, viene configurata un’interruzione di sezione con l’autorizzazione Modifica limitata.
>
>Aggiungere al modulo il tipo di oggetto Portfolio, il che significa che l’opzione di autorizzazione Modifica limitata non è più disponibile per l’interruzione di sezione nel modulo.
>
>Un messaggio sullo schermo richiede di passare all’autorizzazione Modifica, che è il livello minimo di autorizzazioni compatibili sia con il tipo di oggetto Progetto che con il tipo di oggetto Portfolio.


## Posizionare campi e widget personalizzati in un modulo personalizzato


1. Iniziare a creare o modificare un modulo personalizzato, come descritto in [Progettazione di un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Per posizionare campi e widget personalizzati sulla stessa riga, trascinateli uno accanto all’altro fino a quando non compare una linea tra di essi.

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* È possibile utilizzare **Anteprima** nell’angolo in alto a destra per ottenere un’idea di come verranno visualizzati nel modulo i campi e i widget personalizzati.
>* I campi e i widget personalizzati potrebbero non essere sempre visualizzati nello stesso modo nel modulo, a seconda dello spazio disponibile sullo schermo quando un utente li visualizza. Ad esempio, se lo spazio orizzontale è limitato, il terzo campo di una riga di campi può estendersi alla riga successiva.


1. (Facoltativo) Per posizionare un campo o un widget personalizzato sopra o sotto un altro, trascinalo sopra o sotto fino a visualizzare una linea blu orizzontale tra gli elementi.

1. Per salvare le modifiche, fai clic su **Applica**

   oppure

   Fai clic su **Salva e chiudi**.

## Anteprima di un modulo personalizzato

1. Inizia a creare o modificare un modulo personalizzato e aggiungi campi, come descritto in [Progettazione di un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Fai clic su **Anteprima** nell’angolo in alto a sinistra per visualizzare l’aspetto del modulo quando viene utilizzato, quindi fai clic su **Anteprima finale** per tornare alla modifica del modulo.