---
title: Personalizzare il pannello di riepilogo utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Puoi utilizzare un modello di layout per configurare ciò che gli utenti visualizzano quando fanno clic su un’attività o un problema nel Riepilogo. Ogni configurazione effettuata seguendo la procedura riportata di seguito ha effetto sul pannello Riepilogo. Queste personalizzazioni non sono applicabili al pannello Riepilogo documento.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: 76e32fa6b87583d2b8c296045da731afdb6d1f9a
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 2%

---

# Personalizzare il pannello Riepilogo utilizzando un modello di layout

<!--Audited: 11/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>   -->


Puoi utilizzare un modello di layout per configurare ciò che gli utenti visualizzano nel pannello Riepilogo quando fanno clic su un’attività o su un problema. Ogni configurazione effettuata seguendo la procedura riportata di seguito ha effetto sul pannello Riepilogo. Queste personalizzazioni non sono applicabili al pannello Riepilogo documento.

Puoi configurare:

* Quali campi visualizzare per un’attività o un problema nell’area Dettagli e in quale ordine
* Indica se vengono visualizzati aggiornamenti, ora di accesso, documenti allegati e marche temporali per un’attività o un problema selezionato

È inoltre possibile personalizzare i campi visualizzati dagli utenti nell&#39;area Home quando gli utenti fanno clic sull&#39;approvazione di un progetto, di un documento o di una versione del documento ad essi assegnata.

Per informazioni sul pannello Riepilogo, vedere [Panoramica di riepilogo](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Per informazioni sulla creazione di modelli di layout, vedere [Creare e gestire modelli di layout](../use-layout-templates/create-and-manage-layout-templates.md).

Per informazioni sui modelli di layout per i gruppi, vedere [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Dopo aver configurato un modello di layout, è necessario assegnarlo agli utenti affinché le modifiche apportate siano visibili agli altri utenti. Per informazioni sull&#39;assegnazione di un modello di layout agli utenti, vedere [Assegnare gli utenti a un modello di layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.</p>
        <p>Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizzare il pannello Riepilogo utilizzando un modello di layout

1. Iniziare a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Fai clic sulla freccia giù ![freccia giù](assets/dropdown-arrow.png) in **Personalizza gli elementi visualizzati dagli utenti**, quindi fai clic su **Riepilogo**.

1. Nell&#39;elenco visualizzato sotto, fate clic sul tipo di oggetto per il quale desiderate personalizzare il pannello Riepilogo.

   La tabella seguente spiega cosa è possibile personalizzare per ciascun oggetto

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Attività</td> 
      <td> <p>In un elenco di attività, questa impostazione influisce sul pannello Riepilogo visualizzato sul lato destro della pagina quando un utente seleziona un'attività e poi fa clic sull'icona Apri riepilogo <img src="assets/summary-panel-icon.png">.</p>

   <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Problemi</td> 
      <td><p>In un elenco di problemi, questa impostazione influisce sul pannello Riepilogo visualizzato sul lato destro della pagina quando un utente seleziona un problema, quindi fa clic sull'icona Apri riepilogo <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
    </tbody> 
   </table>

<!--These were removed with the new Home: 

<tr> 
      <td role="rowheader">Projects</td> 
      <td><ul><li><p>In Home, when a user clicks a project approval assigned to them, your configuration for this setting affects the area to the right of the approval.</p>
      <p><b>IMPORTANT:</b> </p><p>This is a deprecated feature. Any changes you make to this area are related to a feature that Workfront has removed. This option will be removed from Workfront with a later maintenance update.</p></li>
      </ul> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td>
     <ul><li><p>In Home, when a user clicks a document approval assigned to them, your configuration for this setting affects the area to the right of the approval.</p>
      <p><b>IMPORTANT:</b> </p><p> This is a deprecated feature. Any changes you make to this area are related to a feature that Workfront has removed. This option will be removed from Workfront with a later maintenance update.</p></li>
      </ul>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Document Versions</td> 
      <td><ul><li><p>In Home, when a user clicks an approval assigned to them for a particular version of a document, your configuration for this setting affects the area to the right of the approval.</p>
      <p><p><b>IMPORTANT:</b></p> This is a deprecated feature. Any changes you make to this area are related to a feature that Workfront has removed. This option will be removed from Workfront with a later maintenance update.</p></li>
      </ul>
      </td> 
     </tr> -->


>[!IMPORTANT]
>
>Se un’attività viene revocata, l’utente assegnato al modello di layout non visualizzerà le personalizzazioni dei campi nel Riepilogo.

1. (Condizionale) Se nel passaggio precedente hai fatto clic su Attività o Problemi, seleziona la categoria di attività o problema che desideri personalizzare.

   ![Scegli la categoria da personalizzare](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (Condizionale) Se viene visualizzato il menu a discesa **Imposta pulsante azione principale** (se si seleziona **Attività** o **Problemi** nell&#39;elenco a sinistra), fare clic sull&#39;azione principale (**Fine** o **Stato**) che si desidera rendere disponibile agli utenti nel pannello Riepilogo quando visualizzano un&#39;attività o un problema.

   ![Imposta azione primaria](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. Aggiungi ![Aggiungi elemento](assets/add-item-plus-in-circle-blue.png) o nascondi ![Nascondi campi elemento](assets/close-or-hide---x.png) per il tipo di oggetto selezionato.

   ![Aggiungi e nascondi campi](assets/lt-home-add-hide-fields-adobe-branding.png)

1. Ripetete i passaggi 3-6 per personalizzare il pannello Riepilogo per qualsiasi altro tipo di oggetto.
1. Fai clic su **Impostazioni globali**, nell&#39;angolo inferiore sinistro, quindi attiva o disattiva le seguenti opzioni relative agli oggetti Adobe Workfront nel Riepilogo:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Mostra aggiornamenti per il lavoro</td> 
      <td>Visualizza nel pannello Riepilogo tutti gli aggiornamenti apportati a un’attività o a un problema selezionato. Ciò include sia gli aggiornamenti di sistema che quelli effettuati da un utente. Gli utenti possono ancora filtrare gli aggiornamenti di sistema, come descritto in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">Abilitare o disabilitare gli aggiornamenti di sistema</a> in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Aggiorna lavoro</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Registra ore per lavoro</td> 
      <td>Visualizza l'opzione Registra tempo rispetto al lavoro quando si seleziona un'attività o un problema, consentendo agli utenti di registrare il tempo sugli elementi di lavoro direttamente dall'area Home e Riepilogo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizza documenti associati al lavoro</td> 
      <td>Visualizza un'area Documenti nel pannello Riepilogo quando viene selezionata un'attività o un problema, in cui sono elencati tutti i documenti allegati all'attività o al problema. Gli utenti possono fare clic sui documenti per visualizzarli in una finestra di anteprima.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nascondi data/ora</td> 
      <td>Nasconde i timestamp per i seguenti campi di data nel pannello Riepilogo:
       <ul>
        <li>Data di completamento Pianificata</li>
        <li>Conferma data</li>
        <li>Data di invio</li>
       </ul></td> 
     </tr> 
    </tbody> 
   </table>

1. Continuate a personalizzare il modello di layout.

   Oppure

   Se hai completato la personalizzazione, fai clic su **Salva**.

Per ulteriori informazioni sui modelli di layout, vedere [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
