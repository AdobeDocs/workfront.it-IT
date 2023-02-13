---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Invia [!DNL Adobe Workfront] richieste da [!DNL Salesforce] oggetti
description: Dopo l'installazione [!DNL Adobe Workfront] per [!DNL Salesforce], you can submit [!DNL Workfront] richieste da [!DNL Salesforce] Opportunità e account. Questa funzionalità esiste sia nei framework Classic che Lightning Experience.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 1%

---

# Invia [!DNL Adobe Workfront] richieste da [!DNL Salesforce] oggetti

Dopo l&#39;installazione [!DNL Adobe Workfront for Salesforce], puoi inviare [!DNL Workfront] richieste da [!DNL Salesforce] Opportunità e account. Questa funzionalità esiste in entrambi i [!DNL Classic] e [!DNL Lightning Experience] framework.

## Requisiti di accesso

Per utilizzare la funzionalità descritta in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] piano*</p></td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] licenza*</p></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Prerequisiti

Per inviare un [!DNL Workfront] richiesta di [!DNL Salesforce] Opportunità o account assicurati di disporre dei seguenti elementi nell&#39;ambiente:

* Le [!DNL Workfront] amministratore installato [!DNL Workfront for Salesforce].\
   Per ulteriori informazioni sull’installazione [!DNL Workfront for Salesforce], vedi [Installa [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Le [!DNL Workfront] l&#39;amministratore ha aggiunto [!DNL Workfront] alla sezione [!UICONTROL Opportunità] e [!UICONTROL Account] layout di pagina.\
   Per ulteriori informazioni sull’aggiunta di [!DNL Workfront] al layout di una pagina, vedi [Configura le [!DNL Adobe Workfront] sezione per [!DNL Salesforce] utenti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Hai un [!DNL Workfront] e puoi accedere a da [!DNL Workfront] all&#39;interno della sezione Opportunità o Account.\
   Una volta effettuato l’accesso, puoi visualizzare le [!UICONTROL Nuove richieste] scheda in cui puoi iniziare a immettere le richieste.

## Invia [!DNL Workfront] richieste da [!DNL Salesforce]

1. Vai a un&#39;opportunità o un account in Salesforce.
1. Vai a [!DNL Workfront] sezione .
1. In **[!UICONTROL Nuove richieste]** seleziona un tipo di richiesta nella scheda **[!UICONTROL Selezionare un tipo di richiesta]** menu a discesa.

   Puoi visualizzare le stesse code di richiesta a cui hai accesso per visualizzare in Workfront.

1. Inizia a compilare i campi disponibili per la richiesta.

   Invio di una richiesta da [!DNL Salesforce] è identica all’invio di una richiesta nel [!DNL Workfront] applicazione web.

   >[!NOTE]
   >
   >Caricamento di un documento utilizzando [!DNL Workfront] plug-in [!DNL Salesforce] temporaneamente non disponibile.

   Continua a seguire i passaggi descritti in [Creazione e invio [!DNL Adobe Workfront] requests](../../manage-work/requests/create-requests/create-submit-requests.md).

1. Fai clic su **[!UICONTROL Invia]**.

## Visualizza [!DNL Workfront] requests

1. Vai a un&#39;opportunità o un account in [!DNL Salesforce].
1. Vai a **[!DNL Workfront]** sezione .

   >[!NOTE]
   >
   >A seconda di come [!DNL Workfront] amministratore ha configurato questa sezione, potrebbe avere un nome diverso.

1. Seleziona la **[!UICONTROL Richieste inviate]** scheda .

   È possibile visualizzare tutte le richieste inviate da questa opportunità o account in questa scheda.Le richieste inviate a questa coda di richiesta nell&#39;applicazione Web non vengono visualizzate in questo elenco in [!DNL Salesforce].

   >[!NOTE]
   >
   >Le richieste inviate a questa coda di richiesta nell’applicazione web non vengono visualizzate in questo elenco in Salesforce.

   ![salesforce_submit_requests.png](assets/salesforce-submitted-requests-350x58.png)

   È possibile visualizzare le seguenti informazioni sulle richieste inviate:

   * Nome della richiesta (in [!UICONTROL Oggetto] colonna)
   * Numero di riferimento
   * Tipo di richiesta
   * Stato
   * Inviato alla data
   * Richiesto per nome
   * Assegnato a Nome\

      Quando queste informazioni vengono aggiornate in [!DNL Workfront], viene aggiornato anche in questo elenco.

1. (Facoltativo) Fai clic sul nome della richiesta per aprirla in [!DNL Workfront].

1. (Facoltativo) Fai clic su **[!UICONTROL Vai a[!DNL Salesforce]]** per accedere all&#39;opportunità o all&#39;account in cui il problema ha avuto origine dalle seguenti aree di Workfront:

   * In [!UICONTROL Dettagli] sezione del problema
   * Nel pannello Riepilogo quando selezioni il problema in un elenco, dopo aver fatto clic su [!UICONTROL Apri riepilogo] ![](assets/summary-panel-icon.png) nella barra degli strumenti dell’elenco.
   * Nell’intestazione del problema, quando [!UICONTROL Integrazioni] campo disponibile. L&#39;amministratore di sistema o di gruppo deve aggiungere [!UICONTROL Integrazioni] nel modello di layout per visualizzare il collegamento Vai a Salesforce nell’intestazione del problema. Per ulteriori informazioni, consulta [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >La [!UICONTROL Vai a Salesforce] link è visibile a tutti [!DNL Workfront] utenti che possono visualizzare il problema. Devi avere un [!DNL Salesforce] per poter accedere al [!DNL Salesforce] Opportunità o account in cui è stato registrato il problema.
