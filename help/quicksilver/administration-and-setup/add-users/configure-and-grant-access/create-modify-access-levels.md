---
title: Creare e modificare livelli di accesso personalizzati
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: In qualità di amministratore di Adobe Workfront, puoi creare livelli di accesso personalizzati e applicarli agli utenti.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 6%

---

# Creare e modificare i livelli di accesso personalizzati

<!--Audited: 12/2023-->

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help. -->

In qualità di amministratore di Adobe Workfront, puoi creare livelli di accesso personalizzati e applicarli agli utenti. Quando si lavora con i livelli di accesso, è importante comprendere in che modo collaborano con le autorizzazioni per gli oggetti concesse dagli utenti quando condividono gli oggetti tra loro. Per ulteriori informazioni sui livelli di accesso, vedere:

* [Panoramica dei nuovi livelli di accesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

>[!IMPORTANT]
>
>È consigliabile lasciare invariati i livelli di accesso incorporati in modo da potervi fare riferimento dopo aver configurato gli utenti. Per personalizzare un livello di accesso, copiare il livello di accesso predefinito e modificare la copia. È possibile eseguire questa operazione per ogni livello di accesso, ad eccezione di Amministratore di sistema e Utente esterno.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare o modificare un livello di accesso personalizzato

{{step-1-to-setup}}

1. Fai clic su **Livelli di accesso** nel pannello a sinistra.
1. &#x200B;
   * Nell’ambiente di produzione:
Seleziona il livello di accesso da copiare e personalizzare, quindi fai clic su **Copia**.

     Oppure

     Se si sta modificando un livello di accesso esistente (copiato in precedenza), fare clic sul relativo nome.

   * <span class="preview">Nell&#39;ambiente di anteprima:</span>

     <span class="preview">Selezionare il livello di accesso che si desidera copiare e personalizzare, quindi fare clic sull&#39;icona **Copia** ![Copia icona](assets/copy-icon.png). </span>

     <span class="preview"> O </span>

     <span class="preview">Se stai modificando un livello di accesso esistente, seleziona il livello di accesso facendo clic sulla casella a sinistra di tale livello di accesso, quindi fai clic sull&#39;icona **Modifica** ![Icona Modifica](assets/edit-icon.png). </span>

1. Nella casella visualizzata, eseguire una delle operazioni seguenti per iniziare a configurare il livello di accesso personalizzato:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>Digita un nome per il livello di accesso. </p> <p>Se è stato appena copiato un livello di accesso per crearne uno nuovo, il nome predefinito è Nome livello di accesso (copia), dove Nome livello di accesso è il livello di accesso copiato.</p> <p><strong>Suggerimento</strong>: si consiglia di includere il nome originale del livello di accesso nel nome della copia. Ad esempio, presso la società ACME, una copia del livello di accesso Standard potrebbe essere denominata ACME Standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione </td> 
      <td>Digitare una descrizione per il livello di accesso. È utile elencare qui ciò a cui un utente con questo livello di accesso potrà accedere.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di licenza</td> 
      <td>Assicurarsi che la licenza selezionata sia quella più strettamente associata al tipo di livello di accesso che si sta creando o modificando. La licenza selezionata determina le impostazioni disponibili per il livello di accesso. Per ulteriori informazioni, vedere <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Panoramica nuove licenze</a> o <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Panoramica licenze</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Condizionale) Se nella casella **Tipo di licenza** è selezionato **Standard** o **Piano**, scorrere fino alla sezione **Consenti accesso amministrativo per** e selezionare le autorizzazioni di accesso amministrativo per coloro che avranno questo livello di accesso.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Processi di approvazione</td> 
      <td>Crea e gestisci i processi di approvazione per l’utilizzo in tutto il sistema e per gruppi specifici.<p>Senza questo accesso, gli utenti possono creare solo processi di approvazione ad hoc sugli elementi che hanno accesso da gestire.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aziende</td> 
      <td>Aggiungere nuove società e modificare quelle esistenti in Workfront.<br><p>Senza questo accesso, gli utenti possono solo visualizzare le aziende esistenti.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Moduli personalizzati</td> 
      <td>Crea e gestisci tutti i moduli personalizzati all’interno del loro gruppo. <br><p>Senza questo accesso, gli utenti possono allegare i moduli esistenti solo agli oggetti a cui hanno accesso per contribuire o gestire.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tassi di cambio</td> 
      <td> Aggiungi nuova valuta in Workfront. <p>Senza questo accesso, l’utente può aggiungere una valuta esistente solo a un progetto che ha creato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spese</td> 
      <td>Visualizza tutte le spese sugli oggetti in Workfront.<p>Senza questo accesso, l’utente può visualizzare solo quanto segue:</p>
       <ul>
        <li>Spese per progetti, attività o problemi da loro gestiti</li>
        <li>Le proprie spese</li>
        <li>Le spese dei loro subordinati</li>
       </ul><p><b>NOTA</b>: questo non consente all'utente di creare nuovi tipi di spesa.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mansioni</td> 
      <td> Con questo accesso, l’utente può effettuare le seguenti operazioni: 
       <ul> 
        <li>Visualizza e modifica i ruoli esistenti</li> 
        <li>Aggiungi nuove mansioni</li> 
        <li>Modifica fatturazione mansioni e tassi di costo</li> 
       </ul> 
       <p>Per informazioni importanti sull'accesso ai dati finanziari disponibili per un utente Standard o Planner con accesso amministrativo a ruoli, vedere <a href="#standard-or-planner-users-with-administrative-access-to-job-roles">Utenti Standard o Planner con accesso amministrativo a ruoli</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Milestone nel mio gruppo</td> 
      <td>Visualizza tutti i percorsi milestone nel sistema nel menu Percorsi milestone in Configurazione. Gli utenti possono anche modificare o eliminare qualsiasi percorso milestone appartenente a uno qualsiasi dei loro gruppi. Gli utenti non possono gestire (modificare o eliminare) percorsi milestone non assegnati al proprio gruppo di gruppi.<p>Senza questo accesso, gli utenti possono solo visualizzare i percorsi milestone esistenti e applicarli ai progetti che hanno accesso per gestire.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche promemoria</td> 
      <td>Crea e gestisci le notifiche dei promemoria in Workfront.<p>Senza questo accesso, gli utenti possono solo ricevere e visualizzare le notifiche.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schede orario e ore</td> 
      <td> Gli amministratori di gruppi possono assegnare profili di schede orario agli utenti dei gruppi e dei sottogruppi che gestiscono. <p>Se questa opzione non è abilitata, gli amministratori di gruppi non possono assegnare profili di schede orario ad altri utenti nei gruppi e nei sottogruppi che gestiscono, anche se possono crearli.</p> <p>Tutti gli altri utenti con una licenza Standard o Plan possono visualizzare tutte le ore e le schede orario in Workfront.</p> <p>Se questa opzione non è abilitata, gli utenti possono visualizzare le ore solo per:</p> 
       <ul> 
        <li>Progetti, attività o problemi che gestiscono</li> 
        <li>Scheda orario personale</li> 
        <li>Una scheda orario di qualcuno che fa riferimento a loro</li> 
        <li>Una scheda orario da approvare</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Imposta restrizioni aggiuntive**, quindi imposta una delle seguenti restrizioni per il livello di accesso.

   >[!IMPORTANT]
   >
   >Per gli utenti esterni, ad esempio i fornitori (che non fanno parte dell’organizzazione), consigliamo di limitare l’accesso ad attività, progetti, aggiornamenti, annunci, altre società, team e gruppi.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Non riconoscere mai l'accesso all'intero progetto quando assegnato a un'attività o a un problema</td> 
      <td> Impedisce agli utenti assegnati ad attività o problemi di ottenere autorizzazioni anche per il progetto principale, anche se le autorizzazioni del progetto lo consentono.<p>Per ulteriori informazioni sulla configurazione delle autorizzazioni per un progetto, vedere la sezione <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> nell'articolo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Modifica progetti</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Non ereditare l'accesso ai documenti da progetti. attività, problemi, ecc...</td> 
      <td>Impedisce ai documenti di ereditare le autorizzazioni impostate sull'oggetto padre.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizza solo gli aggiornamenti in cui sono stati inclusi nella conversazione</td> 
      <td> Consente agli utenti di visualizzare solo i commenti in cui è stato incluso il loro nome o il nome del team. <p> <p><b>NOTA</b>: questo impedisce agli utenti di sottoscrivere elementi in Workfront. Per ulteriori informazioni sulla sottoscrizione agli elementi, vedere <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Sottoscrizione agli elementi in Adobe Workfront</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Non consentire mai agli utenti di eliminare i commenti </td> 
      <td> Impedisce agli utenti di eliminare i commenti inseriti sugli elementi.  <p><b>NOTA</b>: nessuno può eliminare i commenti degli altri utenti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizza solo società, gruppi e team di appartenenza</td> 
      <td>Consente agli utenti di visualizzare e condividere gli elementi solo con le società, i gruppi e i team a cui appartengono.<p><strong>NOTA</strong>: gli utenti con licenze Requestor o Contributor non possono visualizzare le società a cui non appartengono, anche se questa opzione è selezionata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Non consentire mai la visualizzazione delle ore pianificate o delle ore effettive</td> 
      <td>Impedisce agli utenti di visualizzare le ore pianificate e effettive degli elementi di lavoro a cui hanno accesso. Tuttavia, possono visualizzare le ore effettive registrate personalmente o le ore registrate da qualcuno che fa riferimento a loro.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Non consentire mai agli utenti di eliminare le notifiche</td> 
      <td>Impedisce agli utenti di eliminare gli annunci nel Centro notifiche. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Inviare annunci</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Condizionale e facoltativo) Se il sistema Workfront è configurato per utenti che appartengono a più società, limita la visibilità ad altri utenti in base alla società a cui appartengono nella sezione **Le persone in altre società devono visualizzare solo gli utenti di**.

   Puoi limitare la visualizzazione degli utenti alla sola società di appartenenza o a quella indicata come società principale. L’azienda principale in genere rappresenta l’account Workfront dove lavora la maggior parte degli utenti. Per ulteriori informazioni sulla società principale, vedere [Creare e modificare società](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >Se due utenti appartengono a due società diverse, ma possono entrambi vedere gli utenti della società principale, possono visualizzare l’area Aggiornamenti associata alla società principale.

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configura l&#39;accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), ad esempio [Concedi l&#39;accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedi l&#39;accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Fai clic su **Salva**.

   Dopo aver creato il livello di accesso, è possibile assegnarlo a un utente (a meno che non si tratti di un livello di accesso Amministratore di sistema).

   Per ulteriori informazioni, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   Per informazioni su come un amministratore di Adobe assegna un livello di accesso Amministratore di sistema a un utente, vedere [Concedere a un utente l&#39;accesso amministrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Utenti Standard o Planner con accesso amministrativo alle mansioni {#planner-users}

Se si concede a un utente Standard o Planner l&#39;accesso amministrativo alle mansioni, l&#39;impostazione Modifica fatturazione mansione e tassi di costo viene abilitata automaticamente per l&#39;utente.

Successivamente, se si disabilita l&#39;accesso amministrativo alle mansioni per l&#39;utente, le mansioni saranno ancora visibili perché l&#39;impostazione Modifica fatturazione mansione e tassi di costo è ancora abilitata.

Se ciò accade e devi rimuovere l’accesso dell’utente per visualizzare le mansioni, devi disabilitare l’impostazione di autorizzazione Modifica fatturazione mansione e tassi di costo dell’utente. Per istruzioni, vedere [Concedere l&#39;accesso ai dati finanziari](grant-access-financial.md).



