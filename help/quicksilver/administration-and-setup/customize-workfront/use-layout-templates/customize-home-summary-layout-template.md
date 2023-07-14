---
title: Personalizzare Home e Riepilogo utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Puoi utilizzare un modello di layout per configurare ciò che gli utenti visualizzano quando fanno clic su un’attività o un problema in Home e nel Riepilogo. Ogni configurazione effettuata utilizzando i passaggi riportati di seguito ha lo stesso effetto sull’area Home e sul pannello Riepilogo. Queste personalizzazioni non sono applicabili al pannello Riepilogo documento.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '993'
ht-degree: 2%

---

# Personalizzare Home e Riepilogo utilizzando un modello di layout

Puoi utilizzare un modello di layout per configurare ciò che gli utenti visualizzano quando fanno clic su un’attività o un problema in Home e nel Riepilogo. Ogni configurazione effettuata utilizzando i passaggi riportati di seguito ha lo stesso effetto sull’area Home e sul pannello Riepilogo. Queste personalizzazioni non sono applicabili al pannello Riepilogo documento.

Puoi configurare:

* Quali campi visualizzare per un’attività o un problema nell’area Dettagli e in quale ordine
* Indica se vengono visualizzati aggiornamenti, ora di accesso, documenti allegati e marche temporali per un’attività o un problema selezionato

È inoltre possibile personalizzare i campi visualizzati dagli utenti nell&#39;area Home quando gli utenti fanno clic sull&#39;approvazione di un progetto, di un documento o di una versione del documento ad essi assegnata.

Per informazioni sull&#39;area Home, vedere [Utilizzare l’area Home](../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md). Per informazioni sul pannello Riepilogo, consulta [Panoramica di riepilogo](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Per informazioni sulla creazione di modelli di layout, vedere [Creare e gestire modelli di layout](../use-layout-templates/create-and-manage-layout-templates.md).

Per informazioni sui modelli di layout per i gruppi, vedere [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Dopo aver configurato un modello di layout, è necessario assegnarlo agli utenti affinché le modifiche apportate siano visibili agli altri utenti. Per informazioni sull&#39;assegnazione di un modello di layout agli utenti, vedere [Assegnare utenti a un modello di layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.
Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizzare Home e Riepilogo utilizzando un modello di layout

1. Iniziare a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Fare clic sulla freccia giù ![](assets/dropdown-arrow.png) in **Personalizzare gli elementi visualizzati dagli utenti**, quindi fai clic su **Home e Riepilogo**.

1. Nell&#39;elenco visualizzato a sinistra, fare clic sul tipo di oggetto (**Attività**, **Problemi**, **Progetti**, **Documenti**, o **Versioni documento**) che desideri personalizzare in Home e Summary.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Attività</td> 
      <td> <p>In Home, la configurazione di questa impostazione influisce sull’area a destra di un’attività quando un utente fa clic su di essa. Inoltre, in un elenco di attività, influisce sul pannello Riepilogo visualizzato sul lato destro della pagina quando un utente seleziona un’attività, quindi fa clic sull’icona Apri riepilogo <img src="assets/summary-panel-icon.png">.</p> <p>Ad esempio, puoi determinare quali campi vengono visualizzati dagli utenti nell’area Dettagli quando selezionano le attività in Home:</p> <p><img src="assets/home-details-adobe branding.jpg"></p> <p>E quando selezionano un'attività nel Riepilogo:</p> <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Problemi</td> 
      <td> <p>In Home, la configurazione di questa impostazione influisce sull’area a destra di un problema quando un utente fa clic sul problema.</p> <p>In un elenco di problemi, questa impostazione influisce sul pannello Riepilogo visualizzato sul lato destro della pagina quando un utente seleziona un problema, quindi fa clic sull’icona Apri riepilogo <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progetti</td> 
      <td>In Home, quando un utente fa clic su un’approvazione del progetto ad esso assegnata, la configurazione di questa impostazione influisce sull’area a destra dell’approvazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenti</td> 
      <td>In Home, quando un utente fa clic su un’approvazione documento ad esso assegnata, la configurazione di questa impostazione influisce sull’area a destra dell’approvazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Versioni documento</td> 
      <td>In Home, quando un utente fa clic su un’approvazione ad esso assegnata per una particolare versione di un documento, la configurazione di questa impostazione influisce sull’area a destra dell’approvazione.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Se un’attività viene revocata, l’utente assegnato al modello di layout non visualizzerà le personalizzazioni dei campi nel Riepilogo.

1. (Condizionale) Se nel passaggio precedente hai fatto clic su Attività o Problemi, seleziona la categoria di attività o problema che desideri personalizzare.

   ![](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (Condizionale) Se **Imposta pulsante azione principale** viene visualizzato il menu a discesa (se si seleziona **Attività** o **Problemi** nell’elenco a sinistra), fai clic sull’azione principale (**Fine** o **Stato**) che desideri rendere disponibile agli utenti nell’area Home e nel pannello Riepilogo quando visualizzano un’attività o un problema.

   ![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. Aggiungi ![](assets/add-item-plus-in-circle-blue.png) o nascondi ![](assets/close-or-hide---x.png) campi per il tipo di oggetto selezionato.

   ![](assets/lt-home-add-hide-fields-adobe-branding.png)

1. Ripetere i passaggi 3-6 per personalizzare l&#39;area Home e il pannello Riepilogo per qualsiasi altro tipo di oggetto.
1. Clic **Impostazioni globali**, nell’angolo in basso a sinistra, quindi attiva o disattiva una delle seguenti opzioni relative agli oggetti di Adobe Workfront in Home e Summary:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Mostra aggiornamenti per il lavoro</td> 
      <td>Visualizza in Home o Riepilogo gli aggiornamenti apportati a un’attività o a un problema selezionato. Ciò include sia gli aggiornamenti di sistema che quelli effettuati da un utente. Gli utenti possono ancora filtrare gli aggiornamenti di sistema, come descritto in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">Attivare o disattivare gli aggiornamenti di sistema</a> in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Aggiorna lavoro</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tempo di connessione rispetto al lavoro</td> 
      <td>Visualizza l'opzione Registra tempo rispetto al lavoro quando si seleziona un'attività o un problema, consentendo agli utenti di registrare il tempo sugli elementi di lavoro direttamente dall'area Home e Riepilogo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizza documenti associati al lavoro</td> 
      <td>Visualizza un'area Documenti in Home e Riepilogo quando viene selezionata un'attività o un problema, elencando tutti i documenti allegati all'attività o al problema. Gli utenti possono fare clic sui documenti per visualizzarli in una finestra di anteprima.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nascondi data/ora</td> 
      <td>Nasconde i timestamp per i seguenti campi data in Home e Summary:
       <ul>
        <li>Data di completamento Pianificata</li>
        <li>Conferma data</li>
        <li><p>Data di invio</p></li>
       </ul><p><b>NOTA</b>: quando questa opzione è abilitata, gli elementi di lavoro scaduti vengono spostati nel raggruppamento In ritardo nella sezione Elenco lavori dell’area Home in base alla sola data e non all’ora.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continuate a personalizzare il modello di layout.

   Oppure

   Se hai finito di personalizzare, fai clic su **Salva**.

Per ulteriori informazioni sui modelli di layout, vedere [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
