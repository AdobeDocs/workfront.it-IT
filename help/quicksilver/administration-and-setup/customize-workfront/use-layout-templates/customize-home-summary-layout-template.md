---
title: Personalizzare Home e Riepilogo utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: È possibile utilizzare un modello di layout per configurare ciò che gli utenti visualizzano quando fanno clic su un’attività o su un problema nella home page e nel riepilogo. Ogni configurazione effettuata utilizzando i passaggi seguenti influisce sull'area Home e sul pannello Riepilogo nello stesso modo. Queste personalizzazioni non si applicano al pannello Riepilogo documento.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 2%

---

# Personalizzare Home e Riepilogo utilizzando un modello di layout

È possibile utilizzare un modello di layout per configurare ciò che gli utenti visualizzano quando fanno clic su un’attività o su un problema nella home page e nel riepilogo. Ogni configurazione effettuata utilizzando i passaggi seguenti influisce sull&#39;area Home e sul pannello Riepilogo nello stesso modo. Queste personalizzazioni non si applicano al pannello Riepilogo documento.

Puoi configurare i seguenti parametri:

* Quali campi vengono visualizzati per un&#39;attività o un problema nell&#39;area Dettagli e in quale ordine
* Aggiornamenti, tempo di registrazione, documenti allegati e timestamp visualizzati per un&#39;attività o un problema selezionato

È inoltre possibile personalizzare i campi visualizzati nell&#39;area Home quando gli utenti fanno clic su un&#39;approvazione del progetto, un&#39;approvazione del documento o un&#39;approvazione della versione del documento assegnata loro.

Per informazioni sull&#39;area Home, vedere [Utilizzare l&#39;area Home](../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md). Per informazioni sul pannello Riepilogo, consulta [Panoramica di riepilogo](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Per informazioni sui modelli di layout per gruppi, consulta [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.
Per eseguirle per un gruppo, devi essere un responsabile di quel gruppo.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizzare Home e Riepilogo utilizzando un modello di layout

1. Inizia a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Fai clic sulla freccia giù ![](assets/dropdown-arrow.png) sotto **Personalizzare ciò che gli utenti visualizzano**, quindi fai clic su **Home e Riepilogo**.

1. Nell’elenco a sinistra, fai clic sul tipo di oggetto (**Attività**, **Problemi**, **Progetti**, **Documenti** oppure **Versioni dei documenti**) che si desidera personalizzare in Home e Riepilogo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Attività</td> 
      <td> <p>In Home, la configurazione di questa impostazione influisce sull'area a destra di un'attività quando un utente fa clic sull'attività. Inoltre, in un elenco di attività, influisce sul pannello Riepilogo visualizzato sul lato destro della pagina quando un utente seleziona un’attività, quindi fa clic sull’icona Apri riepilogo . <img src="assets/summary-panel-icon.png">.</p> <p>Ad esempio, è possibile determinare quali campi vengono visualizzati dagli utenti nell'area Dettagli quando gli utenti selezionano le attività in Home:</p> <p><img src="assets/home-details-adobe branding.jpg"></p> <p>E quando selezionano un'attività nel Riepilogo:</p> <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Problemi</td> 
      <td> <p>In Home, la configurazione di questa impostazione influisce sull'area a destra di un problema quando un utente fa clic sul problema.</p> <p>In un elenco di problemi, questa impostazione ha effetto sul pannello Riepilogo visualizzato sul lato destro della pagina quando un utente seleziona un problema, quindi fa clic sull'icona Apri riepilogo . <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progetti</td> 
      <td>In Home, quando un utente fa clic su un'approvazione di progetto assegnata a un utente, la configurazione di questa impostazione influisce sull'area a destra dell'approvazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenti</td> 
      <td>In Home, quando un utente fa clic su un'approvazione del documento assegnata a un utente, la configurazione di questa impostazione influisce sull'area a destra dell'approvazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Versioni documento</td> 
      <td>In Home, quando un utente fa clic su un'approvazione assegnata a una particolare versione di un documento, la configurazione di questa impostazione influisce sull'area a destra dell'approvazione.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Se un&#39;attività non viene assegnata, l&#39;utente assegnato al modello di layout non vedrà le personalizzazioni dei campi nel Riepilogo.

1. (Condizionale) Se si fa clic su Attività o Problemi nel passaggio precedente, selezionare la categoria di attività o problema che si desidera personalizzare.

   ![](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (Condizionale) Se il valore **Pulsante Imposta azione primaria** viene visualizzato il menu a discesa (se si seleziona **Attività** o **Problemi** nell’elenco a sinistra), fai clic sull’azione principale (**Fine** o **Stato**) che desideri rendere disponibile agli utenti nell’area Home e nel pannello Riepilogo quando visualizzano un’attività o un problema.

   ![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. Aggiungi ![](assets/add-item-plus-in-circle-blue.png) o nascondere ![](assets/close-or-hide---x.png) campi per il tipo di oggetto selezionato.

   ![](assets/lt-home-add-hide-fields-adobe-branding.png)

1. Ripetere i passaggi 3-6 per personalizzare l’area principale e il pannello Riepilogo per qualsiasi altro tipo di oggetto.
1. Fai clic su **Impostazioni globali**, nell’angolo in basso a sinistra, quindi attiva o disattiva una delle seguenti opzioni relative agli oggetti Adobe Workfront in Home and Summary :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Mostra aggiornamenti per il lavoro</td> 
      <td>Visualizza eventuali aggiornamenti apportati a un'attività o a un problema selezionato in Home o Riepilogo. Ciò include sia gli aggiornamenti di sistema che quelli effettuati da un utente. Gli utenti possono comunque filtrare gli aggiornamenti di sistema, come descritto in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">Attiva o disattiva gli aggiornamenti del sistema</a> in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Aggiorna lavoro</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tempo di connessione rispetto al lavoro</td> 
      <td>Visualizza l'opzione Tempo di registrazione rispetto al lavoro quando è selezionata un'attività o un problema, consentendo agli utenti di registrare il tempo sugli elementi di lavoro direttamente dalle aree Home e Riepilogo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizza documenti associati al lavoro</td> 
      <td>Visualizza un'area Documenti in Home e Riepilogo quando viene selezionata un'attività o un problema, elencando tutti i documenti associati all'attività o al problema. Gli utenti possono fare clic sui documenti per visualizzarli in una finestra di anteprima.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nascondi data/ora</td> 
      <td>Nasconde le marche temporali per i seguenti campi data in Home and Summary:
       <ul>
        <li>Data di completamento Pianificata</li>
        <li>Conferma data</li>
        <li><p>Data di invio</p></li>
       </ul><p><b>NOTA</b>: Quando questa opzione è attivata, gli elementi di lavoro che scadono vengono spostati nel raggruppamento Ritardo nell'elenco Lavoro iniziale in base solo alla data e non all'ora.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continua a personalizzare il modello di layout.

   Oppure

   Al termine della personalizzazione, fai clic su **Salva**.

Per ulteriori informazioni sui modelli di layout, consulta [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
