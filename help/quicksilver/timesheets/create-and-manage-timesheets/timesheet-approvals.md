---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Approva una scheda attività
description: Il processo di approvazione dei fogli presenze offre ai manager visibilità sulle ore lavorative dei loro rapporti diretti. Gli approvatori possono verificare che tutto il tempo registrato sia stato assegnato nelle aree corrette e che sia stato registrato un numero sufficiente di ore per il periodo.
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Approva una scheda attività

Il processo di approvazione dei fogli presenze offre ai manager visibilità sulle ore lavorative dei loro rapporti diretti. Gli approvatori possono verificare che tutto il tempo registrato sia stato assegnato nelle aree corrette e che sia stato registrato un numero sufficiente di ore per il periodo.

Adobe Workfront consente di configurare le approvazioni dei fogli presenze per supportare in questa area.

Per informazioni sull&#39;invio di una scheda attività, vedere [Invia una scheda attività per l&#39;approvazione](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Designazione degli approvatori della scheda attività

In genere, i fogli ore sono approvati dai responsabili funzionali o dal personale delle risorse umane. (I fogli ore non vengono normalmente approvati dai project manager).

Durante la creazione del profilo della scheda attività viene definito un approvatore della scheda attività. È necessario disporre di una licenza Plan per essere designato come approvatore.

Per ulteriori informazioni sulla designazione degli approvatori della scheda attività, vedere la sezione [Creare o modificare un profilo di una scheda attività](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) nell&#39;articolo [Creare, modificare e assegnare profili della scheda attività](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Approva una scheda attività

Puoi approvare tutti i fogli ore inviati in cui sei stato designato come approvatore. Quando una scheda attività viene inviata per l&#39;approvazione, la scheda attività è elencata nella **Approvazioni** area **Pagina principale**  pagina. Per ulteriori informazioni, consulta [Approvazione del lavoro](../../review-and-approve-work/manage-approvals/approving-work.md).

Se l&#39;amministratore Workfront ha abilitato l&#39;approvazione della scheda attività per l&#39;utente e il rifiuto della scheda attività per i gestori di eventi utente, viene inviata una notifica dopo l&#39;approvazione o il rifiuto della scheda attività. Per informazioni sull&#39;abilitazione delle notifiche degli eventi, vedi [Notifiche di eventi disponibili in Adobe Workfront](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Per approvare una scheda attività:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.
1. Fai clic su **Schede temporali**.
1. Seleziona la **Approvazioni foglio presenze personali** nell’angolo in alto a destra della pagina per visualizzare solo i fogli presenze approvati

   Oppure

   Seleziona la **Approvazioni foglio presenze personali** nella parte superiore dell&#39;elenco delle schede attività.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >L&#39;opzione Approvazioni foglio presenze personale non viene visualizzata nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo ha rimosso il filtro Approvazioni foglio presenze personali dall&#39;area Controlli elenco nell&#39;area Configurazione o dal modello di layout. Per ulteriori informazioni, consulta i seguenti articoli:
   * [Personalizzare filtri, visualizzazioni e gruppi utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Facoltativo) Fai clic sul pulsante **ricerca** icona ![](assets/search-icon.png) nella parte superiore dell&#39;elenco delle schede attività e digitare una parola chiave per individuare una scheda attività specifica. È possibile cercare un intervallo di tempo o il nome di un proprietario o approvatore.
1. Fare clic sull&#39;intervallo di tempo della scheda attività che si desidera approvare. Viene visualizzata la scheda attività.

   >[!TIP]
   I fogli ore in attesa di approvazione hanno uno stato [!UICONTROL Inviato].


1. Fai clic su **Approva**

   Oppure

   Se si desidera rifiutare la scheda attività, fare clic su **Rifiuta** nell&#39;angolo in basso a sinistra della scheda attività.

   Se approvato, lo stato della scheda attività cambia in **Chiuso**.

   Se rifiutato, lo stato della scheda attività cambia in **Rifiutato**.
