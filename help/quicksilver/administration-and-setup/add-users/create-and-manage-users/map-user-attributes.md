---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Mappa attributi utente
description: Utilizzando il Single Sign-On (SSO), è possibile passare gli attributi da Active Directory del provider di identità agli utenti di Adobe Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
TQID: https://experienceleague.adobe.com/nuU1cn2BDPN7k-gr7a3t5JFR54zD9gHaxBeESEL53p0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 595
ht-degree: 6%

---

# Mappare gli attributi utente

<!--Audited 2/2024-->

Utilizzando il Single Sign-On (SSO), è possibile passare gli attributi da Active Directory del provider di identità agli utenti di Adobe Workfront.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td><p>Standard</p><p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td><p>Devi essere un amministratore di Workfront</p></td>
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Suggerimenti per la mappatura degli attributi

Quando mappate gli attributi, tenete presente quanto segue:

* Esegui sempre il test in una sandbox di anteprima o di aggiornamento cliente (CR).
* Eseguire il test con gli account amministratore e non amministratore per verificare che gli attributi vengano mappati correttamente.
* Gli attributi mappati vengono applicati ogni volta che un utente accede tramite single sign-on.

  Esempio: se mappi &quot;cognome&quot; e aggiorni il loro nome in Workfront senza aggiornare il valore nel loro provider di identità, il cognome verrà sovrascritto in modo che corrisponda al valore di qualsiasi elemento presente nel provider di identità alla successiva connessione dell’utente.

## Mappare gli attributi utente per la tua organizzazione

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-left.png) nell&#39;angolo superiore sinistro di Adobe Workfront, quindi fai clic sull&#39;icona **Setup** ![Gear settings](assets/gear-icon-settings.png).

1. Fare clic su **Sistema** > **Single Sign-On (SSO)**.

1. Selezionare la scheda **Adobe**.

1. (Facoltativo e condizionale) Se per la tua organizzazione è stata configurata la mappatura degli attributi nell&#39;esperienza classica e desideri copiarla nell&#39;esperienza unificata di Adobe, fai clic su **Migra mappature**. Puoi quindi eliminare, eliminare o modificare queste mappature.

   >[!NOTE]
   >
   >È consigliabile eseguire la migrazione delle mappature la prima volta che le si configura nell’esperienza unificata di Adobe. Non c&#39;è alcun danno nel migrarli di nuovo in un secondo momento, ma migrarli più di una volta non è necessario.

1. Per creare un nuovo mapping di attributi, fare clic su **Aggiungi mapping**.

1. Fare clic sulla freccia accanto al nome del campo Workfront e selezionare il campo [!DNL Workfront] che si desidera mappare.

1. (Facoltativo) Se si desidera creare più regole per un determinato campo, fare clic sulla freccia accanto a **Sempre** e selezionare l&#39;operatore che si desidera utilizzare per la regola.

1. (Condizionale) Se hai selezionato un operatore oltre a Sempre, seleziona il campo Workfront e il valore a cui si applica l’operatore.

   >[!NOTE]
   >
   >Gli operatori `Is Truthy` e `Is Falsy` non richiedono valori.

1. Seleziona se desideri applicare il valore di un attributo nel gestore identità al campo Workfront o se desideri applicare un valore costante specifico.

1. Immettere il nome del campo Identity Manager che si desidera applicare oppure immettere il testo del valore costante che si desidera applicare.

1. (Facoltativo) Per aggiungere altre regole per lo stesso campo Workfront, fai clic su **Aggiungi nuova regola** e segui i passaggi 4-9.

   >[!IMPORTANT]
   >
   > * Qualsiasi regola al di sotto di una regola Always verrà ignorata. Se si dispone di una regola Always, è necessario spostarla in fondo all&#39;elenco delle regole. Per spostare le regole nell’elenco, fai clic sul menu a tre punti a destra della regola e spostale verso l’alto o verso il basso.
   > * Per creare una regola al centro dell&#39;elenco, fai clic sul menu a tre punti accanto alla regola che desideri posizionare al di sopra o al di sotto della nuova regola e seleziona **Aggiungi regola al di sopra di** o **Aggiungi regola al di sotto di**.

1. Per eliminare una regola, fare clic sul menu a tre punti accanto alla regola che si desidera eliminare e selezionare **Elimina**.
1. Per eliminare una mappatura, fai clic sull&#39;icona **Elimina** presente nella scheda della mappatura.

1. Per salvare, scorri fino alla parte superiore della pagina e fai clic su **Salva**.


