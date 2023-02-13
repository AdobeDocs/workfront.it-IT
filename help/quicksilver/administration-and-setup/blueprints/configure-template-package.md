---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Configurare una blueprint
description: È possibile configurare i dettagli del modello di progetto o della struttura organizzativa prima di installare la blueprint.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: df10bc8f-b980-4c61-ae6d-bcea03103738
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '1824'
ht-degree: 0%

---

# Configurare una blueprint

È possibile configurare i dettagli di una blueprint prima di installarla. I modelli di progetto e i tipi di blueprint della struttura organizzativa in genere richiedono l’impostazione di alcune preferenze e la mappatura di alcune proprietà. Altri tipi di blueprint potrebbero non richiedere la configurazione e li installerai così come sono. Per ulteriori informazioni sull&#39;installazione, vedi [Installare una blueprint](/help/quicksilver/administration-and-setup/blueprints/blueprints-install.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano</strong></td>
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licenza</strong></td>
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso</strong></td>
   <td> <p>[!UICONTROL System Administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurare una blueprint del modello di progetto

1. Trova il modello da utilizzare.
1. Fai clic su **[!UICONTROL Installa]**, quindi scegli un ambiente:

   <table style="table-layout:auto">
        <tr>
        <td><strong>Produzione</strong></td>
        <td>La produzione è il tuo ambiente live.</td>
    </tr>
    <tr>
        <td><strong>Anteprima Sandbox</strong></td>
        <td>L’anteprima sandbox è un ambiente di test che funge da replica dell’ambiente live e viene aggiornata ogni fine settimana da Workfront.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 e 2</strong></td>
        <td>La Sandbox di aggiornamento personalizzato è un ambiente di test separato che viene aggiornato manualmente dall’utente. È presente un costo aggiuntivo per ottenere la Sandbox di aggiornamento personalizzato.</td>
    </tr>
   </table>

1. Procedi con le sezioni seguenti:

   * [[!UICONTROL Preferenze del modello]](#template-preferences)
   * [[!UICONTROL Mappatura del ruolo]](#role-mapping)
   * [[!UICONTROL Mappatura del team]](#team-mapping)
   * [[!UICONTROL Mappatura dell&#39;azienda]g](#company-mapping)
   * [[!UICONTROL Mappatura del gruppo]](#group-mapping)

## [!UICONTROL Preferenze del modello] {#template-preferences}

Scegli come installare il modello.

È inoltre possibile designare la proprietà del modello prima di installare la blueprint. È possibile apportare modifiche a questi campi dopo aver installato il modello. Per ulteriori informazioni, consulta [Modificare i modelli di progetto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

![[!UICONTROL Preferenze del modello] sezione](assets/Blueprints_TemplatePreferences.png)

1. In [!UICONTROL Preferenze del modello] specificare un nuovo nome di modello.
1. Specifica quanto segue:

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Gestore di modelli]<strong></td>
        <td>Questa persona riceve le autorizzazioni [!UICONTROL Manage] sul modello e diventerà il proprietario del progetto quando il modello viene utilizzato per creare un progetto.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Template sponsor]</strong></td>
        <td>Questa persona è di solito un manager, un dirigente o un stakeholder che deve sapere cosa sta succedendo con il progetto. Lo sponsor del progetto non ottiene alcun accesso aggiuntivo al progetto, ma viene aggiunto alle notifiche e-mail per il progetto.</td>
    </tr>
    <tr>
        <td><strong>Portfolio [!UICONTROL]</strong></td>
        <td>Questo è il portfolio a cui apparirà il progetto quando verrà creato.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Program]</strong></td>
        <td>Questo è il programma a cui apparterrà il progetto quando verrà creato.</td>
    </tr>
   </table>

1. Seleziona se il modello è installato come attivo o inattivo.
1. Seleziona se desideri utilizzare le preferenze per i nuovi problemi definiti, se disponibili.

   Fai clic su **[!UICONTROL Vedere le preferenze relative ai problemi]** per esaminare le preferenze specifiche che verranno installate con la blueprint. I progetti creati dal modello importato utilizzano queste preferenze per i nuovi problemi aggiunti nel [!UICONTROL Problemi] sezione .

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Gruppi di argomenti coda</strong></td> 
      <td> <p>I gruppi di argomenti della coda definiscono il livello più alto di categorie per i problemi o le richieste. Gli utenti visualizzano i gruppi di argomenti come opzioni di menu quando selezionano dove inviare le richieste. Un gruppo di argomenti può contenere più argomenti della coda. Per ulteriori informazioni, consulta <a href="../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Crea gruppi di argomenti</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Argomenti per coda</strong></td> 
      <td> <p>Gli argomenti della coda funzionano insieme alle regole di routing per assegnare problemi o richieste. Sono le opzioni di menu che gli utenti selezionano quando inseriscono un problema o una richiesta, dopo aver selezionato un gruppo di argomenti. Per ulteriori informazioni, consulta <a href="../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Crea argomenti coda</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Regole di instradamento</strong></td> 
      <td>Le regole di instradamento inviano problemi o richieste a ruoli di lavoro , utenti o team specifici. Possono anche inviare le richieste a progetti specifici, diversi da quello associato alla coda delle richieste. Per ulteriori informazioni, consulta <a href="../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Creare regole di routing</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!INFO]
   >
   >**Esempio:** Le preferenze del nuovo problema in questo progetto forniscono quattro argomenti in coda. L&#39;utente seleziona uno di questi argomenti durante la creazione di un problema. Poiché esiste un solo gruppo di argomenti, questo viene applicato automaticamente e l’utente non deve selezionarlo. Quando l&#39;utente completa e invia il problema, le regole di indirizzamento determinano a quale ruolo o gruppo di lavoro viene assegnato.
   >![Esempio di nuove preferenze per i problemi](assets/Blueprints_IssuePrefsDetails.png)
   >![Argomenti della coda per il nuovo problema](assets/blueprints-newissueqtopicsexample-350x204.png)
   >![Problema instradato al ruolo di lavoro](assets/Blueprints_ProjectShowsIssueAssignment.png)

   >[!TIP]
   >
   >* L’utilizzo delle preferenze per i problemi consente di creare coerenza nel modo in cui vengono acquisiti i nuovi problemi o richieste sui progetti.
   >* L’impostazione di queste preferenze non rende automaticamente i progetti creati dal modello in code di richiesta. Per informazioni sulla configurazione di una coda di richiesta, vedi [Creare una coda di richiesta](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   >* Non tutte le blueprint contengono nuove preferenze per i problemi.



## [!UICONTROL Mappatura del ruolo] {#role-mapping}

>[!NOTE]
>
>Questa sezione potrebbe non essere visualizzata in alcune blueprint.

Alcuni modelli includono i ruoli di lavoro prescritti. I ruoli di lavoro consentono di assegnare le persone giuste quando il modello viene convertito in un progetto. Puoi personalizzare il modo in cui i ruoli vengono mappati prima di installare la blueprint. Fai clic su **[!UICONTROL Vedere le descrizioni dei ruoli]** per ulteriori informazioni sui ruoli disponibili nella blueprint.

La blueprint cerca in base al nome del ruolo per vedere se eventuali ruoli esistenti corrispondono. La ricerca distingue tra maiuscole e minuscole, pertanto i nomi devono corrispondere esattamente. Se nessun ruolo esistente corrisponde, puoi crearlo automaticamente tramite la blueprint.

![[!UICONTROL Mappatura del ruolo] sezione](assets/Blueprints_RoleMapping.png)

1. Se esiste un ruolo, puoi scegliere una delle seguenti opzioni:

   1. Creare un nuovo ruolo con un nome diverso, quindi digitare il nome nella casella di testo.
   1. Utilizzare il ruolo esistente, quindi selezionare un ruolo nella casella di selezione.
   1. Non utilizzare il ruolo mappato. Questa opzione non è consigliata perché ad alcune attività non saranno assegnati ruoli.

1. Se un ruolo non esiste, puoi scegliere una delle seguenti opzioni:

   1. Crea un nuovo ruolo. Questa opzione crea il ruolo consigliato dalla blueprint.
   1. Creare un nuovo ruolo con un nome diverso, quindi digitare il nome nella casella di testo.
   1. Utilizzare il ruolo esistente, quindi selezionare un ruolo nella casella di selezione.
   1. Non utilizzare il ruolo mappato. Questa opzione non è consigliata perché ad alcune attività non saranno assegnati ruoli.

>[!NOTE]
>
>Il processo di installazione non applica ruoli a persone specifiche. È necessario verificare le persone presenti in tali ruoli dopo aver installato la soluzione blueprint e assegnare le persone, se necessario. Per informazioni, consulta [Azioni da intraprendere dopo l’installazione di una blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Per ulteriori informazioni sui ruoli di lavoro in [!DNL Workfront], vedi [Creare e gestire ruoli di lavoro](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## [!UICONTROL Mappatura del team] {#team-mapping}

>[!NOTE]
>
>Questa sezione potrebbe non essere visualizzata in alcune blueprint.

Alcuni modelli includono i team prescritti. Il lavoro assegnato a un team può essere completato da qualsiasi membro del team. Puoi personalizzare il modo in cui i team vengono mappati prima di installare il blueprint. Fai clic su **[!UICONTROL Vedere le descrizioni del team]** per ulteriori informazioni sui team disponibili nella blueprint.

Il blueprint cerca in base al nome del team per vedere se i team esistenti corrispondono. La ricerca distingue tra maiuscole e minuscole, pertanto i nomi devono corrispondere esattamente. Se nessun team esistente corrisponde, puoi crearlo con il blueprint.

![[!UICONTROL Mappatura del team] sezione](assets/Blueprints_TeamMapping.png)

1. Se esiste un team, puoi scegliere una delle seguenti opzioni:

   1. Crea un nuovo team con un nome diverso, quindi digita il nome nella casella di testo.
   1. Utilizzo [!UICONTROL team esistente], quindi seleziona un team nella casella di selezione.
   1. Non utilizzare team mappati. Questa opzione non è consigliata perché ad alcune attività non saranno assegnati team.

1. Se un team non esiste, puoi scegliere una delle seguenti opzioni:

   1. Crea un nuovo team. Questa opzione crea il team consigliato dalla blueprint.
   1. Crea un nuovo team con un nome diverso, quindi digita il nome nella casella di testo.
   1. Utilizzo [!UICONTROL team esistente], quindi seleziona un team nella casella di selezione.
   1. Non utilizzare team mappati. Questa opzione non è consigliata perché ad alcune attività non saranno assegnati team.

>[!NOTE]
>
>Il processo di installazione non aggiunge persone ai team. Devi verificare le persone nei team dopo aver installato la soluzione blueprint e assegnare le persone, se necessario. Per informazioni, consulta [Azioni da intraprendere dopo l’installazione di una blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Per ulteriori informazioni sul funzionamento dei team in [!DNL Workfront], vedi [Creare e gestire i team](../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

## Mappatura dell&#39;azienda {#company-mapping}

>[!NOTE]
>
>Questa sezione potrebbe non essere visualizzata in alcune blueprint.

Alcuni progetti includono aziende prescritte. Un&#39;azienda è un&#39;unità organizzativa che può rappresentare la tua organizzazione, un reparto all&#39;interno dell&#39;organizzazione o un cliente con cui lavori. Puoi personalizzare il modo in cui le aziende vengono mappate prima di installare il blueprint. Fai clic su **[!UICONTROL Consulta le descrizioni aziendali]** per saperne di più sulle aziende disponibili nella blueprint.

Il blueprint cerca in base al nome dell&#39;azienda per vedere se le aziende esistenti corrispondono. La ricerca distingue tra maiuscole e minuscole, pertanto i nomi devono corrispondere esattamente. Se nessuna azienda esistente corrisponde, puoi crearla automaticamente tramite la blueprint. La società principale nel blueprint è mappata alla società principale nel tuo ambiente, anche se non hanno lo stesso nome.

![[!UICONTROL Mappatura dell&#39;azienda] sezione](assets/Blueprints_CompanyMapping.png)

1. Se esiste una società, puoi scegliere una delle seguenti opzioni:

   1. Crea una nuova società con un nome diverso, quindi digita il nome nella casella di testo.
   1. Utilizza la società esistente, quindi seleziona una società nella casella di selezione.\

      La società principale nel blueprint è mappata alla società principale nel tuo ambiente, anche se non hanno lo stesso nome.
   1. Non utilizzare società mappata. Questa opzione non è consigliata perché i riferimenti aziendali in altri oggetti saranno vuoti.

1. Se una società non esiste, puoi scegliere una delle seguenti opzioni:

   1. Crea una nuova azienda. Questa opzione crea l’azienda consigliata dalla blueprint.
   1. Crea una nuova società con un nome diverso, quindi digita il nome nella casella di testo.
   1. Utilizza la società esistente, quindi seleziona una società nella casella di selezione.
   1. Non utilizzare società mappata. Questa opzione non è consigliata perché i riferimenti aziendali in altri oggetti saranno vuoti.

>[!NOTE]
>
>Per configurare le aziende dopo l&#39;installazione del blueprint, vedi [Azioni da intraprendere dopo l’installazione di una blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Per informazioni sull&#39;associazione di un modello a un&#39;azienda, consulta [Modificare i modelli di progetto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Per informazioni sul funzionamento delle aziende in [!DNL Workfront], vedi [Creare e modificare aziende](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## [!UICONTROL Mappatura del gruppo] {#group-mapping}

>[!NOTE]
>
>Questa sezione potrebbe non essere visualizzata in alcune blueprint.

Alcuni progetti includono gruppi prescritti. Un gruppo è un gruppo di utenti che coincide con la struttura del reparto. I gruppi sono simili ma diversi dai team e dalle aziende in Workfront. È possibile personalizzare il modo in cui i gruppi vengono mappati prima di installare la blueprint. Fai clic su **[!UICONTROL Vedere le descrizioni dei gruppi]** per ulteriori informazioni sui gruppi disponibili nella blueprint.

La blueprint cerca in base al nome del gruppo per vedere se gli eventuali gruppi esistenti corrispondono. La ricerca distingue tra maiuscole e minuscole, pertanto i nomi devono corrispondere esattamente. Se non corrispondono gruppi esistenti, puoi crearli automaticamente con la blueprint.

![[!UICONTROL Mappatura del gruppo] sezione](assets/Blueprints_GroupMapping.png)

1. Se esiste un gruppo, puoi selezionare **[!UICONTROL Gruppo di rimedi]** e scegli una delle seguenti opzioni:

   1. **[!UICONTROL Crea un nuovo gruppo con un nome diverso]**, quindi digita il nome da assegnare a questo gruppo. I riferimenti al gruppo nella definizione della blueprint saranno invece associati a questo nuovo gruppo.
   1. **[!UICONTROL Sostituisci con un gruppo esistente]**, quindi cerca e seleziona un gruppo nella casella di selezione.

      >[!NOTE]
      >
      >Non è possibile rinominare un gruppo esistente.

1. Se un gruppo non esiste, puoi:

   1. Modificare il nome del gruppo suggerito digitandolo nella casella di testo.
   1. Seleziona **[!UICONTROL Gruppo di rimedi]** e scegli [!UICONTROL Sostituisci con un gruppo esistente], quindi cerca e seleziona un gruppo nella casella di selezione.
   1. Seleziona **[!UICONTROL Gruppo di rimedi]** e scegli **[!UICONTROL Inserisci sotto un gruppo esistente]**, quindi cerca e seleziona un gruppo nella casella di selezione. Questa opzione crea un nuovo sottogruppo sotto il gruppo esistente.

>[!NOTE]
>
>Per configurare i gruppi dopo l’installazione della blueprint, vedi [Azioni da intraprendere dopo l’installazione di una blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Per informazioni sull&#39;utilizzo dei gruppi in [!DNL Workfront], vedi [Panoramica sui gruppi](../../administration-and-setup/manage-groups/groups-overview/groups.md).
