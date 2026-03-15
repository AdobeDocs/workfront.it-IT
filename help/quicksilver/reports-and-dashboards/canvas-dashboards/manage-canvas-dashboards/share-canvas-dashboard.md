---
product-area: Canvas Dashboards
navigation-topic: manage-canvas-dashboards
title: Condividere una dashboard dell’area di lavoro
description: Puoi condividere una dashboard Canvas con altri utenti di Adobe Workfront in modo che possano visualizzarla o modificarla.
author: Courtney
feature: Reports and Dashboards
exl-id: 5cb03113-35b0-49aa-86ec-ec800cd3f4dc
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 10%

---

# Condividere una dashboard dell’area di lavoro

>[!IMPORTANT]
>
>La funzione Dashboard di Canvas è attualmente disponibile solo per gli utenti che partecipano alla fase beta. Durante questa fase, alcune parti della caratteristica potrebbero non essere complete o funzionare come previsto. Invia un feedback relativo alla tua esperienza seguendo le istruzioni riportate nella sezione [Provide feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) dell&#39;articolo di panoramica della versione beta di Canvas Dashboards.<br>
>Se hai un feedback su un possibile bug o problema tecnico, invia un ticket al supporto Workfront. Per ulteriori informazioni, consulta [Contatta l&#39;Assistenza clienti](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Questa versione beta non è disponibile sui seguenti provider cloud:
>
>* Porta la tua chiave per Amazon Web Services
>* Azure
>* Piattaforma Google Cloud

Puoi condividere una dashboard Canvas con altri utenti di Adobe Workfront in modo che possano visualizzarla o modificarla.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td> 
<p>Standard </p> 
<p>Piano</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td> 
   <td><p>Visualizzare l’accesso a report, dashboard e calendari</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td><p>Visualizzare le autorizzazioni per la condivisione del dashboard</p>
   <p>Gestire le autorizzazioni per il dashboard per assegnare le autorizzazioni del dashboard</p>
  </td> 
  </tr>
</tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Considerazioni sulla condivisione delle dashboard

* Le dashboard possono essere condivise con le risorse dell’utente, del team, del gruppo, della mansione o dell’azienda.

* Per impostazione predefinita, l’autore di un dashboard dispone delle autorizzazioni Gestisci per il dashboard.

* Gli amministratori di sistema e gli utenti con autorizzazione Gestisci possono concedere l&#39;accesso Visualizza o Gestisci a un dashboard.

* Gli utenti con autorizzazione Visualizzazione per un dashboard possono concedere l&#39;accesso in visualizzazione a un dashboard.

* Quando si condivide un dashboard, le risorse con cui è condiviso ereditano le autorizzazioni per i report visualizzati nel dashboard.

* Quando un dashboard viene distribuito tramite un modello di layout, un&#39;autorizzazione di visualizzazione automatica per il dashboard (e i relativi report) viene concessa a tutte le risorse assegnate al modello di layout.


## Condividere una dashboard dell’area di lavoro


{{step1-to-dashboards}}

1. Nel pannello a sinistra, fai clic su **Dashboard Canvas**.

1. Nella pagina **Dashboard area di lavoro**, seleziona il dashboard che desideri condividere.

1. Nell&#39;angolo superiore destro della pagina fare clic sul pulsante **Condividi**. Viene visualizzata la finestra di dialogo **Condivisione dashboard**.

   ![Pulsante Condividi](assets/share-button.png)

1. Nel campo **Concedi l&#39;accesso a**, inizia a digitare il nome di un utente, un team, una mansione, un gruppo o un&#39;azienda con cui vuoi condividere il dashboard di Canvas, quindi selezionalo quando viene visualizzato nell&#39;elenco a discesa.

1. (Facoltativo) Per modificare l&#39;accesso di una risorsa al dashboard, fai clic su **Visualizza** accanto al nome della risorsa, quindi seleziona **Gestisci** nell&#39;elenco a discesa visualizzato.

   >[!NOTE]
   >
   > Quando gli utenti non dispongono delle autorizzazioni di modifica per un dashboard assegnate tramite il proprio livello di accesso, non è possibile assegnare autorizzazioni di gestione a un dashboard.

1. Ripetere i passaggi da 5 a 6 per ogni risorsa con cui si desidera condividere il dashboard.

1. Fare clic sul pulsante **Condividi**. I destinatari ricevono una notifica tramite e-mail che li informa che il dashboard è stato condiviso e che ora possono accedervi in **Dashboard** > **Dashboard Canvas** > **Dashboard condivisi**.

   >[!NOTE]
   >
   > Potrebbero essere applicate le preferenze dei singoli utenti e le esclusioni di sistema per le notifiche e-mail. <br>
   > Le notifiche vengono inviate solo quando vengono condivise direttamente con un utente. La condivisione con gruppi, ruoli, società e team non genera notifiche e-mail.<br>
   > Le autorizzazioni ereditate da un modello di layout non generano una notifica e-mail sull’accesso al dashboard.
