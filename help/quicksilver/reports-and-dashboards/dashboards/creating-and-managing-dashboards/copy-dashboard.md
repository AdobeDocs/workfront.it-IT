---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Copiare un dashboard
description: È possibile copiare un dashboard e tutto il relativo contenuto (rapporti, calendari e pagine esterne). Quando copiate i contenuti di un dashboard, potete scegliere di mantenerli come visualizzati nel dashboard originale o creare nuovi elementi che sono copie di quelli nel dashboard originale. È inoltre possibile scegliere di non trasferire o copiare elementi nel nuovo dashboard.
author: Nolan
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Copiare un dashboard

È possibile copiare un dashboard e tutto il relativo contenuto (rapporti, calendari e pagine esterne). Quando copiate i contenuti di un dashboard, potete scegliere di mantenerli come visualizzati nel dashboard originale o creare nuovi elementi che sono copie di quelli nel dashboard originale. È inoltre possibile scegliere di non trasferire o copiare elementi nel nuovo dashboard.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Accesso a Reports, Dashboard e Calendari</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Visualizzare l’accesso a un dashboard</p> <p>Sarà possibile ottenere l'accesso Gestisci al dashboard copiato</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisiti

È necessario creare un dashboard prima di poterlo copiare.

Per informazioni sulla creazione di dashboard, consulta [Creare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Copiare un dashboard

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png), quindi fai clic su **Dashboard**.

1. Seleziona il dashboard da copiare, quindi fai clic su **Copia** ![](assets/copy-icon.png).\
   Oppure\
   Apri il dashboard da copiare, quindi fai clic su **Azioni dashboard** > **Copia**.\
   Viene visualizzata la finestra di dialogo Copia dashboard. Vengono visualizzati tutti gli elementi del dashboard originale.

1. In **Nome dashboard** specificare un nuovo nome per il dashboard.
1. Per selezionare tutti gli elementi del dashboard esistente e copiarli nel dashboard copiato, lasciare **Seleziona tutto** selezionato. Per impostazione predefinita, i rapporti, i calendari o gli elenchi presenti nel dashboard esistente verranno copiati nel nuovo dashboard.\
   Oppure\
   Per trasferire solo elementi specifici dal dashboard originale a quello nuovo, deselezionare gli elementi che non si desidera visualizzare nel nuovo dashboard, quindi per ogni elemento selezionato, scegliere tra le seguenti opzioni:

   * **Crea una copia:** L&#39;elemento viene copiato dal dashboard originale e una nuova versione dell&#39;elemento viene visualizzata sul nuovo dashboard. Le modifiche apportate all&#39;elemento nel nuovo dashboard non vengono applicate all&#39;elemento nel dashboard originale. Allo stesso modo, le modifiche apportate all&#39;elemento nel dashboard originale non vengono applicate all&#39;elemento nel nuovo dashboard.\
      Utilizzare questa opzione quando si desidera modificare il rapporto originale nel dashboard originale.\
      Ad esempio, si copia un dashboard denominato &quot;Team B&quot; e lo si rinomina in &quot;Team A&quot;. Nel dashboard &#39;Team B&#39; è presente un report chiamato &#39;Report Team B&#39;. Poiché il rapporto contiene dati specifici del team B, è possibile selezionare l&#39;opzione per creare una copia del rapporto in modo da personalizzarlo per il team A e rinominarlo in un secondo momento in Report team A.\
      Questa opzione consente di rimuovere le autorizzazioni di condivisione del rapporto originale dal rapporto copiato. Il rapporto Esegui questo rapporto con i diritti di accesso delle informazioni rimane intatto nel rapporto copiato.

   * **Usa originale:** Visualizza l&#39;elemento originale nel nuovo dashboard. Le modifiche apportate all&#39;elemento nel nuovo dashboard vengono riportate anche nell&#39;elemento nel dashboard originale. Allo stesso modo, le modifiche apportate all&#39;elemento nel dashboard originale vengono riportate nell&#39;elemento nel nuovo dashboard.\
      Con questa opzione, mantieni le autorizzazioni di condivisione del rapporto originale. Anche il rapporto Esegui con i diritti di accesso delle informazioni rimane intatto.

1. (Facoltativo) Rinomina gli elementi selezionati.
1. Fai clic su **Copia dashboard**.
1. (Facoltativo) Se desideri modificare uno dei rapporti, calendari o pagine esterne copiati nel dashboard copiato, effettua una delle seguenti operazioni:

   * Per modificare qualsiasi informazione relativa a uno dei rapporti copiati, fare clic sul nome del rapporto nel dashboard, quindi **Azioni dei rapporti** > **Modifica**.

      Ad esempio, è possibile modificare la visualizzazione, il filtro, il raggruppamento, il prompt o il grafico o un rapporto copiato.

   * Per ripristinare le autorizzazioni sui report copiati, fare clic sul nome del report nel nuovo dashboard, quindi fare clic su **Azioni dei rapporti** > **Condivisione** e aggiorna le autorizzazioni sul report.

      Quando copi un rapporto durante la copia di un dashboard, le autorizzazioni relative a tale rapporto vengono rimosse.

   * Per modificare il report Esegui con i diritti di accesso delle informazioni, fai clic sul nome del report nel nuovo dashboard, quindi **Azioni dei rapporti** > **Modifica** > **Opzioni rapporto**.\
      Dopo aver copiato un rapporto, il rapporto Esegui con i diritti di accesso delle autorizzazioni viene mantenuto solo nelle seguenti circostanze:

      (Se nessuna di queste condizioni è vera, l&#39;opzione Esegui questo rapporto con i diritti di accesso delle autorizzazioni viene rimossa e il nuovo rapporto Esegui questo rapporto con i diritti di accesso di viene modificato per l&#39;utente che ha creato il rapporto copiato.)

      Se l&#39;utente che copia il dashboard e i relativi rapporti dispone di diritti di accesso di amministratore.

      * Se l&#39;utente che copia il dashboard e i relativi rapporti dispone di diritti di accesso di amministratore.
      * Se l&#39;utente che copia il dashboard e i relativi rapporti è attualmente impostato come Esegui questo rapporto con i diritti di accesso di per i rapporti da copiare.
      * Se l&#39;utente che copia il rapporto dispone delle autorizzazioni di gestione per il rapporto.
