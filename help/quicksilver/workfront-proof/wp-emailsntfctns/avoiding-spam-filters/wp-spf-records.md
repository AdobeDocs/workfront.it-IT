---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Record SPF di Workfront Proof
description: Workfront Proof invia notifiche e-mail ai revisori da un indirizzo e-mail Workfront Proof, ad esempio notification@proofing.yourdomain.com. Per garantire che i server di posta elettronica dei destinatari si fidino di tutte le notifiche e-mail di Workfront Proof, è necessario impostare un [!DNL Sender Policy] Record del framework (SPF) per il dominio personalizzato connesso al [!DNL Workfront Proof] account (ad esempio, proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Record SPF di Workfront Proof

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] invia notifiche e-mail ai revisori da un [!DNL Workfront Proof] indirizzo e-mail come notification@proofing.yourdomain.com. Al fine di garantire che i server di posta dei destinatari siano affidabili [!DNL Workfront Proof] notifiche e-mail, è necessario impostare un [!UICONTROL Framework dei criteri di invio] (SPF) registra per il dominio personalizzato connesso al [!DNL Workfront Proof] account (ad esempio, **proofing.yourdomain.com**).

Per impostare un record SPF, è necessario includere il record SPF utilizzato per il dominio principale.

1. Aggiungi un **[!UICONTROL TXT DNS]** voce per il dominio con il seguente valore:

   `v=spf1 a:mx.proofhq.com -all`

   L&#39;amministratore di posta elettronica o il personale IT possono aiutarti a configurarlo.

   >[!TIP]
   >
   >È possibile utilizzare lo strumento gratuito in [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) rivedere [!DNL Workfront] record SPF.
