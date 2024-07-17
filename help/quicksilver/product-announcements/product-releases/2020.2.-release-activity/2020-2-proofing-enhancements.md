---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: Miglioramenti alla bozza 2020.2
description: Questa pagina descrive tutti i miglioramenti apportati all’ambiente di produzione con la versione 2020.2. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana dell’11 maggio 2020.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 021c6e0c-3593-40f7-8eeb-7e016001893e
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# Miglioramenti alla bozza 2020.2

Questa pagina descrive tutti i miglioramenti apportati all’ambiente di produzione con la versione 2020.2. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana dell’11 maggio 2020.

Per un elenco di tutte le modifiche disponibili con la versione 2020.2, consulta [Panoramica sulla versione 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Il dominio di verifica sta cambiando da proofhq.com a workfront.com.

>[!NOTE]
>
>Questa funzione è stata originariamente comunicata come parte della versione 2020.1 di, ma è stata rimossa dalla versione prima del rilascio in produzione.

Se il firewall o il server di posta è configurato in modo da consentire l&#39;accesso solo a fornitori specifici, è necessario aggiungere il seguente URL aggiuntivo al inserisco nell&#39;elenco Consentiti per garantire che gli utenti dell&#39;organizzazione possano visualizzare le bozze in Workfront sia nel visualizzatore di bozze del browser che nel visualizzatore di bozze del desktop:

&#42;.workfront.com

Anche l&#39;URL &#42;proofhq.com è obbligatorio.

Per ulteriori informazioni sull&#39;aggiornamento del inserisco nell&#39;elenco Consentiti di installazione del firewall, vedere [Configurare il inserisco nell&#39;elenco Consentiti di installazione del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Questo aggiornamento si applica solo alla verifica in Workfront; non si applica quando si utilizza l’applicazione autonoma Workfront Proof.

## I commenti degli utenti invitati alle bozze vengono visualizzati nell&#39;area Aggiornamenti

Per semplificare la collaborazione sulle bozze, i commenti degli ospiti vengono visualizzati nell’area Aggiornamenti.

In precedenza, i commenti degli ospiti sulle bozze erano disponibili solo all’interno della bozza.
