---
title: Creare o personalizzare le gravità dei problemi
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Gli utenti possono utilizzare le gravità per definire la gravità di un problema. Puoi personalizzare una qualsiasi delle cinque gravità predefinite esistenti in Adobe Workfront o crearne una nuova per i tuoi utenti.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: 5c80dca8a9f7dd5a693db9bf22738602da8b521b
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 4%

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

## Gravità del problema incorporata

Workfront ha cinque livelli di gravità incorporati:

* Cosmetico
* Causa Confusione
* Bug con workaround
* Bug senza workaround
* Errore Fatale

È possibile modificare quanto segue per queste gravità:

* Nome
* Colore

  Il colore di una gravità viene mantenuto in un rapporto grafico, se si raggruppano i risultati in base alla gravità della Issue. Per informazioni sui report grafico, vedere [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Quale gravità è predefinita

  Per ulteriori informazioni sulle gravità predefinite, vedere [Creare o modificare la gravità di un problema](#create-or-edit-an-issue-severity) in questo articolo.

* Descrizione
* Se una gravità è nascosta in Workfront

  Per ulteriori informazioni su come nascondere una gravità, vedere [Creare o modificare la gravità di un problema](#create-or-edit-an-issue-severity) in questo articolo.

* Eliminare una gravità

  In questo caso, è necessario selezionare una gravità di sostituzione.

## Creare o modificare la gravità di un problema {#create-or-edit-an-issue-severity}

In qualità di amministratore di Workfront, puoi creare e modificare le gravità dei problemi in base alle esigenze dei tuoi utenti.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Preferenze progetto** > **Gravità**.

1. Se stai creando una nuova gravità, fai clic su **Nuova riga** nella parte inferiore della tabella.
1. Configurare le seguenti opzioni per la nuova gravità o modificarle per una esistente:

   * **Nome gravità**: digitare un nome per la gravità.
   * **Importanza**: aumentare o diminuire il livello di gravità, originariamente assegnato da Workfront, per la gravità.

     Il numero di importanza per ogni gravità deve essere univoco. Il numero più alto corrisponde al livello di gravità più alto.

     Non è possibile modificare questo numero dopo aver salvato la gravità.

   * **Colore**: scegliere un colore per la gravità.

     Il colore della gravità viene utilizzato nei rapporti grafico quando si raggruppano i risultati per gravità del problema. Per informazioni sui report grafico, vedere [Aggiungere un grafico a un report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

   * **Gravità predefinita**: selezionare la gravità che si desidera venga applicata automaticamente da Workfront a tutti i problemi appena creati.

     **Cosmetic** è la gravità predefinita per i problemi in Workfront.

     Non è possibile impostare come predefinita una gravità nascosta.

     La gravità predefinita è indicata da un&#39;icona ![Icona gravità predefinita](assets/default-icon.png). Per scegliere un nuovo valore predefinito, effettuare una delle seguenti operazioni:

      * Selezionare la casella di controllo accanto al nome della gravità e selezionare **Predefinito** nella barra delle azioni nella parte inferiore dello schermo.
      * Passa il puntatore del mouse sul nome della gravità e fai clic sul menu **Altro** visualizzato. Quindi, selezionare **Rendi predefinito**.

        La nuova gravità predefinita è etichettata con l&#39;icona.

   * **Descrizione**: digitare una descrizione della gravità per spiegarne la funzione.
   * **Nascondi scelta**: selezionare **Sì** per nascondere una gravità non più necessaria.

     Una gravità nascosta non viene visualizzata in alcun punto di Workfront, pertanto gli utenti non possono sceglierla per i problemi.

     >[!IMPORTANT]
     >
     >Invece di eliminare le gravità che non desideri più utilizzare, ti consigliamo di nasconderle. In questo modo, puoi conservare tutti i dati storici sugli oggetti già completati con la gravità, impedendo al contempo alle persone di utilizzare la gravità in futuro.

1. (Facoltativo) Modifica l’ordine di visualizzazione delle gravità trascinandole e rilasciandole nell’ordine desiderato.

   Questo cambia l’ordine in cui vengono visualizzate le Issues. Il numero **Importance** non viene modificato.

1. Fai clic su **Salva**.

Per ulteriori informazioni su come utilizzare le gravità durante l&#39;utilizzo dei problemi, vedere [Aggiorna gravità del problema](../../../manage-work/issues/issue-information/update-issue-severity.md).
