---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Collega elementi tra [!DNL Adobe Workfront] e [!DNL Jira]
description: Puoi collegare [!DNL Jira] problemi alle [!DNL Adobe Workfront] attività o problemi in modo automatico o manuale.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '1378'
ht-degree: 1%

---

# Collega elementi tra [!DNL Adobe Workfront] e [!DNL Jira]

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>Per offrire integrazioni più stabili e scalabili, stiamo passando a un approccio di integrazione moderno e flessibile che utilizza l’automazione e l’integrazione di Workfront (Fusion). Nell&#39;ambito di questo processo di transizione, l&#39;integrazione Workfront for Jira non sarà disponibile dopo il **28 febbraio 2026**.
>
>È consigliabile utilizzare l’automazione e l’integrazione di Workfront per le esigenze di integrazione della tua organizzazione con Jira.
>
>Per una panoramica dell&#39;automazione e dell&#39;integrazione di Workfront, vedere [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Per informazioni sulle funzionalità specifiche dei moduli di automazione e integrazione di Workfront per Jira, vedere [Moduli software Jira](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

È possibile collegare [!DNL Jira] problemi ad attività o problemi [!DNL Adobe Workfront] in modo automatico o manuale.

È possibile collegare un solo elemento in [!DNL Workfront] a un elemento in [!DNL Jira]. Non puoi collegare un elemento [!DNL Workfront] a più problemi [!DNL Jira], né un problema [!DNL Jira] a più elementi [!DNL Workfront].

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Standard </p>
       <p>Piano </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Accesso Jira</td> 
   <td> <p>Accesso amministratore di sistema</p> <p>Importante: è consigliabile creare account amministratore di sistema separati in Jira e Workfront per dedicarsi a questa integrazione, anziché utilizzare account esistenti che potrebbero essere collegati agli utenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Installa [!DNL Workfront] per [!DNL Jira]

L&#39;installazione di [!DNL Workfront] per [!DNL Jira] OnDemand è identica all&#39;installazione in un&#39;istanza del server [!DNL Jira].

Per installare il componente aggiuntivo [!DNL Jira] è necessario essere un amministratore [!DNL Workfront].

Se non sei un amministratore di [!DNL Jira], puoi cercare il componente aggiuntivo [!DNL Workfront] e richiederne l&#39;installazione. La richiesta viene inviata all&#39;amministratore [!DNL Jira] per l&#39;approvazione e l&#39;installazione.

Per ulteriori informazioni sulla richiesta di installazione di un componente aggiuntivo nell&#39;applicazione [!DNL Jira], vedere [Gestione delle richieste degli utenti per i componenti aggiuntivi.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Per installare [!DNL Workfront for Jira]:

1. Accedere a [!DNL Jira] come amministratore [!DNL Jira].
1. Trovare il componente aggiuntivo **[!DNL Workfront for Jira]** in [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview).

1. Fai clic su **[!UICONTROL Ottienila ora]** per installarla.

   Al termine dell&#39;installazione, è possibile accedere a [!DNL Workfront] da [!DNL Jira] e configurare l&#39;integrazione.

   Per ulteriori informazioni, vedere [Configurare Adobe Workfront per Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Prerequisiti

Prima di collegare gli elementi tra [!DNL Workfront] e [!DNL Jira], è necessario effettuare le seguenti operazioni:

* Installa [!DNL Workfront] per [!DNL Jira].

  Per istruzioni, consulta [Installare Adobe Workfront per Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configura [!DNL Workfront] per Jira.

  Per istruzioni, consulta [Configurare Adobe Workfront per Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Collega automaticamente [!DNL Workfront] elementi a [!DNL Jira] problemi

In qualità di amministratore [!DNL Workfront], puoi definire trigger che creeranno automaticamente un problema in [!DNL Jira] ogni volta che vengono soddisfatte determinate condizioni su un&#39;attività o un problema in [!DNL Workfront]. Gli elementi Workfront e [!DNL Jira] diventano collegati.

Dopo aver completato la configurazione di [!DNL Workfront] per Jira, quando un elemento viene creato o aggiornato in [!DNL Workfront] in base ai trigger, in [!DNL Jira] viene creato automaticamente un nuovo elemento.

Gli utenti di Workfront che creano e aggiornano elementi di Workfront non hanno bisogno di una licenza [!DNL Jira] per attivare la creazione di elementi in [!DNL Jira].

Per ulteriori informazioni, vedere [Configurazione [!DNL Adobe Workfront] per Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Puoi creare [!DNL Jira] elementi automaticamente allegando un modello a un progetto. Se il modello contiene attività con assegnazioni che soddisfano i trigger [!DNL Jira], le nuove attività generano nuovi [!DNL Jira] problemi.

Il collegamento automatico di un problema [!DNL Workfront] a un problema [!DNL Jira] è identico al collegamento automatico di un&#39;attività [!DNL Workfront] a un problema [!DNL Jira].

Per collegare automaticamente un&#39;attività [!DNL Workfront] a un problema [!DNL Jira]:

1. Assicurati che il tuo amministratore di sistema [!DNL Jira] abbia configurato i trigger per la creazione automatica di [!DNL Jira] problemi quando vengono assegnati [!DNL Workfront] elementi, quindi accedi a [!DNL Workfront] con un livello di accesso che ti consenta di creare un&#39;attività.

   Per ulteriori informazioni sull&#39;accesso alle attività, vedere [Concedere l&#39;accesso alle attività](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

{{step1-to-projects}}

1. Nella pagina **Progetti**, seleziona un progetto.

1. Nel pannello sinistro del progetto, seleziona **[!UICONTROL Attività]**.

1. Fare clic su **+ Nuova attività**.

   >[!NOTE]
   >
   >Per collegare un elemento di Workfront esistente a un problema Jira, seleziona **Modifica** dal menu dell&#39;elemento **Altro** ![Icona altro](assets/more-icon.png).

1. Specificare o aggiornare uno dei campi disponibili per l&#39;attività.
1. Nel campo **[!UICONTROL Assegnazioni]**, cercare e selezionare l&#39;utente, la mansione o il team specificato come trigger nell&#39;integrazione [!DNL Jira].

1. Fai clic su **Crea attività**. L&#39;attività viene creata in Workfront e nella scheda **Aggiornamenti** dell&#39;attività viene visualizzato un nuovo commento per indicare che è stato creato un nuovo problema anche in [!DNL Jira].

1. (Facoltativo) Nell&#39;area **[!UICONTROL Integrazioni]** della sezione **[!UICONTROL Dettagli]** dell&#39;intestazione dell&#39;attività o del problema, fai clic sul collegamento **[!UICONTROL Vai a Jira]** per aprire il problema in Jira.

   L&#39;amministratore del sistema o del gruppo deve aggiungere il campo [!UICONTROL Integrazioni] al modello di layout per visualizzarlo nell&#39;intestazione dell&#39;attività o del problema. Per informazioni, vedere [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Qualsiasi utente di [!DNL Jira] può iniziare immediatamente a lavorare sugli elementi creati automaticamente da [!DNL Workfront] e i relativi aggiornamenti verranno trasferiti a [!DNL Workfront] senza richiedere una licenza per [!DNL Workfront].

   Vengono aggiornati solo i campi configurati come amministratore [!DNL Workfront] durante la configurazione del componente aggiuntivo [!DNL Workfront].

   Per ulteriori informazioni sulla sincronizzazione dei campi tra Workfront e Jira, consulta la sezione Configurare Workfront per Jira in [Configurare Adobe Workfront per Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >Il problema [!DNL Jira] non viene assegnato a nessuno in [!DNL Jira] quando viene creato automaticamente da Workfront.

## Collega manualmente [!DNL Jira] problemi a [!DNL Workfront] elementi

Dopo aver creato gli elementi in [!DNL Jira] e [!DNL Workfront] in modo indipendente l&#39;uno dall&#39;altro, è possibile collegare manualmente un problema di [!DNL Jira] a un&#39;attività o a un problema di [!DNL Workfront] esistente.

Impossibile collegare manualmente un elemento [!DNL Workfront] da [!DNL Workfront] a un elemento [!DNL Jira] esistente.

>[!NOTE]
>
>Se il problema [!DNL Jira] non si trova in un progetto non identificato come attivatore nell&#39;integrazione [!DNL Workfront], non è possibile collegarlo manualmente a un elemento di Workfront quando si utilizza l&#39;integrazione con [!DNL Jira] On-Premise.\
>Per ulteriori informazioni sulla configurazione dei trigger per il flusso di lavoro da Workfront a Jira, vedi [Collegare automaticamente gli elementi di Workfront ai problemi Jira](#automatically-link-workfront-items-to-jira-issues).

Quando [!DNL Workfront] e [!DNL Jira] elementi sono collegati, alcuni campi di un elemento possono essere aggiornati automaticamente sull&#39;altro.\
Per ulteriori informazioni sull&#39;aggiornamento degli elementi collegati, vedere [Aggiorna elementi collegati tra Jira e Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

Per collegare manualmente [!DNL Jira] problemi a [!DNL Workfront] elementi:

1. (Facoltativo) Accedi a [!DNL Workfront] e trova un problema o un&#39;attività da collegare a un problema di [!DNL Jira].
1. (Condizionale) Nella sezione **Informazioni di base** della scheda **Dettagli attività** o **Dettagli problema**, copia il **[!UICONTROL Numero di riferimento]** dell&#39;elemento in Workfront.

   Oppure

   Dalla barra degli indirizzi dell&#39;elemento, copia **URL** dell&#39;elemento in Workfront.

   >[!IMPORTANT]
   >
   >Se la tua organizzazione è stata integrata in Adobe Unified Experience, devi utilizzare il **Numero di riferimento** per collegare elementi Workfront a Jira. L’opzione URL è disponibile, ma se utilizzi restituirà un errore. Per informazioni sull&#39;esperienza unificata, vedere [Esperienza unificata Adobe per Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
   >
   >Per le organizzazioni che non utilizzano Adobe Unified Experience, non è consigliabile utilizzare l’opzione URL perché gli URL possono cambiare.

   >[!NOTE]
   >
   >Per accedere a [!DNL Workfront] è necessario disporre di una licenza [!DNL Workfront]. In caso contrario, è necessario che un utente di [!DNL Workfront] fornisca queste informazioni.

1. In [!DNL Jira], individuare un problema che si desidera collegare manualmente all&#39;elemento [!DNL Workfront].
1. Nel pannello di destra [!DNL Workfront], incolla il **[!UICONTROL Numero di riferimento]** o il **URL** dell&#39;elemento [!DNL Workfront] a cui vuoi collegarlo.

1. Fai clic su **[!UICONTROL Collegamento]**. I due elementi vengono collegati e il pannello destro [!DNL Workfront] viene compilato con le informazioni dell&#39;elemento [!DNL Workfront].

   Per impostazione predefinita, i seguenti campi [!DNL Workfront] sono visibili in [!DNL Jira] nel pannello destro [!DNL Workfront]:

   * Il **[!UICONTROL Nome]** dell&#39;elemento. Puoi accedere all&#39;elemento [!DNL Workfront] facendo clic sul nome nel pannello.
   * Il **[!UICONTROL Nome Progetto]**.
   * **[!UICONTROL Stato]** dell&#39;elemento.
   * **[!UICONTROL Priorità]** dell&#39;elemento.
   * Data di creazione in [!DNL Workfront].
   * Le **[!UICONTROL ore pianificate]** dell&#39;elemento.
   * Il **[!UICONTROL Numero Di Riferimento]**. Puoi accedere all&#39;elemento [!DNL Workfront] facendo clic sul **Numero di riferimento** nel pannello.

   Per ulteriori informazioni sull&#39;abilitazione della visualizzazione di campi aggiuntivi nel pannello di destra, vedere la sezione Configurare la sincronizzazione dei campi tra [!DNL Jira] e [!DNL Workfront] elementi in [Configurazione [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). Un commento dell&#39;amministratore [!DNL Workfront] associato all&#39;integrazione è pubblicato nella scheda **[!DNL Workfront]** del problema [!DNL Jira] per confermare che è stato creato un nuovo elemento [!DNL Jira]. Il commento contiene un collegamento al problema [!DNL Jira].

## Scollega elementi tra [!DNL Jira] e [!DNL Workfront]

Gli elementi collegati tra [!DNL Jira] e [!DNL Workfront] possono essere scollegati manualmente in [!DNL Jira]. Impossibile scollegare un elemento [!DNL Workfront] dalla controparte [!DNL Jira] in [!DNL Workfront].

Per scollegare manualmente un elemento è necessario disporre del seguente accesso:

* Sei l’utente che ha collegato manualmente gli elementi.
* Sei l&#39;amministratore di sistema [!DNL Jira].

>[!NOTE]
>
>Solo un amministratore [!DNL Workfront] può scollegare gli elementi collegati automaticamente.

Per scollegare un problema di [!DNL Jira] da un elemento di [!DNL Workfront]:

1. Accedi a Jira.
1. Passare al problema collegato a un&#39;attività o a un problema [!DNL Workfront].
1. Passa al pannello destro **Workfront**.
1. Fai clic sull&#39;icona **[!UICONTROL Scollega]**, quindi su **[!UICONTROL Scollega]**. Scollega gli elementi [!DNL Jira] e [!DNL Workfront] precedentemente collegati.

   I campi, i commenti o i documenti aggiornati in futuro non verranno aggiornati rispetto alla controparte precedente nell&#39;altra applicazione.
