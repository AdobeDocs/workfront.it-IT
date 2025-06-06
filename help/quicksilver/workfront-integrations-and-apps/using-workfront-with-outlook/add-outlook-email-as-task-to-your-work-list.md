---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Aggiungere un messaggio e-mail di Outlook come attività all'elenco di lavoro
description: Puoi convertire [!DNL Outlook] e-mail in [!DNL Adobe Workfront] attività. Dopo la conversione di un’e-mail, l’attività è disponibile in Work List (Elenco di lavoro) nella sezione Home.
author: Becky
feature: Workfront Integrations and Apps
exl-id: fcd02116-ffeb-43d3-8541-5e30e6cfdc5e
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---

# Aggiungi un&#39;e-mail di [!DNL Outlook] come attività al tuo elenco di lavoro

>[!IMPORTANT]
>
>Microsoft [È in corso la disabilitazione del supporto per i token online di Exchange legacy](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), attualmente utilizzati dal componente aggiuntivo di Workfront Outlook per l&#39;autenticazione. Questa modifica di Microsoft ha già iniziato a interessare i clienti e continuerà a essere implementata in più fasi fino a ottobre 2025.
>
>* **Dopo la completa disattivazione di questi token da parte di Microsoft, l&#39;integrazione di Workfront per Microsoft Outlook non funzionerà più.**
>
>Come parte di questa modifica, Microsoft ha deciso di cambiare il modo in cui i token vengono riabilitati. Dopo il **30 giugno 2025**, gli amministratori non saranno più in grado di riabilitare i token personalmente. Solo il supporto Microsoft può concedere eccezioni. **Il 1° ottobre 2025, i token legacy verranno disattivati per tutti i tenant. Le eccezioni non verranno concesse.**



È possibile convertire [!DNL Outlook] e-mail in [!DNL Adobe Workfront] attività. Dopo la conversione di un&#39;e-mail, l&#39;attività è disponibile nell&#39;elenco [!UICONTROL Lavoro] nell&#39;area [!UICONTROL Home].

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

## Aggiungi un&#39;e-mail di [!DNL Outlook] come attività al tuo elenco di lavoro

1. Selezionare l&#39;e-mail in [!DNL Outlook] che si desidera convertire in un&#39;attività.
1. Fare clic sull&#39;icona **[!DNL Workfront]** nell&#39;angolo superiore destro del messaggio di posta elettronica per visualizzare il componente aggiuntivo [!DNL Workfront].\
   Per accedere all&#39;icona di [!DNL Workfront], potrebbe essere necessario fare clic sulla freccia rivolta verso il basso in alto a destra nell&#39;e-mail.

1. Fai clic sull&#39;icona **[!UICONTROL Menu]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) per visualizzare l&#39;elenco delle opzioni [!DNL Workfront] disponibili.\


1. Fare clic su **[!UICONTROL Aggiungi a lavoro]**.\

1. Deseleziona il campo **[!UICONTROL Aggiungi al progetto]**.
1. (Facoltativo) Puoi aggiornare le seguenti informazioni dall’e-mail prima di salvarla come attività:

   * **[!UICONTROL Nome attività]:** Per impostazione predefinita, il nome dell&#39;attività corrisponde all&#39;oggetto dell&#39;e-mail. È possibile modificare il nome dell&#39;attività come desiderato.
   * **[!UICONTROL Descrizione]:** Per impostazione predefinita, la descrizione è uguale al corpo dell&#39;e-mail. Puoi modificare la descrizione come desiderato.
   * **[!UICONTROL Allegati]:** Tutti gli allegati e-mail vengono salvati nell&#39;area [!UICONTROL Documenti] dell&#39;attività. Puoi eliminare tutti gli allegati prima di salvare l’e-mail come attività.

1. Fare clic su **[!UICONTROL Aggiungi]**.\
   L&#39;attività viene aggiunta a [!UICONTROL Work List] nella tua area Home senza data di commit.

1. (Facoltativo) Fare clic su **[!UICONTROL Visualizza in Workfront]** per visualizzare l&#39;attività nell&#39;applicazione [!DNL Workfront] in una nuova scheda.

1. (Facoltativo) Tornare a [!DNL Outlook] e selezionare l&#39;e-mail originale.\
   Nella parte superiore del pannello dei componenti aggiuntivi di [!DNL Workfront], noterai la conferma con un collegamento che indica che l&#39;e-mail è stata aggiunta a Workfront come attività. Il collegamento include la data in cui è stato convertito.\
