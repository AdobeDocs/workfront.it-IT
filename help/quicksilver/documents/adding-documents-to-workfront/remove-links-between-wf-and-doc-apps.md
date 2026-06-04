---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Rimuovere i collegamenti tra Adobe Workfront e i provider di archiviazione documenti esterni
description: Quando si carica un documento da un servizio per la prima volta, Adobe Workfront richiede l’autorizzazione all’utente per accedere al servizio documenti. Quando l’utente fornisce le credenziali del servizio documenti per effettuare l’accesso, il servizio si collega a Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: fce8e8aa-fc48-49e1-a71d-c3933a179cf5
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wDii-Gr-3a0NfMhc9VPfbiUNSTyJaJuFHeXACI26NxU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 384
ht-degree: 15%

---

# Rimuovere i collegamenti tra Adobe Workfront e i provider di archiviazione documenti esterni

Quando si carica un documento da un servizio per la prima volta, Adobe Workfront richiede l’autorizzazione all’utente per accedere al servizio documenti. Quando l’utente fornisce le credenziali del servizio documenti per effettuare l’accesso, il servizio si collega a Workfront.

Per informazioni sul collegamento di servizi di documentazione esterni a Workfront, vedere [Collegamento di documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Poiché il servizio documenti è quello che consente il collegamento a Workfront, non è possibile per Workfront rimuovere l&#39;autorizzazione concessa dal servizio documenti. È necessario rimuovere l’autorizzazione all’interno dell’applicazione del servizio di documentazione oppure chiamare il team di supporto per rimuovere il collegamento dai server.

>[!NOTE]
>
>Questa funzionalità non è disponibile nella nuova area Documenti.<br>
>Se la tua organizzazione utilizza l&#39;archiviazione cloud Adobe, quando accedi ai documenti in Workfront visualizzerai la nuova area Documenti. Per ulteriori informazioni sull&#39;archiviazione cloud di Adobe, consulta [Panoramica sull&#39;archiviazione cloud di Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td> 
   <p>Collaboratore o successiva</p>
   <p>Richiedente o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso in modifica ai documenti</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Rimuovere il collegamento tra Workfront e Dropbox

1. Accedi a Dropbox.
1. Fai clic sull&#39;immagine del tuo profilo nell&#39;angolo superiore destro, quindi fai clic su **Impostazioni**.
1. Fai clic sulla scheda **App collegate**, quindi scorri verso il basso fino a **App collegate**.

1. Fai clic su **X** accanto a Workfront.

## Rimuovere il collegamento tra Workfront e Box

1. Accedi al tuo account Box.
1. Fai clic sull’immagine del tuo profilo nell’angolo in alto a destra.
1. Fai clic su **Impostazioni account**, quindi sulla scheda **Sicurezza**.

1. Trova **MyWorkfront** e fai clic su **X** in Dimentica app.

## Rimuovere il collegamento tra Workfront e Google Drive

1. Accedi all&#39;unità Google.
1. Fai clic sull&#39;icona a forma di ingranaggio nell&#39;angolo superiore destro, quindi fai clic su **Impostazioni**.
1. Fai clic su **Gestisci app** a sinistra e trova **Workfront** nell&#39;elenco.

1. Nel menu a discesa Opzioni, fare clic su **Disconnetti dall&#39;unità**.

## Rimuovere i collegamenti tra Workfront e altri provider di archiviazione documenti

È necessario chiamare il team di supporto per disconnettere Microsoft One Drive o WebDAM da Workfront.

Per informazioni su come contattare il team di supporto, vedere [Contattare l&#39;assistenza clienti](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
