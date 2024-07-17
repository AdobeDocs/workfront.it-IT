---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizzazione: percentuale di disponibilità dell''FTE nel ruolo lavorativo dell''utente'''
description: È possibile aggiungere una colonna alla visualizzazione di un elenco di utenti per visualizzare un elenco dei ruoli professionali a cui è associato l'utente, nonché la percentuale di disponibilità di FTE per ciascun ruolo professionale, come definito nel profilo utente.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Visualizza: percentuale di disponibilità FTE per il ruolo utente

È possibile aggiungere una colonna alla vista di un elenco di utenti per visualizzare un elenco dei Ruoli a cui l’utente è associato, nonché la percentuale di disponibilità FTE per ogni Ruolo, come definito nel profilo utente.

Per informazioni sulla definizione della percentuale di disponibilità FTE per gli utenti, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![user_with_percent_avialbility_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## Requisiti di accesso

Per eseguire la procedura descritta in questo articolo, è necessario disporre dell&#39;accesso seguente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualunque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta di modifica di una visualizzazione </p>
   <p>Pianificare la modifica di un report</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> <p><b>NOTA</b>

Se non hai ancora accesso, chiedi all&#39;amministratore di Workfront se imposta ulteriori restrizioni nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli</a> di accesso personalizzati.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un report</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere di quale piano, tipo di licenza o accesso disponi, contatta l&#39;amministratore di Workfront.

## Visualizzazione della percentuale di disponibilità dell&#39;FTE nel ruolo lavorativo dell&#39;utente

1. Vai a un elenco di utenti.
1. Dal menu a discesa **Visualizza**, selezionare **Nuova visualizzazione**.

1. Nell&#39;area **Anteprima colonna** fare clic su **Aggiungi colonna**.

1. Fai clic sull&#39;intestazione della nuova colonna, quindi fai clic su **Passa alla modalità** testo.
1. Posizionare il mouse sull&#39;area della modalità testo e fare clic su Fare clic **per modificare il testo**.
1. Rimuovere il testo trovato nella **casella Modalità** testo e sostituirlo con il codice riportato di seguito:
   <pre>displayname=Ruoli Percentuale<br>tempo listdelimiter=<p><br>listmethod=nested(userRoles).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({role},'-',{timePercentage},'%')<br>valueformat=HTML</pre>

1. Fate clic su Salva **, quindi** su **Salva vista**.

1. (Facoltativo) Specifica un nome per la visualizzazione, quindi fai clic su **Salva visualizzazione**.
