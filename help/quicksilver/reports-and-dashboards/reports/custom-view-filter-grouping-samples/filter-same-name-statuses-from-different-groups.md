---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: consente di visualizzare gli elementi in base agli stati con lo stesso nome quando gli stati sono associati a gruppi diversi'
description: È possibile assegnare uno stato attività al gruppo A denominato Nuovo stato con la chiave di 3 lettere NST. È possibile che al gruppo B venga assegnato un altro stato di attività denominato anche Nuovo stato con la chiave di 3 lettere NES. Anche se i nomi per i 2 stati possono essere identici, il codice di 3 lettere è sempre univoco. Per ulteriori informazioni sugli stati dei gruppi, vedere Creare o modificare uno stato dei gruppi.
author: Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Filtro: consente di visualizzare gli elementi in base agli stati con lo stesso nome quando gli stati sono associati a gruppi diversi

<!--Audited: 10/2024-->

È possibile assegnare uno stato attività al gruppo A denominato *Nuovo stato* con la chiave di 3 lettere *NST*. È possibile che al gruppo B venga assegnato un altro stato di attività denominato anche *Nuovo stato* con la chiave di 3 lettere *NES.* Anche se i nomi per i due stati possono essere identici, il codice di 3 lettere è sempre univoco.

Per ulteriori informazioni sugli stati dei gruppi, vedere [Creare o modificare lo stato di un gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Utilizzando il generatore di filtri, non è possibile identificare tra i 2 stati che hanno lo stesso nome. È necessario utilizzare la modalità Testo in un filtro personalizzato per distinguere i due stati.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un rapporto</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizza gli elementi in base agli stati con lo stesso nome quando gli stati sono associati a gruppi diversi

1. Vai al menu a discesa **Filtro** per il filtro che desideri personalizzare per un elenco di attività, ad esempio.\
   Funziona allo stesso modo anche per progetti e problemi.
1. Fare clic su **Nuovo filtro**.
1. Dal primo elenco a discesa in alto a sinistra, selezionare Task > Status (Attività > Stato).
1. Seleziona **È uguale a** per il modificatore, quindi seleziona uno degli stati su cui vuoi creare un rapporto.

   In un report attività, ad esempio, aggiungere **Stato uguale a nuovo stato** se si desidera visualizzare solo le attività con stato **Nuovo stato**.

   >[!TIP]
   >
   >Si noti che è disponibile una sola opzione per uno stato denominato Nuovo stato.

1. Fare clic su **Modalità testo**.\
   Nello spazio disponibile deve essere visualizzato il seguente codice:

   <pre>OR:1:status=NST<br>OR:1:status_Mod=in </pre>

   >[!NOTE]
   >
   >Qui viene visualizzato un solo stato. Nella riga di stato viene visualizzata una delle chiavi a 3 lettere per uno degli stati.

1. Aggiungi le seguenti 2 righe di codice per aggiungere lo stato mancante dal filtro:

   <pre>OR:2:status=NES<br>OR:2:status_Mod=in</pre>

1. Fai clic su **Applica**, quindi su **Salva come nuovo**.

   Nell&#39;elenco vengono visualizzate entrambe le attività con lo stato &quot;Nuovo stato&quot; dal gruppo A e con lo stato &quot;Nuovo stato&quot; dal gruppo B.
