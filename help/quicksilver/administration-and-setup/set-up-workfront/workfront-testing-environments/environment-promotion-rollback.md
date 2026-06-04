---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Ripristinare la versione precedente di un pacchetto di promozione dell’ambiente
description: La funzionalità di promozione dell’ambiente ha lo scopo di consentire lo spostamento di oggetti correlati alla configurazione da un ambiente all’altro. Scopri come ripristinare un pacchetto di promozione installato da un ambiente di destinazione.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 70f7e2a8-bb27-4546-afb7-53e0eec30bf1
TQID: https://experienceleague.adobe.com/EPjuu-mWZH31cMvN-4tdzD8X-YFoW-DJ6YhfnJ0u06k
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 389
ht-degree: 7%

---

# Ripristinare la versione precedente di un pacchetto di promozione dell’ambiente



Dopo aver installato un pacchetto, puoi ripristinarlo. In questo modo vengono rimosse le modifiche apportate dal pacchetto nell&#39;ambiente di destinazione e vengono ripristinate le configurazioni precedenti degli oggetti interessati.

È possibile eseguire il rollback di un pacchetto promozionale entro 24 ore dall’installazione. Dopo 24 ore, la funzionalità di rollback non è più disponibile per tale installazione.

## Requisiti di accesso

Devi avere i seguenti:

<table>
  <tr>
   <td>Pacchetto Adobe Workfront
   </td>
   <td> <p>PRIME o ULTIMATE</p>
   </td>
  </tr>
  <tr>
   <td><strong>Licenze Workfront</strong>
   </td>
   <td> <p>Standard</p>&gt;
   </td>
  </tr>
   <tr>
   <td>Configurazioni del livello di accesso
   </td>
   <td><p>Devi essere un amministratore di Workfront.</p>
   </td>
  </tr>
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisiti

* Per poter eseguire il rollback di un pacchetto di promozione dell’ambiente, è necessario installarlo.

  Per istruzioni, vedere [Installare un pacchetto di promozione dell&#39;ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).


## Determinare se è possibile eseguire il rollback di una distribuzione di pacchetto specifica

Per sapere se è possibile eseguire il rollback di una specifica distribuzione di pacchetti, considera quanto segue:

* Sono trascorse meno di 24 ore dall’installazione del pacchetto.
* È possibile eseguire il rollback solo della distribuzione più recente del pacchetto.
* È possibile eseguire il rollback di una distribuzione non riuscita.
* Impossibile eseguire il rollback dei rollback.


## Ripristino dello stato precedente di un pacchetto di promozione dell’ambiente installato

1. Passa all’ambiente in cui è stato installato il pacchetto.
1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic sull&#39;icona **[!UICONTROL Setup]** ![Setup](/help/_includes/assets/gear-icon-setup.png).
1. Seleziona **Promozione ambiente** nel menu di navigazione a sinistra.
1. Selezionare il pacchetto di cui si desidera eseguire il rollback e fare clic su **Distribuzioni**.
1. Passa il puntatore del mouse sulla distribuzione (installazione) di cui vuoi eseguire il rollback, quindi fai clic su Ripristina versione precedente quando viene visualizzato a destra della riga della distribuzione.

   Oppure

   Fai clic sulla distribuzione di cui vuoi eseguire il rollback, quindi fai clic su **Ripristina pacchetto** nell&#39;angolo superiore destro della schermata.

   >[!IMPORTANT]
   >
   >La distribuzione deve essersi verificata meno di 24 ore prima del rollback. Non è possibile eseguire il rollback delle installazioni che hanno più di 24 ore.

1. (Facoltativo) Nell’area Anteprima rollback, visualizza le modifiche che si verificheranno quando viene eseguito il rollback della distribuzione.
1. Fai clic su **Ripristina versione precedente** nell&#39;angolo superiore destro dello schermo.
