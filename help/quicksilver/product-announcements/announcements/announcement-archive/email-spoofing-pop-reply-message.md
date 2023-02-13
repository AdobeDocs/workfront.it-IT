---
content-type: reference
navigation-topic: announcements
title: Rimozione di spoofing e risposta POP via e-mail
description: Stiamo apportando due modifiche al modo in cui Adobe Workfront invia e riceve le e-mail con la versione 20.3 (prevista per agosto 2020).
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Spoofing e risposta POP per e-mail

Stiamo apportando due modifiche al modo in cui Adobe Workfront invia e riceve le e-mail con la versione 20.3 (prevista per agosto 2020).

## E-mail in uscita da Workfront

Nel tentativo di aumentare la consegna di e-mail con successo, verrà eliminato lo spoofing delle e-mail, che viene spesso taggato come spam (consulta Spoofing delle e-mail). Tutte le e-mail da Workfront verranno inviate da notifications@my.workfront.com, inclusi gli avvisi automatizzati e la comunicazione utente-utente. Un esempio di e-mail di Joan Harris apparirà così nell&#39;area della tua e-mail:

![](assets/noreply.png)

*Consigliamo vivamente di contattare il team IT* per assicurarti che le e-mail da notifications@my.workfront.com non vengano bloccate per le e-mail in arrivo sul tuo sistema. È inoltre possibile fare riferimento a [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) per informazioni dettagliate su quali indirizzi IP provengono dal traffico e dall’e-mail.

## Risposte e-mail in entrata alle notifiche (risposta POP)

Alcune notifiche e-mail consentono agli utenti di rispondere tramite e-mail e fanno sì che la risposta venga copiata in Workfront come risposta di commento nel sistema Workfront. Gli amministratori di sistema di Workfront sono stati tradizionalmente in grado di scegliere se fornire il proprio server e-mail POP per ricevere tali risposte o utilizzare il sistema di risposta Workfront integrato. La scelta del server e-mail POP personalizzato verrà rimossa con la versione 20.3. A tutti gli account configurati per utilizzare un server personalizzato verrà automaticamente eseguita la transizione per utilizzare il sistema di risposta e-mail nativo di Workfront. Non è necessaria alcuna azione per gli amministratori di sistema o altri utenti di Workfront.

Non ci saranno modifiche alle e-mail provenienti direttamente dal sistema di prova Workfront. Continuerai a ricevere queste e-mail come in passato.

Se hai altre domande o dubbi, contatta il [Team di supporto Workfront](https://one.workfront.com/s/support?language=en_US).
