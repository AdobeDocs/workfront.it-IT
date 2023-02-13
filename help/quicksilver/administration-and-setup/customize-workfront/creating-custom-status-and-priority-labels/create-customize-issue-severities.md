---
title: Creare o personalizzare le gravità dei problemi
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Gli utenti possono utilizzare le gravità per definire la gravità del problema. Puoi personalizzare una delle cinque severità predefinite esistenti in Adobe Workfront o crearne una nuova per gli utenti.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 4%

---

# Creare o personalizzare le gravità dei problemi

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

Gli utenti possono utilizzare le gravità per definire la gravità del problema. Puoi personalizzare una delle cinque severità predefinite esistenti in Adobe Workfront o crearne una nuova per gli utenti.

>[!NOTE]
>
>Le attività e i progetti non hanno gravità.

## Requisiti di accesso

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
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Gravità dei problemi incorporati

Workfront ha cinque problemi incorporati:

* Cosmetico
* Causa Confusione
* Bug con workaround
* Bug senza workaround
* Errore Fatale

<p>È possibile modificare quanto segue per queste gravità:</p>

* Nome
* Clr icn

   Il colore di una gravità viene mantenuto in un rapporto grafico se i risultati vengono raggruppati per gravità del problema. Per informazioni sui report grafici, consulta [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Quale severità è l&#39;impostazione predefinita

   Per ulteriori informazioni sulle severità predefinite, consulta [Creare o modificare una gravità del problema](#create-or-edit-an-issue-severity) in questo articolo.
* Descrizione
* Se una gravità è nascosta in Workfront

   Per ulteriori informazioni su come nascondere una gravità, vedi [Creare o modificare una gravità del problema](#create-or-edit-an-issue-severity")

* Eliminare una gravità

   Quando si esegue questa operazione, è necessario selezionare una gravità di sostituzione.

## Creare o modificare una gravità del problema {#create-or-edit-an-issue-severity}

In qualità di amministratore di Workfront, puoi creare e modificare le gravità dei problemi in base alle esigenze degli utenti.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Preferenze del progetto** > **Gravità**.

1. Se stai creando una nuova gravità, fai clic su **Aggiungere una nuova gravità**.
1. Configura le seguenti opzioni per la nuova gravità o modificale per una esistente:

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
      <td>Aumenta o diminuisce il livello di serietà, originariamente assegnato da Workfront, per la gravità.
      <p>Il numero di importanza per ogni gravità deve essere univoco. Il numero più alto corrisponde al livello di gravità più alto.</p> <p>Non è possibile modificare questo numero dopo aver salvato la gravità.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clr icn</td> 
      <td> <p>Scegli un colore per la gravità.</p> 
      <p>Il colore della gravità viene utilizzato nei rapporti sui grafici quando si raggruppano i risultati per Gravità del problema. Per informazioni sui report grafici, consulta <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Aggiungere un grafico a un report</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gravità predefinita</td> 
      <td>Seleziona la gravità da selezionare automaticamente da Workfront per tutti i nuovi problemi creati.</p>
      <p>Cosmetic è la gravità predefinita dei problemi in Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Digita una descrizione della gravità per spiegarne la funzione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nascondi</td> 
      <td> Nascondere una gravità non più necessaria. 
      <p>Una gravità nascosta non viene visualizzata in alcun punto di Workfront, pertanto gli utenti non possono sceglierla per i propri problemi.</p> 
      <p><b>IMPORTANTE</b>: Invece di eliminare le gravità che non desideri più utilizzare, ti consigliamo di nasconderle. In questo modo, puoi conservare tutti i tuoi dati storici su oggetti già completati con la gravità, impedendo al contempo alle persone di utilizzare la gravità in futuro.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Modifica l’ordine di elencazione delle tue severità trascinandole e rilasciandole nell’ordine desiderato.

   Questo modifica l’ordine in cui vengono visualizzati per i problemi. Non cambia la **Importanza** numero.

1. Fai clic su **Salva**.

Per ulteriori informazioni su come utilizzare le gravità durante l’utilizzo dei problemi, consulta [Aggiorna gravità del problema](../../../manage-work/issues/issue-information/update-issue-severity.md).
