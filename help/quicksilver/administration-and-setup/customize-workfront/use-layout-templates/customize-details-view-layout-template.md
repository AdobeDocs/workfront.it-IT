---
title: Personalizzare la visualizzazione Dettagli utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In qualità di amministratore di Workfront, è possibile utilizzare un modello di layout per determinare quali informazioni vengono visualizzate quando un utente seleziona la sezione Dettagli nel pannello a sinistra durante la visualizzazione di un'attività, un problema, un documento, un programma o un portfolio.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: 92fb1ee0b641d2f4b527e17df272e4c37c0feaef
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Personalizzare la visualizzazione Dettagli utilizzando un modello di layout

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

In qualità di amministratore di Adobe Workfront, puoi utilizzare un modello di layout per determinare quali informazioni vengono visualizzate quando un utente fa clic sull’icona Dettagli ![](assets/project-details-icon.png) nel pannello a sinistra durante la visualizzazione di un&#39;attività, un problema, un documento, un programma o un portfolio.

<!--
or billing record
-->

È inoltre possibile modificare l&#39;ordine delle informazioni in cui vengono visualizzate. Ad esempio, per tutte le attività visualizzate dagli utenti, è possibile spostare le informazioni personalizzate di Forms nella parte superiore della visualizzazione Dettagli per tutte le attività visualizzate dagli utenti.

Le modifiche apportate alla visualizzazione Dettagli di un oggetto determinano anche la disponibilità e l&#39;ordine dei campi visualizzati dagli utenti nelle aree seguenti:

* Caselle &quot;Nuovo oggetto&quot;, ad esempio Nuova attività e Nuovo problema

   ![](assets/new-task-dialog.png)

* Schermate &quot;Modifica oggetto&quot;, ad esempio Modifica attività, Modifica problema e Modifica progetto

   ![](assets/edit-task-screen.png)


* Le schermate &quot;Modifica oggetti&quot; vengono visualizzate durante la modifica collettiva di oggetti. Attualmente è supportato per la modifica collettiva di progetti.

   ![](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* Riepilogo ![](assets/summary-panel-icon.png) pannello per l’elenco delle attività e dei problemi

   ![](assets/summary-area.png)

   >[!NOTE]
   >
   >Le modifiche ai modelli di layout influiscono sull&#39;ordine e la disponibilità dei campi nel pannello Riepilogo solo per le attività e i problemi assegnati all&#39;utente connesso.

* Caselle di conversione, ad esempio le caselle Converti problema in attività o Converti problema in progetto.

   ![Converti problema in casella attività](assets/convert-issue-to-task-box.png)

Per informazioni sui modelli di layout per gruppi, consulta [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

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
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.
Per eseguirle per un gruppo, devi essere un responsabile di quel gruppo</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizzare gli elementi visualizzati dagli utenti nella vista Dettagli

1. Inizia a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Fai clic sulla freccia giù ![](assets/dropdown-arrow-12x12.png) sotto **Personalizzare ciò che gli utenti visualizzano**, quindi fai clic su **Progetto**, **Attività**, **Problema**, **Programma** oppure **Portfolio.**
<!--
, or billing record
-->

1. In **Dettagli** eseguire una delle operazioni seguenti per personalizzare gli elementi visualizzati dagli utenti nella visualizzazione Dettagli:

   * Trascina le intestazioni di sezione ![](assets/move-icon---dots.png) per cambiare il loro ordine.
   * Attiva o disattiva le opzioni in **Panoramica** e **Forms personalizzato** per mostrarle o nasconderle.

      Se nascondi tutti i campi in una di queste sezioni, l’intera sezione viene nascosta.

      Tutti i campi sono abilitati per impostazione predefinita.

1. Continua a personalizzare il modello di layout.

   Oppure

   Al termine della personalizzazione, fai clic su **Salva**.

   >[!TIP]
   >
   >Puoi fare clic su Salva in qualsiasi momento per salvare l&#39;avanzamento, quindi continuare a modificare il modello in un secondo momento.
