---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza: percentuale di disponibilità FTE per ruolo utente"
description: È possibile aggiungere una colonna alla vista di un elenco di utenti per visualizzare un elenco dei Ruoli a cui l’utente è associato, nonché la percentuale di disponibilità FTE per ogni Ruolo, come definito nel profilo utente.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# Visualizza: percentuale di disponibilità FTE per il ruolo utente

È possibile aggiungere una colonna alla vista di un elenco di utenti per visualizzare un elenco dei Ruoli a cui l’utente è associato, nonché la percentuale di disponibilità FTE per ogni Ruolo, come definito nel profilo utente.

Per informazioni sulla definizione della percentuale di disponibilità FTE per gli utenti, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![user_with_percent_availability_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta di modifica di una vista </p>
   <p>Pianificare la modifica di un rapporto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Visualizza percentuale di disponibilità FTE per Ruolo utente

1. Consente di passare a un elenco di utenti.
1. Dalla sezione **Visualizza** menu a discesa, seleziona **Nuova visualizzazione**.

1. In **Anteprima colonna** , fare clic su **Aggiungi colonna**.

1. Fai clic sull’intestazione della nuova colonna, quindi fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull&#39;area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuove il testo trovato in **Modalità testo** e sostituirlo con il seguente codice:

   <pre>displayname=Percentuale tempo ruoli<br>listdelimiter=<p><br>listmethod=nested(userRoles).LISTS<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({role},'-',{timePercentage},'%')<br>valueformat=HTML</pre>

1. Clic **Salva**, quindi **Salva visualizzazione**.

1. (Facoltativo) Specifica un nome per la vista, quindi fai clic su **Salva visualizzazione**.
