---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Installa [!DNL Adobe Workfront] per [!DNL Jira]
description: È possibile utilizzare [!DNL Adobe Workfront] per [!DNL Jira] per integrare [!DNL Jira] e [!DNL Workfront] sistemi.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Installa [!DNL Adobe Workfront for Jira]

È possibile utilizzare [!DNL Adobe Workfront for Jira] per integrare [!DNL Jira] e [!DNL Workfront] sistemi.

Dopo aver installato il componente aggiuntivo, puoi definire i flussi di lavoro che creano [!DNL Jira] si verifica automaticamente quando [!DNL Workfront] gli elementi di lavoro vengono creati. Gli elementi di entrambe le applicazioni vengono collegati e alcune delle relative informazioni possono essere aggiornate automaticamente in entrambi i sistemi.

Tutti gli utenti in [!DNL Workfront] e [!DNL Jira] può trarre vantaggio da questa integrazione. Hanno solo bisogno di una licenza per il sistema in cui funzionano di più, e non per entrambi i sistemi.

Questo componente aggiuntivo è disponibile per il [!UICONTROL Server] e [!UICONTROL OnDemand] o [!UICONTROL Cloud]) versioni di [!DNL Jira] Software. Questo componente aggiuntivo non è disponibile per il [!DNL Data Center] versione di [!DNL Jira] Software.

Per un elenco di [!DNL Jira] versioni [!DNL Workfront for Jira] supporta attualmente, vedi [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) al mercato Atlassian.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] piano</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] panoramica delle licenze</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] accesso</td> 
   <td> <p>Accesso amministratore di sistema</p> <p>Importante: È consigliabile creare account di amministratore di sistema separati in [!DNL Jira] e [!DNL Workfront] per dedicare a questa integrazione, anziché utilizzare quelle esistenti che potrebbero essere collegate agli utenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Installa [!DNL Workfront] per [!DNL Jira]

Installazione [!DNL Workfront] per [!DNL Jira] OnDemand è identico all’installazione su un [!DNL Jira] Istanza del server.

Devi essere un [!DNL Jira] l&#39;amministratore deve installare [!DNL Workfront] add-on.

Se non sei un [!DNL Jira] amministratore, puoi cercare [!DNL Workfront] add-on e richiedi l&#39;installazione. La richiesta viene inviata al [!DNL Jira] amministratore per l&#39;approvazione e l&#39;installazione.

Per ulteriori informazioni sulla richiesta di un componente aggiuntivo da installare nel [!DNL Jira] applicazione, vedi [Gestione delle richieste degli utenti per i componenti aggiuntivi.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Per installare [!DNL Workfront for Jira]:

1. Accedi a [!DNL Jira] come [!DNL Jira] amministratore.
1. Trova il **[!DNL Workfront for Jira]** componente aggiuntivo nel [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. Fai clic su **[!UICONTROL Scarica subito]** per installarlo.

   Al termine dell’installazione, puoi accedere a [!DNL Workfront] da [!DNL Jira] e configura l’integrazione.
   [!DNL ]
Per ulteriori informazioni, consulta [Configurare Adobe Workfront per Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Considerazioni per un [!DNL Jira Server] installazione

>[!NOTE]
>
>Questi requisiti non si applicano al [!UICONTROL OnDemand] ([!UICONTROL Cloud]) versione di [!DNL Jira] Software.

Anche se si installa [!DNL Workfront] componente aggiuntivo nei due [!DNL Jira] ambienti simili, è necessario tenere presente quanto segue quando si lavora con un [!DNL Jira Server] installazione:

* Durante la configurazione del componente aggiuntivo in [!DNL Jira], l&#39;indirizzo specificato nel **[!DNL JIRA Base URL]** Il campo potrebbe non essere lo stesso URL utilizzato per accedere [!DNL Jira] sul server privato. La **[!DNL JIRA Base URL]** deve essere un indirizzo accessibile al pubblico connesso al server privato utilizzando protocolli NAT o reverse proxy, in modo che [!DNL Workfront] può accedervi per effettuare richieste al server.

* Per proteggere la comunicazione tra [!DNL Jira] e [!DNL Workfront]. Quando abiliti SSL, devi disporre di uno stack di certificati SSL completo da un’autorità di certificazione. Non sono supportati i certificati autofirmati.
* È necessario assicurarsi che il [!DNL jira.workfront.com] Il dominio è accessibile dai server aziendali. Funge da ambiente middleware tra [!DNL Workfront] e [!DNL Jira] ed è necessario per il funzionamento del componente aggiuntivo.

   È inoltre necessario aggiungere i seguenti indirizzi IP statici all’inserire nell&#39;elenco Consentiti sul firewall per le connessioni in uscita e in entrata.

   `35.162.128.73`

   `34.213.36.118`

   `35.160.0.242`

   `3.209.27.146`

   `18.205.251.4`

   Per ulteriori informazioni sulla configurazione del firewall per funzionalità ottimali con [!DNL Workfront], vedi [Configurazione del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
