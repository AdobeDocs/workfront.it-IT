---
title: Organizzare e visualizzare in anteprima un modulo
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile organizzare un modulo personalizzato con il Designer modulo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 08de894a-82f0-4440-a350-680d6648f01e
source-git-commit: 8d9a9d8356f195d1e1fcbf0ae6c9b08f20ba4bbf
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 0%

---

# Organizzare un modulo e visualizzarne l’anteprima

È possibile organizzare un modulo personalizzato con il progettista del modulo e visualizzarlo in anteprima per verificarne la corretta configurazione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>piano Adobe Workfront</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Nuovo: Standard</p>
   <p>oppure</p>
   <p>Corrente: Piano</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungere un’interruzione di sezione

È possibile raggruppare i campi personalizzati e i widget in un modulo personalizzato in sezioni con intestazioni. Ciò è utile per presentare un’esperienza organizzata agli utenti che compileranno il modulo. Inoltre, se devi limitare l’accesso a determinati campi personalizzati e widget a determinati utenti, puoi inserirli in una sezione e quindi concedere l’accesso alla sezione solo a tali utenti.

Ad esempio, se devi tenere traccia delle informazioni riservate che solo gli amministratori di sistema possono visualizzare o modificare, puoi creare un’interruzione di sezione con le autorizzazioni Solo amministratore e inserire i campi sensibili in tale sezione.

Le impostazioni di accesso selezionate per una sezione sono direttamente correlate alle autorizzazioni di cui dispongono gli utenti sull’oggetto Workfront a cui è allegato il modulo personalizzato. È possibile nascondere o visualizzare una sezione a seconda che l&#39;utente disponga dell&#39;accesso per visualizzare, contribuire o gestire l&#39;oggetto. In alternativa, è possibile impostare una sezione su Solo amministratore in modo che solo gli utenti con un livello di accesso amministratore di sistema possano accedervi.

Per informazioni sulle autorizzazioni per gli oggetti, vedere [Panoramica sulle autorizzazioni di condivisione per gli oggetti](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Per informazioni sui campi personalizzati e i widget nei moduli personalizzati, vedere [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Creare e configurare l’accesso per una sezione in un modulo personalizzato

1. Inizia a creare o modificare un modulo personalizzato e ad aggiungere campi, come descritto in [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Fare clic su **Interruzione di sezione** e trascinarla nella posizione desiderata nell&#39;area di lavoro.

1. Nel pannello a destra, configura le opzioni desiderate per la sezione:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra la sezione. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: evitare di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Digita del testo per spiegare agli utenti a cosa serve la sezione. Questo viene visualizzato sotto l’etichetta della sezione nel modulo personalizzato.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Concedi l’accesso</p> </td> 
      <td> <p> Per visualizzare questa sezione e modificare i valori dei campi, seleziona le autorizzazioni necessarie per un oggetto a cui è allegato il modulo personalizzato. 
       <p>Le seguenti autorizzazioni sono disponibili in <b>Gli utenti con questo accesso all'oggetto possono visualizzare i valori dei campi</b>:</p> 
         <ul>
          <li><strong>Visualizza</strong>: visualizza le autorizzazioni per l'oggetto</li>
          <li><p><b>Modifica limitata</b>: (disponibile solo se l'oggetto è un progetto, attività, problema o utente):</p> 
          <p>Consente agli utenti di contribuire all'oggetto se si tratta di un progetto, attività o problema.</p>
          <p>Consente agli utenti di modificare il profilo o di disporre dell'autorizzazione di profilo per l'oggetto, se si tratta di un utente.</p></li> 
          <li><b>Modifica</b>: gestisci le autorizzazioni per l'oggetto </li> 
          <li><b>Solo amministratore</b>: livello di accesso Amministratore di sistema</li> 
         </ul> </li> 
        <p>Le seguenti autorizzazioni sono disponibili in <b>Gli utenti con questo accesso all'oggetto possono modificare i valori dei campi</b>: </p> 
         <ul> 
          <li> <p><b>Modifica limitata</b>: (disponibile solo se l'oggetto è un progetto, attività, problema o utente):</p> 
           <p>Se l'oggetto rappresenta un progetto, un'attività o un problema, questa autorizzazione consente agli utenti di contribuire all'oggetto</p>
          <p>Se l’oggetto è un utente, questa autorizzazione consente agli utenti di modificare il profilo o di essere proprietari dell’autorizzazione di profilo per l’oggetto.</p> 
          <li><b>Modifica</b>: gestisci le autorizzazioni per l'oggetto </li> 
          <li><b>Solo amministratore</b>: livello di accesso Amministratore di sistema</li> 
         </ul> </li> 
       </ul> 
       <p>Per informazioni sulle autorizzazioni per gli oggetti, vedere <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Panoramica sulle autorizzazioni di condivisione per gli oggetti</a>.</p> 
       <p><b>NOTA</b>:  
       <ul> 
       <li> <p>Gli utenti senza le autorizzazioni specificate qui non possono visualizzare i campi personalizzati e i widget nella sezione. </p> <p>Questo vale anche se visualizzi i valori dei campi nei rapporti o li utilizzi nei campi calcolati nella generazione rapporti in modalità testo.</p> </li> 
       <li><p>Per i moduli personalizzati per richieste/problemi: se è necessario l’accesso di visualizzazione per visualizzare i campi nell’interruzione di sezione, ma è necessario l’accesso di amministratore per modificare i campi, la sezione e tutti i relativi campi non saranno visibili agli utenti non amministratori durante la compilazione del modulo. Una volta creata la richiesta, gli utenti con accesso di visualizzazione possono visualizzare i campi nella sezione.</p></li>
       <li> <p>L'associazione di più tipi di oggetto al modulo può modificare le autorizzazioni di visualizzazione e modifica disponibili in questi passaggi. Per ulteriori informazioni, vedere <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Come più tipi di oggetto possono influire sulle autorizzazioni di interruzione di sezione in un modulo personalizzato</a> in questo articolo.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Aggiungi logica</p></td> 
      <td><p>Utilizza la logica di visualizzazione per specificare se la sezione deve essere visualizzata nel modulo, in base alle selezioni effettuate dagli utenti nei campi personalizzati a scelta multipla durante la compilazione del modulo.</p><p><strong>NOTA:</strong> se a tutti i singoli campi di un'interruzione di sezione viene applicata la logica di visualizzazione e tutti i campi sono nascosti come risultato della logica, l'intera sezione verrà nascosta nel modulo personalizzato. Ciò si verifica anche se la logica di visualizzazione non viene applicata all’interruzione di sezione.</p><p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md" class="MCXref xref">Aggiungere logica di visualizzazione e logica di salto con la finestra di progettazione del modulo</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Trascina o aggiungi almeno un campo personalizzato o un widget nella nuova sezione. Questa operazione è necessaria prima di salvare la sezione.

1. Fai clic su **Fine**.

   >[!TIP]
   >
   >Puoi fare clic su **Applica** in qualsiasi momento durante la creazione di un modulo personalizzato per salvare le modifiche e mantenere aperto il modulo.

### Come più tipi di oggetto possono influire sulle autorizzazioni dell’interruzione di sezione {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

L’autorizzazione Modifica limitata per le interruzioni di sezione del modulo personalizzato è disponibile solo per i tipi di oggetto Progetto, Attività, Problema e Utente.

In un modulo personalizzato con un&#39;interruzione di sezione configurata con l&#39;autorizzazione Modifica limitata, se si aggiunge uno degli altri tipi di oggetto al modulo (Portfolio, Programma, Documento, Società, Fatturazione, Iterazione, Spesa o Gruppo), verrà richiesto di passare all&#39;autorizzazione Modifica, che è compatibile sia con il tipo di oggetto sia con i tipi di oggetto esistenti nel modulo.

>[!INFO]
>
>**Esempio:** In un modulo personalizzato associato al tipo di oggetto Progetto, viene configurata un&#39;interruzione di sezione con l&#39;autorizzazione Modifica limitata.
>
>Aggiungendo al modulo il tipo di oggetto Portfolio, l&#39;opzione di autorizzazione Modifica limitata non sarà più disponibile per l&#39;interruzione di sezione nel modulo.
>
>In un messaggio sullo schermo viene richiesto di passare all&#39;autorizzazione Modifica, che è il livello di autorizzazioni minimo compatibile sia con il tipo di oggetto Progetto che con il tipo di oggetto Portfolio.


## Posizionare campi e widget personalizzati in un modulo personalizzato


1. Iniziare a creare o modificare un modulo personalizzato, come descritto in [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Per posizionare campi personalizzati e widget sulla stessa riga, trascinare uno accanto all&#39;altro fino a visualizzare una linea tra di essi.

   >[!NOTE]
   >
   >* Puoi usare il pulsante **Anteprima** nell&#39;angolo superiore destro per avere un&#39;idea di come verranno visualizzati i campi personalizzati e i widget nel modulo.
   >* I campi personalizzati e i widget potrebbero non essere sempre visualizzati allo stesso modo nel modulo, a seconda dello spazio disponibile sullo schermo quando viene visualizzato da un utente. Ad esempio, il terzo campo di una riga di campi può essere disposto alla riga successiva di campi se lo spazio orizzontale è limitato.

1. (Facoltativo)Per posizionare un campo personalizzato o un widget sopra o sotto un altro campo, trascinarlo sopra o sotto fino a visualizzare una linea blu orizzontale tra gli elementi.

1. Per salvare le modifiche, fai clic su **Applica**

   oppure

   Fare clic su **Salva e chiudi**.

## Visualizzare in anteprima un modulo personalizzato

1. Inizia a creare o modificare un modulo personalizzato e ad aggiungere campi, come descritto in [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Fai clic su **Anteprima** nell&#39;angolo in alto a destra per vedere come si presenterà il modulo durante l&#39;utilizzo, quindi fai clic su **Fine anteprima** per tornare alla modifica del modulo.

