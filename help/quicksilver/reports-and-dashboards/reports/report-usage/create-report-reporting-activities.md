---
product-area: reporting
keywords: cambia, proprietario, condiviso, rapporto, condivisione, esecuzione, utente, accesso, diritti, inserito, ultimo, visualizzato, data, reporting, attività
navigation-topic: report-usage
title: Creare un rapporto sulle attività di reporting
description: Quando crei un rapporto sui rapporti, puoi identificare informazioni specifiche sui rapporti, che possono includere se i rapporti sono assegnati a utenti disattivati, se i rapporti sono impostati per essere eseguiti con i diritti di accesso di un utente disattivato, se gli utenti accedono a un rapporto che intendi eliminare e così via.
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 1%

---

# Creare un rapporto sulle attività di reporting

Quando crei un rapporto sui rapporti, puoi identificare informazioni specifiche sui rapporti, che possono includere se i rapporti sono assegnati a utenti disattivati, se i rapporti sono impostati per essere eseguiti con i diritti di accesso di un utente disattivato, se gli utenti accedono a un rapporto che intendi eliminare e così via.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare un rapporto sui rapporti esistenti {#create-the-report-about-existing-reports}

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.
1. Fai clic su **Rapporti**, quindi **Nuovo rapporto**.
1. In **Nuovo rapporto** menu a discesa, seleziona **Rapporto** per creare un report sui report esistenti.

1. In **Colonne (visualizzazione)** aggiungi le colonne desiderate nel rapporto.\
   Alcuni dei campi seguenti possono essere utili:

   | Campo | Descrizione |
   |---|---|
   | **Esegui come utente: Nome** | Questo è l&#39;utente specificato nel **Esegui questo rapporto con i diritti di accesso di:** sul report. Se l’utente è disattivato, il rapporto non viene visualizzato per gli utenti con cui è condiviso il rapporto. |
   | **Condivisione con** | Sono tutte le entità con cui il rapporto è condiviso. |
   | **Immesso da** | Questo è il proprietario del report. |
   | **Data ultima visualizzazione** | Data e ora dell’ultima visualizzazione del rapporto da parte di un utente. |

   {style=&quot;table-layout:auto&quot;}

1. (Facoltativo) Per limitare l&#39;elenco dei rapporti a specifici utenti disattivati:

   1. Seleziona la **Filtri** scheda , quindi fai clic su **Aggiungere una regola filtro**.

   1. Aggiungi il filtro **Esegui come ID utente** > **Uguale**.

   1. Digitare il nome dell&#39;utente disattivato che si desidera aggiungere al filtro, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco.
   1. Ripetere il passaggio C finché non sono stati selezionati tutti gli utenti disattivati che si desidera includere nel rapporto.

1. (Facoltativo) Per limitare l&#39;elenco dei report ai report pianificati:

   1. Seleziona la **Filtri** scheda , quindi fai clic su **Aggiungere una regola filtro**.

   1. Aggiungi il filtro **ID rapporto pianificato** > **Non vuoto**.

1. Fai clic su **Salva e chiudi**, quindi digita un nome per il rapporto e fai clic su **Salva rapporto**.

   Vengono visualizzate le informazioni sul rapporto.

1. (Facoltativo) Esporta questo rapporto in Excel e salvalo sul computer.\
   Per informazioni sull&#39;esportazione di un rapporto, vedi [Esportare i dati](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Aggiornare informazioni su un rapporto

Dopo aver creato il rapporto, puoi aggiornarlo in base alle esigenze.

1. Passa al rapporto da aggiornare.
1. A seconda dell’azione che desideri eseguire, effettua una delle seguenti operazioni:

   * Aggiorna **Esegui questo rapporto con i diritti di accesso di:** a un utente attivo: Per ulteriori informazioni, consulta [Eseguire e distribuire un rapporto con i diritti di accesso di un altro utente](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * Crea una copia del rapporto: Per ulteriori informazioni, consulta [Creare una copia di un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * Eliminare un rapporto: per ulteriori informazioni, consulta [Creare una copia esatta di un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) sezione dell&#39;articolo [Creare una copia di un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * Condivisione di un rapporto: per ulteriori informazioni, consulta [Condivisione di un rapporto in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Condizionale) Se copi i rapporti originali, utilizza le informazioni del rapporto creato in [Creare un rapporto sui rapporti esistenti](#create-the-report-about-existing-reports) condividere le nuove copie con le stesse entità dei rapporti originali.
