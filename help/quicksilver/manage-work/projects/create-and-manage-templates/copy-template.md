---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copiare un modello di progetto
description: Oltre a creare un modello di progetto da zero, puoi anche copiarne uno esistente e modificarlo.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 3%

---

# Copiare un modello di progetto

<!--Audited: 5/2025-->

Oltre a creare un modello di progetto da zero, puoi anche copiarne uno esistente e modificarlo in Adobe Workfront.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

È necessario disporre dei seguenti diritti di accesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td><p>Nuovo: Standard</p> 
   <p>Corrente:Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso ai modelli</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per un modello</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sulla copia dei modelli

I seguenti elementi vengono sempre copiati da un modello esistente a uno nuovo:

* Attività modello
* Informazioni predefinite attività modello (processo di approvazione predefinito attività, Forms personalizzato predefinito attività)
* Moduli personalizzati
* Rischi
* Informazioni impostazione coda
* Portfolio e programma
* Approvazioni
* Documenti
* I giorni delle attività modello originale vengono trasferiti al nuovo modello. Se necessario, è necessario modificare il giorno di inizio o di completamento del modello (a seconda della modalità di pianificazione) per aggiornare i giorni delle attività del modello.

I seguenti elementi non vengono mai copiati da un modello esistente a uno nuovo:

* Tariffe di fatturazione
* Commenti utente

## Copiare un modello


<!--ensure steps and casing on the fields and buttons is accurate with unshim-->

1. Vai al modello da copiare.
1. Fai clic sul menu **Altro** ![Icona Altro](assets/qs-more-icon-on-an-object.png) a destra del nome del modello nell&#39;intestazione, quindi fai clic su **Copia**.

   Viene visualizzata la casella **Copia modello**.
1. Specificare un nome per il modello nel campo **Nuovo nome modello**.

   Per impostazione predefinita, il nuovo nome è `Copy of Original template name`.

1. Seleziona se desideri **Mantenere le assegnazioni utente per attività e modello**: seleziona questa opzione per trasferire tutte le assegnazioni di attività e modello dal modello originale al nuovo modello.
1. Fai clic su **Salva** per creare una copia del modello.
