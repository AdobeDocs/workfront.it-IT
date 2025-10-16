---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visualizzazione: visualizzare un''immagine anziché una stringa in una colonna'
description: È possibile sostituire il nome di un oggetto in una visualizzazione con un'immagine utilizzando la modalità testo. È inoltre possibile aggiungere all'immagine un collegamento che consenta di aprire l'oggetto che sostituisce.
author: Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Visualizza: visualizza un’immagine invece di una stringa in una colonna

<!--Audited: 11/2024-->

È possibile sostituire il nome di un oggetto in una visualizzazione con un&#39;immagine utilizzando la modalità testo. È inoltre possibile aggiungere all&#39;immagine un collegamento che consenta di aprire l&#39;oggetto che sostituisce.

>[!NOTE]
>
>Le immagini vengono visualizzate nella loro risoluzione effettiva, quindi prova a utilizzare immagini piccole.

![Sostituisci nome progetto con immagine e collegamento](assets/replace-project-name-with-image-and-link-350x125.png)

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

   1. Fai clic con il pulsante destro del mouse e seleziona **Copia percorso immagine** o **Ottieni collegamento**, a seconda del browser in uso. Ora disponi dell’URL per quell’immagine specifica e puoi incollarla dagli Appunti.
   1. Assicurati che tutti coloro che dispongono di quel collegamento siano autorizzati a visualizzare l’immagine semplicemente andando sul collegamento e che non abbiano bisogno di un accesso per accedervi.

1. Vai a un progetto, fai clic sul menu **Altro** ![Icona Altro](assets/more-icon-45x33.png) accanto al nome del progetto, quindi fai clic su **Modifica**.

1. Aggiungi il collegamento all&#39;immagine nel campo **URL**.
1. Consente di passare a una visualizzazione di progetto in un elenco di progetti.
1. Fai clic sul menu a discesa **Visualizza**, quindi fai clic su **Nuova visualizzazione**.
1. Fai clic sull&#39;intestazione della colonna per il **Nome progetto**, quindi fai clic su **Passa a modalità testo**.

1. Aggiungi il seguente codice alla colonna del codice esistente:

   ```
   displayname=Link Project
   image.name=Link Project
   image.valuefield=URL
   link.linkproperty.0.name=projectID
   link.linkproperty.0.value=ID
   link.lookup=link.edit
   link.page=/view
   link.valuefield=objCode
   link.valueformat=val
   textmode=true
   type=image
   valueformat=
   ```

1. Fai clic su **Fine** > **Salva visualizzazione**.
L&#39;immagine selezionata sostituisce il nome del progetto nella vista Progetto e l&#39;immagine è un collegamento al progetto.
