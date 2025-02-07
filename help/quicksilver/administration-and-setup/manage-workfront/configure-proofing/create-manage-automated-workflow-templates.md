---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Creare e gestire modelli di flussi di lavoro automatizzati
description: In qualità di amministratore di Adobe Workfront, se il processo di revisione del contenuto dell’organizzazione viene spesso ripetuto o se il contenuto viene spesso rivisto dalle stesse persone, puoi creare modelli di Flusso di lavoro automatizzato che contengano i revisori con i ruoli delle bozze e le impostazioni di notifica specificati. Un modello di flusso di lavoro automatizzato può essere semplice con uno o due revisori o complesso con molte fasi e dipendenze.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '2079'
ht-degree: 0%

---

# Creare e gestire modelli di flussi di lavoro automatizzati

<!-- Audited: 2/2024 -->

In qualità di amministratore di Adobe Workfront, se il processo di revisione del contenuto dell’organizzazione viene spesso ripetuto o se il contenuto viene spesso rivisto dalle stesse persone, puoi creare modelli di Flusso di lavoro automatizzato che contengano i revisori con i ruoli delle bozze e le impostazioni di notifica specificati. Un modello di flusso di lavoro automatizzato può essere semplice con uno o due revisori o complesso con molte fasi e dipendenze.

I modelli di flusso di lavoro automatizzato semplificano la creazione di una bozza con un flusso di lavoro automatizzato. Quando un utente crea una bozza, sceglie semplicemente il modello necessario.

Puoi modificare facilmente qualsiasi modello di flusso di lavoro automatico, aggiungendo o rimuovendo revisori e fasi in qualsiasi momento. I creatori di bozze che utilizzano il modello possono aggiungere o rimuovere revisori per la bozza.

Quando si utilizza un modello di flusso di lavoro automatizzato, tenere presente quanto segue:

1. Le impostazioni di un modello di flusso di lavoro automatico determinano le operazioni che è possibile eseguire con il flusso di lavoro automatico per una bozza. Ad esempio, se il pulsante Aggiungi un’area di visualizzazione è disabilitato nel modello, non sarà visibile durante l’utilizzo delle impostazioni del flusso di lavoro automatico per la bozza.
1. Quando una persona viene aggiunta a una fase di un modello di flusso di lavoro automatico, ma è già presente come revisore nella bozza, l’applicazione del modello rimuove il revisore dalla fase. Se non si aggiunge un altro revisore all&#39;area di visualizzazione, verrà visualizzato un messaggio che richiede di aggiungerne uno.
1. La possibilità di modificare un modello di flusso di lavoro automatico dipende dalle impostazioni del modello configurate dall&#39;amministratore di Workfront, come descritto in . Se la possibilità di modificare il modello è disabilitata, solo il proprietario del modello può modificarlo.

Per informazioni sui flussi di lavoro automatizzati, vedere [Panoramica sui flussi di lavoro automatizzati](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Nuovo: Qualsiasi</p><p>Corrente: Pro o superiore</p><p>Legacy: Premium o Select</p> <p>Per ulteriori informazioni sulla verifica dell'accesso con i diversi piani, vedere <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alla funzionalità di verifica in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Nuovo: Standard</p><p>Corrente: Lavoro o Piano</p> <p>Legacy: qualsiasi (gli strumenti di correzione devono essere abilitati per l’utente)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Nel profilo di autorizzazione bozza deve essere selezionato Amministratore. </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare un modello di flusso di lavoro automatico

{{step1-to-proofing}}

1. Fai clic su **Flussi di lavoro** nel pannello a sinistra.
1. Nella scheda **Flusso di lavoro**, fai clic su **Nuovo** > **Nuovo modello**.

1. Nella sezione **Dettagli**, specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome modello</td> 
      <td>(Obbligatorio) Immetti un nome per il modello. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proprietario del modello</td> 
      <td>Puoi selezionare l’amministratore Workfront o Workfront Proof che gestirà il modello.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppo di modelli</td> 
      <td> <p> Se i flussi di lavoro automatizzati della tua organizzazione sono organizzati in gruppi, puoi selezionare il nome del gruppo. Per ulteriori informazioni, vedere <a href="#create-automated-workflow-template-groups" class="MCXref xref">Creare gruppi di modelli di flussi di lavoro automatizzati</a> più avanti in questo articolo.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Fuso orario modello </td> 
      <td> <p>Il fuso orario predefinito per il modello è quello in cui stai lavorando. Se il fuso orario dei creatori e dei revisori della bozza che utilizzeranno il modello è diverso, è possibile modificarlo qui per garantire che le scadenze dell’area di visualizzazione siano impostate nei momenti giusti per tali utenti. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti</td> 
      <td> <p>Puoi selezionare le attività dell’area di visualizzazione che desideri rendere disponibili alla persona che crea le bozze utilizzando il modello.</p> 
      <p><b>AVVISO</b>: se non si selezionano le opzioni Aggiungi un'area di visualizzazione e Aggiungi persone alle aree di visualizzazione, né il proprietario del modello né il proprietario di alcuna bozza che utilizza questo modello potranno aggiungere un'area di visualizzazione o condividere la bozza. 
      </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Nella sezione **Stadi**, configura ogni fase del modello di flusso di lavoro automatico.

   Puoi aggiungere più stadi e crearli tra di essi.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>Il nome dell’area di visualizzazione viene visualizzato nel diagramma Flusso di lavoro automatico nella parte superiore della sezione Flusso di lavoro, nella pagina Dettagli bozza e nelle notifiche e-mail inviate ai revisori.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attiva fase</td> 
      <td> <p>Specificare se la fase viene attivata automaticamente o manualmente. Per la prima fase, puoi selezionare <strong>Alla creazione della bozza</strong>, <strong>A una data e un'ora specifiche</strong> o <strong>Manualmente</strong>.</p> <p>Le altre opzioni diventano disponibili quando si aggiunge una seconda fase, poiché richiedono la selezione di una fase padre. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Scadenza calcolata a partire da</td> 
      <td> <p>Specificare la modalità di calcolo della scadenza:</p> 
       <ul> 
        <li> <p><strong>Creazione bozza</strong>: nell'elenco a discesa in <strong>Scadenza (+ giorni lavorativi)</strong>, selezionare il numero di giorni lavorativi da aggiungere alla data di creazione della bozza per impostare automaticamente una scadenza sulla bozza.</p> </li> 
        <li><strong>All'avvio della fase</strong>: nell'elenco a discesa in <strong>Scadenza (+ giorni lavorativi)</strong>, selezionare il numero di giorni lavorativi da aggiungere alla data di attivazione della fase per impostare automaticamente una scadenza sulla bozza.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fase di blocco</td> 
      <td>Specificare se si desidera consentire il blocco della fase per i commenti. Le opzioni consentono di bloccare una fase manualmente o automaticamente, all'avvio della fase successiva o quando tutte le decisioni vengono prese nella fase padre.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Principale responsabile delle decisioni</td> 
      <td> <p>I responsabili delle decisioni disponibili vengono visualizzati nell’elenco solo dopo l’aggiunta dei revisori all’area di visualizzazione.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Occorre solo una decisione</td> 
      <td>Il processo di riesame per la fase sarà completato non appena uno dei responsabili decisionali presenterà la propria decisione. Per ulteriori informazioni, vedere <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configurare le impostazioni di bozza in Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fase privata</td> 
      <td>Nasconde commenti e decisioni da a utenti che non sono aggiunti alla fase o che non sono amministratori di Workfront. Per ulteriori informazioni, vedere <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Panoramica del flusso di lavoro automatico</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Non consentire eliminazione di questa fase</td> 
      <td> <p>Rende obbligatoria la fase.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Se le bozze che utilizzeranno questo modello vengono sempre inviate alle stesse persone nell’area di visualizzazione, aggiungile qui in modo che gli utenti non debbano aggiungerle ogni volta che creano una bozza.

   Scegli il **Ruolo** di ogni persona nelle bozze che utilizzeranno questo modello e gli **avvisi e-mail** che desideri ricevere dall&#39;utente quando lavora sulle bozze che utilizzano questo modello.

   Per informazioni sui ruoli in una bozza, vedere [Configurare i ruoli di verifica predefiniti](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). Per informazioni sugli avvisi e-mail relativi alle bozze, vedere la sezione [Configurare i valori predefiniti per le bozze per un utente](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) nell&#39;articolo [Configurare le impostazioni delle notifiche e-mail in Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Ogni utente può essere aggiunto a una sola fase. È possibile aggiungere tutti gli utenti desiderati a una fase.

   >[!TIP]
   >
   >È possibile trascinare i nomi dei revisori tra le fasi del diagramma fasi. Le fasi disponibili sono evidenziate in blu.

1. Ripetere i due passaggi precedenti per qualsiasi altra fase che si desidera aggiungere al modello.

   Nella parte superiore della sezione **Flusso di lavoro** è possibile visualizzare un diagramma del flusso di lavoro automatico che si sta impostando. Man mano che continuate ad aggiungere stadi, questi vengono visualizzati nel diagramma con linee che mostrano le dipendenze tra di essi. È possibile fare clic su uno stadio nel diagramma per visualizzarne le impostazioni.

   Se non è necessario visualizzare il diagramma, fare clic su **Nascondi diagramma**.

1. Nella sezione **Condividi modello con** fare clic su un&#39;opzione (se il modello non è già condiviso con l&#39;intera organizzazione) per specificare gli utenti che potranno utilizzarlo.

   Per impostazione predefinita, i nuovi modelli di flussi di lavoro automatizzati sono condivisi con tutti gli utenti dell’organizzazione.

1. Fai clic su **Crea**.

## Modificare un modello di flusso di lavoro automatico

In qualità di amministratore di Workfront Proof, puoi modificare un modello di flusso di lavoro automatico. Le modifiche apportate vengono salvate automaticamente.

{{step1-to-proofing}}

1. Fai clic su **Flussi di lavoro** nel pannello a sinistra.
1. Nell&#39;elenco **Modelli di flusso di lavoro** visualizzato fare clic sul modello che si desidera modificare.
1. Nella sezione **Dettagli**, specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome modello</td> 
      <td>(Obbligatorio) Immetti un nome per il modello. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proprietario del modello</td> 
      <td>Puoi selezionare l’amministratore Workfront o Workfront Proof che gestirà il modello.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppo di modelli</td> 
      <td> <p> Se i flussi di lavoro automatizzati della tua organizzazione sono organizzati in gruppi, puoi selezionare il nome del gruppo. Per ulteriori informazioni, vedere <a href="#create-automated-workflow-template-groups" class="MCXref xref">Creare gruppi di modelli di flussi di lavoro automatizzati</a> più avanti in questo articolo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fuso orario modello </td> 
      <td> <p>Il fuso orario predefinito per il modello è quello in cui stai lavorando. Se il fuso orario dei creatori e dei revisori della bozza che utilizzeranno il modello è diverso, è possibile modificarlo qui per garantire che le scadenze dell’area di visualizzazione siano impostate nei momenti giusti per tali utenti. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti</td> 
      <td> <p>Seleziona le attività di staging che desideri rendere disponibili a coloro che creano bozze utilizzando il modello. </p> <p><b>AVVISO</b>: se non si selezionano le opzioni Aggiungi un'area di visualizzazione e Aggiungi persone alle aree di visualizzazione, né il proprietario del modello né il proprietario di alcuna bozza che utilizza questo modello potranno aggiungere un'area di visualizzazione o condividere la bozza.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Nella sezione **Flusso di lavoro**, modifica il nome di una fase ed espandine le impostazioni ![Pulsante Espandi](assets/arrow-button.png) per apportare le modifiche necessarie:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Scadenza calcolata a partire da</td> 
      <td> <p>Specificare la modalità di calcolo della scadenza:</p> 
       <ul> 
        <li> <p><strong>Scadenza calcolata dalla creazione della bozza</strong>: nell'elenco a discesa <strong>Imposta la scadenza dell'area di visualizzazione</strong>, selezionare il numero di giorni lavorativi da aggiungere alla data di creazione della bozza per impostare automaticamente una scadenza sulla bozza.</p> </li> 
        <li><strong>Scadenza calcolata dall'attivazione della fase</strong>: nell'elenco a discesa <strong>Imposta la scadenza della fase</strong>, selezionare il numero di giorni lavorativi da aggiungere alla data di attivazione della fase per impostare automaticamente una scadenza sulla bozza.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attiva fase</td> 
      <td> <p>Specificare se la fase viene attivata automaticamente o manualmente. Per la prima fase, puoi selezionare <strong>Alla creazione della bozza</strong>, <strong>A una data e un'ora specifiche</strong> o <strong>Manualmente</strong>.</p> <p>Le altre opzioni diventano disponibili quando si aggiunge una seconda fase, poiché richiedono la selezione di una fase padre. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fase di blocco</td> 
      <td>Specificare se si desidera consentire il blocco della fase per i commenti. Le opzioni consentono di bloccare una fase manualmente o automaticamente, all'avvio della fase successiva o quando tutte le decisioni vengono prese nella fase padre.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisione</td> 
      <td>Termina la fase la prima volta che uno dei decisori presenta la propria decisione. Per ulteriori informazioni, vedere <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configurare le impostazioni di bozza in Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Privacy</td> 
      <td>Nasconde i commenti e le decisioni da a persone che non sono aggiunte alla fase o che non sono supervisori e superiori nell’account. Per ulteriori informazioni, vedere <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Panoramica del flusso di lavoro automatico</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminazione fase</td> 
      <td>Rende obbligatoria la fase.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Altro <img src="assets/more-icon.png"></td> 
      <td>Aggiungere revisori all'area di visualizzazione o eliminare l'area di visualizzazione.<p>Se ciascuna bozza viene inviata alle stesse persone in una determinata fase, è possibile specificarne il nome in modo da non doverla aggiungere ogni volta che si crea una bozza. Digita e seleziona il nome di un utente che desideri aggiungere all'area di visualizzazione, quindi aggiungi il relativo <strong>Ruolo</strong> nella bozza e le <strong>impostazioni degli avvisi e-mail</strong> desiderate per l'utente. Per informazioni sui ruoli di verifica, vedere <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Configurare i ruoli di verifica predefiniti</a>. Per informazioni sugli avvisi e-mail relativi alle bozze, vedere la sezione <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Configurare i valori predefiniti per le bozze per un utente</a> nell'articolo <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configurare le impostazioni delle notifiche e-mail in Workfront Proof</a>.</p><p>È possibile aggiungere tutti gli utenti desiderati a una fase</p><p>Suggerimento: è possibile trascinare i nomi dei revisori tra le fasi del diagramma fasi. Le fasi disponibili sono evidenziate in blu.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Ripetere il passaggio per tutte le altre fasi che si desidera aggiungere al modello.

   Nella parte superiore della sezione **Flusso di lavoro** è possibile visualizzare un diagramma del flusso di lavoro automatico che si sta impostando. Man mano che continuate ad aggiungere stadi, questi vengono visualizzati nel diagramma con linee che mostrano le dipendenze tra di essi. È possibile fare clic su uno stadio nel diagramma per visualizzarne le impostazioni.

   Se non è necessario visualizzare il diagramma, fare clic su **Nascondi diagramma**.

1. Nella sezione **Condiviso con**, se desideri eliminare un utente, fai clic sul pulsante Altro ![Icona Altro](assets/more-icon.png) a destra, quindi fai clic su **Rimuovi**.

## Creare gruppi di modelli di flussi di lavoro automatizzati {#create-automated-workflow-template-groups}

In qualità di amministratore di Workfront, puoi visualizzare e gestire tutti i modelli di flussi di lavoro automatizzati nell’account della tua organizzazione. Può essere utile organizzare i modelli in gruppi.

Per creare un gruppo di modelli di flusso di lavoro automatizzato:

{{step1-to-proofing}}

1. Fai clic su **Flussi di lavoro** nel pannello a sinistra.
1. Nella scheda **Flusso di lavoro**, fai clic su **Nuovo** > **Nuovo gruppo di modelli**.
1. Digitare un nome descrittivo per il nuovo gruppo di modelli, quindi premere **Invio**.

Puoi spostare i modelli da un gruppo all’altro trascinandoli.

## Gestire i modelli di flussi di lavoro automatizzati

{{step1-to-proofing}}

1. Nel pannello a sinistra di Workfront Proof, fai clic su **Flussi di lavoro**.
1. Nella pagina **Flussi di lavoro** visualizzata eseguire una delle operazioni seguenti:

   * Aggiungi un nuovo modello
   * Aggiungi un nuovo gruppo di modelli
   * Elimina uno o più gruppi di modelli
   * Accedere ai dettagli di un modello
   * Trascinare un modello in un gruppo di modelli diverso
