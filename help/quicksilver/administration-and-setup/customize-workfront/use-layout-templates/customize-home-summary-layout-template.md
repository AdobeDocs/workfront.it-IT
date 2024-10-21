---
title: Personalizzare il pannello di riepilogo utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Puoi utilizzare un modello di layout per configurare ciò che gli utenti visualizzano quando fanno clic su un’attività o un problema nel Riepilogo. Ogni configurazione effettuata seguendo la procedura riportata di seguito ha effetto sul pannello Riepilogo. Queste personalizzazioni non sono applicabili al pannello Riepilogo documento.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: 43cf88c533b80324266f0660648c6a1ab13ca8fc
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 2%

---

# Personalizzare il pannello Riepilogo utilizzando un modello di layout


Puoi utilizzare un modello di layout per configurare ciò che gli utenti visualizzano quando fanno clic su un’attività o un problema nel Riepilogo. Ogni configurazione effettuata seguendo la procedura riportata di seguito ha effetto sul pannello Riepilogo. Queste personalizzazioni non sono applicabili al pannello Riepilogo documento.

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
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td><p>Nuovo: Standard</p>
  <p> Corrente: Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.
Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizzare il pannello Riepilogo utilizzando un modello di layout

1. Iniziare a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Fare clic sulla freccia giù ![](assets/dropdown-arrow.png) in **Personalizza gli elementi visualizzati dagli utenti**, quindi fare clic su **Riepilogo**.

1. Nell&#39;elenco a sinistra fare clic sul tipo di oggetto (**Attività**, **Problemi**, **Progetti**, **Documenti** o **Versioni documento**) che si desidera personalizzare nel pannello Riepilogo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Attività</td> 
      <td><p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Problemi</td> 
      <td><p>In un elenco di problemi, questa impostazione influisce sul pannello Riepilogo visualizzato sul lato destro della pagina quando un utente seleziona un problema, quindi fa clic sull'icona Apri riepilogo <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progetti</td> 
      <td><p>In Home, quando un utente fa clic su un’approvazione del progetto ad esso assegnata, la configurazione di questa impostazione influisce sull’area a destra dell’approvazione.</p>
      <p>IMPORTANTE: questa è una funzione obsoleta. Qualsiasi modifica apportata a questa area è relativa a una funzione rimossa da Workfront. Questa opzione verrà rimossa da Workfront con un successivo aggiornamento di manutenzione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenti</td> 
      <td><p>In Home, quando un utente fa clic su un’approvazione documento ad esso assegnata, la configurazione di questa impostazione influisce sull’area a destra dell’approvazione.</p>
      <p>IMPORTANTE: questa è una funzione obsoleta. Qualsiasi modifica apportata a questa area è relativa a una funzione rimossa da Workfront. Questa opzione verrà rimossa da Workfront con un successivo aggiornamento di manutenzione.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Versioni documento</td> 
      <td><p>In Home, quando un utente fa clic su un’approvazione ad esso assegnata per una particolare versione di un documento, la configurazione di questa impostazione influisce sull’area a destra dell’approvazione.</p>
      <p>IMPORTANTE: questa è una funzione obsoleta. Qualsiasi modifica apportata a questa area è relativa a una funzione rimossa da Workfront. Questa opzione verrà rimossa da Workfront con un successivo aggiornamento di manutenzione.</p>
      </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Se un’attività viene revocata, l’utente assegnato al modello di layout non visualizzerà le personalizzazioni dei campi nel Riepilogo.

1. (Condizionale) Se nel passaggio precedente hai fatto clic su Attività o Problemi, seleziona la categoria di attività o problema che desideri personalizzare.

   ![](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (Condizionale) Se viene visualizzato il menu a discesa **Imposta pulsante azione principale** (se si seleziona **Attività** o **Problemi** nell&#39;elenco a sinistra), fare clic sull&#39;azione principale (**Fine** o **Stato**) che si desidera rendere disponibile agli utenti nel pannello Riepilogo quando visualizzano un&#39;attività o un problema.

   ![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. Aggiungi ![](assets/add-item-plus-in-circle-blue.png) o nascondi ![](assets/close-or-hide---x.png) campi per il tipo di oggetto selezionato.

   ![](assets/lt-home-add-hide-fields-adobe-branding.png)

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
      <td role="rowheader">Tempo di connessione rispetto al lavoro</td> 
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
