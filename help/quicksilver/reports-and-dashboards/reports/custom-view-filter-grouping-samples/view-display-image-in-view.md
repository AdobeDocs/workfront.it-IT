---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizzazione: visualizza un’immagine invece di una stringa in una colonna"
description: È possibile sostituire il nome di un oggetto in una visualizzazione con un'immagine utilizzando la modalità testo. È inoltre possibile aggiungere all'immagine un collegamento che consenta di aprire l'oggetto che sostituisce.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# Visualizza: visualizza un’immagine invece di una stringa in una colonna

È possibile sostituire il nome di un oggetto in una visualizzazione con un&#39;immagine utilizzando la modalità testo. È inoltre possibile aggiungere all&#39;immagine un collegamento che consenta di aprire l&#39;oggetto che sostituisce.

>[!NOTE]
>
>Le immagini vengono visualizzate nella loro risoluzione effettiva, quindi prova a utilizzare immagini piccole.

![](assets/replace-project-name-with-image-and-link-350x125.png)

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
   <td> <p>Richiesta di modifica di una vista </p>
   <p>Pianificare la modifica di un rapporto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Esempio: sostituisci il nome di un progetto in una vista progetto con un’immagine:

1. Carica un’immagine su un sito web o un server esterno a Adobe Workfront. Devi essere in grado di accedere all’immagine utilizzando il browser web.

   >[!TIP]
   >
   >* Ogni tipo di browser è diverso, ma tutti possono visualizzare gli URL.
   >* Evita l&#39;uso di immagini caricate su Workfront. Poiché le immagini memorizzate in Workfront non sono disponibili al pubblico e dispongono di una chiave di accesso che scade dopo un certo periodo di tempo, con il passare del tempo questa visualizzazione non viene più visualizzata.
   >* Un&#39;immagine salvata nel computer non ha un URL intrinseco. Trova un sito che fornisca hosting di immagini e ospiti la tua immagine lì. È possibile che l&#39;organizzazione disponga già di un sito di questo tipo.


1. Utilizzando il browser Web, accedi all’immagine salvata.
1. Per ottenere l’URL dell’immagine, effettua le seguenti operazioni:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. Fai clic con il pulsante destro del mouse e seleziona (Copia negli Appunti) **Copia posizione immagine**, o **Ottieni collegamento**, a seconda del browser. Ora disponi dell’URL per quell’immagine specifica e puoi incollarla dagli Appunti.
   1. Assicurati che tutti coloro che dispongono di quel collegamento siano autorizzati a visualizzare l’immagine semplicemente andando sul collegamento e che non abbiano bisogno di un accesso per accedervi.

1. Vai a un progetto, fai clic su **Altro** menu ![](assets/more-icon-45x33.png) accanto al nome del progetto, quindi fai clic su **Modifica**.

1. In **URL** , aggiungi il collegamento all&#39;immagine.
1. Passare a una visualizzazione di progetto in un elenco o in un report e personalizzare la visualizzazione.
1. Fai clic sull’intestazione della colonna per il **Nome progetto**, quindi fai clic su **Passa alla modalità testo**.

1. Aggiungi il seguente codice alla colonna del codice esistente:

   ```
   displayname=Link Project
   ```

   ```
   image.name=Link Project
   ```

   ```
   image.valuefield=URL
   ```

   ```
   link.linkproperty.0.name=projectID
   ```

   ```
   link.linkproperty.0.value=ID
   ```

   ```
   link.lookup=link.edit
   ```

   ```
   link.page=/view
   ```

   ```
   link.valuefield=objCode
   ```

   ```
   link.valueformat=val
   ```

   ```
   textmode=true
   ```

   ```
   type=image
   ```

   ```
   valueformat=
   ```

   L&#39;immagine selezionata sostituisce il nome del progetto nella vista Progetto e l&#39;immagine è un collegamento al progetto.

1. Clic **Salva visualizzazione**.
