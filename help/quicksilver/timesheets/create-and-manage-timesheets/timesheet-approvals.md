---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Approva una scheda orario
description: Il processo di approvazione delle schede orario fornisce ai responsabili visibilità sulle ore lavorative dei loro referenti diretti. Gli approvatori possono verificare che tutto il tempo registrato sia stato assegnato nelle aree corrette e che sia stato registrato un numero sufficiente di ore per il periodo.
author: Lisa
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 0%

---

# Approvare una scheda orario

<!--Audited: 8/2024-->

Il processo di approvazione delle schede orario fornisce ai responsabili visibilità sulle ore lavorative dei loro referenti diretti. Gli approvatori possono verificare che tutto il tempo registrato sia stato assegnato nelle aree corrette e che sia stato registrato un numero sufficiente di ore per il periodo.

Adobe Workfront consente di configurare le approvazioni delle schede orario per il supporto in quest’area.

Per informazioni sull&#39;invio di una scheda orario, vedere [Inviare una scheda orario per l&#39;approvazione](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

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
   <td>
   <p>Standard</p>
   <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td><p>Accesso amministrativo a schede orario e ore</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Designa approvatori scheda orario

In genere, le schede orario vengono approvate da responsabili funzionali o dal personale delle risorse umane. Le schede orario in genere non vengono approvate dai project manager. I project manager possono approvare i progetti connessi all&#39;ora, ma i team o i responsabili delle risorse umane devono approvare le schede orario.

Durante la creazione del profilo della scheda orario viene definito un approvatore della scheda orario. È necessario disporre di una licenza Pianificazione per essere designato come approvatore.

Per ulteriori informazioni sulla designazione degli approvatori della scheda orario, vedere la sezione [Creare o modificare un profilo della scheda orario](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) nell&#39;articolo [Creare, modificare e assegnare profili della scheda orario](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Approvare una scheda orario

Puoi approvare qualsiasi scheda orario inviata se sei stato designato come approvatore. Quando una scheda orario viene inviata per l&#39;approvazione, la scheda orario è elencata nel widget **Approvazioni personali** nell&#39;area **Home**. Per ulteriori informazioni, vedere [Approvazione del lavoro](../../review-and-approve-work/manage-approvals/approving-work.md).

Se sono attive le seguenti impostazioni di notifica, l’utente che invia la scheda orario per l’approvazione riceve un’e-mail dopo l’approvazione di una scheda orario:

* L&#39;amministratore di Workfront ha abilitato i gestori eventi Approvazione scheda orario per utente e Rifiuto scheda orario per utente. Per informazioni sull&#39;attivazione delle notifiche degli eventi, vedere [Tipi di notifica degli eventi](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
* La notifica personale La mia scheda orario è approvata è abilitata nella pagina del profilo dell&#39;utente. Per ulteriori informazioni, vedere [Modificare le proprie notifiche e-mail](/help/quicksilver/workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Approvare una scheda orario dall&#39;area Schede orario

{{step1-to-timesheets}}

Verrà aperta l&#39;area **Schede orario**.

1. (Condizionale) Se l&#39;ultimo accesso è avvenuto, fai clic su **Torna alle schede orario** nell&#39;angolo in alto a sinistra dello schermo.

1. Seleziona **Le mie approvazioni schede orario** nell&#39;angolo superiore destro della pagina per visualizzare solo le schede orario che hai approvato

   Oppure

   Seleziona il filtro **Le mie approvazioni scheda orario** nella parte superiore dell&#39;elenco delle schede orario.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >L&#39;opzione Approvazioni schede attività personali non viene visualizzata nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo ha rimosso il filtro Approvazioni schede attività personali dai controlli elenco nell&#39;area Configura o dal modello di layout.
   >
   >Per ulteriori informazioni, vedere [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
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

### Approvare una scheda orario dalla sezione Home

{{step1-to-home}}

Viene visualizzata l’area Home.

1. Verifica che il widget **Le mie approvazioni** sia stato aggiunto alla tua area Home. Per ulteriori informazioni, vedere [Aggiungere, modificare o rimuovere widget nella nuova home](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md).
1. Trova un&#39;approvazione della scheda orario nel widget Le mie approvazioni.
1. (Facoltativo) Espandi il menu a discesa a destra dei pulsanti Approva o Rifiuta per aggiungere un commento sulla tua decisione, quindi fai clic su **Aggiungi**.
1. Fai clic su uno dei seguenti pulsanti per prendere la decisione relativa all’approvazione:

   * Approvazione
   * Rifiuta

   L&#39;approvazione è stata rimossa dal widget **Approvazioni personali**.


