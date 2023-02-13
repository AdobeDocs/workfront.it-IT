---
title: Creare e personalizzare le priorità
description: È possibile controllare le priorità per progetti, attività e problemi nell'area Configurazione di Workfront. Le priorità attribuiscono importanza ai progetti, alle attività o ai problemi in Adobe Workfront.
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

È possibile controllare le priorità per progetti, attività e problemi nell&#39;area Configurazione di Workfront. Le priorità attribuiscono importanza ai progetti, alle attività o ai problemi in Adobe Workfront.

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

## Personalizzazione delle priorità esistenti

In qualità di amministratore di Workfront, puoi apportare le seguenti modifiche alle priorità predefinite fornite in Workfront:

* Rinominare le priorità.
* Riordinare le priorità.

   Per ulteriori informazioni su come riordinare le priorità, vedi [Crea una priorità per un’attività di progetto o un problema](#create-a-priority-for-a-project-task-or-issue).

* Modificare la priorità predefinita.

   Per ulteriori informazioni sulla funzionalità di modifica della priorità predefinita, consulta [Crea una priorità per un’attività di progetto o un problema](#create-a-priority-for-a-project-task-or-issue).

* Modifica la descrizione delle priorità.
* Imposta un colore per ogni priorità.

   Il colore della priorità viene utilizzato nei rapporti sui grafici quando si raggruppano i risultati per **Priorità**.

   Per ulteriori informazioni sui rapporti sui grafici, vedi [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Eliminare le priorità.

   Quando elimini una priorità esistente, devi selezionarne una sostitutiva.

* Nascondere le priorità.

   Per ulteriori informazioni sulla funzionalità di nascondere le priorità, vedi [Crea una priorità per un’attività di progetto o un problema](#create-a-priority-for-a-project-task-or-issue).

   >[!NOTE]
   >
   >Devi avere almeno una priorità nell’account Workfront per ogni oggetto.

Le priorità fornite per impostazione predefinita per ogni tipo di oggetto (progetto, attività e problema) sono identiche:

* Nessuno
* Basso
* Normal
* Alta
* Urgente

## Crea una priorità per un’attività di progetto o un problema {#create-a-priority-for-a-project-task-or-issue}

Oltre alle priorità predefinite fornite in Workfront, puoi aggiungere le tue priorità in base alle esigenze della tua organizzazione.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Preferenze del progetto** > **Priorità**.

1. Fare clic sulla scheda relativa al tipo di oggetto per il quale si desidera creare una priorità (**Progetto**, **Attività** oppure **Problema**).
1. Fai clic su **Aggiungi una nuova priorità**.
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
      <td> <p>Quando si aggiunge una nuova priorità, per impostazione predefinita gli viene assegnato un numero. Modifica questo numero, se non corrisponde alle tue esigenze.</p> <p>La <strong>Importanza</strong> il numero di ogni priorità deve essere univoco per l'oggetto selezionato.<br>Il numero di priorità riflette l'importanza del progetto, del compito o del problema: il numero più alto corrisponde alla priorità più alta.</p> <p><b>NOTA</b>: Non è possibile modificare il numero di Importanza dopo aver salvato la priorità. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clr icn</td> 
      <td> <p>Scegli un colore per la tua priorità.</p> <p>Il colore della priorità viene utilizzato nei rapporti grafico e nelle impostazioni team Agile. Per ulteriori informazioni sui rapporti sui grafici, vedi <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Aggiungere un grafico a un report</a>.</p> <p>Per ulteriori informazioni sulle impostazioni del team Agile, consulta in .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Priorità predefinita</td> 
      <td> <p>Seleziona il pulsante di scelta per decidere se si tratta di una priorità predefinita o meno.</p> <p>Se una priorità è designata come <strong>Priorità predefinita</strong>, viene selezionato automaticamente per tutti i progetti, le attività o i problemi in Workfront. <strong>Normale</strong> è la priorità predefinita per tutti gli oggetti in Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Aggiungi una descrizione della priorità per spiegarne la funzione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nascondi</td> 
      <td> <p>Selezionare questa casella se si desidera nascondere la priorità.</p><p>Quando selezioni la <b>Nascondi</b> la priorità non viene visualizzata in alcun punto di Workfront e gli utenti non possono sceglierla per i progetti, le attività e i problemi.</p> 
      <p><b>IMPORTANTE</b>: È consigliabile nascondere le priorità che non si desidera più utilizzare, anziché eliminarle. Nascondendoli, si conservano ancora tutti i dati storici, di oggetti che sono stati completati con questa priorità, impedendo al contempo alle persone di scegliere questa priorità in futuro. </p>
      <p>Facoltativamente, puoi modificare l’ordine di inserimento delle priorità trascinandole e rilasciandole nell’ordine desiderato. In questo modo viene modificato l’ordine in cui vengono visualizzati per progetti, attività e problemi. Questo non cambia il <b>Importanza</b> numero. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

Per istruzioni sull&#39;applicazione delle priorità a progetti, compiti e problemi, vedi i seguenti articoli:

* [Comprendere e aggiornare le priorità del progetto](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Aggiorna priorità attività](../../../manage-work/tasks/task-information/task-priority.md)
* [Aggiorna priorità del problema](../../../manage-work/issues/issue-information/update-issue-priority.md)
