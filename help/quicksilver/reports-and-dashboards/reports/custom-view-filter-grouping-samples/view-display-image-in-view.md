---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: visualizza un''immagine invece di una stringa in una colonna"'
description: È possibile sostituire il nome di un oggetto in una visualizzazione con un'immagine utilizzando la modalità testo. È inoltre possibile aggiungere all’immagine un collegamento che consenta di aprire l’oggetto che sostituisce.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Visualizza: visualizzare un&#39;immagine invece di una stringa in una colonna

È possibile sostituire il nome di un oggetto in una visualizzazione con un&#39;immagine utilizzando la modalità testo. È inoltre possibile aggiungere all’immagine un collegamento che consenta di aprire l’oggetto che sostituisce.

>[!NOTE]
>
>Le immagini appaiono nella loro risoluzione effettiva, quindi cerca di usare immagini di piccole dimensioni.

![](assets/replace-project-name-with-image-and-link-350x125.png)

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

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Esempio: Sostituisci il nome di un progetto in una visualizzazione del progetto con un’immagine:

1. Carica un’immagine in un sito web o in un server esterno ad Adobe Workfront. Devi essere in grado di accedere all’immagine utilizzando il browser web.

   >[!TIP]
   >
   >* Ogni tipo di browser è diverso, ma tutti sono in grado di visualizzare gli URL.
   >* Evita di utilizzare immagini caricate in Workfront. Poiché le immagini archiviate in Workfront non sono disponibili al pubblico e dispongono di una chiave di accesso che scade dopo un periodo di tempo, queste immagini smettono di essere visualizzate nella visualizzazione nel tempo.
   >* Un&#39;immagine salvata sul computer non dispone di un URL intrinseco. Trova un sito che offre l&#39;hosting delle immagini e ospita la tua immagine. Un sito di questo tipo potrebbe essere già presente nell’organizzazione.


1. Utilizzando il browser Web, passa all’immagine salvata.
1. Per ottenere l’URL dell’immagine, procedi come segue:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. Fai clic con il pulsante destro del mouse e seleziona **Copia posizione immagine** oppure **Ottieni collegamento**, a seconda del browser. Ora disponi dell’URL per quell’immagine specifica e puoi incollarla dagli Appunti.
   1. Assicurati che tutti coloro che hanno quel collegamento abbiano le autorizzazioni per visualizzare l&#39;immagine semplicemente andando al collegamento e che non abbiano bisogno di un accesso per accedervi.

1. Passa a un progetto e fai clic sul pulsante **Altro** menu ![](assets/more-icon-45x33.png) accanto al nome del progetto, fai clic su **Modifica**.

1. In **URL** aggiungi il collegamento all’immagine.
1. Passa a una visualizzazione del progetto in un elenco o in un rapporto e personalizzala.
1. Fai clic sull’intestazione della colonna per **Nome progetto**, quindi fai clic su **Passa alla modalità testo**.

1. Aggiungi il codice seguente alla colonna al codice esistente:

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

   L’immagine selezionata sostituisce il Nome progetto nella visualizzazione del progetto e l’immagine è un collegamento al progetto.

1. Fai clic su **Salva visualizzazione**.
