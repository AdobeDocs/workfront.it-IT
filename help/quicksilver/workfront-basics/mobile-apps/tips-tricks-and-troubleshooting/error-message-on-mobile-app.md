---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: "Messaggio di errore sull'app mobile  [!DNL Adobe Workfront] : 'L'account non è abilitato per l'API.'"
description: "Messaggio di errore sull'app mobile  [!DNL Adobe Workfront] : 'L'account non è abilitato per l'API.'"
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
source-git-commit: fdef22d9685d349a6f9492dec98475493ee9c048
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 2%

---

# Messaggio di errore sull&#39;app mobile [!DNL Adobe Workfront]: &quot;[!UICONTROL Il tuo account non è abilitato per l&#39;API.]&quot;

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano</strong></td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe [!DNL Workfront]</strong></td> 
   <td> <p>Piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso</strong></td> 
   <td> <p>[!UICONTROL Amministratore di sistema] </p> </td> 
  </tr> 
 </tbody> 
</table>

## Problema

Quando si tenta di accedere all&#39;app mobile [!DNL Adobe Workfront], viene visualizzato il seguente errore: *[!UICONTROL L&#39;account non è abilitato per l&#39;API. Informa l’amministratore di sistema che ti configurerà. Spiacenti.]*

## Causa

L&#39;amministratore di [!DNL Workfront] non ha abilitato l&#39;ambiente [!DNL Workfront] per l&#39;accesso da un dispositivo mobile.

## Soluzione

1. Accedere all&#39;applicazione Web [!DNL Workfront] come amministratore [!DNL Workfront].
1. Passare all&#39;area **[!UICONTROL Configurazione]**.
1. Espandere il menu **[!UICONTROL Sistema]**, quindi fare clic su **[!UICONTROL Preferenze]**.

1. Nella sezione **[!UICONTROL Sicurezza]** selezionare **[!UICONTROL Consenti alle persone di utilizzare le applicazioni mobili di [!DNL Workfront] e l&#39;opzione [!DNL Workfront Outlook] Componente aggiuntivo]** per abilitarlo.

1. Fai clic su **[!UICONTROL Salva]**.\
   Tutti gli utenti del sistema possono ora accedere a [!DNL Workfront] dalle loro app mobili e da [!DNL Outlook].
