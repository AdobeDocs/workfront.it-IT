---
product-area: reporting
keywords: modifica,proprietario,condiviso,report,condivisione,esecuzione,utente,accesso,diritti,inserito,ultimo,visualizzato,data,report,attività
navigation-topic: report-usage
title: Creare un rapporto sulle attività di reporting
description: Quando si crea un report sui report, è possibile identificare informazioni specifiche, che possono includere se i report sono assegnati a utenti disattivati, se i report sono impostati per l'esecuzione con i diritti di accesso di un utente disattivato, se gli utenti accedono a un report che si intende eliminare e così via.
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# Creare un rapporto sulle attività di reporting

Quando si crea un report sui report, è possibile identificare informazioni specifiche, che possono includere se i report sono assegnati a utenti disattivati, se i report sono impostati per l&#39;esecuzione con i diritti di accesso di un utente disattivato, se gli utenti accedono a un report che si intende eliminare e così via.

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
   <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare il rapporto sui rapporti esistenti {#create-the-report-about-existing-reports}

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront.
1. Fai clic su **Rapporti**, quindi su **Nuovo rapporto**.
1. Nel menu a discesa **Nuovo report**, seleziona **Report** per creare un report sui report esistenti.

1. Nella scheda **Colonne (visualizzazione)**, aggiungi le colonne desiderate nel report.\
   Alcuni dei seguenti campi possono essere utili:

   | Campo | Descrizione |
   |---|---|
   | **Esegui come utente: Nome** | Questo è l&#39;utente specificato in **Esegui il report con i diritti di accesso di:** nel report. Se l&#39;utente è disattivato, il report non viene visualizzato per nessuno con cui è condiviso. |
   | **Condiviso con** | Queste sono tutte le entità con cui è condiviso il report. |
   | **Inserito da** | Questo è il proprietario del rapporto. |
   | **Data ultima visualizzazione** | Data e ora dell&#39;ultima visualizzazione del report da parte di un utente. |

   {style="table-layout:auto"}

1. (Facoltativo) Per limitare l’elenco dei rapporti a specifici utenti disattivati:

   1. Seleziona la scheda **Filtri**, quindi fai clic su **Aggiungi regola filtro**.

   1. Aggiungi il filtro **Esegui come ID utente** > **Uguale**.

   1. Digita il nome dell’utente disattivato che desideri aggiungere al filtro, quindi fai clic sul nome quando viene visualizzato nell’elenco.
   1. Ripetere il passaggio C fino a selezionare tutti gli utenti disattivati che si desidera includere nel rapporto.

1. (Facoltativo) Per limitare l’elenco dei rapporti ai rapporti pianificati:

   1. Seleziona la scheda **Filtri**, quindi fai clic su **Aggiungi regola filtro**.

   1. Aggiungi il filtro **ID report pianificato** > **Non è vuoto**.

1. Fai clic su **Salva + Chiudi**, quindi digita un nome per il report e fai clic su **Salva report**.

   Vengono visualizzate le informazioni del rapporto.

1. (Facoltativo) Esporta il report in Excel e salvalo nel computer.\
   Per informazioni sull&#39;esportazione di un report, vedere [Esporta dati](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Aggiornare le informazioni su un report

Dopo aver creato il rapporto, puoi aggiornarlo in base alle esigenze.

1. Vai al rapporto che desideri aggiornare.
1. A seconda dell&#39;azione che si desidera eseguire, eseguire una delle operazioni seguenti:

   * Aggiornare **Esegui il report con i diritti di accesso di:** a un utente attivo: per ulteriori informazioni, vedere [Esegui e recapita un report con i diritti di accesso di un altro utente](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * Creare una copia del report: per ulteriori informazioni, vedere [Creare una copia di un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * Eliminare un report: per ulteriori informazioni, vedere la sezione [Creare una copia esatta di un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) dell&#39;articolo [Creare una copia di un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * Condividi un report: per ulteriori informazioni, consulta [Condividi un report in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Condizionale) Se si copiano i report originali, utilizzare le informazioni del report creato in [Creare il report sui report esistenti](#create-the-report-about-existing-reports) per condividere le nuove copie con le stesse entità dei report originali.
