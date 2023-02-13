---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Panoramica di Adobe Workfront for Salesforce
description: È possibile installare [!DNL Adobe Workfront] per Salesforce per consentire agli utenti Salesforce di inviare [!DNL Workfront] richiede e crea automaticamente progetti senza mai lasciare Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] panoramica

A [!UICONTROL Pro] [!DNL Workfront] Per utilizzare questa funzione è necessario pianificare. Per ulteriori informazioni sui vari piani disponibili, vedi [[!DNL Workfront] Piani.](https://www.workfront.com/plans)

È possibile installare [!DNL Adobe Workfront for Salesforce] consente [!DNL Salesforce] utenti da inviare [!DNL Workfront] richiede e crea automaticamente progetti senza mai uscire [!DNL Salesforce].

Come [!DNL Workfront] amministratore, puoi scaricare e configurare [!DNL Workfront for Salesforce]. Poi puoi condividerlo, tutti gli altri [!DNL Salesforce] utenti.

Per ulteriori informazioni sull’installazione [!DNL Workfront for Salesforce], vedi [Installa [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
Per ulteriori informazioni sulla configurazione di [!DNL Workfront] sezione [!DNL Salesforce] per tutti gli utenti, vedi [Configura le [!DNL Adobe Workfront] sezione per [!DNL Salesforce] utenti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## Requisiti di accesso

Per utilizzare la funzionalità descritta in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## [!DNL Workfront for Salesforce]

È possibile effettuare le seguenti operazioni quando si utilizza [!DNL Workfront for Salesforce]:

* Creare manualmente nuovi [!DNL Workfront] richieste da [!DNL Salesforce] in un&#39;opportunità o un account.

   Per ulteriori informazioni sulla creazione [!DNL Workfront] richieste da [!DNL Salesforce], vedi [Invia [!DNL Adobe Workfront] richieste da [!DNL Salesforce] oggetti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Attiva automaticamente la creazione di progetti in [!DNL Workfront] quando determinati criteri sono soddisfatti in [!DNL Salesforce]. Le [!DNL Salesforce] l&#39;amministratore di sistema deve configurare i trigger per la creazione di progetti da [!DNL Salesforce].

   Per ulteriori informazioni sulla creazione [!DNL Workfront] progetti da [!DNL Salesforce], vedi [Crea [!DNL Adobe Workfront] progetti da [!DNL Salesforce] oggetti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Quando si lavora con , considera quanto segue [!DNL Workfront] per [!DNL Salesforce]:

* Sosteniamo entrambe le [!DNL Salesforce Classic] e [!DNL Lightning Experience] framework.
* Gli elementi possono essere creati solo da [!DNL Salesforce] in [!DNL Workfront].
* È possibile visualizzare alcune informazioni sul [!DNL Workfront] elementi in [!DNL Salesforce].

   Queste informazioni non possono essere personalizzate.

   Per un elenco di [!DNL Workfront] campi visualizzabili da [!DNL Salesforce], vedi  [Invia [!DNL Adobe Workfront] richieste da [!DNL Salesforce] oggetti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)  e [Crea [!DNL Adobe Workfront] progetti da [!DNL Salesforce] oggetti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Puoi accedere direttamente agli elementi collegati a [!DNL Salesforce] facendo clic sul pulsante **[!UICONTROL Vai a Salesforce]** collegamento da Workfront.

   Non è possibile visualizzare informazioni sulla [!DNL Salesforce] elementi in [!DNL Workfront], ma hai un collegamento alla [!UICONTROL Salesforce] elemento da [!DNL Workfront] per esaminarlo [!DNL Salesforce].

   [!UICONTROL La **Vai a Salesforce**] Il collegamento viene visualizzato nelle seguenti aree:

   * La [!UICONTROL Dettagli] sezione di un progetto o un problema
   * Intestazione di un progetto o di un problema.

      L&#39;amministratore di sistema o di gruppo deve aggiungere [!UICONTROL Integrazioni] nel modello di layout per visualizzare il campo [!UICONTROL Vai a Salesforce] nell’intestazione del progetto o del problema.
   * La [!DNL Summary] pannello di un problema durante la selezione del problema in un elenco, dopo aver fatto clic su [!UICONTROL Apri riepilogo] ![](assets/summary-panel-icon.png) nella barra degli strumenti dell’elenco.

      >[!NOTE]
      >
      >La [!UICONTROL Vai a Salesforce] link è visibile a tutti [!DNL Workfront] utenti che possono visualizzare il progetto o il problema. Devi avere un [!DNL Salesforce] per poter accedere al [!DNL Salesforce] Opportunità o account in cui è stato registrato il problema.

* L&#39;aggiornamento dei campi su un elemento in un&#39;applicazione non aggiorna le informazioni sugli elementi collegati nell&#39;altra applicazione.
