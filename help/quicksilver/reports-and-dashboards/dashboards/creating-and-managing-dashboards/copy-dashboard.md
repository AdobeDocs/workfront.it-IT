---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Copiare una dashboard
description: È possibile copiare un dashboard e tutto il relativo contenuto (report, calendari e pagine esterne). Quando si copiano i contenuti di un dashboard, è possibile scegliere di mantenerli così come vengono visualizzati nel dashboard originale oppure di creare nuovi elementi, ovvero copie di quelli presenti nel dashboard originale. È inoltre possibile scegliere di non trasferire o copiare elementi nel nuovo dashboard.
author: Courtney
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 6%

---

# Copiare una dashboard

<!-- Audited: 1/2025 -->

È possibile copiare un dashboard e tutto il relativo contenuto (report, calendari e pagine esterne). Quando si copiano i contenuti di un dashboard, è possibile scegliere di mantenerli così come vengono visualizzati nel dashboard originale oppure di creare nuovi elementi, ovvero copie di quelli presenti nel dashboard originale. È inoltre possibile scegliere di non trasferire o copiare elementi nel nuovo dashboard.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
      <p>Standard</p>
      <p>Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a report, dashboard e calendari</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Visualizzare l’accesso a un dashboard</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di poter copiare un dashboard, è necessario crearne uno.

Per informazioni sulla creazione dei dashboard, vedere [Creare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Copiare una dashboard

1. Fate clic sull&#39;icona **[!UICONTROL Menu principale]** ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fate clic sull&#39;icona **[!UICONTROL Menu principale]** ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fate clic su **[!UICONTROL Dashboard]**.

1. Seleziona il dashboard da copiare, quindi fai clic sull&#39;icona **Copia** ![Copia](assets/copy-icon.png).\
   Oppure\
   Apri il dashboard da copiare, quindi fai clic su **Azioni dashboard** > **Copia**.\
   Viene visualizzata la finestra di dialogo Copia dashboard. Tutti gli elementi del dashboard originale vengono visualizzati.

1. Nel campo **Nome dashboard**, specificare un nuovo nome per il dashboard.
1. Per selezionare tutti gli elementi nel dashboard esistente e copiarli nel dashboard copiato, lasciare selezionato **Seleziona tutto**. Per impostazione predefinita, i report, i calendari o gli elenchi nel dashboard esistente verranno copiati nel nuovo dashboard.\
   Oppure\
   Per trasferire solo elementi specifici dal dashboard originale a quello nuovo, deselezionare gli elementi che non si desidera visualizzare nel nuovo dashboard, quindi scegliere tra le opzioni seguenti per ogni elemento selezionato:

   * **Crea una copia:** l&#39;elemento viene copiato dal dashboard originale e una nuova versione dell&#39;elemento viene visualizzata nel nuovo dashboard. Le modifiche apportate all&#39;elemento nel nuovo dashboard non vengono riportate nell&#39;elemento nel dashboard originale. Analogamente, le modifiche apportate all&#39;elemento nel dashboard originale non vengono applicate all&#39;elemento nel nuovo dashboard.\
     Utilizzare questa opzione se si desidera modificare il report originale nel dashboard originale.\
     Ad esempio, puoi copiare un dashboard denominato &quot;Team B&quot; e rinominarlo in &quot;Team A&quot;. Nel dashboard &#39;Team B&#39; è presente un report denominato &#39;Team B Report&#39;. Poiché questo report contiene dati specifici del team B, puoi selezionare l’opzione per creare una copia del report in modo da personalizzarlo per il team A e rinominarlo in seguito in &quot;Report team A&quot;.\
     Con questa opzione, rimuovi le autorizzazioni di condivisione del report originale dal report copiato. Il report Esegui con diritti di accesso alle informazioni rimane intatto nel report copiato.

   * **Usa originale:** Visualizza l&#39;elemento originale nel nuovo dashboard. Le modifiche apportate all&#39;elemento nel nuovo dashboard vengono applicate anche all&#39;elemento nel dashboard originale. Analogamente, le modifiche apportate all&#39;elemento nel dashboard originale vengono applicate anche all&#39;elemento nel nuovo dashboard.\
     Con questa opzione, manterrai le autorizzazioni di condivisione del report originale. Anche il report Esegui con diritti di accesso alle informazioni rimane intatto.

1. (Facoltativo) Rinominate gli elementi selezionati.
1. Fai clic su **Copia dashboard**.
1. (Facoltativo) Per modificare i report, i calendari o le pagine esterne copiati nel dashboard copiato, effettua una delle seguenti operazioni:

   * Per modificare le informazioni per i report copiati, fai clic sul nome del report nel dashboard, quindi seleziona **Azioni report** > **Modifica**.

     È ad esempio possibile modificare la visualizzazione, il filtro, il raggruppamento, il prompt o il grafico o un report copiato.

   * Per ripristinare le autorizzazioni sui report copiati, fai clic sul nome del report nel nuovo dashboard, quindi fai clic su **Azioni report** > **Condivisione** e aggiorna le autorizzazioni sul report.

     Quando si copia un report durante la copia di un dashboard, le autorizzazioni per tale report vengono rimosse.

   * Per modificare il report Esegui con i diritti di accesso alle informazioni, fai clic sul nome del report nel nuovo dashboard, quindi **Azioni report** > **Modifica** > **Opzioni report**.\
     Dopo aver copiato un report, il report Esegui con i diritti di accesso delle autorizzazioni viene mantenuto solo nelle seguenti circostanze:

     Se nessuna di queste condizioni è vera, il comando Esegui questo report con i diritti di accesso delle autorizzazioni viene rimosso e il nuovo comando Esegui questo report con i diritti di accesso di viene modificato nell&#39;utente che ha creato il report copiato.

     Se l’utente che copia il dashboard e i relativi report dispone dei diritti di accesso come Amministratore.

      * Se l’utente che copia il dashboard e i relativi report dispone dei diritti di accesso come Amministratore.
      * Se l’utente che copia il dashboard e i relativi report sono attualmente impostati come Esegui questo report con i diritti di accesso di per i report copiati.
      * Se l’utente che copia il report dispone delle autorizzazioni Gestione per il report.
