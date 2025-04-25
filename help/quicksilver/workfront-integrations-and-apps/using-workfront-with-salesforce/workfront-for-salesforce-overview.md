---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Panoramica di Adobe Workfront per Salesforce
description: Puoi installare  [!DNL Adobe Workfront] per Salesforce per consentire agli utenti di Salesforce di inviare [!DNL Workfront] richieste e creare automaticamente progetti senza mai uscire da Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Panoramica di [!DNL Adobe Workfront for Salesforce]

Per utilizzare questa funzionalità è necessario un piano [!UICONTROL Pro] [!DNL Workfront]. Per ulteriori informazioni sui vari piani disponibili, vedere [[!DNL Workfront] Piani.](https://business.adobe.com/products/workfront/pricing.html)

È possibile installare [!DNL Adobe Workfront for Salesforce] per consentire agli utenti di [!DNL Salesforce] di inviare [!DNL Workfront] richieste e creare automaticamente progetti senza mai uscire da [!DNL Salesforce].

In qualità di amministratore di [!DNL Workfront], puoi scaricare e configurare [!DNL Workfront for Salesforce]. Quindi, puoi condividerlo con tutti gli altri [!DNL Salesforce] utenti.

Per ulteriori informazioni sull&#39;installazione di [!DNL Workfront for Salesforce], vedere [Installa [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
Per ulteriori informazioni sulla configurazione della sezione [!DNL Workfront] in [!DNL Salesforce] per tutti gli utenti, vedere [Configurare la sezione  [!DNL Adobe Workfront] per [!DNL Salesforce] utenti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## Requisiti di accesso

Per utilizzare le funzionalità descritte in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## [!DNL Workfront for Salesforce]

Quando si utilizza [!DNL Workfront for Salesforce], è possibile effettuare le seguenti operazioni:

* Crea manualmente nuove richieste [!DNL Workfront] da [!DNL Salesforce] in un&#39;opportunità o in un account.

  Per ulteriori informazioni sulla creazione di [!DNL Workfront] richieste da [!DNL Salesforce], vedere [Invia [!DNL Adobe Workfront] richieste da [!DNL Salesforce] oggetti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Attiva automaticamente la creazione di progetti in [!DNL Workfront] quando vengono soddisfatti determinati criteri in [!DNL Salesforce]. L&#39;amministratore di sistema [!DNL Salesforce] deve configurare i trigger per la creazione di progetti da [!DNL Salesforce].

  Per ulteriori informazioni sulla creazione di [!DNL Workfront] progetti da [!DNL Salesforce], vedere [Crea [!DNL Adobe Workfront] progetti da [!DNL Salesforce] oggetti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Quando si lavora con [!DNL Workfront] per [!DNL Salesforce], tenere presente quanto segue:

* Supportiamo entrambi i framework [!DNL Salesforce Classic] e [!DNL Lightning Experience].
* Gli elementi possono essere creati solo da [!DNL Salesforce] in a [!DNL Workfront].
* È possibile visualizzare alcune informazioni sugli elementi [!DNL Workfront] in [!DNL Salesforce].

  Queste informazioni non possono essere personalizzate.

  Per un elenco di [!DNL Workfront] campi visualizzabili da [!DNL Salesforce], vedi [Invia [!DNL Adobe Workfront] richieste da [!DNL Salesforce] oggetti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md) e [Crea [!DNL Adobe Workfront] progetti da [!DNL Salesforce] oggetti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Puoi accedere direttamente agli elementi collegati a [!DNL Salesforce] facendo clic sul collegamento **[!UICONTROL Vai a Salesforce]** da Workfront.

  Non è possibile visualizzare informazioni sugli elementi [!DNL Salesforce] in [!DNL Workfront], ma si dispone di un collegamento all&#39;elemento [!UICONTROL Salesforce] di [!DNL Workfront] per esaminarlo in [!DNL Salesforce].

  [!UICONTROL Il collegamento **Vai a Salesforce**] viene visualizzato nelle seguenti aree:

   * La sezione [!UICONTROL Dettagli] di un progetto o di un problema e
   * L’intestazione di un progetto o di un problema.

     L&#39;amministratore del sistema o del gruppo deve aggiungere il campo [!UICONTROL Integrazioni] al modello di layout per visualizzare il collegamento [!UICONTROL Vai a Salesforce] nell&#39;intestazione del progetto o del problema.
   * Pannello [!DNL Summary] di un problema durante la selezione del problema in un elenco, dopo aver fatto clic sull&#39;icona del pannello [!UICONTROL Apri riepilogo] ![Riepilogo](assets/summary-panel-icon.png) nella barra degli strumenti dell&#39;elenco.

     >[!NOTE]
     >
     >Il collegamento [!UICONTROL Vai a Salesforce] è visibile a tutti gli utenti [!DNL Workfront] che possono visualizzare il progetto o il problema. È necessario disporre di un account [!DNL Salesforce] per poter accedere all&#39;opportunità [!DNL Salesforce] o all&#39;account in cui è stato registrato il problema.

* L&#39;aggiornamento dei campi su un elemento in un&#39;applicazione non aggiorna le informazioni sugli elementi collegati nell&#39;altra applicazione.
