---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copiare un modello di progetto
description: Invece di creare un nuovo modello di progetto da zero, puoi copiare un modello esistente e apportarvi modifiche, se necessario.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 3%

---

# Copiare un modello di progetto

Invece di creare un nuovo modello di progetto da zero, puoi copiare un modello esistente e apportarvi modifiche, se necessario.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso ai modelli</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per un modello</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.


## Considerazioni sulla copia dei modelli

I seguenti elementi vengono sempre copiati da un progetto esistente a uno nuovo:

* Attività modello
* Informazioni predefinite attività modello (processo di approvazione predefinito attività, Forms personalizzato predefinito attività)
* Moduli personalizzati
* Rischi
* Informazioni impostazione coda
* Portfolio e programma
* Approvazioni
* Documenti
* I giorni delle attività modello originale vengono trasferiti al nuovo modello. Se necessario, è necessario modificare il giorno di inizio o di completamento del modello (a seconda della modalità di pianificazione) per aggiornare i giorni delle attività del modello.

I seguenti elementi non vengono mai copiati da un progetto esistente a uno nuovo:

* Tariffe di fatturazione
* Commenti utente

## Copiare un modello

1. Vai al modello da copiare.
1. Fai clic sul menu **Altro** ![](assets/qs-more-icon-on-an-object.png), quindi fai clic su **Copia**.
1. Specificare un nome per il modello nel campo **Nuovo nome modello**.

   Per impostazione predefinita, il nuovo nome è **Copia di `<original template name>`.**

1. Seleziona se desideri **Mantenere le assegnazioni utente per attività e modello**: seleziona questa opzione per trasferire tutte le assegnazioni di attività e modello dal modello originale al nuovo modello.
1. Fai clic su **Salva** per creare una copia del modello.
