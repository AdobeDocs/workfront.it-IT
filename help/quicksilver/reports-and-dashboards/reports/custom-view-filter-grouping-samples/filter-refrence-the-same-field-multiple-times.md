---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Filtro: crea più regole di filtro che fanno riferimento allo stesso campo (istruzioni "AND")"'
description: Nell’interfaccia in modalità standard, quando tenti di creare più filtri che fanno riferimento allo stesso campo (utilizzando il qualificatore AND), uno dei filtri viene eliminato quando salvi il rapporto e chiudi il generatore di rapporti.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Filtro: crea più regole di filtro che fanno riferimento allo stesso campo (istruzioni &quot;AND&quot;)

Nell’interfaccia in modalità standard, quando tenti di creare più filtri che fanno riferimento allo stesso campo (utilizzando il qualificatore AND), uno dei filtri viene eliminato quando salvi il rapporto e chiudi il generatore di rapporti.

**Esempio:** È possibile visualizzare solo le attività che contengono la parola &quot;verde&quot; ma non la parola &quot;rosso&quot; nel nome. Adobe Workfront non consente di salvare le seguenti regole di filtro utilizzando l’interfaccia in modalità standard: fa riferimento allo stesso campo (Nome attività), ma utilizza modificatori diversi e fa riferimento a valori diversi:

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
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta di modifica di un filtro </p>
   <p>Pianificare la modifica di un rapporto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Creare più regole di filtro che fanno riferimento allo stesso campo

1. Consente di passare a un elenco di attività.
1. Dalla sezione **Filtro** menu a discesa, seleziona **Nuovo filtro**.
1. Clic **Passa alla modalità testo**.
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
   >Per creare filtri simili, genera prima la prima istruzione. Ad esempio:
   >
   >
   ```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >Copia e incolla l’istruzione il numero di volte necessario. Puoi quindi aggiungere tutte le istruzioni necessarie per fare riferimento allo stesso campo (nel nostro caso &quot;name&quot;) e apportare le seguenti modifiche alle istruzioni aggiuntive:
   >
   >1. Anteponete &quot;AND&quot; alle due linee copiate:1:&quot;, &quot;E:2:&quot;, &quot;E:3:&quot;, ecc. per ogni nuovo valore possibile del campo.
   >1. Sostituisci la riga del campo con il nuovo valore del campo (dopo il segno &quot;=&quot;).
   >1. Sostituire la linea del modificatore (_Mod) con il nuovo modificatore.

   >   
   >Queste istruzioni distinguono tra maiuscole e minuscole.

1. Clic **Fine**, quindi **Salva filtro**.
