---
content-type: reference
navigation-topic: announcements
title: Modifica necessaria per aggiungere le bozze al inserisco nell'elenco Consentiti di lavoro di un’organizzazione
description: Il dominio di verifica sta cambiando da proofhq.com a workfront.com.
author: Luke
feature: Product Announcements
exl-id: 05a1fd37-224b-4a0b-abef-4d9a015de524
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Modifica necessaria per aggiungere le bozze al inserisco nell&#39;elenco Consentiti di lavoro di un’organizzazione

Il dominio di verifica sta modificando from proofhq.com in workfront.com.

Se il firewall o il server di posta è configurato in modo da consentire l’accesso solo a fornitori specifici, è necessario aggiungere il seguente URL aggiuntivo al inserisco nell&#39;elenco Consentiti per garantire che gli utenti dell’organizzazione possano visualizzare le bozze all’interno di Adobe Workfront sia nel visualizzatore di bozze del browser che nel visualizzatore di bozze del desktop:

&#42;.workfront.com

Anche l&#39;URL &#42;proofhq.com è obbligatorio.

Per ulteriori informazioni sull&#39;aggiornamento del inserisco nell&#39;elenco Consentiti di installazione del firewall, vedere [Configurare il inserisco nell&#39;elenco Consentiti di installazione del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>Questo aggiornamento si applica solo alla verifica in Workfront; non si applica quando si utilizza l’applicazione autonoma Workfront Proof.
