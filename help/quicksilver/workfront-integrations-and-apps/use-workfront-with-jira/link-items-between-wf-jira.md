---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Collega elementi tra [!DNL Adobe Workfront] e [!DNL Jira]
description: Puoi collegare [!DNL Jira] problemi alle [!DNL Adobe Workfront] attività o problemi in modo automatico o manuale.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1231'
ht-degree: 0%

---

# Collega elementi tra [!DNL Adobe Workfront] e [!DNL Jira]

È possibile collegare [!DNL Jira] problemi ad attività o problemi [!DNL Adobe Workfront] in modo automatico o manuale.

È possibile collegare un solo elemento in [!DNL Workfront] a un elemento in [!DNL Jira]. Non puoi collegare un elemento [!DNL Workfront] a più problemi [!DNL Jira], né un problema [!DNL Jira] a più elementi [!DNL Workfront].

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] piano]</a>*</td> 
   <td> <p>[!UICONTROL Pro] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica delle licenze di Adobe [!DNL Workfront]</a>*</td> 
   <td> <p>Piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Accesso Jira</td> 
   <td> <p>Accesso amministratore di sistema</p> <p><b>IMPORTANTE</b>

È consigliabile creare account di amministratore di sistema separati in [!DNL Jira] e [!DNL Workfront] per dedicarsi a questa integrazione, anziché utilizzare account esistenti che potrebbero essere collegati agli utenti.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Devi essere un amministratore [!DNL Workfront]. Per informazioni sugli amministratori di [!DNL Workfront], vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> <p><b>NOTA</b>

Se non disponi ancora dell&#39;accesso, chiedi all&#39;amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## Prerequisiti

Prima di collegare gli elementi tra [!DNL Workfront] e [!DNL Jira], è necessario

* Installa [!DNL Workfront] per [!DNL Jira]

  Per istruzioni sull&#39;installazione di Workfront per Jira, vedere [Installare Adobe Workfront per Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configura [!DNL Workfront] per Jira

  Per istruzioni sulla configurazione di Workfront per Jira, consulta [Configurare Adobe Workfront per Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Collega automaticamente [!DNL Workfront] elementi a [!DNL Jira] problemi

In qualità di amministratore [!DNL Workfront], puoi definire trigger che possono creare automaticamente un problema in [!DNL Jira] ogni volta che vengono soddisfatte determinate condizioni su un&#39;attività o un problema in [!DNL Workfront]. Gli elementi Workfront e [!DNL Jira] diventano collegati.

Dopo aver completato la configurazione di [!DNL Workfront] per Jira, quando un elemento viene creato o aggiornato in [!DNL Workfront] in base ai trigger, in [!DNL Jira] viene creato automaticamente un nuovo elemento.\
Gli utenti di Workfront che creano e aggiornano elementi di Workfront non hanno bisogno di una licenza [!DNL Jira] per attivare la creazione di elementi in [!DNL Jira].

Per ulteriori informazioni sulla definizione dei trigger per la creazione automatica dei problemi Jira, vedi [Configurazione [!DNL Adobe Workfront] per Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Puoi creare [!DNL Jira] elementi automaticamente allegando un modello a un progetto. Se il modello contiene attività con assegnazioni che soddisfano i trigger [!DNL Jira], le nuove attività generano nuovi [!DNL Jira] problemi.

Il collegamento automatico di un problema [!DNL Workfront] a un problema [!DNL Jira] è identico al collegamento automatico di un&#39;attività [!DNL Workfront] a un problema [!DNL Jira].

Per collegare automaticamente un&#39;attività [!DNL Workfront] a un problema [!DNL Jira]:

1. Assicurati che il tuo amministratore di sistema [!DNL Jira] abbia configurato i trigger per la creazione automatica di [!DNL Jira] problemi quando vengono assegnati [!DNL Workfront] elementi, quindi accedi a [!DNL Workfront] con un livello di accesso che ti consenta di creare un&#39;attività.

   Per ulteriori informazioni sull&#39;accesso alle attività, vedere [Concedere l&#39;accesso alle attività](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

1. Vai a un progetto e seleziona **[!UICONTROL Attività]** ![Attività icona](assets/tasks-icon-in-left-panel-14x14.png) nel pannello a sinistra.

1. Fai clic su **[!UICONTROL Nuova attività]**

   Oppure

   Seleziona un&#39;attività esistente, quindi fai clic su **Modifica**.

1. Specificare o aggiornare uno dei campi disponibili per l&#39;attività.
1. Fai clic su **[!UICONTROL Assegnazioni]** e assegna l&#39;attività a un utente, una mansione o un team specificato come attivatore nell&#39;integrazione [!DNL Jira].

1. Fai clic su **Salva modifiche**.

   In Workfront viene creata una nuova attività.

   Nell&#39;area **[!UICONTROL Aggiornamenti]** della nuova attività è presente un commento per indicare che è stato creato un nuovo problema anche in [!DNL Jira].

1. (Facoltativo) Fai clic sul collegamento al problema Jira per aprirlo in Jira.

   Oppure

   Fai clic sul collegamento **[!UICONTROL Vai a Jira]** nell&#39;area **[!UICONTROL Integrazioni]** della sezione **[!UICONTROL Dettagli]** o nell&#39;intestazione dell&#39;attività o del problema, per aprire il problema [!DNL Jira].

   L&#39;amministratore del sistema o del gruppo deve aggiungere il campo [!UICONTROL Integrazioni] al modello di layout per visualizzarlo nell&#39;intestazione dell&#39;attività o del problema. Per informazioni, vedere [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Qualsiasi utente di [!DNL Jira] può iniziare immediatamente a lavorare sugli elementi creati automaticamente da [!DNL Workfront] e i relativi aggiornamenti verranno trasferiti a [!DNL Workfront] senza richiedere una licenza per [!DNL Workfront].

   Vengono aggiornati solo i campi configurati come amministratore [!DNL Workfront] durante la configurazione del componente aggiuntivo [!DNL Workfront].

   Per ulteriori informazioni sulla sincronizzazione dei campi tra Workfront e Jira, consulta la sezione [Configurare Workfront per Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira) in [Configurare Adobe Workfront per Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >Il problema [!DNL Jira] non è assegnato a nessuno in [!DNL Jira] quando viene creato automaticamente da Workfront.

## Collega manualmente [!DNL Jira] problemi a [!DNL Workfront] elementi

Dopo la creazione degli elementi in [!DNL Jira] e [!DNL Workfront], indipendentemente l&#39;uno dall&#39;altro, è possibile collegare manualmente un problema di [!DNL Jira] a un&#39;attività o a un problema di [!DNL Workfront] esistente.\
Impossibile collegare manualmente un elemento [!DNL Workfront] da [!DNL Workfront] a un elemento [!DNL Jira] esistente.

>[!NOTE]
>
>Se il problema [!DNL Jira] non si trova in un progetto non identificato come attivatore nell&#39;integrazione [!DNL Workfront], non è possibile collegarlo manualmente a un elemento di Workfront quando si utilizza l&#39;integrazione con [!DNL Jira] On-Premise.\
>Per ulteriori informazioni sulla configurazione dei trigger per il flusso di lavoro da Workfront a Jira, vedi [Collegare automaticamente gli elementi di Workfront ai problemi Jira](#automatically-link-workfront-items-to-jira-issues).

Quando [!DNL Workfront] e [!DNL Jira] elementi sono collegati, alcuni campi di un elemento possono essere aggiornati automaticamente sull&#39;altro.\
Per ulteriori informazioni sull&#39;aggiornamento degli elementi collegati, vedere [Aggiorna elementi collegati tra Jira e Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

Per collegare manualmente [!DNL Jira] problemi a [!DNL Workfront] elementi:

1. (Facoltativo) Accedi a [!DNL Workfront] e trova un problema o un&#39;attività da collegare al problema [!DNL Jira].
1. (Condizionale) Dall&#39;area [!UICONTROL Dettagli], copiare il **[!UICONTROL Numero di riferimento]** dell&#39;elemento in Workfront.

   Oppure

   Dalla barra degli indirizzi dell&#39;elemento, copia **URL** dell&#39;elemento in Workfront.

   >[!IMPORTANT]
   >
   >Se la tua organizzazione è stata integrata in Adobe Unified Experience, devi utilizzare il **Numero di riferimento** per collegare elementi Workfront a Jira. L’opzione URL è disponibile, ma se utilizzi restituirà un errore. Per informazioni sull&#39;esperienza unificata, vedere [Esperienza unificata Adobe per Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
   >
   >Per le organizzazioni che non utilizzano Adobe Unified Experience, non è consigliabile utilizzare l’opzione URL in quanto gli URL possono cambiare.

   >[!NOTE]
   >
   >Per accedere a [!DNL Workfront] è necessario disporre di una licenza [!DNL Workfront]. In caso contrario, è necessario che un utente di [!DNL Workfront] fornisca queste informazioni.

1. In [!DNL Jira], individuare un problema che si desidera collegare manualmente all&#39;elemento [!DNL Workfront].
1. Nel pannello di destra [!DNL Workfront], incolla il **[!UICONTROL Numero di riferimento]** o il **URL** dell&#39;elemento [!DNL Workfront] che desideri collegare.

1. Fai clic su **[!UICONTROL Collegamento]**.

   I due elementi vengono collegati e il pannello destro [!DNL Workfront] viene compilato con le informazioni dell&#39;elemento [!DNL Workfront].

   I seguenti campi [!DNL Workfront] sono visibili in [!DNL Jira], per impostazione predefinita, nel pannello destro [!DNL Workfront]:

   * **[!UICONTROL Nome]** dell&#39;elemento: è possibile accedere all&#39;elemento [!DNL Workfront] facendo clic sul nome nel pannello.
   * **[!UICONTROL Nome progetto]**
   * **[!UICONTROL Stato]** dell&#39;elemento
   * **[!UICONTROL Priorità]** dell&#39;elemento
   * Data di creazione in [!DNL Workfront]
   * Le **[!UICONTROL ore pianificate]** dell&#39;elemento
   * **[!UICONTROL Numero di riferimento]**: è possibile accedere all&#39;elemento [!DNL Workfront] facendo clic sul [!UICONTROL Numero di riferimento] nel pannello.

Per ulteriori informazioni sull&#39;abilitazione della visualizzazione di campi aggiuntivi nel pannello di destra, vedere [Configurare la sincronizzazione dei campi tra [!DNL Jira] e [!DNL Workfront] Elementi](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization) nella sezione [Configurare [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). Un commento dell&#39;amministratore [!DNL Workfront] associato all&#39;integrazione è pubblicato nella scheda **[!DNL Workfront]** del problema [!DNL Jira] per confermare che è stato creato un nuovo elemento [!DNL Jira]. Il commento contiene un collegamento al problema [!DNL Jira].

## Scollega elementi tra [!DNL Jira] e [!DNL Workfront]

Gli elementi collegati tra [!DNL Jira] e [!DNL Workfront] possono essere scollegati manualmente da [!DNL Jira].\
Impossibile scollegare un elemento [!DNL Workfront] dalla controparte [!DNL Jira] in [!DNL Workfront].

Per scollegare manualmente un elemento è necessario disporre del seguente accesso:

* Utente che ha collegato manualmente gli elementi
* Sei l&#39;amministratore di sistema [!DNL Jira]

Solo un amministratore [!DNL Workfront] può scollegare gli elementi collegati automaticamente.

Per scollegare un problema di [!DNL Jira] da un elemento di [!DNL Workfront]:

1. In [!DNL Jira], passare a un problema collegato a un&#39;attività o a un problema [!DNL Workfront].
1. Vai al pannello di destra [!DNL Workfront] e fai clic sull&#39;icona **[!UICONTROL Scollega]**, quindi fai clic su **[!UICONTROL Scollega]**.

   Gli elementi [!DNL Jira] e [!DNL Workfront] precedentemente collegati sono ora scollegati. Eventuali campi, commenti o documenti che potrebbero essere aggiornati singolarmente su di essi in futuro non vengono aggiornati sulla controparte precedente nell&#39;altra applicazione.
