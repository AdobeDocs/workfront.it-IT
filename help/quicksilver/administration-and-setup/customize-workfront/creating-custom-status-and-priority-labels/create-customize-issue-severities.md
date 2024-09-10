---
title: Creare o personalizzare le gravità dei problemi
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Gli utenti possono utilizzare le gravità per definire la gravità di un problema. Puoi personalizzare una qualsiasi delle cinque gravità predefinite esistenti in Adobe Workfront o crearne una nuova per i tuoi utenti.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 5%

---

# Creare o personalizzare le gravità dei problemi

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

Gli utenti possono utilizzare le gravità per definire la gravità di un problema. Puoi personalizzare una qualsiasi delle cinque gravità predefinite esistenti in Adobe Workfront o crearne una nuova per i tuoi utenti.

>[!NOTE]
>
>Le attività e i progetti non hanno gravità.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
     <p>Nuovo: Standard</p>
     <p>oppure</p>
     <p>Corrente: Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gravità del problema incorporata

Workfront ha cinque livelli di gravità incorporati:

* Cosmetico
* Causa Confusione
* Bug con workaround
* Bug senza workaround
* Errore Fatale

<p>È possibile modificare quanto segue per queste gravità:</p>

* Nome
* Colore

  Il colore di una gravità viene mantenuto in un rapporto grafico, se si raggruppano i risultati in base alla gravità della Issue. Per informazioni sui report grafico, vedere [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Quale gravità è predefinita

  Per ulteriori informazioni sulle gravità predefinite, vedere [Creare o modificare la gravità di un problema](#create-or-edit-an-issue-severity) in questo articolo.
* Descrizione
* Se una gravità è nascosta in Workfront

  Per ulteriori informazioni su come nascondere una gravità, vedere [Creare o modificare la gravità di un problema](#create-or-edit-an-issue-severity")

* Eliminare una gravità

  In questo caso, è necessario selezionare una gravità di sostituzione.

## Creare o modificare la gravità di un problema {#create-or-edit-an-issue-severity}

In qualità di amministratore di Workfront, puoi creare e modificare le gravità dei problemi in base alle esigenze dei tuoi utenti.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Preferenze progetto** > **Gravità**.

1. Se stai creando una nuova gravità, fai clic su **Aggiungi una nuova gravità**.
1. Configurare le seguenti opzioni per la nuova gravità o modificarle per una esistente:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome gravità</td> 
      <td>Digita un nome per la gravità</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Importanza</td> 
      <td>Aumentare o diminuire il livello di gravità, originariamente assegnato da Workfront, per la gravità.
      <p>Il numero di importanza per ogni gravità deve essere univoco. Il numero più alto corrisponde al livello di gravità più alto.</p> <p>Non è possibile modificare questo numero dopo aver salvato la gravità.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Colore</td> 
      <td> <p>Scegliere un colore per la gravità.</p> 
      <p>Il colore della gravità viene utilizzato nei rapporti grafico quando si raggruppano i risultati per gravità del problema. Per informazioni sui report grafico, vedere <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Aggiungere un grafico a un report</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gravità predefinita</td> 
      <td>Selezionare la gravità che si desidera venga selezionata automaticamente da Workfront per tutti i nuovi problemi creati.</p>
      <p>La gravità predefinita dei problemi in Workfront è Cosmetic.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Digitare una descrizione della gravità per illustrarne la funzione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nascondi</td> 
      <td> Nascondere una gravità non più necessaria. 
      <p>Una gravità nascosta non viene visualizzata in alcun punto di Workfront, pertanto gli utenti non possono sceglierla per i problemi.</p> 
      <p><b>IMPORTANTE</b>: anziché eliminare le gravità che non si desidera più utilizzare, è consigliabile nasconderle. In questo modo, puoi conservare tutti i dati storici sugli oggetti già completati con la gravità, impedendo al contempo alle persone di utilizzare la gravità in futuro.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Modifica l’ordine di visualizzazione delle gravità trascinandole e rilasciandole nell’ordine desiderato.

   Questo cambia l’ordine in cui vengono visualizzate le Issues. Il numero **Importance** non viene modificato.

1. Fai clic su **Salva**.

Per ulteriori informazioni su come utilizzare le gravità durante l&#39;utilizzo dei problemi, vedere [Aggiorna gravità del problema](../../../manage-work/issues/issue-information/update-issue-severity.md).
