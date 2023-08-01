---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Risolvere i problemi relativi all’integrazione di Adobe Experience Manager
description: Collega il tuo lavoro con i contenuti di Experience Manager Assets Essentials - MODIFICA.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: e4bf79b8c5d53870aec6d415510acccb53a5c7f6
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Risoluzione dei problemi relativi all’integrazione di Adobe Experience Manager

## Problema: le risorse non vengono salvate in Adobe Experience Manager

Quando un utente seleziona una risorsa o una cartella da esportare in Experience Manager Assets e fa clic su Seleziona, la finestra del selettore si chiude ma le risorse non vengono salvate in Experience Manager Assets. In Workfront non vi è alcuna indicazione che le risorse non siano state salvate in Experience Manager Assets.

### Causa

Ciò può verificarsi a causa del inserisco nell&#39;elenco Consentiti di in Adobe Cloud Manager. Se l’Adobe di elenco Consentiti di Cloud Manager è vuoto, gli indirizzi IP non sono limitati e Workfront può accedere alle cartelle e alle risorse dell’organizzazione in Adobe Experience Manager. Tuttavia, se viene aggiunto anche un singolo indirizzo IP al inserire nell&#39;elenco Consentiti inserisco nell&#39;elenco Consentiti di di Cloud Manager, il processo di presuppone che non sia consentito alcun indirizzo IP non presente nell’elenco. Pertanto, se il inserisco nell&#39;elenco Consentiti di di Cloud Manager include qualsiasi indirizzo IP, è necessario aggiungere anche gli indirizzi IP di Workfront al inserisco nell&#39;elenco Consentiti di per consentire a Workfront di inviare risorse a Experience Manager Assets.

### Soluzione:

Aggiungi gli indirizzi IP di Workfront all’Adobe inserii nell&#39;elenco Consentiti Cloud Manager di.

* Per istruzioni sull’aggiunta di indirizzi IP all’Adobe Cloud Manager, consulta [Introduzione agli Elenchi consentiti IP](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction.html?lang=en) nella documentazione di Adobe Experience Manager.
* Per un elenco degli indirizzi IP di Workfront da aggiungere al inserisco nell&#39;elenco Consentiti di, consulta [Configurare il firewall](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).


