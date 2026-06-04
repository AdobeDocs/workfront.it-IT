---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 - Miglioramenti per le bozze
description: Questa pagina descrive tutti i miglioramenti apportati all’ambiente di produzione con la versione 2020.2. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana dell’11 maggio 2020.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 021c6e0c-3593-40f7-8eeb-7e016001893e
TQID: https://experienceleague.adobe.com/Z86GWBBVdj1DPENzHS7wKI1ViRGFzov8L3sNtss4iJU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 2%

---

# 2020.2 - Miglioramenti per le bozze

Questa pagina descrive tutti i miglioramenti apportati all’ambiente di produzione con la versione 2020.2. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana dell’11 maggio 2020.

Per un elenco di tutte le modifiche disponibili con la versione 2020.2, consulta [Panoramica sulla versione 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Il dominio di verifica sta cambiando da proofhq.com a workfront.com.

>[!NOTE]
>
>Questa funzione è stata originariamente comunicata come parte della versione 2020.1 di, ma è stata rimossa dalla versione prima del rilascio in produzione.

Se il firewall o il server di posta è configurato in modo da consentire l&#39;accesso solo a fornitori specifici, è necessario aggiungere il seguente URL aggiuntivo al inserisco nell&#39;elenco Consentiti di verifica per assicurarsi che gli utenti dell&#39;organizzazione possano visualizzare le bozze all&#39;interno di Workfront sia nel visualizzatore di bozze del browser che nel visualizzatore di bozze del desktop:

&#42;.workfront.com

Anche l&#39;URL &#42;proofhq.com è obbligatorio.

Per ulteriori informazioni sull&#39;aggiornamento del inserisco nell&#39;elenco Consentiti di aggiornamento del tuo, consulta [Configurare il inserisco nell&#39;elenco Consentiti di aggiornamento del tuo firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Questo aggiornamento si applica solo alla verifica in Workfront; non si applica quando si utilizza l’applicazione autonoma Workfront Proof.

## I commenti degli utenti invitati alle bozze vengono visualizzati nell&#39;area Aggiornamenti

Per semplificare la collaborazione sulle bozze, i commenti degli ospiti vengono visualizzati nell’area Aggiornamenti.

In precedenza, i commenti degli ospiti sulle bozze erano disponibili solo all’interno della bozza.
