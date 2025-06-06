---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Crea una  [!DNL Adobe Workfront] richiesta da un'e-mail di Outlook
description: È possibile creare una  [!DNL Adobe Workfront] richiesta da un indirizzo e-mail in Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4ecfe632-5f2e-4dc2-8c88-6a8229887f53
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Crea una richiesta [!DNL Adobe Workfront] da un&#39;e-mail [!UICONTROL Outlook]

>[!IMPORTANT]
>
>Microsoft [È in corso la disabilitazione del supporto per i token online di Exchange legacy](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), attualmente utilizzati dal componente aggiuntivo di Workfront Outlook per l&#39;autenticazione. Questa modifica di Microsoft ha già iniziato a interessare i clienti e continuerà a essere implementata in più fasi fino a ottobre 2025.
>
>* **Dopo la completa disattivazione di questi token da parte di Microsoft, l&#39;integrazione di Workfront per Microsoft Outlook non funzionerà più.**
>
>Come parte di questa modifica, Microsoft ha deciso di cambiare il modo in cui i token vengono riabilitati. Dopo il **30 giugno 2025**, gli amministratori non saranno più in grado di riabilitare i token personalmente. Solo il supporto Microsoft può concedere eccezioni. **Il 1° ottobre 2025, i token legacy verranno disattivati per tutti i tenant. Le eccezioni non verranno concesse.**

È possibile creare una richiesta [!DNL Adobe Workfront] da un indirizzo e-mail in Outlook.

Quando si crea una richiesta [!DNL Workfront] basata su un&#39;e-mail, il contenuto dell&#39;e-mail (inclusi l&#39;oggetto e il corpo) viene incluso nella richiesta per impostazione predefinita.

>[!NOTE]
>
>Impossibile creare una richiesta [!DNL Workfront] da una cassetta postale [!UICONTROL Outlook] condivisa.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Lavoro], [!UICONTROL Piano]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## Prerequisiti

L&#39;amministratore di [!DNL Workfront] deve abilitare [!DNL Outlook for Office] con [!DNL Workfront] prima di poter utilizzare questa integrazione.

## Crea una richiesta da un&#39;e-mail [!DNL Outlook]

Per creare una richiesta [!DNL Workfront] da [!DNL Outlook]:

1. Selezionare l&#39;e-mail contenente le informazioni da includere in una richiesta [!DNL Workfront].
1. Fare clic sull&#39;icona **[!DNL Workfront]** nell&#39;angolo superiore destro del messaggio di posta elettronica per visualizzare il componente aggiuntivo Workfront.\
   Per accedere all&#39;icona di [!DNL Workfront], potrebbe essere necessario fare clic sulla freccia rivolta verso il basso in alto a destra nell&#39;e-mail.

1. Fai clic sull&#39;icona **[!UICONTROL Menu]** ![o365_addin_menu2_icon.png](assets/o365-addin-menu2-icon.png) per visualizzare l&#39;elenco delle opzioni [!DNL Workfront] disponibili.

1. Fai clic su **[!UICONTROL Invia richiesta]**.
1. Nel campo **[!UICONTROL Selezionare un tipo di richiesta]**, selezionare la coda di richieste in cui si desidera inviare la richiesta.

1. Specifica le seguenti informazioni:\
   A seconda di come è stata impostata la coda di richieste, i campi disponibili possono variare. Per un elenco completo e una descrizione dei campi possibili, consulta l&#39;articolo [Creare e inviare [!DNL Adobe Workfront] richieste](../../manage-work/requests/create-requests/create-submit-requests.md).

   * **[!UICONTROL Oggetto]:** Specificare un oggetto per la richiesta. Per impostazione predefinita, viene utilizzato l’oggetto dell’e-mail.
   * **[!UICONTROL Descrizione]:** Specificare una descrizione per la richiesta. Per impostazione predefinita, viene utilizzato il corpo dell’e-mail.
   * **[!UICONTROL Documenti]:** Allegare tutti i documenti che si desidera includere nella richiesta. È possibile allegare i documenti tramite trascinamento oppure facendo clic su **[!UICONTROL Seleziona file]** e individuando e selezionando il documento.\

     Per impostazione predefinita, tutti i documenti allegati all’e-mail vengono inclusi nella richiesta.

1. Fai clic su **[!UICONTROL Invia richiesta]**.\
   La richiesta viene inviata a [!DNL Workfront], nella coda richieste specificata.

1. (Facoltativo) Tornare a [!DNL Outlook] e selezionare l&#39;e-mail originale.\
   Nella parte superiore del pannello del componente aggiuntivo [!DNL Workfront], noterai la conferma con un collegamento che indica che l&#39;e-mail è stata aggiunta a Workfront come richiesta. Il collegamento include la data in cui è stato convertito.\
