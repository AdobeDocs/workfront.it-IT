---
title: Creare e personalizzare le priorità
description: Puoi controllare le priorità per progetti, attività e problemi nell’area Configurazione di Workfront. Le priorità danno importanza ai tuoi progetti, attività o problemi in Adobe Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: 5c80dca8a9f7dd5a693db9bf22738602da8b521b
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 2%

---

# Creare e personalizzare le priorità

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Puoi controllare le priorità per progetti, attività e problemi nell’area Configurazione di Workfront. Le priorità danno importanza ai tuoi progetti, attività o problemi in Adobe Workfront.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Amministratore di Sistema</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizzazione delle priorità esistenti

In qualità di amministratore di Workfront, puoi apportare le seguenti modifiche alle priorità predefinite fornite in Workfront:

* Rinominare le priorità.
* Riordina le priorità.

  Per ulteriori informazioni su come riordinare le priorità, vedere [Creare una priorità per un progetto, attività o problema](#create-a-priority-for-a-project-task-or-issue).

* Modifica la priorità predefinita.

  Per ulteriori informazioni sulla funzionalità di modifica della priorità predefinita, vedere [Creare una priorità per un progetto, attività o problema](#create-a-priority-for-a-project-task-or-issue).

* Modifica la descrizione delle priorità.
* Imposta un colore per ogni priorità.

  Il colore della priorità viene utilizzato nei report grafico quando si raggruppano i risultati per **Priorità**.

  Per ulteriori informazioni sui report grafico, vedere [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Eliminare le priorità.

  Quando si elimina una priorità esistente, è necessario selezionarne una sostitutiva.

* Nascondi le priorità.

  Per ulteriori informazioni sulla funzionalità di nascondere le priorità, vedere [Creare una priorità per un progetto, attività o problema](#create-a-priority-for-a-project-task-or-issue).

  >[!NOTE]
  >
  >Devi avere almeno una priorità nel tuo account Workfront per ogni oggetto.

Le priorità fornite per impostazione predefinita per ciascun tipo di oggetto (progetto, attività e problema) sono identiche:

* Nessuno
* Basso
* Normal
* Alta
* Urgente

## Creare una priorità per un progetto, un’attività o un problema {#create-a-priority-for-a-project-task-or-issue}

Oltre alle priorità predefinite fornite in Workfront, puoi aggiungere altre priorità per riflettere le esigenze della tua organizzazione.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Preferenze progetto** > **Priorità**.

1. Fare clic sulla scheda relativa al tipo di oggetto per cui si desidera creare una priorità per (**Progetto**, **Attività** o **Problema**).
1. Fai clic su **Nuova riga** nella parte inferiore della tabella.
1. Configura le seguenti opzioni per la priorità:

   * **Nome priorità**: digitare un nome per la priorità.
   * **Importanza**: quando si aggiunge una nuova priorità, viene assegnato un numero per impostazione predefinita. Modifica questo numero, se non corrisponde alle tue esigenze.

     Il numero di importanza per ogni priorità deve essere univoco. Il numero di priorità riflette l&#39;importanza del progetto, dell&#39;attività o del problema: il numero più alto corrisponde alla priorità più alta.

     Impossibile modificare questo numero dopo aver salvato la priorità.

   * **Colore**: scegliere un colore per la priorità.

     Il colore della priorità viene utilizzato nei rapporti grafico e nelle impostazioni del team Agile. Per informazioni sui report grafico, vedere [Aggiungere un grafico a un report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md). Per informazioni sulle impostazioni del team Agile, consulta [Creare un team Agile](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

   * **Priorità predefinita**: selezionare la priorità che si desidera applicare automaticamente a tutti i nuovi progetti, attività o problemi creati da Workfront.

     **Normale** è la priorità predefinita per tutti gli oggetti in Workfront.

     Non è possibile impostare una priorità nascosta come predefinita.

     La priorità predefinita è indicata da un&#39;icona ![Icona di priorità predefinita](assets/default-icon.png). Per scegliere un nuovo valore predefinito, effettuare una delle seguenti operazioni:

      * Selezionare la casella di controllo accanto al nome della priorità e selezionare **Rendi predefinito** nella barra delle azioni nella parte inferiore dello schermo.
      * Passa il puntatore del mouse sul nome della priorità e fai clic sul menu **Altro** visualizzato. Quindi, selezionare **Rendi predefinito**.

        La nuova priorità predefinita è etichettata con l’icona.

   * **Descrizione**: digitare una descrizione della priorità per spiegarne la funzione.
   * **Nascondi scelta**: selezionare **Sì** per nascondere una priorità non più necessaria.

     Una priorità nascosta non viene visualizzata in alcun punto di Workfront, pertanto gli utenti non possono sceglierla per i loro progetti, attività o problemi.

     >[!IMPORTANT]
     >
     >Invece di eliminare le priorità che non desideri più utilizzare, ti consigliamo di nasconderle. In questo modo, puoi conservare tutti i dati storici sugli oggetti già completati con la priorità, impedendo alle persone di utilizzare la priorità in futuro.

1. (Facoltativo) Modifica l’ordine di visualizzazione delle priorità trascinandole e rilasciandole nell’ordine desiderato.

   Questo cambia l’ordine in cui vengono visualizzate per i progetti, le attività o i problemi. Il numero **Importance** non viene modificato.

1. Fai clic su **Salva**.

Per istruzioni sull&#39;applicazione delle priorità a progetti, attività e problemi, vedi i seguenti articoli:

* [Comprendere e aggiornare le priorità del progetto](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Aggiorna priorità attività](../../../manage-work/tasks/task-information/task-priority.md)
* [Aggiorna la priorità del problema](../../../manage-work/issues/issue-information/update-issue-priority.md)
