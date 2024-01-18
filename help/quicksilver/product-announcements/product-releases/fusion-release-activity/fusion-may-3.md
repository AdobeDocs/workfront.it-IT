---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: "Attività di rilascio di Workfront Fusion: settimana del 3 maggio 2021"
description: Questa pagina descrive tutti i miglioramenti apportati ad Adobe Workfront Fusion la settimana del 3 maggio 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: af3312c5-3416-4c03-8528-6a2c0240110e
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Attività di rilascio di Workfront Fusion: settimana del 3 maggio 2021

Questa pagina descrive tutti i miglioramenti apportati ad Adobe Workfront Fusion la settimana del 3 maggio 2021.

Per un elenco di tutte le modifiche recenti, vedi [Attività di rilascio di Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Per un elenco delle correzioni di bug recenti in Workfront Fusion, vedi [Aggiornamenti di manutenzione per Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) e verificare la presenza di eventuali aggiornamenti etichettati Aggiornamento di manutenzione di Workfront Fusion.

## Il connettore Salesforce può ora effettuare ricerche utilizzando SOQL

Il modulo Salesforce > Cerca record dispone ora dell’opzione per eseguire ricerche utilizzando SOQL (Salesforce Object Query Language). È inoltre possibile eseguire ricerche utilizzando le opzioni disponibili in precedenza (SOSL e ricerche semplici).

Per ulteriori informazioni, consulta [Moduli Salesforce](../../../workfront-fusion/apps-and-their-modules/salesforce-modules.md).

## Il nuovo tipo di connessione nel connettore DevOps di Azure richiede un numero inferiore di ambiti

Per migliorare la sicurezza, è stato aggiunto un nuovo tipo di connettore al connettore DevOps di Workfront Fusion Azure. Ora, quando crei una connessione in un modulo DevOps di Azure, puoi selezionare tra due tipi di connessioni:

* Azure DevOps

  Questo nuovo tipo di connessione limita gli ambiti a quelli specificamente necessari per Workfront Fusion.

* Azure DevOps (Richiedi tutti gli ambiti)

  Si tratta del tipo di connessione legacy, che richiede tutti gli ambiti disponibili in una connessione ad Azure DevOps.

È consigliabile utilizzare il tipo di connessione DevOps di Azure in tutti i nuovi scenari che utilizzano DevOps di Azure. È inoltre consigliabile modificare i moduli DevOps di Azure negli scenari esistenti per utilizzare il nuovo tipo di connessione. Il tipo di connessione legacy Azure DevOps (Richiedi tutti gli ambiti) diventerà obsoleto nel prossimo futuro.

Per ulteriori informazioni, consulta [Moduli DevOps di Azure](../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md).
