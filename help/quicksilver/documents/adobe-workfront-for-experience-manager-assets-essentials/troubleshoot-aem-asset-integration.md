---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Risolvere i problemi relativi all’integrazione di Adobe Experience Manager
description: 'Problema: Assets non vengono salvati in Adobe Experience Manager'
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Risolvere i problemi relativi all’integrazione di Adobe Experience Manager

## Problema: Assets non vengono salvati in Adobe Experience Manager

Quando un utente seleziona una risorsa o una cartella da esportare in Experience Manager Assets e fa clic su Seleziona, la finestra del selettore si chiude ma le risorse non vengono salvate in Experience Manager Assets. In Workfront non vi è alcuna indicazione che le risorse non siano state salvate in Experience Manager Assets.

### Causa

Ciò può verificarsi a causa del inserisco nell&#39;elenco Consentiti di in Adobe Cloud Manager. Se il Adobe di Cloud Manager di inserire nell&#39;elenco Consentiti è vuoto, gli indirizzi IP non sono limitati e Workfront può accedere alle cartelle e alle risorse dell’organizzazione in Adobe Experience Manager. Tuttavia, se al Cloud Manager di inserire nell&#39;elenco Consentiti viene aggiunto anche un solo indirizzo IP, il inserisco nell&#39;elenco Consentiti di presuppone che non sia consentito alcun indirizzo IP non presente nell’elenco. Pertanto, se il Cloud Manager di di inserire nell&#39;elenco Consentiti include qualsiasi indirizzo IP, è necessario aggiungere anche gli indirizzi IP di Workfront inserire nell&#39;elenco Consentiti al per consentire a Workfront di inviare risorse a Experience Manager Assets.

### Soluzione:

Aggiungi gli indirizzi IP di Workfront al inserisco nell&#39;elenco Consentiti Adobe Cloud Manager.

* Per istruzioni sull&#39;aggiunta di indirizzi IP al Cloud Manager di Adobe, vedi [Introduzione agli Elenchi consentiti IP](https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction) nella documentazione di Adobe Experience Manager.
* Per un elenco degli indirizzi IP di Workfront da aggiungere al inserisco nell&#39;elenco Consentiti di, vedere [Configurare il firewall](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
