---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Aggiornare un oggetto esistente da un messaggio e-mail di Outlook
description: È possibile aggiornare un progetto, un'attività o un problema esistente con le informazioni contenute in un messaggio e-mail di Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 297eb1c4-ee9f-4bb3-a412-18f23c74b0eb
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Aggiornare un oggetto esistente da un&#39;e-mail [!DNL Outlook]

>[!IMPORTANT]
>
>Microsoft [È in corso la disabilitazione del supporto per i token online di Exchange legacy](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), attualmente utilizzati dal componente aggiuntivo di Workfront Outlook per l&#39;autenticazione. Questa modifica di Microsoft ha già iniziato a interessare i clienti e continuerà a essere implementata in più fasi fino a ottobre 2025.
>
>* **Dopo la completa disattivazione di questi token da parte di Microsoft, l&#39;integrazione di Workfront per Microsoft Outlook non funzionerà più.**
>
>Come parte di questa modifica, Microsoft ha deciso di cambiare il modo in cui i token vengono riabilitati. Dopo il **30 giugno 2025**, gli amministratori non saranno più in grado di riabilitare i token personalmente. Solo il supporto Microsoft può concedere eccezioni. **Il 1° ottobre 2025, i token legacy verranno disattivati per tutti i tenant. Le eccezioni non verranno concesse.**

È possibile aggiornare un progetto, un&#39;attività o un problema esistente con le informazioni di un&#39;e-mail di [!DNL Outlook].

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

## Aggiornare un oggetto esistente da un&#39;e-mail [!DNL Outlook]

1. In [!DNL Outlook] selezionare l&#39;indirizzo di posta elettronica contenente le informazioni che si desidera includere in un [!DNL Adobe Workfront update].
1. Fare clic sull&#39;icona **[!DNL Workfront]** nell&#39;angolo superiore destro del messaggio di posta elettronica per visualizzare il componente aggiuntivo Workfront.\
   Per accedere all&#39;icona di [!DNL Workfront], potrebbe essere necessario fare clic sulla freccia rivolta verso il basso in alto a destra nell&#39;e-mail.

1. Fai clic sull&#39;icona **[!UICONTROL Menu]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) per visualizzare l&#39;elenco delle opzioni [!DNL Workfront] disponibili.\


1. Fare clic su **[!UICONTROL Aggiorna] in Workfront**.\
   Puoi aggiornare le seguenti informazioni dall’e-mail prima di salvarla come attività:

   * **[!UICONTROL Tipo]**: selezionare il tipo di oggetto da aggiornare. È possibile selezionare **[!UICONTROL Progetto]**, **[!UICONTROL Attività]** o **[!UICONTROL Problema]**. L&#39;oggetto selezionato determina i risultati visualizzati nel campo **[!UICONTROL Name]** sottostante. Se non sei sicuro del tipo di oggetto, seleziona **[!UICONTROL Tutti]** per cercare progetti, attività e problemi contemporaneamente.

   * **[!UICONTROL Nome]**: inizia a digitare il nome del progetto, dell&#39;attività o del problema che desideri aggiornare. Fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.
   * **[!UICONTROL Aggiornamento]**: per impostazione predefinita, l&#39;aggiornamento corrisponde al corpo dell&#39;e-mail. È possibile modificare l&#39;aggiornamento in base alle proprie esigenze.\

     Questo [!UICONTROL aggiornamento] viene visualizzato come stato di aggiornamento in Workfront.

   * **[!UICONTROL Allegati]**: tutti gli allegati e-mail vengono salvati nell&#39;area [!UICONTROL Documenti] dell&#39;attività. È possibile eliminare tutti gli allegati prima di inviare l&#39;aggiornamento.

1. (Facoltativo) Fai clic su **[!UICONTROL Includi altri]**, inizia a digitare il nome degli utenti che desideri includere nell&#39;aggiornamento, quindi fai clic sul nome quando viene visualizzato nell&#39;elenco a discesa.\
   Ripeti questo processo per includere altri utenti, quindi fai clic su **[!UICONTROL Fine]**.\
   Per impostazione predefinita, l’utente a cui si risponde riceve una notifica indipendentemente dal fatto che li si includa o meno.\

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Blocca]** per limitare l&#39;aggiornamento agli utenti della tua azienda. Quando l’aggiornamento è bloccato, gli utenti esterni alla società non possono visualizzarlo.

   * **[!UICONTROL Sbloccato]:** Qualsiasi utente con accesso al progetto, all&#39;attività o al problema in cui si trova l&#39;aggiornamento può visualizzare l&#39;aggiornamento.\

     Per impostazione predefinita, l’aggiornamento è sbloccato.\
      ![o365_addin_unlock.png](assets/o365-addin-unlock.png)

   * **[!UICONTROL Bloccato]:** Solo gli utenti della tua azienda possono visualizzare l&#39;aggiornamento.\

     ![o365_addin_lock.png](assets/o365-addin-lock.png)

1. Fai clic su **[!UICONTROL Aggiorna]**.
1. (Facoltativo) Fare clic su **[!UICONTROL Visualizza in Workfront]** per visualizzare l&#39;elemento aggiornato con l&#39;integrazione [!DNL Workfront] in [!UICONTROL Outlook].
