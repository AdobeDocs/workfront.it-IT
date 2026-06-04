---
content-type: reference
navigation-topic: announcements
title: Rimozione di e-mail spoofing e risposta POP
description: Stiamo apportando due modifiche al modo in cui Adobe Workfront invia e riceve e-mail con la versione 20.3 (prevista per agosto 2020).
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
TQID: https://experienceleague.adobe.com/eOFRSbJicMbYHqq74-O9VW0c73RDQmAC-OIkLX-FKFw
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
source-wordcount: 319
ht-degree: 3%

---

# Spoofing delle e-mail e risposta POP

Stiamo apportando due modifiche al modo in cui Adobe Workfront invia e riceve e-mail con la versione 20.3 (prevista per agosto 2020).

## E-mail in uscita da Workfront

Nel tentativo di aumentare il successo della consegna delle e-mail, elimineremo lo spoofing delle e-mail, che viene spesso taggato come spam (vedi Spoofing delle e-mail). Tutti i messaggi di posta elettronica provenienti da Workfront verranno inviati da `notifications@my.workfront.com`, inclusi gli avvisi automatici e la comunicazione tra utenti. Un esempio di e-mail da Joan Harris si presenterà così nella sezione da dell’e-mail:

![E-mail di esempio](assets/noreply.png)

*Ti consigliamo di contattare il tuo team IT* per assicurarti che l&#39;e-mail di `notifications@my.workfront.com` non venga bloccata per le e-mail in arrivo nel tuo sistema. Puoi anche fare riferimento a [Configurare il inserisco nell&#39;elenco Consentiti di del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) per i dettagli sugli indirizzi IP da cui provengono il traffico e l&#39;e-mail.

## Risposte e-mail in entrata alle notifiche (POP Reply)

Alcune notifiche e-mail consentono agli utenti di rispondere tramite e-mail e di copiare la risposta in Workfront come risposta a un commento nel sistema Workfront. Gli amministratori di sistema di Workfront sono tradizionalmente in grado di scegliere se fornire il proprio server di posta elettronica POP per ricevere tali risposte o utilizzare il sistema di risposta integrato di Workfront. La scelta del server e-mail POP personalizzato verrà rimossa con la versione 20.3. A tutti gli account configurati per l&#39;utilizzo di un server personalizzato verrà automaticamente applicata la transizione al sistema di risposta e-mail nativo di Workfront. Non è richiesta alcuna azione da parte degli amministratori di sistema o di altri utenti di Workfront.

Le e-mail provenienti direttamente dal sistema Workfront Proof non subiranno modifiche. Continuerai a ricevere queste e-mail come in passato.

Per ulteriori domande o dubbi, contatta il [team di supporto Workfront](https://experienceleague.adobe.com/?support-tab=home&lang=it#support).
