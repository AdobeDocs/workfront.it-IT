---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: consente di visualizzare gli elementi in base agli stati con lo stesso nome quando gli stati sono associati a gruppi diversi.'
description: È possibile assegnare uno stato attività al gruppo A denominato Nuovo stato con la chiave di tre lettere NST. È possibile che al gruppo B sia assegnato un altro stato di attività denominato anche Nuovo stato con la chiave di tre lettere NES. Anche se i nomi per i due stati possono essere identici, il codice a 3 lettere è sempre univoco. Per ulteriori informazioni sugli stati dei gruppi, vedere Creare o modificare uno stato dei gruppi.
author: Courtney
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 11%

---

# Filtro: visualizzare gli elementi in base agli stati con lo stesso nome quando gli stati sono associati a gruppi diversi

<!--Audited: 10/2024-->

È possibile assegnare uno stato dell&#39;attività al gruppo A denominato *Nuovo stato* con la chiave a 3 lettere *NST*. È possibile che al gruppo B sia assegnato un altro stato di attività denominato anche *Nuovo stato* con la chiave di 3 lettere *NES.* Sebbene i nomi per i due stati possano essere identici, il codice di tre lettere è sempre univoco.

Per ulteriori informazioni sugli stati dei gruppi, vedere [Creare o modificare uno stato dei gruppi](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Utilizzando il generatore di filtri, non è possibile identificare tra i due stati che hanno lo stesso nome. È necessario utilizzare la modalità Testo in un filtro personalizzato per distinguere tra i due stati.

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
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a report, dashboard, calendari</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un report</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizza gli elementi in base allo stato con lo stesso nome quando gli stati sono associati a gruppi diversi

1. Andare all&#39;elenco a discesa **Filtro** per il filtro che si desidera personalizzare per un elenco di attività, ad esempio.\
   Funziona allo stesso modo anche per i progetti e i problemi.
1. Fai clic su **Nuovo filtro**.
1. Dal primo menu a discesa nell&#39;angolo superiore sinistro, seleziona Attività > Stato.
1. Selezionare **Uguale a** per il modificatore, quindi selezionare uno degli stati per cui si desidera creare il report.

   Ad esempio, in un report attività aggiungere **Stato uguale a nuovo stato** se si desidera visualizzare solo le attività con stato **Nuovo stato**.

   >[!TIP]
   >
   >Si noti che è disponibile una sola opzione per uno stato denominato Nuovo stato.

1. Fai clic su **Modalità testo**.\
   Nello spazio disponibile deve essere visualizzato il seguente codice:

   <pre>OR:1:status=NST<br>OR:1:status_Mod=in </pre>

   >[!NOTE]
   >
   >Qui viene visualizzato un solo stato. Nella riga di stato viene visualizzato uno dei tasti di tre lettere per uno degli stati.

1. Aggiungi le seguenti due righe di codice per aggiungere lo stato mancante dal filtro:

   <pre>OR:2:status=NES<br>OR:2:status_Mod=in</pre>

1. Fare clic su **Applica**, quindi su **Salva come nuovo**.

   L&#39;elenco mostra entrambi i task con uno stato &quot;Nuovo stato&quot; dal gruppo A e con uno stato &quot;Nuovo stato&quot; dal gruppo B.
