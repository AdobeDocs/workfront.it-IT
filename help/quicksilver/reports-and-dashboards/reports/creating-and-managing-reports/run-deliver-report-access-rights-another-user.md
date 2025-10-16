---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Eseguire e consegnare un report con i diritti di accesso di un altro utente
description: Per impostazione predefinita, gli utenti possono visualizzare solo gli oggetti di un report per il quale dispongono delle autorizzazioni di visualizzazione.
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1185'
ht-degree: 1%

---

# Eseguire e consegnare un report con i diritti di accesso di un altro utente

<!-- Audited: 11/2024 -->

Per impostazione predefinita, gli utenti possono visualizzare solo gli oggetti di un report per il quale dispongono delle autorizzazioni di visualizzazione.

È possibile consentire a tutti gli utenti di visualizzare in un report gli stessi risultati di un altro utente, indipendentemente dal loro livello di accesso o di autorizzazione sugli oggetti all&#39;interno del report.

Se esegui un rapporto con i diritti di accesso di un altro utente con un livello di accesso superiore (ad esempio, i diritti di accesso di un amministratore di Adobe Workfront), tutti gli utenti che dispongono delle autorizzazioni per visualizzare il rapporto possono visualizzare le informazioni contenute nel rapporto come l’utente specificato nel generatore di rapporti. Puoi impostare questa opzione sia per i rapporti trovati dagli utenti nell’interfaccia di Workfront, sia per i rapporti consegnati agli utenti come allegato a un messaggio e-mail.

>[!TIP]
>
>Sostituire **Esegui report con il campo Diritti di accesso di:** con un utente attivo solo quando si desidera visualizzare il report con i diritti di accesso di tale utente. Ad esempio, un utente con licenza Lavoro potrebbe non disporre delle autorizzazioni necessarie per visualizzare tutti gli elementi di un report creato da un utente con licenza Pianificazione o da un amministratore di sistema, a meno che il report non venga visualizzato con i diritti di accesso di un planner o di un amministratore di sistema.\
>Se il report è condiviso con utenti con accesso simile a quello specificato dall&#39;utente nel campo **Esegui report con diritti di accesso di:**, è possibile lasciare vuoto il campo.

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
      <p>Piano</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
     <td> <p>Visualizzare le autorizzazioni per un report per visualizzare il report consegnato</p>
     <p>Gestire le autorizzazioni per un report per eseguire il report</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare un report con i diritti di accesso di un altro utente

Compilando il campo **Esegui report con i diritti di accesso di:** si garantisce che un report contenga gli stessi dati, indipendentemente dall&#39;utente che accede al report. Il report viene visualizzato come per l&#39;utente specificato.

Per essere in grado di visualizzare il report, gli utenti che vi accedono devono disporre almeno delle autorizzazioni di visualizzazione. Se l&#39;utente elencato nel campo **Esegui il report con i diritti di accesso di:** è disattivato, il report non verrà più visualizzato per gli altri utenti con cui è condiviso.

Per eseguire un report con i diritti di accesso di un altro utente:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **[!UICONTROL Reports]**.

1. Seleziona il report da visualizzare con i diritti di accesso di un altro utente.
1. Fai clic su **Azioni report**, quindi su **Modifica**.

1. Fare clic su **Impostazioni report**.

1. Nel campo **Esegui il report con i diritti di accesso di:**, iniziare a digitare il nome dell&#39;utente con cui si desidera visualizzare il report, quindi selezionarlo quando viene visualizzato nell&#39;elenco.\
   ![Esegui con diritti di accesso di](assets/unshimmed-access-rights-of.png)

   >[!NOTE]
   >
   >Gli utenti con un livello di accesso inferiore che sono autorizzati a generare report non possono selezionare un utente diverso da se stessi per il campo **Esegui report con diritti di accesso di:**.

1. Fai clic su **Fine**.
1. Fai clic su **Salva e Chiudi**.\
   Il report viene ora visualizzato per tutti gli utenti con cui è condiviso come se fosse visualizzato dall&#39;utente specificato nel campo **Esegui il report con i diritti di accesso di:**.

>[!IMPORTANT]
>
>L&#39;immissione di un utente diverso dall&#39;utente connesso per il campo **Esegui il report con i diritti di accesso di:** ha effetto sulle informazioni visualizzate nel report se il report contiene un filtro che utilizza un carattere jolly che fa riferimento all&#39;utente connesso. Il report viene visualizzato in base al valore specificato in **Esegui il report con i diritti di accesso di:** anziché in base a quanto definito nel filtro con caratteri jolly.
>
>Per ulteriori informazioni sui caratteri jolly per i campi utente, vedere la sezione &quot;Variabili basate sull&#39;utente&quot; in [Panoramica sulle variabili filtro con caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Consegna di un report con i diritti di accesso di un altro utente

Puoi impostare i rapporti da consegnare come allegati a un messaggio e-mail. Puoi impostare questi rapporti consegnati in modo che vengano visualizzati così come sono per gli utenti di un livello di accesso più alto, in modo che tutti gli utenti possano visualizzare le stesse informazioni nei rapporti consegnati. Gli utenti che vedranno il rapporto consegnato nell’e-mail devono essere aggiunti all’elenco Invia a dei destinatari all’interno della consegna del rapporto. Per ulteriori informazioni sulla configurazione di un report per la consegna, consulta l&#39;articolo [Panoramica sulla consegna del report](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Per consegnare un report con i diritti di accesso di un altro utente:

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Workfront, quindi fai clic su **Reports**.

1. Seleziona il rapporto che desideri consegnare con i diritti di accesso di un altro utente.
1. Fai clic sul nome del rapporto per selezionarlo.
1. Fai clic su **Azioni report**.
1. Fare clic su **Invia report**.

1. Nel campo **Consegna il report con i diritti di accesso di:**, iniziare a digitare il nome dell&#39;utente che si desidera visualizzare nel report come quando viene consegnato in un&#39;e-mail, quindi selezionarlo quando viene visualizzato nell&#39;elenco. L’impostazione predefinita è il nome dell’utente che genera il rapporto.\
   ![Report inviato con diritti di accesso di](assets/unshimmed-send-report-access-rights-of.png)

   >[!NOTE]
   >
   >Gli utenti con un livello di accesso inferiore che sono autorizzati a generare report non possono selezionare un utente diverso da loro per il campo **Consegna il report con i diritti di accesso di:**.

1. Selezionare il **Formato** che si desidera venga visualizzato nel messaggio di posta elettronica:

   * HTML
   * PDF
   * Excel
   * Excel (.xlsx)
   * TSV

1. Fai clic su **Invia ora** per inviarlo immediatamente.\
   Oppure\
   Fare clic su **Crea consegna ripetuta** per pianificare una consegna ricorrente per il report.\
   Per ulteriori informazioni sulle consegne dei report, consulta l&#39;articolo [Panoramica sulla consegna dei report](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Limitazioni per i rapporti con una colonna Source

Nei seguenti rapporti viene visualizzata una colonna Source in cui è possibile visualizzare informazioni sull&#39;oggetto padre:

* Rapporti sui problemi
* Rapporti orari
* Report documenti

Se gli utenti non dispongono delle autorizzazioni per l’oggetto principale di un problema, un’ora o un documento, la colonna Source del rapporto risulta vuota, anche se il rapporto è configurato per la visualizzazione, o per essere consegnato con i diritti di accesso di un altro utente.

Per visualizzare informazioni sull&#39;oggetto padre nel report, è consigliabile aggiungere una colonna per l&#39;oggetto padre in cui è possibile visualizzare il nome dell&#39;oggetto padre.

Ad esempio, puoi aggiungere uno dei seguenti elementi a un rapporto con una colonna Source:

* Le colonne Nome progetto, Nome attività o Nome problema in un documento o in una relazione sulle ore.
* Le colonne Nome progetto o Nome attività di un report sui problemi.
* Colonna che utilizza espressioni in modalità testo che fa riferimento a tutti e tre gli oggetti. Di seguito è riportato un esempio per un rapporto di ore:

  ```
  displayname=Custom Source
  
  linkedname=opTask
  
  namekey=view.relatedcolumn
  
  namekeyargkey.0=opTask
  
  namekeyargkey.1=name
  
  textmode=true
  
  valueexpression=IF(!ISBLANK({opTaskID}),{opTask}.{name},IF(!ISBLANK({taskID}),{task}.{name},IF(!ISBLANK({projectID}),{project}.{name},IF(!ISBLANK({timesheetID}),CONCAT({owner}.{name}," ",{timesheet}.{startDate}," - ",{timesheet}.{endDate}),""))))
  
  valueformat=HTML
  ```

  Per informazioni sulle visualizzazioni in modalità testo, vedere [Modificare una visualizzazione utilizzando la modalità testo](../text-mode/edit-text-mode-in-view.md).
