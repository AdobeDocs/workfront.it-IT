---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Panoramica di Adobe Workfront per Salesforce
description: Puoi installare  [!DNL Adobe Workfront] per Salesforce per consentire agli utenti di Salesforce di inviare [!DNL Workfront] richieste e creare automaticamente progetti senza mai uscire da Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---

# Panoramica di [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>Per offrire integrazioni più stabili e scalabili, stiamo passando a un approccio di integrazione moderno e flessibile che utilizza l’automazione e l’integrazione di Workfront (Fusion). Come parte di questo processo di transizione, l&#39;integrazione di Workfront for Salesforce non sarà disponibile dopo il **28 febbraio 2026**.
>
>È consigliabile utilizzare l’automazione e l’integrazione di Workfront per le esigenze di integrazione della tua organizzazione con Salesforce.
>
>Per una panoramica dell&#39;automazione e dell&#39;integrazione di Workfront, vedere [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Per informazioni sulle funzionalità specifiche dei moduli di automazione e integrazione di Workfront per Salesforce, vedere [Moduli Salesforce](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

È possibile installare [!DNL Adobe Workfront for Salesforce] per consentire agli utenti di [!DNL Salesforce] di inviare [!DNL Workfront] richieste e creare automaticamente progetti senza mai uscire da [!DNL Salesforce].

In qualità di amministratore di [!DNL Workfront], puoi scaricare e configurare [!DNL Workfront for Salesforce]. Potrai quindi condividerlo con tutti gli altri [!DNL Salesforce] utenti.

Per ulteriori informazioni sull&#39;installazione di [!DNL Workfront for Salesforce], vedere [Installa [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Per ulteriori informazioni sulla configurazione della sezione [!DNL Workfront] in [!DNL Salesforce] per tutti gli utenti, vedere [Configurare la sezione  [!DNL Adobe Workfront] per [!DNL Salesforce] utenti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

>[!NOTE]
>
>Per utilizzare questa funzionalità è necessario un piano [!UICONTROL Pro] [!DNL Workfront]. Per ulteriori informazioni sui vari piani disponibili, vedere [[!DNL Workfront] Piani.](https://business.adobe.com/it/products/workfront/pricing.html)

## Requisiti di accesso

Per utilizzare le funzionalità descritte in questo articolo, è necessario disporre dei seguenti diritti di accesso:

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td> <p>[!UICONTROL Pro] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> <p>Nuovo: Standard<p>
   <p>Oppure</p>
   <p>Corrente: Piano</p>


</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## [!DNL Workfront for Salesforce]

Quando si utilizza [!DNL Workfront for Salesforce], è possibile effettuare le seguenti operazioni:

* Crea manualmente nuove richieste [!DNL Workfront] da [!DNL Salesforce] in un&#39;opportunità o in un account.

  Per ulteriori informazioni, vedere [Invia [!DNL Adobe Workfront] richieste da [!DNL Salesforce] oggetti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Attiva automaticamente la creazione di progetti in [!DNL Workfront] quando vengono soddisfatti determinati criteri in [!DNL Salesforce]. L&#39;amministratore di sistema [!DNL Salesforce] deve configurare i trigger per la creazione di progetti da [!DNL Salesforce].

  Per ulteriori informazioni sulla creazione di [!DNL Workfront] progetti da [!DNL Salesforce], vedere [Crea [!DNL Adobe Workfront] progetti da [!DNL Salesforce] oggetti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Quando si lavora con [!DNL Workfront] per [!DNL Salesforce], tenere presente quanto segue:

* Supportiamo entrambi i framework [!DNL Salesforce Classic] e [!DNL Lightning Experience].
* È possibile creare elementi solo da [!DNL Salesforce] a [!DNL Workfront].
* È possibile visualizzare alcune informazioni sugli elementi [!DNL Workfront] in [!DNL Salesforce]. Queste informazioni non possono essere personalizzate.

  Per un elenco di [!DNL Workfront] campi visualizzabili da [!DNL Salesforce], vedi [Invia [!DNL Adobe Workfront] richieste da [!DNL Salesforce] oggetti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md) e [Crea [!DNL Adobe Workfront] progetti da [!DNL Salesforce] oggetti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Puoi accedere direttamente agli elementi collegati a [!DNL Salesforce] facendo clic sul collegamento [!UICONTROL Vai a Salesforce] da Workfront.

  Non è possibile visualizzare informazioni sugli elementi [!DNL Salesforce] in [!DNL Workfront], ma in Workfront è presente un collegamento che consente di accedere all&#39;elemento in Salesforce in modo da poterlo esaminare.

  [!UICONTROL Il collegamento Vai a Salesforce] viene visualizzato nelle seguenti aree:

   * La sezione [!UICONTROL Dettagli] di un progetto o di un problema.
   * L’intestazione di un progetto o di un problema.

     L&#39;amministratore del sistema o del gruppo deve aggiungere il campo [!UICONTROL Integrazioni] al modello di layout per visualizzare il collegamento [!UICONTROL Vai a Salesforce] nell&#39;intestazione del progetto o del problema.
   * Pannello [!DNL Summary] di un problema durante la selezione del problema in un elenco, dopo aver fatto clic sull&#39;icona del pannello [!UICONTROL Apri riepilogo] ![Riepilogo](assets/summary-panel-icon.png) nella barra degli strumenti dell&#39;elenco.

     >[!NOTE]
     >
     >Il collegamento [!UICONTROL Vai a Salesforce] è visibile a tutti gli utenti [!DNL Workfront] che possono visualizzare il progetto o il problema. È necessario disporre di un account [!DNL Salesforce] per poter accedere all&#39;opportunità [!DNL Salesforce] o all&#39;account in cui è stato registrato il problema.

* L&#39;aggiornamento dei campi su un elemento in un&#39;applicazione non aggiorna le informazioni sugli elementi collegati nell&#39;altra applicazione.
