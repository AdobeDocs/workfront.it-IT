---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Come condividere gli oggetti senza generare notifiche
description: Scopri come condividere gli oggetti ed evitare l’invio di notifiche relative a questa modifica. Questa funzione è particolarmente utile quando si condividono oggetti in blocco.
author: Alina
feature: Get Started with Workfront
exl-id: 02106282-addb-4bdd-82d2-9da5a5f6a687
TQID: https://experienceleague.adobe.com/zhNlFwg-1UuNKXxqIj-H62rGdewhbqKHLz4NbzkEqP8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 577
ht-degree: 11%

---

# Come condividere gli oggetti senza generare notifiche

<!--Audited: 12/2024-->

Quando condividi un oggetto in Adobe Workfront, le persone con cui stai condividendo l’oggetto ricevono una notifica e-mail relativa alla condivisione.

Ricevere una notifica e-mail quando qualcuno condivide un oggetto con te è importante per essere consapevoli di questa modifica. Tuttavia, troppe notifiche potrebbero confondere eccessivamente gli utenti. Se si desidera condividere un numero elevato di oggetti con gli utenti contemporaneamente, la disattivazione temporanea delle notifiche consente di evitare confusione.

Le persone ricevono notifiche e-mail quando le seguenti impostazioni sono abilitate contemporaneamente:

* A livello di sistema o di gruppo è abilitata una o entrambe le notifiche di evento seguenti:

   * Condivisione oggetto con utente
   * La condivisione degli oggetti con il team è abilitata a livello di sistema o di gruppo.
* Nel profilo dell’utente è abilitata una o entrambe le seguenti notifiche e-mail:

   * Qualcuno condivide un oggetto con me
   * Qualcuno condivide un oggetto con il mio team

Se è necessario condividere più oggetti con più persone (in blocco), ma non si desidera che ricevano notifiche e-mail su questa modifica, eseguire le operazioni seguenti:

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore agli oggetti da condividere</p>
   <p>Modifica l'accesso agli utenti</p>
   <p><b>NOTA</b></p>
   <p> Per verificare lo stato delle notifiche degli eventi per il sistema o il gruppo, è necessario essere un amministratore di sistema o di gruppo</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Visualizzare le autorizzazioni o versioni successive per gli oggetti da condividere</p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Condividere gli oggetti senza generare notifiche

1. Verifica che le **Notifiche evento** seguenti siano abilitate a livello di sistema o di gruppo:

   * **Condivisione oggetto con utente**
   * **La condivisione degli oggetti con il team è abilitata a livello di sistema o di gruppo**.

   Per informazioni, vedere [Configurare le notifiche degli eventi per tutti gli utenti del sistema](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   Se queste notifiche di eventi non sono attivate, le notifiche relative alla condivisione di un oggetto non verranno inviate agli utenti. Se uno o entrambi sono abilitati, continua con i passaggi seguenti.

{{step-1-to-users}}

1. Seleziona più utenti nell&#39;elenco, quindi fai clic su **Notifiche** > **Varie**.
1. Disattiva una o entrambe le notifiche seguenti (a seconda di quelle abilitate a livello di sistema o di gruppo):

   * **Qualcuno condivide un oggetto con me**
   * **Qualcuno condivide un oggetto con il mio team**

   Prima di disabilitare gli utenti selezionati, assicurati che per tutti siano selezionate queste notifiche. In questo modo, dopo aver condiviso gli oggetti, è possibile riabilitarli in blocco per tutti gli oggetti.

1. Fai clic su **Salva modifiche**.
1. Vai a un elenco di oggetti che desideri condividere e seleziona gli oggetti, quindi fai clic sull&#39;icona **Condividi** nella parte superiore dell&#39;elenco.

   Per informazioni sulla condivisione di un oggetto in blocco, vedere [Condividere un oggetto](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

1. Torna all’elenco degli utenti per i quali hai disattivato le notifiche e seleziona gli stessi utenti.
1. Seleziona gli stessi utenti nell&#39;elenco, quindi fai clic su **Notifiche** > **Varie**.
1. Abilita una o entrambe le notifiche seguenti (a seconda di quali sono abilitate dal livello di sistema o di gruppo):

   * **Qualcuno condivide un oggetto con me**
   * **Qualcuno condivide un oggetto con il mio team**

1. Fai clic su **Salva modifiche**.

   Gli oggetti sono stati condivisi con gli utenti selezionati e nessuno di loro ha ricevuto notifiche e-mail relative a questa modifica.
