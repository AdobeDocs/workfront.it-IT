---
product-area: Canvas Dashboards
navigation-topic: manage-canvas-dashboards
title: Condividere una dashboard dell’area di lavoro
description: Puoi condividere un dashboard Canvas con altri utenti di Adobe Workfront in modo che possano visualizzarlo o modificarlo.
author: Courtney
feature: Reports and Dashboards
exl-id: 5cb03113-35b0-49aa-86ec-ec800cd3f4dc
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 3e76f4a798a55a674a5ada2661c4b6bbb55195f2
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 9%

---

# Condividere una dashboard dell’area di lavoro

>[!IMPORTANT]
>
>La funzione Dashboard di Canvas è attualmente disponibile solo per gli utenti che partecipano alla fase beta. Alcune parti della caratteristica potrebbero non essere complete o non funzionare come previsto in questa fase. Invia un feedback relativo alla tua esperienza seguendo le istruzioni riportate nella sezione [Provide feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) dell&#39;articolo di panoramica della versione beta di Canvas Dashboards.<br>
>In caso di feedback su un possibile bug o problema tecnico, invia un ticket al supporto Workfront. Per ulteriori informazioni, vedere [Contattare l&#39;Assistenza clienti](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tieni presente che questa versione beta non è disponibile sui seguenti provider cloud:
>
>* Porta la tua chiave per Amazon Web Services
>* Azure
>* Piattaforma Google Cloud

Puoi condividere un dashboard Canvas con altri utenti di Adobe Workfront in modo che possano visualizzarlo o modificarlo.

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
   <td><p>Accesso a report, dashboard e calendari</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td><p>Visualizzare le autorizzazioni per la dashboard per condividere la dashboard</p>
   <p>Gestisci le autorizzazioni per il dashboard per assegnare le autorizzazioni del dashboard</p>
  </td> 
  </tr>
</tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Considerazioni sulla condivisione delle dashboard

* Le dashboard possono essere condivise con le risorse dell’utente, del team, del gruppo, della mansione o dell’azienda.

* Per impostazione predefinita, l’autore di un dashboard dispone delle autorizzazioni di gestione per il dashboard.

* Gli amministratori di sistema e gli utenti con l’autorizzazione Gestione possono concedere l’accesso Visualizzazione o Gestione a un dashboard.

* Gli utenti con l’autorizzazione Visualizzazione di un dashboard possono concedere l’accesso Visualizzazione a un dashboard.

* Quando condividi un dashboard, le risorse con cui è condiviso ereditano le autorizzazioni per i report visualizzati nel dashboard.

* Quando un dashboard viene distribuito tramite un modello di layout, a tutte le risorse assegnate al modello di layout viene concessa un’autorizzazione di visualizzazione automatica per il dashboard (e i relativi report).

* Quando un report su un dashboard è configurato con l’opzione Esegui come utente, tutti i visualizzatori visualizzano i dati in base alle autorizzazioni dell’utente selezionato anziché alle proprie. Ciò significa che i visualizzatori potrebbero visualizzare dati a cui normalmente non hanno accesso. Se alcuni rapporti in un dashboard utilizzano Esegui come utente e altri no, i visualizzatori potrebbero visualizzare dati non coerenti tra i rapporti.


## Condividere una dashboard dell’area di lavoro


{{step1-to-dashboards}}

1. Nel pannello a sinistra, fai clic su **Dashboard Canvas**.

1. Nella pagina **Dashboard area di lavoro** selezionare il dashboard che si desidera condividere.

1. Nell&#39;angolo superiore destro della pagina fare clic sul pulsante **Condividi**. Viene visualizzata la finestra di dialogo **Condivisione dashboard**.

   ![Pulsante Condividi](assets/share-button.png)

1. Nel campo **Concedi l&#39;accesso a**, inizia a digitare il nome di un utente, un team, una mansione, un gruppo o un&#39;azienda con cui vuoi condividere il dashboard di Canvas, quindi selezionalo quando viene visualizzato nell&#39;elenco a discesa.

1. (Facoltativo) Per modificare l&#39;accesso di una risorsa al dashboard, fai clic su **Visualizza** accanto al nome, quindi seleziona **Gestisci** nell&#39;elenco a discesa visualizzato.

   >[!NOTE]
   >
   > Se gli utenti non dispongono delle autorizzazioni di modifica per un dashboard assegnato tramite il proprio livello di accesso, non è possibile assegnare loro le autorizzazioni di gestione per un dashboard.

1. Ripeti i passaggi 5-6 per ogni risorsa con cui desideri condividere il dashboard.

1. Fai clic sul pulsante **Condividi**. I destinatari ricevono una notifica e-mail con la quale vengono informati che il dashboard è stato condiviso con loro. È ora possibile accedervi da **Dashboard** > **Dashboard canvas** > **Dashboard condivisi**.

   >[!NOTE]
   >
   > Possono essere applicate le preferenze dei singoli utenti e le esclusioni di sistema per le notifiche e-mail. <br>
   > Le notifiche vengono inviate solo se condivise direttamente con un utente. La condivisione con gruppi, ruoli, società e team non genera notifiche e-mail.<br>
   > Le autorizzazioni ereditate da un modello di layout non generano una notifica e-mail sull’accesso al dashboard.
