---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Approvare una scheda orario
description: Il processo di approvazione delle schede orario fornisce ai responsabili visibilità sulle ore lavorative dei loro referenti diretti. Gli approvatori possono verificare che tutto il tempo registrato sia stato assegnato nelle aree corrette e che sia stato registrato un numero sufficiente di ore per il periodo.
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# Approvare una scheda orario

Il processo di approvazione delle schede orario fornisce ai responsabili visibilità sulle ore lavorative dei loro referenti diretti. Gli approvatori possono verificare che tutto il tempo registrato sia stato assegnato nelle aree corrette e che sia stato registrato un numero sufficiente di ore per il periodo.

Adobe Workfront consente di configurare le approvazioni delle schede orario per il supporto in quest’area.

Per informazioni sull&#39;invio di una scheda orario, vedere [Inviare una scheda orario per l&#39;approvazione](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
 </tbody> 
</table>

*Per conoscere il piano o il tipo di licenza di cui si dispone, contattare l&#39;amministratore Workfront.

## Designa approvatori scheda orario

In genere, le schede orario vengono approvate da responsabili funzionali o dal personale delle risorse umane. Le schede orario non vengono normalmente approvate dai project manager.

Durante la creazione del profilo della scheda orario viene definito un approvatore della scheda orario. È necessario disporre di una licenza Pianificazione per essere designato come approvatore.

Per ulteriori informazioni sulla designazione degli approvatori della scheda orario, vedere la sezione [Creare o modificare un profilo della scheda orario](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) nell&#39;articolo [Creare, modificare e assegnare profili della scheda orario](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Approvare una scheda orario

Puoi approvare qualsiasi scheda orario inviata se sei stato designato come approvatore. Quando una scheda orario viene inviata per l&#39;approvazione, questa è elencata nell&#39;area **Approvazioni** della **Home**  pagina. Per ulteriori informazioni, vedere [Approvazione del lavoro](../../review-and-approve-work/manage-approvals/approving-work.md).

Se l&#39;amministratore di Workfront ha attivato i gestori eventi Approvazione scheda orario e Rifiuto scheda orario per utente, l&#39;utente riceverà una notifica dopo l&#39;approvazione o il rifiuto della scheda orario. Per informazioni sull&#39;attivazione delle notifiche degli eventi, vedere [Tipi di notifica degli eventi](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Per approvare una scheda orario:

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront.
1. Fai clic su **Schede orario**.
1. Seleziona **Le mie approvazioni schede orario** nell&#39;angolo superiore destro della pagina per visualizzare solo le schede orario che hai approvato

   Oppure

   Seleziona il filtro **Le mie approvazioni scheda orario** nella parte superiore dell&#39;elenco delle schede orario.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >L&#39;opzione Approvazioni schede attività personali non viene visualizzata nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo ha rimosso il filtro Approvazioni schede attività personali dai controlli elenco nell&#39;area Configura o dal modello di layout. Per ulteriori informazioni, consulta i seguenti articoli:
   >
   >   
   >   
   >   * [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Facoltativo) Fai clic sull&#39;icona **ricerca** ![](assets/search-icon.png) nella parte superiore dell&#39;elenco delle schede orario e digita una parola chiave per individuare una scheda orario specifica. È possibile cercare un intervallo di tempo o il nome di un proprietario o di un approvatore.
1. Fai clic sull’intervallo di tempo per la scheda orario da approvare. Viene visualizzata la scheda orario.

   >[!TIP]
   >
   >Le schede orario in attesa di approvazione hanno lo stato [!UICONTROL Inviato].


1. Fai clic su **Approva**

   Oppure

   Se desideri rifiutare la scheda orario, fai clic su **Rifiuta** nell&#39;angolo inferiore sinistro della scheda orario.

   Se approvato, lo stato della scheda orario diventa **Chiuso**.

   Se viene rifiutato, lo stato della scheda orario diventa **Rifiutato**.
