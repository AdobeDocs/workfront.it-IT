---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza: percentuale ruolo utente della disponibilità FTE"
description: È possibile aggiungere una colonna alla vista di un elenco di utenti per visualizzare un elenco dei Ruoli a cui l’utente è associato, nonché la percentuale di disponibilità FTE per ogni Ruolo, come definito nel profilo utente.
author: Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 66de6c952272f52876f8e912c96d1526575b6f0b
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Visualizza: percentuale di disponibilità FTE per il ruolo utente

<!--Audited: 11/2024-->

È possibile aggiungere una colonna alla vista di un elenco di utenti per visualizzare un elenco dei Ruoli a cui l’utente è associato, nonché la percentuale di disponibilità FTE per ogni Ruolo, come definito nel profilo utente.

Per informazioni sulla definizione della percentuale di disponibilità FTE per gli utenti, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![utente_con_percentuale_disponibilità_per_ruolo.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p> Corrente: 
   <ul>
   <li>Richiesta di modifica di una vista</li> 
   <li>Pianificare la modifica di un rapporto</li>
   </ul>
     </p>
     <p> Nuovo: 
   <ul>
   <li>Collaboratore per modificare una visualizzazione</li> 
   <li>Standard per modificare un rapporto</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizza percentuale di disponibilità FTE per Ruolo utente

1. Consente di passare a un elenco di utenti.
1. Dal menu a discesa **Visualizza**, selezionare **Nuova visualizzazione**.

1. Nell&#39;area **Anteprima colonna** fare clic su **Aggiungi colonna**.

1. Fai clic sull&#39;intestazione della nuova colonna, quindi fai clic su **Passa a modalità testo** > **Modifica modalità testo**.
1. Rimuovere il testo trovato nella casella **Modifica modalità testo** e sostituirlo con il seguente codice:

   ```
   displayname=Roles Time Percentage
   listdelimiter=
   listmethod=nested(userRoles).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({role},'-',{timePercentage},'%')
   valueformat=HTML
   ```

1. Fai clic su **Fine**, quindi su **Salva visualizzazione**.

1. (Facoltativo) Aggiorna il nome della visualizzazione, quindi fai clic su **Salva visualizzazione**.
