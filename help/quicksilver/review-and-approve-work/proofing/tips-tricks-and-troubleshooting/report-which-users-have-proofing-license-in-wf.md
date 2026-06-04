---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Elencare gli utenti con una licenza di bozza in Adobe Workfront
description: Puoi visualizzare quali utenti in Adobe Workfront dispongono attualmente dell’opzione "L’utente può generare delle bozze" abilitata in uno dei seguenti modi.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
TQID: https://experienceleague.adobe.com/9P5Bp9TrJ1ECSwpK7C4AW4rQlTQOBH4U7-CPYl92RKU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 312
ht-degree: 20%

---

# Elencare gli utenti con una licenza di bozza in Adobe Workfront

Puoi visualizzare quali utenti in Adobe Workfront dispongono attualmente dell’opzione &quot;L’utente può generare delle bozze&quot; abilitata in uno dei seguenti modi.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

Per eseguire i passaggi descritti in questo articolo, devi disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> 
   <p>Standard</p> 
   <p>Piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Modifica accesso a:</p> 
    <ul> 
     <li> <p>Creare rapporti, dashboard e calendari</p> </li> 
     <li> <p>Creare filtri, visualizzazioni e raggruppamenti</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare un rapporto utente

Puoi creare un rapporto utente per visualizzare quali utenti possono generare le bozze:

1. Passa all&#39;area **Reporting**.
1. Fai clic sul menu a discesa **Nuovo report**, quindi fai clic su **Report utente**.

1. Nella scheda **Filtri**, fai clic su **Aggiungi regola filtro**.

1. Nel campo disponibile, espandi **Utente**, quindi fai clic su **Ha licenza Verifica**.

1. Seleziona **Uguale** > **Vero**.

   ![prooflicenses.png](assets/report-prooflicenses-350x135.png)

1. Fai clic su **Salva+Chiudi**.

   Nel report vengono visualizzati tutti gli utenti di Workfront a cui è stata assegnata una licenza di verifica.

## Aggiornare la visualizzazione Persone

È possibile aggiungere una nuova colonna nella vista Persone per visualizzare quali utenti possono generare le bozze:

1. Vai all&#39;area **Persone**.
1. Fare clic sulla scheda **Persone**.
1. Nel menu a discesa **Visualizza** eseguire una delle operazioni seguenti:

   * Per aggiungere queste informazioni a una visualizzazione esistente, selezionare la visualizzazione da personalizzare, quindi fare clic su **Personalizza visualizzazione**.
   * Per aggiungere queste informazioni a una nuova visualizzazione, fare clic su **Nuova visualizzazione**.

1. Fai clic su **Aggiungi colonna**.
1. Nel campo disponibile, espandi **Utente**, quindi fai clic su **Ha licenza Verifica**.

1. Fai clic su **Fine**, quindi fai clic su **Salva visualizzazione** o **Salva come nuova visualizzazione**.

   La visualizzazione visualizza **True** o **False** a seconda che all&#39;utente sia stata assegnata una licenza di verifica.
