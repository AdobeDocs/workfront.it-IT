---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Installa [!DNL Adobe Workfront] per [!DNL Jira]
description: È possibile utilizzare [!DNL Adobe Workfront] per [!DNL Jira] per integrare [!DNL Jira] e [!DNL Workfront] sistemi.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: b98a7fa48e60f1f2c2ea938b14b88e0c5a2ee418
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Installa [!DNL Adobe Workfront for Jira]

È possibile utilizzare [!DNL Adobe Workfront for Jira] per integrare [!DNL Jira] e [!DNL Workfront] sistemi.

Dopo aver installato il componente aggiuntivo, è possibile definire i flussi di lavoro che creano [!DNL Jira] problemi automaticamente quando [!DNL Workfront] vengono creati elementi di lavoro. Gli elementi di entrambe le applicazioni vengono collegati e alcune delle relative informazioni possono essere aggiornate automaticamente in entrambi i sistemi.

Tutti gli utenti in [!DNL Workfront] e [!DNL Jira] può trarre vantaggio da questa integrazione. È sufficiente una licenza per il sistema in cui operano maggiormente e non per entrambi i sistemi.

Questo componente aggiuntivo è disponibile per [!UICONTROL Server] e [!UICONTROL On demand] (o [!UICONTROL Cloud]) versioni di [!DNL Jira] Software. Questo componente aggiuntivo non è disponibile per [!DNL Data Center] versione di [!DNL Jira] Software.

Per un elenco di [!DNL Jira] versioni che [!DNL Workfront for Jira] attualmente supporta, vedi [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) nel Marketplace Atlassian.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td> 
   <p>Nuovo: Qualsiasi</p>
   <p>Corrente: [!UICONTROL Pro] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] panoramica sulle licenze</td> 
   <td> 
   <p>Nuovo: Standard</p>
   <p>Corrente: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] accesso</td> 
   <td> <p>Accesso amministratore di sistema</p> <p>Importante: è consigliabile creare account di amministratore di sistema separati in [!DNL Jira] e [!DNL Workfront] per dedicarsi a questa integrazione, anziché utilizzare quelle esistenti che potrebbero essere collegate agli utenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td><p>Devi essere un [!DNL Workfront] amministratore.</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Installa [!DNL Workfront] per [!DNL Jira]

Installazione [!DNL Workfront] per [!DNL Jira] OnDemand è identico all&#39;installazione su un [!DNL Jira] Istanza del server.

Devi essere un [!DNL Jira] l&#39;amministratore per installare [!DNL Workfront] componente aggiuntivo.

Se non sei un [!DNL Jira] amministratore, è possibile cercare [!DNL Workfront] e richiederne l&#39;installazione. La richiesta viene inviata al [!DNL Jira] per l&#39;approvazione e l&#39;installazione.

Per ulteriori informazioni sulla richiesta di installazione di un componente aggiuntivo nel [!DNL Jira] applicazione, vedi [Gestione delle richieste degli utenti di componenti aggiuntivi.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Per installare [!DNL Workfront for Jira]:

1. Accedi a [!DNL Jira] as a [!DNL Jira] amministratore.
1. Trova il **[!DNL Workfront for Jira]** componente aggiuntivo in [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. Clic **[!UICONTROL Ottieni subito]** per installarlo.

   Al termine dell’installazione, puoi accedere a [!DNL Workfront] da [!DNL Jira] e configurare l’integrazione.

   Per ulteriori informazioni, consulta [Configurare Adobe Workfront per Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Considerazioni per un [!DNL Jira Server] installazione

>[!NOTE]
>
>Questi requisiti non si applicano al [!UICONTROL On demand] ([!UICONTROL Cloud]) versione di [!DNL Jira] Software.

Anche se si installa [!DNL Workfront] componente aggiuntivo nei due [!DNL Jira] simili, quando si lavora con un [!DNL Jira Server] installazione:

* Configurazione del componente aggiuntivo in [!DNL Jira], l&#39;indirizzo specificato nella **[!DNL JIRA Base URL]** non può essere lo stesso URL utilizzato per accedere [!DNL Jira] sul server privato. Il **[!DNL JIRA Base URL]** deve essere un indirizzo accessibile al pubblico connesso al server privato utilizzando protocolli NAT o reverse proxy, in modo da [!DNL Workfront] può accedervi per effettuare richieste al server.

* È necessario utilizzare la crittografia SSL per proteggere la comunicazione tra [!DNL Jira] e [!DNL Workfront]. Quando abiliti SSL, devi disporre di uno stack di certificati SSL completo da un’autorità di certificazione. I certificati autofirmati non sono supportati.
* È necessario assicurarsi che [!DNL jira.workfront.com] è accessibile dai server aziendali. Funge da ambiente middleware tra [!DNL Workfront] e [!DNL Jira] ed è richiesto per il funzionamento del componente aggiuntivo.

  È inoltre necessario aggiungere i seguenti indirizzi IP statici al inserisco nell&#39;elenco Consentiti di sul firewall per le connessioni in uscita e in entrata.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  Per ulteriori informazioni sulla configurazione del firewall per ottenere funzionalità ottimali con [!DNL Workfront], vedi [Configurazione del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
