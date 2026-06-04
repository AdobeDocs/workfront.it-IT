---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Record SPF di Workfront Proof
description: Workfront Proof invia notifiche e-mail ai revisori da un indirizzo e-mail di Workfront Proof come notification@proofing.yourdomain.com. Per assicurarsi che i server di posta dei destinatari considerino attendibili tutte le notifiche e-mail di Workfront Proof, è necessario impostare un record  [!DNL Sender Policy] Framework (SPF) per il dominio personalizzato connesso all'account  [!DNL Workfront Proof]  (ad esempio, proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
TQID: https://experienceleague.adobe.com/LTZzs99Zzsn5dbOlu4wP1coyJAMDnnCZZ1pTTbEjT24
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 181
ht-degree: 4%

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
