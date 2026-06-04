---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Risolvere i problemi relativi all’integrazione di Adobe Experience Manager
description: 'Problema: Assets non vengono salvati in Adobe Experience Manager'
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
TQID: https://experienceleague.adobe.com/VaiQnZXQe39sYlnJOblWoea9UwOaujEU3ME-jh7-0EI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 247
ht-degree: 0%

---

# Risolvere i problemi relativi all’integrazione di Adobe Experience Manager

## Problema: Assets non vengono salvati in Adobe Experience Manager

Quando un utente seleziona una risorsa o una cartella da esportare in Experience Manager Assets e fa clic su Seleziona, la finestra del selettore si chiude ma le risorse non vengono salvate in Experience Manager Assets. In Workfront non vi è alcuna indicazione che le risorse non siano state salvate in Experience Manager Assets.

### Causa

Ciò può verificarsi a causa del inserisco nell&#39;elenco Consentiti di in Adobe Cloud Manager. Se l’Adobe di inserire nell&#39;elenco Consentiti Cloud Manager per un’organizzazione è vuoto, gli indirizzi IP non sono limitati e Workfront può accedere alle cartelle e alle risorse dell’organizzazione in Adobe Experience Manager. Tuttavia, se all’Cloud Manager di inserire nell&#39;elenco Consentiti viene aggiunto anche un solo indirizzo IP, l’presuppone che non sia consentito nessun indirizzo IP non presente nell’elenco. Pertanto, se il Cloud Manager di di inserire nell&#39;elenco Consentiti include qualsiasi indirizzo IP, è necessario aggiungere anche gli indirizzi IP di Workfront all’per consentire a Workfront di inviare risorse a Experience Manager Assets.

### Soluzione:

Aggiungi gli indirizzi IP di Workfront al inserisco nell&#39;elenco Consentiti di Adobe Cloud Manager.

* Per istruzioni sull&#39;aggiunta di indirizzi IP al Cloud Manager di Adobe, vedi [Introduzione agli Elenchi consentiti IP](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction) nella documentazione di Adobe Experience Manager.
* Per un elenco degli indirizzi IP di Workfront da aggiungere al inserisco nell&#39;elenco Consentiti di, vedere [Configurare il firewall](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
