---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Copiare un dashboard
description: È possibile copiare un dashboard e tutto il relativo contenuto (report, calendari e pagine esterne). Quando copiate il contenuto di un quadro comandi, potete scegliere di mantenerlo così come viene visualizzato nel quadro comandi originale oppure creare nuovi elementi, ovvero copie di quelli presenti nel quadro comandi originale. È inoltre possibile scegliere di non trasferire o copiare elementi nel nuovo dashboard.
author: Nolan
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Copiare un dashboard

È possibile copiare un dashboard e tutto il relativo contenuto (report, calendari e pagine esterne). Quando copiate il contenuto di un quadro comandi, potete scegliere di mantenerlo così come viene visualizzato nel quadro comandi originale oppure creare nuovi elementi, ovvero copie di quelli presenti nel quadro comandi originale. È inoltre possibile scegliere di non trasferire o copiare elementi nel nuovo dashboard.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>Modificare l’accesso a rapporti, dashboard e calendari</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Visualizzare l’accesso a un dashboard</p> <p>Otterrai l’accesso Gestisci al dashboard copiato</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisiti

È necessario creare una dashboard prima di poterla copiare.

Per informazioni sulla creazione di dashboard, vedere [Creare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Copiare un dashboard

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale**, quindi fai clic su **Dashboard**.

1. Seleziona il dashboard da copiare, quindi fai clic su **Copia** ![](assets/copy-icon.png).\
   Oppure\
   Apri il dashboard da copiare, quindi fai clic su **Azioni dashboard** > **Copia**.\
   Viene visualizzata la finestra di dialogo Copia dashboard. Vengono visualizzati tutti gli elementi nel quadro comandi originale.

1. Nel campo **Nome dashboard**, specificare un nuovo nome per il dashboard.
1. Per selezionare tutti gli elementi nel dashboard esistente e copiarli nel dashboard copiato, lasciare selezionato **Seleziona tutto**. Per impostazione predefinita, i report, i calendari o gli elenchi del dashboard esistente verranno copiati nel nuovo dashboard.\
   Oppure\
   Per trasferire solo elementi specifici dal dashboard originale a quello nuovo, deselezionare gli elementi che non si desidera visualizzare nel nuovo dashboard, quindi per ogni elemento selezionato, scegliere una delle opzioni seguenti:

   * **Copia:** l&#39;elemento viene copiato dal dashboard originale e nel nuovo dashboard viene visualizzata una nuova versione dell&#39;elemento. Le modifiche apportate all&#39;elemento nel nuovo dashboard non vengono applicate all&#39;elemento nel dashboard originale. Analogamente, le modifiche apportate all&#39;elemento nel dashboard originale non vengono applicate all&#39;elemento nel nuovo dashboard.\
     Utilizzate questa opzione per modificare il report originale nel quadro comandi originale.\
     Ad esempio, si copia un dashboard denominato &quot;Team B&quot; e lo si rinomina &quot;Team A&quot;. Nel dashboard &quot;Team B&quot; è presente un report denominato &quot;Report team B&quot;. Poiché questo report contiene dati specifici del Team B, è possibile selezionare l&#39;opzione per creare una copia del report in modo da personalizzarlo per il Team A e rinominarlo successivamente in &quot;Report Team A&quot;.\
     Con questa opzione, rimuovi le autorizzazioni di condivisione del rapporto originale dal rapporto copiato. Il report Esegui con i diritti di accesso alle informazioni rimane intatto nel report copiato.

   * **Usa originale:** Visualizza l&#39;elemento originale nel nuovo dashboard. Le modifiche apportate all&#39;elemento nel nuovo dashboard vengono applicate anche all&#39;elemento nel dashboard originale. Analogamente, le modifiche apportate all&#39;elemento nel dashboard originale vengono applicate all&#39;elemento nel nuovo dashboard.\
     Con questa opzione, mantieni le autorizzazioni di condivisione del rapporto originale. Anche il report Esegui con i diritti di accesso alle informazioni rimane intatto.

1. (Facoltativo) Rinomina gli elementi selezionati.
1. Fai clic su **Copia dashboard**.
1. (Facoltativo) Se desiderate modificare i rapporti, i calendari o le pagine esterne copiati nel dashboard copiato, effettuate una delle seguenti operazioni:

   * Per modificare le informazioni per i report copiati, fare clic sul nome del report nel dashboard e quindi **Azioni report** > **Modifica**.

     È ad esempio possibile modificare la visualizzazione, il filtro, il raggruppamento, il prompt o il grafico oppure un report copiato.

   * Per ripristinare le autorizzazioni sui report copiati, fare clic sul nome del report nel nuovo dashboard, quindi fare clic su **Azioni report** > **Condivisione** e aggiornare le autorizzazioni sul report.

     Quando copi un report durante la copia di un dashboard, le autorizzazioni su tale report vengono rimosse.

   * Per modificare il report Esegui con i diritti di accesso alle informazioni, fare clic sul nome del report nel nuovo dashboard, quindi **Azioni report** > **Modifica** > **Opzioni report**.\
     Dopo aver copiato un report, il report Esegui con i diritti di accesso delle autorizzazioni viene mantenuto solo nelle seguenti circostanze:

     Se nessuna di queste condizioni è vera, Esegui questo report con i diritti di accesso delle autorizzazioni viene rimosso e la nuova opzione Esegui questo report con i diritti di accesso di viene modificata per l’utente che ha creato il report copiato.

     Se l’utente che copia il dashboard e i relativi report dispone dei diritti di accesso di amministratore.

      * Se l’utente che copia il dashboard e i relativi report dispone dei diritti di accesso di amministratore.
      * Se l’utente che copia il dashboard e i relativi rapporti è attualmente impostato come Esegui questo rapporto con i diritti di accesso di per i rapporti da copiare.
      * Se l’utente che copia il rapporto dispone delle autorizzazioni di gestione per il rapporto.
