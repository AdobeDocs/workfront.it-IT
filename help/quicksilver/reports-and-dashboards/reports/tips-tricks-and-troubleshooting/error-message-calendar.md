---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: "Messaggio di errore sul calendario: 'Questo calendario dispone dei diritti di visualizzazione di un utente disattivato.'"
description: Scopri di più sul messaggio di errore "Questo calendario dispone dei diritti di visualizzazione di un utente disattivato".
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 5%

---

# Messaggio di errore sul calendario: &quot;Questo calendario dispone dei diritti di visualizzazione di un utente disattivato.&quot;

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano, Lavoro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un calendario</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Problema

Quando si accede a un calendario condiviso con l&#39;utente viene visualizzato il messaggio di errore seguente: 

*Questo calendario ha i diritti di visualizzazione di un utente disattivato. Richiedere a un amministratore di sistemare i privilegi del calendario.*

## Causa

L&#39;utente che ha creato il calendario (proprietario originale) è un utente che è stato disattivato. 

## Soluzione

Puoi risolvere il problema nel modo seguente:

1. Copia il calendario originale. Quando si copia un calendario, l&#39;utente diventa il proprietario del calendario. Il calendario copiato deve mostrare tutte le informazioni del calendario originale.\
   Per ulteriori informazioni sulla copia di un calendario, vedere [Copiare un report calendario](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. Condividere il calendario copiato con gli stessi utenti del calendario originale. Tutti gli utenti devono visualizzare le stesse informazioni nel nuovo calendario.
1. (Facoltativo e condizionale) Se si dispone delle autorizzazioni per gestire il calendario originale, rimuovere tutti gli altri utenti con cui il calendario è condiviso dall&#39;area Condivisione calendario. In questo modo si evita di confondere gli utenti che tentano di visualizzare un calendario errato.
