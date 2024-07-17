---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Record SPF di Workfront Proof
description: Workfront Proof invia notifiche e-mail ai revisori da un indirizzo e-mail di Workfront Proof come notification@proofing.yourdomain.com. Per assicurarsi che i server di posta dei destinatari considerino attendibili tutte le notifiche e-mail di Workfront Proof, è necessario impostare un record  [!DNL Sender Policy] Framework (SPF) per il dominio personalizzato connesso all'account  [!DNL Workfront Proof]  (ad esempio, proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---

# Record SPF di Workfront Proof

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] invia notifiche e-mail ai revisori da un indirizzo e-mail di [!DNL Workfront Proof] come notification@proofing.yourdomain.com. Per assicurarsi che i server di posta dei destinatari considerino attendibili tutte le [!DNL Workfront Proof] notifiche e-mail, è necessario impostare un record [!UICONTROL Sender Policy Framework] (SPF) per il dominio personalizzato connesso all&#39;account [!DNL Workfront Proof] (ad esempio, **proofing.yourdomain.com**).

Per impostare un record SPF, è necessario includere il record SPF utilizzato per il dominio principale.

1. Aggiungi una voce **[!UICONTROL DNS TXT]** per il dominio con il seguente valore:

   `v=spf1 a:mx.proofhq.com -all`

   L&#39;amministratore della posta elettronica o il personale IT possono aiutarti a eseguire questa configurazione.

   >[!TIP]
   >
   >È possibile utilizzare lo strumento gratuito in [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) per esaminare [!DNL Workfront] record SPF.
