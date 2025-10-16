---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Invia [!DNL Adobe Workfront] richieste da [!DNL Salesforce] oggetti
description: Dopo aver installato  [!DNL Adobe Workfront] per [!DNL Salesforce], you can submit [!DNL Workfront] richieste da [!DNL Salesforce] Opportunità e account. Questa funzionalità esiste sia nel framework Classic che nel framework Lightning Experience.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 1%

---

# Invia [!DNL Adobe Workfront] richieste da [!DNL Salesforce] oggetti

>[!IMPORTANT]
>
>Per offrire integrazioni più stabili e scalabili, stiamo passando a un approccio di integrazione moderno e flessibile che utilizza l’automazione e l’integrazione di Workfront (Fusion). Come parte di questo processo di transizione, l&#39;integrazione di Workfront for Salesforce non sarà disponibile dopo il **28 febbraio 2026**.
>
>È consigliabile utilizzare l’automazione e l’integrazione di Workfront per le esigenze di integrazione della tua organizzazione con Salesforce.
>
>Per una panoramica dell&#39;automazione e dell&#39;integrazione di Workfront, vedere [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Per informazioni sulle funzionalità specifiche dei moduli di automazione e integrazione di Workfront per Salesforce, vedere [Moduli Salesforce](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Dopo aver installato [!DNL Adobe Workfront for Salesforce], puoi inviare [!DNL Workfront] richieste da [!DNL Salesforce] opportunità e account. Questa funzionalità esiste sia nel framework [!DNL Classic] che nel framework [!DNL Lightning Experience].

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <p>Piano</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Per inviare una richiesta [!DNL Workfront] da un&#39;opportunità [!DNL Salesforce] o da un account, verificare di disporre dei seguenti elementi nell&#39;ambiente:

* L&#39;amministratore di [!DNL Workfront] ha installato [!DNL Workfront for Salesforce].\
   Per ulteriori informazioni sull&#39;installazione di [!DNL Workfront for Salesforce], vedere [Installa [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* L&#39;amministratore di [!DNL Workfront] ha aggiunto la sezione [!DNL Workfront] ai layout di pagina [!UICONTROL Opportunity] e [!UICONTROL Account].\
   Per ulteriori informazioni sull&#39;aggiunta della sezione [!DNL Workfront] a un layout di pagina, vedere [Configurare la sezione  [!DNL Adobe Workfront] per [!DNL Salesforce] utenti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Hai un account [!DNL Workfront] e puoi accedervi dalla sezione [!DNL Workfront] all&#39;interno dell&#39;opportunità o dell&#39;account.\
   Dopo aver effettuato l&#39;accesso, è possibile visualizzare la scheda [!UICONTROL Nuove richieste] in cui è possibile iniziare a immettere le richieste.

## Invia [!DNL Workfront] richieste da [!DNL Salesforce]

1. Vai a un’opportunità o a un account in Salesforce.
1. Passare alla sezione [!DNL Workfront].
1. Nella scheda **[!UICONTROL Nuove richieste]**, seleziona un tipo di richiesta nel menu a discesa **[!UICONTROL Seleziona un tipo di richiesta]**.

   Puoi visualizzare le stesse code di richieste a cui hai accesso in Workfront.

1. Inizia a compilare i campi disponibili per la richiesta.

   L&#39;invio di una richiesta da [!DNL Salesforce] è identico all&#39;invio di una richiesta nell&#39;applicazione Web [!DNL Workfront].

   >[!NOTE]
   >
   >Il caricamento di un documento con il plug-in [!DNL Workfront] in [!DNL Salesforce] non è al momento disponibile.

   Continua a seguire i passaggi descritti in [Crea e invia [!DNL Adobe Workfront] richieste](../../manage-work/requests/create-requests/create-submit-requests.md).

1. Fai clic su **[!UICONTROL Invia]**.

## Visualizza [!DNL Workfront] richieste

1. Passare a un&#39;opportunità o a un account in [!DNL Salesforce].
1. Passare alla sezione **[!DNL Workfront]**.

   >[!NOTE]
   >
   >A seconda del modo in cui l&#39;amministratore di [!DNL Workfront] ha configurato questa sezione, potrebbe avere un nome diverso.

1. Selezionare la scheda **[!UICONTROL Richieste inviate]**.

   È possibile visualizzare tutte le richieste inviate da questa opportunità o account in questa scheda.Le richieste inviate a questa coda di richieste nell&#39;applicazione Web non vengono visualizzate in questo elenco in [!DNL Salesforce].

   >[!NOTE]
   >
   >Le richieste inviate a questa coda di richieste nell’applicazione web non vengono visualizzate in questo elenco in Salesforce.

   ![richieste_sottomesse_salesforce.png](assets/salesforce-submitted-requests-350x58.png)

   È possibile visualizzare le seguenti informazioni sulle richieste inviate:

   * Nome richieste (nella colonna [!UICONTROL Oggetto])
   * Numero di riferimento
   * Tipo di richiesta
   * Stato
   * Inviato il
   * Richiesto per nome
   * Assegnato a Nome\

     Quando queste informazioni vengono aggiornate in [!DNL Workfront], vengono aggiornate anche in questo elenco.

1. (Facoltativo) Fare clic sul nome della richiesta per aprirla in [!DNL Workfront].

1. (Facoltativo) Fai clic su **[!UICONTROL Vai a[!DNL Salesforce]]** per accedere all&#39;opportunità o all&#39;account in cui il problema ha avuto origine dalle seguenti aree di Workfront:

   * Nella sezione [!UICONTROL Dettagli] del problema
   * Nel pannello Riepilogo quando si seleziona il problema in un elenco, dopo aver fatto clic su [!UICONTROL Apri riepilogo] ![icona del pannello Riepilogo](assets/summary-panel-icon.png) nella barra degli strumenti dell&#39;elenco.
   * Nell&#39;intestazione del problema, quando è disponibile il campo [!UICONTROL Integrazioni]. L&#39;amministratore del sistema o del gruppo deve aggiungere il campo [!UICONTROL Integrazioni] al modello di layout per visualizzare il collegamento Vai a Salesforce nell&#39;intestazione del problema. Per ulteriori informazioni, vedere [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >Il collegamento [!UICONTROL Vai a Salesforce] è visibile a tutti gli utenti [!DNL Workfront] che possono visualizzare il problema. È necessario disporre di un account [!DNL Salesforce] per poter accedere all&#39;opportunità [!DNL Salesforce] o all&#39;account in cui è stato registrato il problema.
