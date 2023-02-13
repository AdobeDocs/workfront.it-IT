---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: creare più regole di filtro che fanno riferimento allo stesso campo ('istruzioni AND')"
description: Nell’interfaccia in modalità standard, quando si tenta di creare più filtri che fanno riferimento allo stesso campo (utilizzando il qualificatore AND), uno dei filtri viene eliminato quando si salva il report e si esce dal generatore di report.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 8b6324302a70319f387d1e09d1eb92fbdabf7e32
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Filtro: creare più regole di filtro che fanno riferimento allo stesso campo (&quot;istruzioni AND&quot;)

Nell’interfaccia in modalità standard, quando si tenta di creare più filtri che fanno riferimento allo stesso campo (utilizzando il qualificatore AND), uno dei filtri viene eliminato quando si salva il report e si esce dal generatore di report.

**Esempio:** È possibile visualizzare solo le attività che contengono la parola &quot;verde&quot; ma non contengono la parola &quot;rosso&quot; nel nome. Adobe Workfront non consente di salvare le seguenti regole di filtro utilizzando l’interfaccia in modalità standard perché fa riferimento allo stesso campo (Nome attività) ma utilizza modificatori diversi e fa riferimento a valori diversi:

* Nome attività > Contiene > Verde
* Nome attività > Non contiene > Rosso

Tuttavia, puoi creare questo filtro utilizzando la modalità testo.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare più regole di filtro che fanno riferimento allo stesso campo

1. Passare a un elenco di attività.
1. Da **Filtro** menu a discesa, seleziona **Nuovo filtro**.
1. Fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Nell’area Imposta regole filtro per il rapporto, aggiungi il seguente codice:

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >Per creare filtri simili, crea prima la prima istruzione . Ad esempio:
   >
   >
   ```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >Copia e incolla l’istruzione il numero di volte necessario. Puoi quindi aggiungere tutte le istruzioni necessarie per fare riferimento allo stesso campo (nel nostro caso &quot;nome&quot;) e apportare le seguenti modifiche alle istruzioni aggiuntive:
   >
   >1. Precede le due righe copiate con &quot;AND&quot; (E):1:&quot;, &quot;AND:2:&quot;, &quot;AND:3:&quot;, ecc. per ogni nuovo valore possibile del campo.
   >1. Sostituisci la riga del campo con il nuovo valore del campo (dopo il segno &quot;=&quot;).
   >1. Sostituire la linea del modificatore (_Mod) con il nuovo modificatore.

   >   
   >Queste istruzioni sono sensibili all’uso di maiuscole e minuscole.

1. Fai clic su **Fine**, quindi **Salva filtro**.
