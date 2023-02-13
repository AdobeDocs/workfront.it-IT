---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '"Messaggio di errore sul calendario: ''Questo calendario ha i diritti di visualizzazione di un utente disattivato''".'
description: 'Per eseguire i passaggi di questo articolo, è necessario disporre del seguente accesso: MODIFICA ME.'
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 5%

---

# Messaggio di errore nel calendario: &quot;Questo calendario dispone dei diritti di visualizzazione di un utente disattivato.&quot;

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
   <td> <p>Gestire le autorizzazioni in un calendario</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Problema

Ricevi il seguente errore quando accedi a un calendario condiviso con te: 

*Questo calendario ha i diritti di visualizzazione di un utente disattivato. Richiedere a un amministratore di sistemare i privilegi del calendario.*

## Causa

L&#39;utente che ha creato questo calendario (il relativo proprietario originale) è un utente che è stato disattivato. 

## Soluzione

Puoi risolvere il problema nel modo seguente:

1. Copia il calendario originale. Quando si copia un calendario, si diventa il proprietario del calendario. Il calendario copiato deve mostrare tutte le informazioni del calendario originale.\
   Per ulteriori informazioni sulla copia di un calendario, consulta [Copiare un rapporto sul calendario](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. Condividi il calendario copiato con gli stessi utenti del calendario originale. Tutti gli utenti devono visualizzare le stesse informazioni nel nuovo calendario.
1. (Facoltativo e condizionale) Se si dispone delle autorizzazioni per gestire il calendario originale, rimuovere dall&#39;area Condivisione calendario tutti gli altri utenti con cui è condiviso il calendario. Questo elimina la confusione causata dal tentativo degli utenti di visualizzare il calendario errato.
