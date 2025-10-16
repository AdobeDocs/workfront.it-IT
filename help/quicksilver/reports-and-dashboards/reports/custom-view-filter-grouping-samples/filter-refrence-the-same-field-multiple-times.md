---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: crea più regole di filtro che fanno riferimento allo stesso campo (istruzioni "AND")'
description: Nell’interfaccia in modalità standard, quando tenti di creare più filtri che fanno riferimento allo stesso campo (utilizzando il qualificatore AND), uno dei filtri viene eliminato quando salvi il rapporto e chiudi il generatore di rapporti.
author: Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# Filtro: crea più regole di filtro che fanno riferimento allo stesso campo (istruzioni &quot;AND&quot;)

<!--Audited: 10/2024-->

Nell’interfaccia in modalità standard, quando tenti di creare più filtri che fanno riferimento allo stesso campo (utilizzando il qualificatore AND), uno dei filtri viene eliminato quando salvi il rapporto e chiudi il generatore di rapporti.

**Esempio:** È possibile visualizzare solo le attività che contengono la parola &quot;verde&quot; ma non la parola &quot;rosso&quot; nel nome. Adobe Workfront non consente di salvare le seguenti regole di filtro utilizzando l’interfaccia in modalità standard: fa riferimento allo stesso campo (Nome attività), ma utilizza modificatori diversi e fa riferimento a valori diversi:

* Nome attività > Contiene > Verde
* Nome attività > Non contiene > Rosso

Tuttavia, puoi creare questo filtro utilizzando la modalità testo.

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

## Creare più regole di filtro che fanno riferimento allo stesso campo

1. Consente di passare a un elenco di attività.
1. Dal menu a discesa **Filtro**, selezionare **Nuovo filtro**.
1. Fare clic su **Modalità testo**.
1. Nella casella visualizzata, aggiungi il seguente codice:

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >Per creare filtri simili, genera prima la prima istruzione. Ad esempio:
   >
   >```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >Copia e incolla l’istruzione il numero di volte necessario. Puoi quindi aggiungere tutte le istruzioni necessarie per fare riferimento allo stesso campo (nel nostro caso &quot;name&quot;) e apportare le seguenti modifiche alle istruzioni aggiuntive:
   >
   >1. Anteporre le due righe copiate con &quot;AND:1:&quot;, &quot;AND:2:&quot;, &quot;AND:3:&quot; e così via per ogni nuovo valore possibile del campo.
   >1. Sostituisci la riga del campo con il nuovo valore del campo (dopo il segno &quot;=&quot;).
   >1. Sostituire la linea del modificatore (_Mod) con il nuovo modificatore.
   >   
   >Queste istruzioni distinguono tra maiuscole e minuscole.

1. Fai clic su **Applica**, quindi su **Salva come nuovo**.
