---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Messaggio di errore sul calendario: ''Questo calendario dispone dei diritti di visualizzazione di un utente disattivato.'''
description: Scopri di più sul messaggio di errore "Questo calendario dispone dei diritti di visualizzazione di un utente disattivato".
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 1%

---

# Messaggio di errore sul calendario: &quot;Questo calendario dispone dei diritti di visualizzazione di un utente disattivato.&quot;

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
     <p>Standard</p>
     <p>Lavoro o superiore</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un calendario</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Problema

Quando si accede a un calendario condiviso con l&#39;utente viene visualizzato il messaggio di errore seguente: 

*Questo calendario dispone dei diritti di visualizzazione di un utente disattivato. Richiedere a un amministratore di correggere i privilegi del calendario.*

## Causa

L&#39;utente che ha creato il calendario (proprietario originale) è un utente che è stato disattivato. 

## Soluzione

Puoi risolvere il problema nel modo seguente:

1. Copia il calendario originale. Quando si copia un calendario, l&#39;utente diventa il proprietario del calendario. Il calendario copiato deve mostrare tutte le informazioni del calendario originale.\
   Per ulteriori informazioni sulla copia di un calendario, vedere [Copiare un report del calendario](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. Condividere il calendario copiato con gli stessi utenti del calendario originale. Tutti gli utenti devono visualizzare le stesse informazioni nel nuovo calendario.
1. (Facoltativo e condizionale) Se si dispone delle autorizzazioni per gestire il calendario originale, rimuovere tutti gli altri utenti con cui il calendario è condiviso dall&#39;area Condivisione calendario. In questo modo si evita di confondere gli utenti che tentano di visualizzare un calendario errato.
