---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Stampare un dashboard
description: È possibile stampare o esportare un dashboard in un file PDF. Per stampare un dashboard, è necessario disporre dell'autorizzazione per visualizzarlo.
author: Nolan
feature: Reports and Dashboards
exl-id: 30f3481b-23b6-4dc9-be0d-9cffd5d4dfed
source-git-commit: a9abbeaa9abd0e905c60000a218eddb85d0389b9
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Stampare un dashboard

<!-- Audited: 1/2025 -->

È possibile stampare o esportare un dashboard in un file PDF. Per stampare un dashboard, è necessario disporre dell&#39;autorizzazione per visualizzarlo.

>[!NOTE]
>
>Questa funzione può essere utilizzata solo con la vista Dashboard standard. Non è disponibile per le dashboard incorporate nell’area Progetti o impostate come schede personalizzate.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>piano Adobe Workfront</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront</strong></td> 
      <td> 
      <p>Nuovo:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Corrente:</p>
         <ul>
         <li><p>Lavoro o superiore</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso</strong></td> 
   <td> <p>Accesso a report, dashboard e calendari</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong>/td&gt; 
   <td> <p>Visualizzare le autorizzazioni per il dashboard</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

È necessario creare il dashboard prima di stamparlo.

Per informazioni sulla creazione di dashboard, vedere [Creare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Informazioni da stampare durante la stampa di un dashboard

Quando si stampa un dashboard o lo si salva come file PDF, è possibile che alcune informazioni del dashboard non vengano visualizzate nel file stampato o esportato, come quelle visualizzate nell’applicazione Web Adobe Workfront.

* [Cosa viene visualizzato?](#what-is-displayed)
* [Cosa non viene visualizzato?](#what-is-not-displayed)

### Cosa viene visualizzato? {#what-is-displayed}

Le seguenti informazioni sono incluse nel file del dashboard stampato o esportato:

* Titolo dashboard
* Titoli dei rapporti
* Timestamp dell’ultima generazione del rapporto
* Tutti gli oggetti nel dashboard, incluse le visualizzazioni elenco, le pagine Web esterne, i report e i calendari
* Logo della società, se personalizzato dall&#39;amministratore di Workfront nella barra di navigazione globale. Per ulteriori informazioni sul branding del sito Workfront, consulta [Personalizza l&#39;istanza Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### Cosa non viene visualizzato? {#what-is-not-displayed}

Le seguenti informazioni non sono incluse nel file del dashboard stampato o esportato:

* Barra di navigazione di Workfront
* Qualsiasi altra formattazione specifica di Workfront
* A seconda delle dimensioni dei report e del numero e della larghezza delle singole colonne, l’esportazione e la stampa di un dashboard potrebbero causare la disattivazione di alcune colonne.

## Stampare un dashboard

1. Passare alla dashboard che si desidera stampare.
1. Effettuare una delle seguenti operazioni:

   * Fai clic su **Azioni dashboard** > **Anteprima di stampa**

   * Premi **Ctrl+P** (su Windows) o **Comando+P** (su Mac)

     >[!IMPORTANT]
     >
     >* Nessuna di queste opzioni è disponibile quando il dashboard è incorporato in una scheda personalizzata. Per informazioni sulla creazione di schede personalizzate, vedere [Creare schede o sezioni personalizzate](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
     >* L&#39;opzione scelta rapida da tastiera non è disponibile quando si utilizza Internet Explorer.

1. Nel campo **Destinazione**, seleziona tra le varie opzioni di stampa disponibili.\
   Le opzioni di stampa variano a seconda del browser e della versione del browser utilizzati.

1. (Facoltativo) Salva il dashboard come file PDF, quindi fai clic su **Salva** per salvare il file PDF.\
   Per informazioni su come salvare il dashboard come file PDF, vedere [Esportare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

1. Fare clic su **Stampa**.
