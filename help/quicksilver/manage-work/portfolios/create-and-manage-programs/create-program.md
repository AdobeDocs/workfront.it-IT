---
product-area: programs
navigation-topic: create and manage programs
title: Creare un programma
description: Un programma rappresenta una raccolta di progetti che condividono una strategia, un obiettivo o un obiettivo comune che trascende i limiti del progetto. I programmi sono una suddivisione dei portafogli e non possono esistere al di fuori di un portfolio. In genere, i programmi condividono le stesse risorse di altri programmi all’interno dello stesso portfolio. Puoi creare programmi per organizzare i portfolio quando diventano troppo grandi.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 6ec353c2-2241-47c2-8c59-1d8ddc43781e
source-git-commit: 594504c6a7acc9341471371ca279379042a45457
workflow-type: tm+mt
source-wordcount: '1288'
ht-degree: 0%

---

# Creare un programma

<!-- Audited: 1/2024 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Un programma rappresenta una raccolta di progetti che condividono una strategia, un obiettivo o un obiettivo comune che trascende i limiti del progetto.
I programmi sono una suddivisione dei portafogli e non possono esistere al di fuori di un portfolio. In genere, i programmi condividono le stesse risorse di altri programmi all’interno dello stesso portfolio.

Puoi creare programmi per organizzare i portfolio quando diventano troppo grandi.

Ad esempio, puoi avere un Portfolio Marketing Fiscal Year 2024 che contiene tutti i progetti della tua divisione Marketing. È consigliabile organizzare ulteriormente i progetti in trimestri fiscali e aggiungere programmi Marketing Fiscal Quarter 1-4 2024 all&#39;interno del Portfolio Marketing Fiscal Year 2024.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td>

<td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> <p>Nuovo: [!UICONTROL Standard] </p><p>Oppure </p><p>Corrente: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso a portafogli e programmi tramite [!UICONTROL Edit] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di [!UICONTROL Manage] per il portfolio</p> <p>Per impostazione predefinita, dopo aver creato un programma, si dispone di autorizzazioni [!UICONTROL Manage].</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modalità di creazione dei programmi

È possibile creare un programma in Workfront utilizzando uno dei metodi seguenti:

* Creare un programma partendo da zero dall&#39;area Programmi del menu principale o dalla sezione Programmi di un portfolio. Questo articolo descrive come creare un programma da zero.

* Importa un programma utilizzando i kick-start.

  In qualità di amministratore di Workfront, puoi importare programmi utilizzando una funzione di avvio.

  Per informazioni sull&#39;importazione di dati tramite Kick-Start in Workfront, vedere [Importare dati in Adobe Workfront utilizzando un modello Kick-Start](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).


* Aggiungere i programmi quando vengono collegati da un tipo di record in Workfront Planning.

  È necessario disporre di un pacchetto Workfront Planning aggiuntivo.

  Per informazioni sull&#39;accesso a Workfront Planning, vedere [Panoramica dell&#39;accesso ad Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

  Per informazioni sulla creazione di portafogli tramite l&#39;aggiunta di tali portafogli ai record, vedere la sezione &quot;Creare record durante la connessione&quot; nell&#39;articolo [Creare record](/help/quicksilver/planning/records/create-records.md).

## Creare un programma

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro.

1. Effettuare una delle seguenti operazioni.

   * Crea un programma dall&#39;area [!UICONTROL Programmi]:

      1. Fare clic su **[!UICONTROL Programmi]** nel menu principale.
      1. Fai clic su **[!UICONTROL Nuovo programma]**.
      1. Nella casella visualizzata digitare il nome di un Portfolio esistente nel campo **[!UICONTROL Seleziona Portfolio]**.
      1. Digitare il nome del nuovo programma nel campo **[!UICONTROL Nome]**.
      1. Fai clic su **[!UICONTROL Salva]**.
   * Crea un programma dall&#39;area [!UICONTROL Portfolio]:

      1. Fai clic su **[!UICONTROL Portfolio]** nel [!UICONTROL Menu principale], quindi apri un portfolio.
      1. Nel pannello a sinistra, fai clic su **[!UICONTROL Programmi]**.
      1. Fai clic sul menu a discesa **[!UICONTROL Nuovo programma]**, quindi su **[!UICONTROL Nuovo programma]**.


1. (Condizionale) Se il programma è stato creato da un portfolio, specificare il nome del programma nel campo **[!UICONTROL Programma senza titolo]**.

   Il nome può contenere fino a 255 caratteri.

1. (Facoltativo) Fai clic su **[!UICONTROL Responsabile del programma]** nell&#39;intestazione del programma per aggiornarla.

   >[!TIP]
   >
   >In qualità di creatore del programma, per impostazione predefinita viene impostato come responsabile del programma.

1. Fai clic su **[!UICONTROL Dettagli programma]** nel pannello a sinistra.
1. Fare doppio clic su un campo per aggiornare le informazioni nell&#39;area **[!UICONTROL Panoramica]**.

È possibile specificare le seguenti informazioni:

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Campo</th> 
      <th>Descrizione</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td> <p>Specificare una descrizione per il programma.</p> <p>La descrizione viene visualizzata nella pagina di destinazione del programma.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Program Manager]</td> 
      <td> <p>Iniziare a digitare il nome dell'utente che si desidera utilizzare come responsabile del programma, quindi fare clic sul nome dell'utente quando viene visualizzato nell'elenco a discesa. È lo stesso del [!UICONTROL Proprietario del programma]. </p> <p>Suggerimento: puoi anche aggiornare il Responsabile del programma nell’intestazione del programma. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Group] </td> 
      <td> <p>Aggiungere il nome di un singolo gruppo se il gruppo è proprietario del programma o se ne è responsabile. </p> <p>Per assicurarsi di selezionare il gruppo corretto, posizionare il puntatore del mouse su di esso e fare clic sull'icona [!UICONTROL information] <img src="assets/info-icon.png"> visualizzata accanto ad esso. In questo modo viene visualizzata una descrizione del gruppo contenente informazioni sul gruppo stesso, ad esempio la gerarchia dei gruppi al di sopra del gruppo e i relativi amministratori.</p> 
       <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
        <img src="assets/group-details-widget-programs-350x268.png" style="width: 350;height: 268;"> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo e condizionale) Fai clic nella casella **[!UICONTROL Aggiungi modulo personalizzato]** per selezionare un modulo personalizzato per il portfolio e aggiornare i campi personalizzati.

   >[!TIP]
   >
   >Prima di allegare i moduli personalizzati ai programmi, è necessario che siano già stati creati.

1. (Facoltativo e condizionale) Se si aggiunge un modulo personalizzato, fare clic su un campo del modulo personalizzato per aggiornare le informazioni contenute in tale campo.
1. Fai clic su **[!UICONTROL Salva modifiche]**.
1. Fai clic su **[!UICONTROL Progetti]** nel pannello a sinistra, quindi su **[!UICONTROL Aggiungi progetti]** per aggiungere progetti al programma.

   Per informazioni sull&#39;aggiunta di progetti ai programmi, vedere [Aggiungere un progetto a un programma](../../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

1. Fai clic su **[!UICONTROL Salva modifiche]**.
1. (Facoltativo) Fai clic sul **[!UICONTROL Altro menu]** ![Altro menu](assets/more-icon.png) accanto al nome del programma e fai clic su **[!UICONTROL Disattiva programma]**.

   Quando si disattiva un programma, il programma non viene più visualizzato in un elenco di programmi quando gli utenti tentano di aggiungerlo a un progetto. Puoi comunque accedere al programma dall&#39;area [!UICONTROL Programmi].

## Panoramica dell’intestazione del programma

Puoi trovare alcune informazioni sul programma nella sua intestazione.

Le seguenti informazioni vengono visualizzate nell’intestazione di un programma:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Informazioni intestazione</td> 
   <td> <strong>Note</strong> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Breadcrumb con il nome del portfolio</td> 
   <td>Puoi accedere al portfolio a cui appartiene il programma dall’intestazione del programma. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del programma</td> 
   <td>Puoi modificare il nome del programma nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto e stato di attivazione</td> 
   <td>La parola "Programma" viene visualizzata con un'icona arancione quando si visualizza un programma. Accanto alla parola "[!UICONTROL Disattivato]" viene visualizzata la struttura grigia se il programma non è contrassegnato come [!UICONTROL Attivo]. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Il settore d'azione del programma </td> 
   <td> <p>Fare clic su una delle opzioni seguenti per accedere a ulteriori informazioni o opzioni di modifica per il programma:</p> 
    <ul> 
     <li>Icona a forma di stella per aggiungere il programma all'elenco dei preferiti</li> 
     <li> <p>Il menu [!UICONTROL Altro] <img src="assets/qs-more-menu.png"> consente di eseguire una delle operazioni seguenti: </p> 
      <ul> 
       <li>Modifica il programma</li> 
       <li>Disattivala. Quando un programma viene disattivato, non è più possibile associarlo ai progetti a livello di progetto. </li> 
       <li> <p>Eliminalo. L’eliminazione del programma non comporta l’eliminazione dei progetti al suo interno. Elimina l'associazione dei progetti al programma. </p> </li> 
       <li>Condividi con altri</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percent Complete]</td> 
   <td> <p>Impossibile modificare il [!UICONTROL Percent Complete] del programma nell'intestazione. Queste informazioni vengono aggiornate dai progetti nel programma. Per impostazione predefinita, la percentuale di completamento del programma corrisponde alla media dei valori della percentuale di completamento dei progetti in uno stato [!UICONTROL Current] o [!UICONTROL Approved] che appartengono al programma.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Manager]</td> 
   <td> <p>Puoi modificare il Responsabile del programma nell’intestazione. È lo stesso del [!UICONTROL Proprietario del programma]. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di completamento Pianificata]</td> 
   <td>Non puoi modificare la Data di completamento pianificata del programma nell’intestazione. Queste informazioni vengono aggiornate dai progetti nel programma. La data di completamento pianificata dell'ultimo progetto del programma diventa la data di completamento pianificata del programma.  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Condizione progetti attivi </td> 
   <td>Questo è un calcolo della percentuale di progetti nel programma per cui la condizione  è impostata come [!UICONTROL On Target], [!UICONTROL At Risk] o [!UICONTROL In Trouble]. I progetti qui rappresentati sono progetti con uno stato di [!UICONTROL Current] e [!UICONTROL Approved]. </td> 
  </tr> 
 </tbody> 
</table>

## Spostare un programma

È possibile aggiungere programmi esistenti a un portfolio. Poiché i programmi non possono esistere in due portafogli diversi, l&#39;aggiunta di un programma esistente comporta lo spostamento permanente da un portfolio all&#39;altro.

Per ulteriori informazioni, vedere [Aggiungere un programma esistente a un portfolio](../../../manage-work/portfolios/create-and-manage-programs/move-program.md).
