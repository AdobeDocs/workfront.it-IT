---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Creare e gestire modelli di flussi di lavoro automatizzati
description: In qualità di amministratore di Adobe Workfront, se il processo di revisione del contenuto dell’organizzazione viene spesso ripetuto o il contenuto viene spesso esaminato dalle stesse persone, puoi creare modelli di flusso di lavoro automatizzato che contengono i revisori con i ruoli di bozza e le impostazioni di notifica specificate. Un modello di flusso di lavoro automatizzato può essere semplice con uno o due revisori o complesso con molte fasi e dipendenze.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '2096'
ht-degree: 0%

---

# Creare e gestire modelli di flussi di lavoro automatizzati

In qualità di amministratore di Adobe Workfront, se il processo di revisione del contenuto dell’organizzazione viene spesso ripetuto o il contenuto viene spesso esaminato dalle stesse persone, puoi creare modelli di flusso di lavoro automatizzato che contengono i revisori con i ruoli di bozza e le impostazioni di notifica specificate. Un modello di flusso di lavoro automatizzato può essere semplice con uno o due revisori o complesso con molte fasi e dipendenze.

I modelli di flusso di lavoro automatizzato semplificano la creazione di una bozza con un flusso di lavoro automatizzato. Quando un utente crea una bozza, sceglie semplicemente il modello di cui ha bisogno.

È possibile modificare facilmente qualsiasi modello di flusso di lavoro automatizzato, aggiungendo o rimuovendo revisori e aree di visualizzazione, in qualsiasi momento. Inoltre, i creatori di prove che utilizzano il modello possono aggiungere o rimuovere i revisori per la bozza.

Quando utilizzi un modello di flusso di lavoro automatizzato, considera quanto segue:

1. Le impostazioni di un modello di flusso di lavoro automatizzato determinano le operazioni che è possibile eseguire con il flusso di lavoro automatico per una bozza. Ad esempio, se il pulsante Aggiungi un passaggio è disabilitato nel modello, questo non è visibile perché lavori con le impostazioni del flusso di lavoro automatizzato per la bozza.
1. Quando una persona viene aggiunta a una pagina in un modello di flusso di lavoro automatizzato, ma è già presente come revisore sulla bozza, l’applicazione del modello rimuove il revisore dal passaggio. Se non aggiungi un altro revisore all’area di visualizzazione, viene visualizzato un messaggio per richiedere di aggiungerne uno.
1. La possibilità di modificare un modello di flusso di lavoro automatizzato dipende dalle impostazioni del modello configurate dall’amministratore di Workfront, come descritto in . Se la possibilità di modificare il modello è disabilitata, solo il proprietario del modello può modificarlo.

Per informazioni sui flussi di lavoro automatizzati, consulta [Panoramica del flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Piano attuale: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Premium o Select</p> <p>Per ulteriori informazioni sulla verifica dell’accesso con i diversi piani, consulta <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alle funzionalità di correzione in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano attuale: Lavoro o piano</p> <p>Piano legacy: Qualsiasi (è necessario che la correzione sia attivata per l’utente)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>È necessario che l’amministratore sia selezionato nel profilo delle autorizzazioni di prova. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configurare l’accesso per la correzione di un utente</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare un modello di flusso di lavoro automatizzato

1. In Workfront, fai clic sul menu principale ![](assets/main-menu-icon.png), quindi fai clic su Proofing ![](assets/proofing-in-main-menu.png) per accedere a Workfront Proof.
1. Fai clic su **Flussi di lavoro** nel pannello a sinistra.
1. Sulla **Flusso di lavoro** scheda , fai clic su **Nuovo** > **Nuovo modello**.

1. In **Dettagli** specificare le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome del modello</td> 
      <td>(Obbligatorio) Immetti un nome per il modello. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proprietario del modello</td> 
      <td>Puoi selezionare l’amministratore Workfront o l’amministratore di Workfront Proof che gestirà il modello.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppo di modelli</td> 
      <td> <p> Se i flussi di lavoro automatizzati della tua organizzazione sono organizzati in gruppi, puoi selezionare il nome del gruppo. Vedi <a href="#create-automated-workflow-template-groups" class="MCXref xref">Creare gruppi di modelli di flussi di lavoro automatizzati</a> più avanti in questo articolo per ulteriori informazioni.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Fuso orario modello </td> 
      <td> <p>Il fuso orario predefinito per il modello è quello in cui si sta lavorando. Se il fuso orario dei creatori e revisori delle prove che utilizzeranno il modello è diverso, puoi modificarlo qui per garantire che le scadenze dello stadio siano impostate nei momenti giusti per tali utenti. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti</td> 
      <td> <p>Puoi selezionare le attività dell’area di visualizzazione che desideri rendere disponibili all’utente che crea le bozze utilizzando il modello .</p> <!--
        <p><b>WARNING</b>: If you don't select the options Add a stage and Add people to stages, neither the template owner nor the owner of any proof using this template will be able to add a stage or share the proof. <!--
          <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Test this. Andrzej thinks it's wrong info or a bug.</span>
         --></p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. In **Fasi** configura ogni fase del modello Flusso di lavoro automatizzato.

   È possibile aggiungere più fasi e crearle tra loro.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>Il nome dell’area di visualizzazione viene visualizzato nel diagramma del flusso di lavoro automatizzato nella parte superiore della sezione Flusso di lavoro, nella pagina Dettagli bozza e nelle notifiche e-mail inviate ai revisori.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attiva fase</td> 
      <td> <p>Specifica se l’area di visualizzazione viene attivata automaticamente o manualmente. Per il primo passaggio, puoi selezionare <strong>Creazione a prova di</strong>, <strong>In una data e un’ora specifiche</strong>oppure <strong>Manualmente</strong>.</p> <p>Le altre opzioni diventano disponibili quando si aggiunge una seconda fase perché richiedono la selezione di uno stadio padre. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Termine calcolato a partire da</td> 
      <td> <p>Specificare la modalità di calcolo della scadenza:</p> 
       <ul> 
        <li> <p><strong>Creazione di prove</strong>: Nell’elenco a discesa sotto <strong>Scadenza (+ giorni lavorativi)</strong>, seleziona il numero di giorni lavorativi da aggiungere alla data di creazione della bozza per impostare automaticamente una scadenza sulla bozza.</p> </li> 
        <li><strong>All'inizio dello stage</strong>: Nell’elenco a discesa sotto <strong>Scadenza (+ giorni lavorativi)</strong>, seleziona il numero di giorni lavorativi che desideri aggiungere alla data di attivazione dell’area di visualizzazione per impostare automaticamente una scadenza sulla bozza.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Blocca fase</td> 
      <td>Specifica se consentire il blocco dell’area di visualizzazione per i commenti. Le opzioni sono quelle di bloccare un passaggio manualmente o automaticamente, sia all'avvio della fase successiva che quando tutte le decisioni vengono prese sullo stage principale.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Principale responsabile delle decisioni</td> 
      <td> <p>I responsabili decisionali disponibili vengono visualizzati nell’elenco solo dopo l’aggiunta dei revisori allo stadio.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Occorre solo una decisione</td> 
      <td>Il processo di revisione per la fase sarà completato non appena uno dei decisori presenterà la propria decisione. Per ulteriori informazioni, consulta <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configurare le impostazioni di bozza in Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stage privato</td> 
      <td>Nasconde i commenti e le decisioni di a persone che non vengono aggiunte allo stage o che non sono amministratori di Workfront&lt;!&gt;— DISEGNATO IN FLARE: Autorità di vigilanza e versioni successive

       -->. Per ulteriori informazioni, consulta &lt;a href=&quot;../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md&quot; class=&quot;MCXref xref&quot;>Panoramica del flusso di lavoro automatizzato&lt;/a>.&lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader">Non consentire l'eliminazione di questa fase</td> 
      <td> <p>Rende obbligatoria la fase.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Se le bozze che useranno questo modello vengono sempre inviate alle stesse persone nel passaggio , aggiungili qui in modo che gli utenti non debbano aggiungerle ogni volta che creano una bozza.

   Scegli il **Ruolo** sulle bozze che utilizzeranno questo modello e il **Avvisi e-mail** desideri che l’utente riceva quando lavora alle bozze che utilizzano questo modello.

   Per informazioni sui ruoli in una bozza, consulta [Configurare i ruoli di correzione predefiniti](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). Per informazioni sugli avvisi e-mail di bozza, consulta la sezione . [Configurare i valori predefiniti della bozza per un utente](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) nell&#39;articolo  [Configurare le impostazioni di notifica e-mail in Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Ogni utente può essere aggiunto a una sola fase. È possibile aggiungere un numero illimitato di utenti a un&#39;area di visualizzazione.

   >[!TIP]
   >
   >È possibile trascinare e rilasciare i nomi dei revisori tra le diverse aree nel diagramma delle aree di visualizzazione. Le tappe disponibili sono evidenziate in blu.

1. Ripetere i due passaggi precedenti per tutti gli altri passaggi che si desidera aggiungere al modello.

   Nella parte superiore del **Flusso di lavoro** Puoi vedere un diagramma del flusso di lavoro automatizzato che stai impostando. Man mano che si aggiungono gli stadi, questi compaiono nel diagramma con linee che mostrano le dipendenze tra di loro. È possibile fare clic su un&#39;area di visualizzazione nel diagramma per visualizzare le impostazioni relative a tale area di visualizzazione.

   Se non è necessario visualizzare il diagramma, è possibile fare clic su **Nascondi diagramma**.

1. In **Condividi modello con** fai clic su un’opzione (se il modello non è già condiviso con l’intera organizzazione) per specificare chi potrà utilizzarlo.

   Per impostazione predefinita, i nuovi modelli di flusso di lavoro automatizzato sono condivisi con tutti gli utenti dell’organizzazione.

1. Fai clic su **Crea**.

## Modificare un modello di flusso di lavoro automatizzato

In qualità di amministratore di Workfront Proof, puoi modificare un modello di flusso di lavoro automatizzato. Le modifiche vengono salvate automaticamente mentre le apporti.

1. In Workfront, fai clic sul menu principale ![](assets/main-menu-icon.png), quindi fai clic su Proofing ![](assets/proofing-in-main-menu.png) per accedere a Workfront Proof.
1. Fai clic su **Flussi di lavoro** nel pannello a sinistra.
1. In **Modelli di flusso di lavoro** elenco visualizzato, fare clic sul modello da modificare.
1. In **Dettagli** specificare le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome del modello</td> 
      <td>(Obbligatorio) Immetti un nome per il modello. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proprietario del modello</td> 
      <td>Puoi selezionare l’amministratore Workfront o l’amministratore di Workfront Proof che gestirà il modello.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppo di modelli</td> 
      <td> <p> Se i flussi di lavoro automatizzati della tua organizzazione sono organizzati in gruppi, puoi selezionare il nome del gruppo. Vedi <a href="#create-automated-workflow-template-groups" class="MCXref xref">Creare gruppi di modelli di flussi di lavoro automatizzati</a> più avanti in questo articolo per ulteriori informazioni.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fuso orario modello </td> 
      <td> <p>Il fuso orario predefinito per il modello è quello in cui si sta lavorando. Se il fuso orario dei creatori e revisori delle prove che utilizzeranno il modello è diverso, puoi modificarlo qui per garantire che le scadenze dello stadio siano impostate nei momenti giusti per tali utenti. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti</td> 
      <td> <p>Seleziona le attività dell’area di visualizzazione che desideri rendere disponibili a coloro che creano bozze utilizzando il modello. </p> <p><b>AVVISO</b>: Se non selezioni le opzioni Aggiungi un passaggio e Aggiungi persone alle aree di visualizzazione, né il proprietario del modello né il proprietario di alcuna bozza che utilizza questo modello saranno in grado di aggiungere un'area di visualizzazione o condividere la bozza.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. In **Flusso di lavoro** sezione , modifica il nome di qualsiasi area di visualizzazione ed espandi le relative impostazioni ![](assets/arrow-button.png) per apportare le modifiche necessarie:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Termine calcolato a partire da</td> 
      <td> <p>Specificare la modalità di calcolo della scadenza:</p> 
       <ul> 
        <li> <p><strong>Termine calcolato dalla creazione della bozza</strong>: In <strong>Imposta la scadenza della fase</strong> elenco a discesa, selezionare il numero di giorni lavorativi che si desidera aggiungere alla data di creazione della bozza per impostare automaticamente una scadenza sulla bozza.</p> </li> 
        <li><strong>Termine calcolato dall’attivazione dell’area di visualizzazione</strong>: In <strong>Imposta la scadenza della fase</strong> dall’elenco a discesa, seleziona il numero di giorni lavorativi che desideri aggiungere alla data di attivazione dell’area di visualizzazione per impostare automaticamente una scadenza sulla bozza.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attiva fase</td> 
      <td> <p>Specifica se l’area di visualizzazione viene attivata automaticamente o manualmente. Per il primo passaggio, puoi selezionare <strong>Creazione a prova di</strong>, <strong>In una data e un’ora specifiche</strong>oppure <strong>Manualmente</strong>.</p> <p>Le altre opzioni diventano disponibili quando si aggiunge una seconda fase perché richiedono la selezione di uno stadio padre. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Blocca fase</td> 
      <td>Specifica se consentire il blocco dell’area di visualizzazione per i commenti. Le opzioni sono quelle di bloccare un passaggio manualmente o automaticamente, sia all'avvio della fase successiva che quando tutte le decisioni vengono prese sullo stage principale.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisione</td> 
      <td>Termina la fase la prima volta che uno dei decisori presenta la propria decisione. Per ulteriori informazioni, consulta <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configurare le impostazioni di bozza in Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Privacy</td> 
      <td>Nasconde i commenti e le decisioni di a persone che non sono aggiunte alla fase o che non sono autorità di vigilanza e sopra nel conto. Per ulteriori informazioni, consulta <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Panoramica del flusso di lavoro automatizzato</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminazione fase</td> 
      <td>Rende obbligatoria la fase.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Altro <img src="assets/more-icon.png"></td> 
      <td>Aggiungi i revisori all’area di visualizzazione o elimina l’area di visualizzazione.<p>Se ciascuna delle tue bozze viene inviata alle stesse persone in un particolare passaggio, puoi specificarne il nome qui in modo da non doverle aggiungere ogni volta che crei una bozza. Digita e seleziona il nome di un utente da aggiungere all’area di visualizzazione, quindi aggiungi il relativo <strong>Ruolo</strong> sulla prova e <strong>Avvisi e-mail</strong> impostazioni desiderate per l'utente. Per informazioni sui ruoli di correzione, consulta <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Configurare i ruoli di correzione predefiniti</a>. Per informazioni sugli avvisi e-mail di bozza, consulta la sezione . <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Configurare i valori predefiniti della bozza per un utente</a> nell'articolo <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configurare le impostazioni di notifica e-mail in Workfront Proof</a>.</p><p>Puoi aggiungere quanti utenti desideri a un’area di visualizzazione</p><p>Suggerimento: È possibile trascinare e rilasciare i nomi dei revisori tra le diverse aree nel diagramma delle aree di visualizzazione. Le tappe disponibili sono evidenziate in blu.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Ripetere il passaggio per tutti gli altri passaggi che si desidera aggiungere al modello.

   Nella parte superiore del **Flusso di lavoro** Puoi vedere un diagramma del flusso di lavoro automatizzato che stai impostando. Man mano che si aggiungono gli stadi, questi compaiono nel diagramma con linee che mostrano le dipendenze tra di loro. È possibile fare clic su un&#39;area di visualizzazione nel diagramma per visualizzare le impostazioni relative a tale area di visualizzazione.

   Se non è necessario visualizzare il diagramma, è possibile fare clic su **Nascondi diagramma**.

1. In **Condiviso con** Se desideri eliminare un utente, fai clic su Altro ![](assets/more-icon.png) a destra, quindi fare clic su **Rimuovi**.

## Creare gruppi di modelli di flussi di lavoro automatizzati {#create-automated-workflow-template-groups}

In qualità di amministratore di Workfront, puoi visualizzare e gestire tutti i modelli di flusso di lavoro automatizzato nell’account della tua organizzazione. Può essere utile organizzare i modelli in gruppi.

Per creare un gruppo di modelli di flusso di lavoro automatizzato:

1. In Workfront, fai clic sul menu principale ![](assets/main-menu-icon.png), quindi fai clic su Proofing ![](assets/proofing-in-main-menu.png) per accedere a Workfront Proof.
1. Fai clic su **Flussi di lavoro** nel pannello a sinistra.
1. Sulla **Flusso di lavoro** scheda , fai clic su **Nuovo** > **Nuovo gruppo di modelli**.
1. Digitare un nome descrittivo per il nuovo gruppo di modelli, quindi premere **Invio**.

È possibile spostare i modelli tra gruppi mediante trascinamento.

## Gestire i modelli di flussi di lavoro automatizzati

1. In Workfront, fai clic sul menu principale ![](assets/main-menu-icon.png), quindi fai clic su Proofing ![](assets/proofing-in-main-menu.png) per accedere a Workfront Proof.

1. Nel pannello a sinistra in Workfront Proof, fai clic su **Flussi di lavoro**.
1. Sulla **Flussi di lavoro** pagina visualizzata, effettuare una delle seguenti operazioni:

   * Aggiungi un nuovo modello
   * Aggiungi un nuovo gruppo di modelli
   * Elimina uno o più gruppi di modelli
   * Accedere ai dettagli di un modello
   * Trascina un modello in un gruppo di modelli diverso
