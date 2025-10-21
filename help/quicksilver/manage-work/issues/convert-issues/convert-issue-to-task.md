---
product-area: projects
navigation-topic: convert-issues
title: Convertire un problema in un'attività
description: Se è necessario fare di più per completare un problema dopo l’invio del problema, puoi convertire il problema in un’attività in Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 1%

---

# Convertire un problema in un’attività

<!--Audited: 08/2025-->

Se è necessario fare di più per completare un problema dopo l’invio del problema, puoi convertire il problema in un’attività in Adobe Workfront.

Per informazioni generali sulla conversione dei problemi, vedere [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Lavoro o superiore</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Issues, Tasks, and Projects</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni per il problema</p> <p>Autorizzazioni per contribuire al progetto</p> <p>Ottieni le autorizzazioni di gestione per l’attività dopo la conversione del problema</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues, Tasks, and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the issue</p> <p>Contribute permissions to the project</p> <p>You obtain&nbsp;Manage permissions to the task after the issue is converted</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table> -->

## Considerazioni

* Quando si converte un problema in un’attività, è previsto un limite di elaborazione di 5 minuti. Se al problema è allegato un numero elevato di documenti e la conversione non riesce, potrebbe essere necessario rimuovere alcuni documenti e riprovare.

## Convertire un problema in un’attività

1. Vai a un progetto e fai clic su [!UICONTROL **Problemi**] nel pannello a sinistra.
1. Fai clic sul problema da convertire per passare alla pagina di destinazione del problema.
1. Fai clic sul menu [!UICONTROL **Altro**] sul problema, quindi [!UICONTROL **Converti in attività**].

   ![Menu Altro problema](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >Se il problema è associato a un processo di approvazione o è già associato a un oggetto di risoluzione, Workfront visualizza un avviso nella parte superiore della casella [!UICONTROL Converti in progetto] per avvisarti che l&#39;approvazione è stata rimossa o che l&#39;oggetto di risoluzione è stato sovrascritto durante la conversione. Per ulteriori informazioni, vedere [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Aggiorna il nome dell&#39;attività nella sezione [!UICONTROL Nome attività]. Per impostazione predefinita, il nome dell’attività corrisponde a quello del problema originale.

   ![Converti in casella attività](assets/convert-to-task-box-nwe.png)

1. Fai clic su [!UICONTROL **Progetto di destinazione**], quindi inizia a digitare il nome del progetto in cui desideri inserire la nuova attività nel campo [!UICONTROL **Progetto di destinazione**] e selezionalo quando viene visualizzato nell&#39;elenco. Il progetto del problema è selezionato per impostazione predefinita.

1. Fai clic su [!UICONTROL **Panoramica**], quindi digita una [!UICONTROL **Descrizione**] per l&#39;attività.

   >[!TIP]
   >
   >   Un amministratore di sistema o di gruppo può modificare l’ordine delle sezioni nel pannello a sinistra della casella di conversione modificando il modello di layout.

1. (Facoltativo e condizionale) Fare clic su [!UICONTROL **Opzioni**] e selezionare una delle opzioni seguenti.

   L’amministratore di Workfront o l’amministratore di gruppo deve abilitare queste preferenze prima che siano visibili durante la conversione dei problemi:

   * [!UICONTROL **Mantieni il problema originale e collegane la risoluzione all&#39;attività**]

     Se non è selezionata, il problema originale viene eliminato.

     >[!NOTE]
     >
     >Gli utenti che non dispongono dell’accesso o delle autorizzazioni necessarie per eliminare un problema non potranno eliminarlo mentre lo stanno convertendo, indipendentemente dallo stato di questa impostazione. Per informazioni sull’accesso e le autorizzazioni per i problemi, consulta:
     >   
     >   * [Concedi l&#39;accesso ai problemi](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     >   * [Condividi un problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)
     >   
     >

   * [!UICONTROL **Consenti a (Nome utente) di accedere a questa attività**]

     Se non è selezionata, il contatto principale del problema non ha accesso alla nuova attività.

   * [!UICONTROL **Mantieni la data di completamento pianificata del problema**]

     Se non è selezionata, la [!UICONTROL Data di completamento pianificata] della nuova attività viene calcolata a partire dalla [!UICONTROL Data di inizio pianificata] dell&#39;attività. La [!UICONTROL Data inizio pianificata] della nuova attività è impostata in base alle preferenze di sistema per le nuove attività.

     >[!NOTE]
     >
     >
     >Le opzioni visualizzate dipendono dalla configurazione effettuata dall&#39;amministratore di Workfront per tutti gli utenti del sistema. Per ulteriori informazioni, consulta [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >Oppure, se i gruppi di primo livello dell’organizzazione li hanno configurati separatamente, le opzioni visualizzate dipendono dal gruppo associato al progetto selezionato al passaggio 6. Per ulteriori informazioni, consulta [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. (Facoltativo) Fare clic su [!UICONTROL **Forms personalizzato**] e allegare un modulo personalizzato per la nuova attività.

   >[!TIP]
   >
   >* Se un modulo personalizzato con più oggetti allegato al problema è configurato per l’utilizzo sia con problemi che con attività, tutte le informazioni salvate nel modulo vengono mantenute quando si effettua la conversione, se i campi sono presenti sia sul problema che nei moduli personalizzati dell’attività.
   >* Se al problema e all’attività è allegato un modulo personalizzato con più oggetti con un campo calcolato, il problema e l’attività devono essere compatibili con tutti i campi a cui si fa riferimento nei campi personalizzati calcolati del modulo. In caso di incompatibilità, un messaggio ti avvisa di apportare le modifiche necessarie. Per ulteriori informazioni, vedere [Aggiungere campi calcolati a un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).
   >* Se nel progetto di destinazione sono definiti moduli predefiniti nel campo Forms personalizzato predefinito attività durante la modifica del progetto, anche tali moduli verranno aggiunti alla nuova attività. Eventuali campi personalizzati comuni tra il problema originale e i campi dei moduli attività predefiniti vengono precompilati con le informazioni dei campi del problema.


1. Fare clic su [!UICONTROL **Converti in attività**].

   Se hai deciso di eliminare il problema originale, il problema diventa un’attività del progetto designato.

   Oppure

   Il problema è ora collegato alla nuova attività sul progetto scelto e verrà completato al termine dell&#39;attività, se hai deciso di mantenere il problema originale.

   Alcuni campi del problema vengono trasferiti all’attività. Per informazioni, consulta la sezione [Visualizzare le informazioni originali sul problema su progetti e attività](#view-original-issue-information-on-projects-and-tasks) in questo articolo.

1. (Facoltativo) Continua a modificare l’attività secondo necessità.

## Visualizza le informazioni originali sul problema relative a progetti e attività {#view-original-issue-information-on-projects-and-tasks}

È possibile visualizzare le informazioni originali sul problema in elenchi e rapporti di progetti e attività o nell&#39;area Dettagli progetto. Per informazioni sulla creazione di report, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

La tabella seguente illustra quali campi dei problemi sono visibili dai progetti e dalle attività convertiti.

| Campi problema | Campo progetto o attività | Elenco o rapporto del progetto | Area Dettagli progetto | Elenco o rapporto attività | Area Dettagli attività |
|---|---|---|---|---|---|
| [!UICONTROL Nome problema] | [!UICONTROL Nome problema convertito] | ✔ | ✔ | ✔ | ✔ |
| [!UICONTROL Contatto principale] | [!UICONTROL Nome del mittente del problema convertito] | ✔ | ✔ | ✔ |  |
| [!UICONTROL Data di ingresso] | [!UICONTROL Data voce problema convertito] | ✔ |  | ✔ |  |


>[!CAUTION]
>
>Se il [!UICONTROL contatto principale] di un problema cambia o se il problema viene scollegato dal progetto o dall&#39;attività dopo la conversione del problema, il [!UICONTROL nome dell&#39;iniziatore del problema convertito]non viene aggiornato e visualizza il [!UICONTROL contatto principale] originale del problema al momento della conversione.
