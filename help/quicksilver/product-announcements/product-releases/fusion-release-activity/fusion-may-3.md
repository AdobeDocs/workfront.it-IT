---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: '''Attività di rilascio di Workfront Fusion: 3 maggio 2021"'
description: Questa pagina descrive tutti i miglioramenti effettuati in Adobe Workfront Fusion la settimana del 3 maggio 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: af3312c5-3416-4c03-8528-6a2c0240110e
hidefromtoc: true
source-git-commit: 9c2321794c5ba773bfda1d6e9dfda6b8de1a1449
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# Attività di rilascio di Workfront Fusion: settimana 3 maggio 2021

Questa pagina descrive tutti i miglioramenti effettuati in Adobe Workfront Fusion la settimana del 3 maggio 2021.

Per un elenco di tutte le modifiche recenti, vedi [Attività di rilascio di Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Per un elenco delle correzioni di bug recenti in Workfront Fusion, vedi [Aggiornamenti alla manutenzione di Workfront](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) e controlla eventuali aggiornamenti etichettati Workfront Fusion Maintenance Update.

## Il connettore Salesforce può ora eseguire ricerche utilizzando SOQL

Il modulo Salesforce > Cerca record ora ha l’opzione di cercare utilizzando SOQL (Salesforce Object Query Language). È inoltre possibile eseguire ricerche utilizzando le opzioni disponibili in precedenza (SOSL e ricerche semplici).

Per ulteriori informazioni, consulta [Moduli Salesforce](../../../workfront-fusion/apps-and-their-modules/salesforce-modules.md).

## Il nuovo tipo di connessione nel connettore Azure DevOps richiede meno ambiti

Per migliorare la sicurezza, è stato aggiunto un nuovo tipo di connettore al connettore Workfront Fusion Azure DevOps. Ora, quando crei una connessione in un modulo DevOps di Azure, puoi scegliere tra due tipi di connessioni:

* DevOps di Azure

   Questo nuovo tipo di connessione limita gli ambiti a quelli specificamente necessari per Workfront Fusion.

* Azure DevOps (Richiedi tutti gli ambiti)

   Questo è il tipo di connessione legacy, che richiede tutti gli ambiti disponibili in una connessione ad Azure DevOps.

È consigliabile utilizzare il tipo di connessione Azure DevOps in tutti i nuovi scenari che utilizzano Azure DevOps. È inoltre consigliabile modificare qualsiasi modulo Azure DevOps negli scenari esistenti per utilizzare il nuovo tipo di connessione. Il tipo di connessione legacy Azure DevOps (Richiedi tutti gli ambiti) diventerà obsoleto nel prossimo futuro.

Per ulteriori informazioni, consulta [Moduli Azure DevOps](../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md).
