---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Installa [!DNL Adobe Workfront] per [!DNL Jira]
description: Puoi utilizzare  [!DNL Adobe Workfront] for [!DNL Jira] per integrare i tuoi [!DNL Jira] e [!DNL Workfront] sistemi.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# Installa [!DNL Adobe Workfront for Jira]

>[!IMPORTANT]
>
>Per offrire integrazioni più stabili e scalabili, stiamo passando a un approccio di integrazione moderno e flessibile che utilizza l’automazione e l’integrazione di Workfront (Fusion). Nell&#39;ambito di questo processo di transizione, l&#39;integrazione Workfront for Jira non sarà disponibile dopo il **28 febbraio 2026**.
>
>È consigliabile utilizzare l’automazione e l’integrazione di Workfront per le esigenze di integrazione della tua organizzazione con Jira.
>
>Entro agosto saranno disponibili otto modelli di automazione e integrazione Workfront pronti all’uso per Jira, per consentire la replica dei flussi di lavoro comuni e accelerare l’implementazione. I modelli sono completamente personalizzabili per soddisfare specifiche esigenze aziendali e possono essere estesi in base all&#39;evoluzione dei requisiti.
> 
>Per una panoramica dell&#39;automazione e dell&#39;integrazione di Workfront, vedere [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Per informazioni sulle funzionalità specifiche dei moduli di automazione e integrazione di Workfront per Jira, vedere [Moduli software Jira](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

È possibile utilizzare [!DNL Adobe Workfront for Jira] per integrare i sistemi [!DNL Jira] e [!DNL Workfront].

Dopo aver installato il componente aggiuntivo, è possibile definire flussi di lavoro che creano automaticamente [!DNL Jira] problemi alla creazione di [!DNL Workfront] elementi di lavoro. Gli elementi di entrambe le applicazioni vengono collegati e alcune delle relative informazioni possono essere aggiornate automaticamente in entrambi i sistemi.

Tutti gli utenti in [!DNL Workfront] e [!DNL Jira] possono beneficiare di questa integrazione. È sufficiente una licenza per il sistema in cui operano maggiormente e non per entrambi i sistemi.

Questo componente aggiuntivo è disponibile per le versioni [!UICONTROL Server] e [!UICONTROL OnDemand] (o [!UICONTROL Cloud]) del software [!DNL Jira]. Questo componente aggiuntivo non è disponibile per la versione [!DNL Data Center] del software [!DNL Jira].

Per un elenco di [!DNL Jira] versioni attualmente supportate da [!DNL Workfront for Jira], vedere [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) nel Marketplace Atlassian.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td role="rowheader">Panoramica delle licenze di Adobe [!DNL Workfront]</td> 
   <td> 
   <p>Nuovo: Standard</p>
   <p>Corrente: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] accesso</td> 
   <td> <p>Accesso amministratore di sistema</p> <p>Importante: è consigliabile creare account di amministratore di sistema separati in [!DNL Jira] e [!DNL Workfront] per dedicarsi a questa integrazione, anziché utilizzare account esistenti che potrebbero essere collegati agli utenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td><p>Devi essere un amministratore [!DNL Workfront].</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

## Considerazioni per un&#39;installazione di [!DNL Jira Server]

>[!NOTE]
>
>Questi requisiti non si applicano alla versione [!UICONTROL OnDemand] ([!UICONTROL Cloud]) del software [!DNL Jira].

Sebbene l&#39;installazione del componente aggiuntivo [!DNL Workfront] nei due ambienti [!DNL Jira] sia simile, è necessario considerare quanto segue quando si lavora con un&#39;installazione di [!DNL Jira Server]:

* Durante la configurazione del componente aggiuntivo in [!DNL Jira], l&#39;indirizzo specificato nel campo **[!DNL JIRA Base URL]** potrebbe non essere lo stesso URL utilizzato per accedere a [!DNL Jira] sul server privato. **[!DNL JIRA Base URL]** deve essere un indirizzo accessibile al pubblico connesso al server privato tramite protocolli NAT o reverse proxy, in modo che [!DNL Workfront] possa accedervi per effettuare richieste al server.

* Utilizzare la crittografia SSL per proteggere la comunicazione tra [!DNL Jira] e [!DNL Workfront]. Quando abiliti SSL, devi disporre di uno stack di certificati SSL completo da un’autorità di certificazione. I certificati autofirmati non sono supportati.
* È necessario assicurarsi che il dominio [!DNL jira.workfront.com] sia accessibile dai server aziendali. Funge da ambiente middleware tra [!DNL Workfront] e [!DNL Jira] ed è necessario per il funzionamento del componente aggiuntivo.

  È inoltre necessario aggiungere i seguenti indirizzi IP statici al elenco Consentiti di accesso al firewall per le connessioni in uscita e in entrata.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  Per ulteriori informazioni sulla configurazione del firewall per una funzionalità ottimale con [!DNL Workfront], vedere [Configurazione del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
