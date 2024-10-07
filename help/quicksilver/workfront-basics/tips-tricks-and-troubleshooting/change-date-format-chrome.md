---
filename: change-date-format-chrome
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Cambia il formato delle date in [!DNL Adobe Workfront]
description: Per modificare il formato della data per le date in [!DNL Adobe Workfront] è necessario modificare le impostazioni della lingua nel browser.
feature: Get Started with Workfront
exl-id: 9fac92fb-e3d1-4537-b324-4b35447cef28
source-git-commit: 5d924e510ad94098b9f417494f9fc6e8696c90d6
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Cambia il formato delle date in [!DNL Adobe Workfront]

<!--this article used to be called "Change the date format in Adobe Workfront when using Chrome". The team decieded to make it more generic and hide the steps. Also see drafted content below-->

>[!IMPORTANT]
>
> Le informazioni contenute in questo articolo si applicano solo alle organizzazioni che non hanno ancora effettuato l’onboarding in Adobe Unified Experience.
> Se per la tua organizzazione è stato eseguito l’onboarding in Adobe Unified Experience, la preferenza relativa alla data è controllata dalla preferenza relativa alla lingua impostata in Adobe Unified Shell. L&#39;impostazione predefinita per la lingua, e quindi per la data, è `en-US`.

È possibile modificare il formato della data in [!DNL Adobe Workfront], ad esempio [!UICONTROL Data di completamento pianificata], [!UICONTROL Data di completamento effettiva] o [!UICONTROL Data di completamento prevista].

Ad esempio, puoi modificare un formato di data da _GG/MM/AAAA_ a _MM/GG/AAAA_ o viceversa.
In alternativa, è possibile modificare il formato della data da _MM/GG/AA_ a _GG/MM/AAAA_.

In Workfront è possibile modificare i formati delle date nei modi seguenti, a seconda delle modifiche che si desidera visualizzare e del punto in cui si desidera visualizzarle.

* Per modificare tutti i formati di data per tutte le pagine in [!DNL Workfront] in base alla posizione e alla lingua, è necessario modificare le impostazioni della lingua nel browser.

  Ad esempio, se la lingua predefinita nel browser è impostata su *[!UICONTROL Inglese (Stati Uniti)]*, le date verranno visualizzate nei seguenti formati:

   * DD/MM/YYYY
   * GG mese AAAA

  Per modificare le impostazioni della lingua in [!DNL Chrome] o in qualsiasi altro browser, è necessario modificare le impostazioni di tale browser. I passaggi per modificare le impostazioni di un browser variano da un browser all’altro. Per informazioni su come modificarne le impostazioni, consulta le aree [!UICONTROL Aiuto], [!UICONTROL Preferenze] o [!UICONTROL Impostazioni] del browser.

* Per modificare il formato delle date solo nei report e nelle visualizzazioni, è necessario aggiornare l&#39;impostazione [!UICONTROL Formato campo] nell&#39;area [!UICONTROL Opzioni avanzate] di una colonna durante la creazione del report o della visualizzazione. Questo non modifica il formato della data in base alla posizione o alla lingua. Modifica il formato delle date nel contesto della stessa posizione o lingua.

  ![](assets/field-format-in-advanced-options-of-a-view-highlighted.png)

  Per ulteriori informazioni, vedere [Creare un report personalizzato](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Per modificare il formato delle date in tutte le notifiche e-mail in uscita per l&#39;intera organizzazione, è necessario aggiornare l&#39;impostazione [!UICONTROL Impostazioni internazionali e-mail predefinite] nell&#39;area [!UICONTROL Informazioni cliente] in [!UICONTROL Configurazione].

  ![](assets/default-email-locale-field.png)

  Per ulteriori informazioni, vedere [Configurare le informazioni di base per il sistema](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Per modificare il formato di tutte le date in tutte le notifiche e-mail in uscita per un singolo utente, è necessario aggiornare l&#39;impostazione [!UICONTROL Impostazioni internazionali e-mail] nella casella [!UICONTROL Modifica persona] durante la modifica del profilo di un utente.

  ![](assets/email-locale-for-user-profile-highlighted.png)

  Per ulteriori informazioni, vedere [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

<!--drafted because we should not document steps for a third-party application

To change your language settings in Chrome:

1. Click the 3-dots in the top right corner of your Chrome interface, then click **Settings**.
1. On the left area of the Settings page, expand **Advanced**, then click **Languages**.  
   Or  
   Search for *language*&nbsp;at the top of the Settings page, then click **Languages**.

1. In the **Language** list, locate the language and region that use your preferred date format.

   **Example:** If you speak English and you want the date format to be MM/DD/YYYY, you would select **English (United States)**. If you speak English and you want the date format to be DD/MM/YYY, you would select **English (United Kingdom)**.

1. (Conditional) If the language and region you want to use are not visible in the list, click **Add languages** to add it to the list.
1. Click the 3-dot menu next to the language and region you want to use, then click **Move to the top**.
1. Return to the Workfront interface, then refresh the page.  
   The date format is now updated in projects and other areas of Workfront that use MM/DD/YYYY or DD/MM/YYYY format when displaying dates.

   -->
