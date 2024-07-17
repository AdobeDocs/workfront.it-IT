---
title: Creare e personalizzare le priorità
description: Puoi controllare le priorità per progetti, attività e problemi nell’area Configurazione di Workfront. Le priorità danno importanza ai tuoi progetti, attività o problemi in Adobe Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 2%

---

# Creare e personalizzare le priorità

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Puoi controllare le priorità per progetti, attività e problemi nell’area Configurazione di Workfront. Le priorità danno importanza ai tuoi progetti, attività o problemi in Adobe Workfront.

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
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizzazione delle priorità esistenti

In qualità di amministratore di Workfront, puoi apportare le seguenti modifiche alle priorità predefinite fornite in Workfront:

* Rinominare le priorità.
* Riordina le priorità.

  Per ulteriori informazioni su come riordinare le priorità, vedere [Creare una priorità per un&#39;attività di progetto o un problema](#create-a-priority-for-a-project-task-or-issue).

* Modifica la priorità predefinita.

  Per ulteriori informazioni sulla funzionalità di modifica della priorità predefinita, vedere [Creare una priorità per un&#39;attività o un problema di progetto](#create-a-priority-for-a-project-task-or-issue).

* Modifica la descrizione delle priorità.
* Imposta un colore per ogni priorità.

  Il colore della priorità viene utilizzato nei report grafico quando si raggruppano i risultati per **Priorità**.

  Per ulteriori informazioni sui report grafico, vedere [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Eliminare le priorità.

  Quando si elimina una priorità esistente, è necessario selezionarne una sostitutiva.

* Nascondi le priorità.

  Per ulteriori informazioni sulla funzionalità di nascondere le priorità, vedere [Creare una priorità per un&#39;attività o un problema di progetto](#create-a-priority-for-a-project-task-or-issue).

  >[!NOTE]
  >
  >Devi avere almeno una priorità nel tuo account Workfront per ogni oggetto.

Le priorità fornite per impostazione predefinita per ciascun tipo di oggetto (progetto, attività e problema) sono identiche:

* Nessuno
* Basso
* Normal
* Alta
* Urgente

## Creare una priorità per un’attività o un problema di progetto {#create-a-priority-for-a-project-task-or-issue}

Oltre alle priorità predefinite fornite in Workfront, puoi aggiungere altre priorità per riflettere le esigenze della tua organizzazione.

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Preferenze progetto** > **Priorità**.

1. Fare clic sulla scheda relativa al tipo di oggetto per cui si desidera creare una priorità per (**Progetto**, **Attività** o **Problema**).
1. Fare clic su **Aggiungi nuova priorità**.
1. Specifica le seguenti informazioni per la nuova priorità:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome priorità</td> 
      <td>Digita un nome per la priorità.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Importanza</td> 
      <td> <p>Quando si aggiunge una nuova priorità, viene assegnato un numero per impostazione predefinita. Modifica questo numero, se non corrisponde alle tue esigenze.</p> <p>Il numero <strong>Importance</strong> per ogni priorità deve essere univoco per l'oggetto selezionato.<br>Il numero di priorità riflette l'importanza del progetto, dell'attività o del problema: il numero più alto corrisponde alla priorità più alta.</p> <p><b>NOTA</b>: non è possibile modificare il numero di importanza dopo aver salvato la priorità. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Colore</td> 
      <td> <p>Scegli un colore per la tua priorità.</p> <p>Il colore della priorità viene utilizzato nei rapporti grafico e nelle impostazioni del team Agile. Per ulteriori informazioni sui report grafico, vedere <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Aggiungere un grafico a un report</a>.</p> <p>Per ulteriori informazioni sulle impostazioni del team Agile, consulta in .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Priorità predefinita</td> 
      <td> <p>Per decidere se questa deve essere o meno una priorità predefinita, seleziona il pulsante di opzione.</p> <p>Se una priorità è designata come <strong>Priorità predefinita</strong>, viene selezionata automaticamente per tutti i progetti, le attività o i problemi in Workfront. <strong>Normale</strong> è la priorità predefinita per tutti gli oggetti in Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Aggiungi una descrizione della priorità per spiegarne la funzione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nascondi</td> 
      <td> <p>Selezionare questa casella per nascondere la priorità.</p><p>Quando selezioni l'opzione <b>Nascondi</b>, la priorità non viene visualizzata in alcun punto di Workfront e gli utenti non possono sceglierla per i loro progetti, attività e problemi.</p> 
      <p><b>IMPORTANTE</b>: è consigliabile nascondere le priorità che non si desidera più utilizzare, anziché eliminarle. Nascondendoli, conservi comunque tutti i tuoi dati storici, degli oggetti che sono stati completati con questa priorità, impedendo al contempo alle persone di scegliere questa priorità in futuro. </p>
      <p>Se necessario, puoi modificare l’ordine di visualizzazione delle priorità trascinandole e rilasciandole nell’ordine desiderato. Questo cambia l’ordine in cui vengono visualizzate per i progetti, le attività e i problemi. Il numero <b>Importance</b> non viene modificato. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

Per istruzioni sull&#39;applicazione delle priorità a progetti, attività e problemi, vedi i seguenti articoli:

* [Comprendere e aggiornare le priorità del progetto](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Aggiorna priorità attività](../../../manage-work/tasks/task-information/task-priority.md)
* [Aggiorna la priorità del problema](../../../manage-work/issues/issue-information/update-issue-priority.md)
