---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: "Messaggio di errore durante l'esecuzione di un report: 'Non hai effettuato l'accesso.'"
description: 'Per eseguire i passaggi di questo articolo, è necessario disporre del seguente accesso: MODIFICA ME.'
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 4%

---

# Messaggio di errore durante l&#39;esecuzione di un report: &quot;Al momento non hai effettuato l&#39;accesso.&quot;

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano, Lavoro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Problema

Quando si esegue un report o lo si visualizza in un dashboard, viene restituito il seguente errore:\
*Riproviamo. Non si è al momento connessi.*

Nel rapporto non vengono visualizzati risultati.

## Causa

Il rapporto è attualmente impostato per essere eseguito come utente disattivato.

## Soluzione

Per poter modificare le impostazioni del rapporto, è necessario disporre delle autorizzazioni Gestisci per il rapporto.\
Per regolare il rapporto e visualizzare i risultati:

1. Vai al rapporto.
1. Fai clic su **Azioni dei rapporti** > **Modifica** > **Impostazioni dei rapporti**.

1. Specifica il nome di un utente attivo nel **Esegui questo rapporto con i diritti di accesso di:** campo .\
   Oppure\
   Lascia la **Esegui questo rapporto con i diritti di accesso di:** campo vuoto.

1. Fai clic su **Fine**.
1. Fai clic su **Salva e chiudi**.\
   L&#39;errore non deve essere visualizzato nuovamente durante l&#39;esecuzione del report.
