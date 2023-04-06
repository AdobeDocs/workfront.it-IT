---
title: Creare o modificare livelli di accesso personalizzati
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: In qualità di amministratore di Adobe Workfront, puoi creare livelli di accesso personalizzati e applicarli agli utenti.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: 4a7999e6cb46d5b6933f44f1f19ff1979cb68a85
workflow-type: tm+mt
source-wordcount: '1405'
ht-degree: 6%

---

# Creare e modificare livelli di accesso personalizzati

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help.-->

In qualità di amministratore di Adobe Workfront, puoi creare livelli di accesso personalizzati e applicarli agli utenti. Quando si lavora con i livelli di accesso, è importante comprendere come funzionano insieme alle autorizzazioni per gli oggetti concesse dagli utenti quando condividono gli oggetti tra loro. Per ulteriori informazioni sui livelli di accesso, consulta

* [Panoramica dei livelli di accesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [Panoramica dei livelli di accesso legacy](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!IMPORTANT]
>
>È vivamente consigliato lasciare invariati i livelli di accesso incorporati, in modo da potervi fare riferimento dopo aver configurato gli utenti. Per personalizzare un livello di accesso, copia il livello di accesso predefinito e modifica la copia. Puoi eseguire questa operazione per ogni livello di accesso, ad eccezione di Amministratore di sistema e Utente esterno.

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
   <td>Piano attuale: Standard
   <p>oppure</p>
   <p>Piano legacy: Pianificare</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

## Creare o modificare un livello di accesso personalizzato

{{step-1-to-setup}}

1. Fai clic su **Livelli di accesso** nel pannello a sinistra.
1. Seleziona il livello di accesso da copiare e personalizzare, quindi fai clic su **Copia**.

   Oppure

   Se stai modificando un livello di accesso esistente (copiato in precedenza), fai clic sul suo nome.

1. Nella casella visualizzata, effettua una delle seguenti operazioni per iniziare a configurare il livello di accesso personalizzato:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>Digita un nome per il livello di accesso. </p> <p>Se hai appena copiato un livello di accesso per crearne uno nuovo, il nome predefinito è Nome livello di accesso (copia), dove Nome livello di accesso è il livello di accesso copiato.</p> <p><strong>Suggerimento</strong>: È consigliabile includere il nome originale del livello di accesso nel nome della copia. Ad esempio, nella società ACME, una copia del livello di accesso Standard potrebbe essere denominata ACME Standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione </td> 
      <td>Digita una descrizione per il livello di accesso. È utile elencare qui ciò a cui un utente con questo livello di accesso sarà in grado di accedere.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di licenza</td> 
      <td>Assicurati che la licenza selezionata qui sia quella più strettamente associata al tipo di livello di accesso che stai creando o modificando. La licenza selezionata determina le impostazioni disponibili per il livello di accesso. Per ulteriori informazioni, consulta <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">Panoramica sulle licenze legacy</a> o <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica delle licenze legacy di Adobe Workfront</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Condizionale) Se **Standard** o **Pianificare** è selezionato in **Tipo di licenza** casella, scorri fino alla sezione **Consenti accesso amministrativo per** e selezionare le autorizzazioni di accesso amministrativo per gli utenti che avranno questo livello di accesso.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Processi di approvazione</td> 
      <td>Creare e gestire processi di approvazione da utilizzare in tutto il sistema e per gruppi specifici.<p>Senza questo accesso, gli utenti possono creare solo processi di approvazione ad hoc sugli elementi che possono gestire.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aziende</td> 
      <td>Aggiungi nuove società e modifica società esistenti in Workfront.<br><p>Senza questo accesso, gli utenti possono visualizzare solo le aziende esistenti.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Moduli personalizzati</td> 
      <td>Crea e gestisci tutti i moduli personalizzati all’interno del gruppo. <br><p>Senza questo accesso, gli utenti possono solo allegare i moduli esistenti agli oggetti a cui hanno accesso per contribuire o gestire.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tassi di cambio</td> 
      <td> <p>Aggiungi nuova valuta in Workfront.</p> <p>Senza questo accesso, l'utente può aggiungere una valuta esistente solo a un progetto creato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spese</td> 
      <td>Visualizza tutte le spese relative agli oggetti in Workfront.<p>Senza questo accesso, l'utente può solo visualizzare quanto segue:</p>
       <ul>
        <li>Spese relative a progetti, attività o problemi che gestiscono</li>
        <li>Le proprie spese</li>
        <li>Le spese dei loro subordinati</li>
       </ul><p><b>NOTA</b>: Ciò non consente all'utente di creare nuovi tipi di spesa.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mansioni</td> 
      <td> <p>Con questo accesso, l'utente può effettuare le seguenti operazioni:</p> 
       <ul> 
        <li>Visualizzare e modificare i ruoli di lavoro esistenti</li> 
        <li>Aggiungi nuovi ruoli di lavoro</li> 
        <li>Modificare la fatturazione dei ruoli e le tariffe dei costi</li> 
       </ul> 
       <p>Per informazioni importanti sull'accesso ai dati finanziari disponibili per un utente Standard o Planner con accesso amministrativo ai ruoli di lavoro, consulta <a href="#planner-users-with-administrative-access-to-job-roles">Utenti standard o planner con accesso amministrativo ai ruoli di lavoro</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Milestone nel mio gruppo</td> 
      <td>Visualizzare tutti i percorsi delle fasi cardine nel sistema nel menu Percorsi Milestone in Configurazione. Gli utenti possono inoltre modificare o eliminare qualsiasi percorso cardine appartenente a uno qualsiasi dei loro gruppi. Gli utenti non possono gestire (modificare o eliminare) percorsi delle attività cardine non assegnati ai rispettivi di gruppi.<p>Senza questo accesso, gli utenti possono visualizzare solo i percorsi cardine esistenti e applicarli ai progetti a cui hanno accesso per la gestione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche promemoria</td> 
      <td>Crea e gestisci notifiche di promemoria in Workfront.<p>Senza questo accesso, gli utenti sono limitati alla ricezione e alla visualizzazione di notifiche.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schede orario e ore</td> 
      <td> <p>Gli amministratori dei gruppi possono assegnare profili della scheda attività agli utenti dei gruppi e dei sottogruppi gestiti.</p> <p>Senza questa opzione abilitata, gli amministratori dei gruppi non possono assegnare profili della scheda attività ad altri utenti nei gruppi e sottogruppi gestiti, anche se possono crearli.</p> <p>Tutti gli altri utenti con una licenza Standard o Plan possono visualizzare tutte le ore e i fogli ore in Workfront.</p> <p>Senza questa opzione abilitata, gli utenti possono visualizzare le ore solo nei seguenti casi:</p> 
       <ul> 
        <li>Progetti, attività o problemi che gestiscono</li> 
        <li>Scheda attività propria</li> 
        <li>Scheda attività di un utente che effettua un report</li> 
        <li>Scheda attività approvata</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Imposta restrizioni aggiuntive**, quindi imposta una qualsiasi delle seguenti restrizioni per il livello di accesso.

   >[!IMPORTANT]
   >
   >Per gli utenti esterni, come i fornitori (tutti coloro che non fanno parte dell’organizzazione), consigliamo di limitare l’accesso a attività, progetti, aggiornamenti, annunci, altre aziende, team e gruppi.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Non riconoscere mai l'accesso all'intero progetto quando assegnato a un'attività o a un problema</td> 
      <td> Impedisce agli utenti assegnati a attività o problemi di ottenere anche le autorizzazioni per il progetto principale, anche se le autorizzazioni del progetto lo consentono.<p>Per ulteriori informazioni sulla configurazione delle autorizzazioni per un progetto, consulta la sezione . <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> nell'articolo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Modifica progetti</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Non ereditare l'accesso ai documenti da progetti. attività, problemi, ecc...</td> 
      <td>Impedisce ai documenti di ereditare le autorizzazioni impostate sul relativo oggetto padre.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizza solo gli aggiornamenti in cui sono stati inclusi nella conversazione</td> 
      <td> <p>Consente agli utenti di visualizzare solo i commenti in cui sono stati inclusi il nome o il nome del proprio team.</p> <p> <p><b>NOTA</b>: Questo impedisce agli utenti di effettuare l’iscrizione agli elementi in Workfront. Per ulteriori informazioni sull'iscrizione agli elementi, vedi <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Aggiungi utenti</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Non consentire mai agli utenti di eliminare i commenti </td> 
      <td> <p>Impedisce agli utenti di eliminare i commenti sugli elementi. </p> <p><b>NOTA</b>: Nessuno può eliminare i commenti degli altri utenti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizza solo società, gruppi e team di appartenenza</td> 
      <td>Consente agli utenti di visualizzare e condividere gli elementi solo con società, gruppi e team a cui appartengono.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Non consentire mai la visualizzazione delle ore pianificate o delle ore effettive</td> 
      <td>Impedisce agli utenti di visualizzare l'orario pianificato e effettivo degli elementi di lavoro a cui hanno accesso. Possono, tuttavia, vedere Ore effettive che si registrano da soli, o ore registrate da qualcuno che gli riferisce.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Non consentire mai agli utenti di eliminare le notifiche</td> 
      <td>Impedisce agli utenti di eliminare gli annunci nel Centro annunci. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Inviare annunci</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Condizionale e facoltativo) Se il tuo sistema Workfront è configurato per gli utenti che appartengono a più aziende, limita la visibilità ad altri utenti in base alla società a cui appartengono nella sezione . **Le persone di altre aziende devono visualizzare solo gli utenti di**.

   Puoi limitare gli utenti a vedere solo gli utenti dalla loro azienda o dalla società che hai designato come azienda principale. Per ulteriori informazioni sull&#39;azienda primaria, vedi [Creare e modificare aziende](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >Se due utenti appartengono a due società diverse, ma possono visualizzare entrambi gli utenti della società principale, possono visualizzare l’area Aggiornamenti associata alla società principale.

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configurare l’accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), quali [Concedere l’accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Fai clic su **Salva**.

   Una volta creato il livello di accesso, è possibile assegnarlo a un utente (a meno che non si tratti di un livello di accesso amministratore di sistema).

   Per ulteriori informazioni, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   Per informazioni su come un amministratore di Adobe assegna un livello di accesso amministratore di sistema a un utente, vedere [Concedere a un utente pieno accesso amministrativo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Utenti standard o planner con accesso amministrativo ai ruoli di lavoro {#planner-users}

Se si concede a un utente Standard o Planner l&#39;accesso amministrativo ai ruoli di lavoro, l&#39;impostazione Modifica fatturazione ruolo e tassi di costo viene abilitata automaticamente per l&#39;utente.

Successivamente, se si disabilita l&#39;accesso amministrativo ai ruoli di lavoro per l&#39;utente, i ruoli di lavoro saranno ancora visibili all&#39;utente perché l&#39;impostazione Modifica fatturazione e tassi di costo ruolo è ancora abilitata.

Se questo accade e devi rimuovere l&#39;accesso dell&#39;utente per visualizzare i ruoli di lavoro, devi disabilitare l&#39;impostazione di autorizzazione Modifica fatturazione ruolo e tassi di costo dell&#39;utente. Per istruzioni, consulta [Concedere l’accesso ai dati finanziari](grant-access-financial.md).
