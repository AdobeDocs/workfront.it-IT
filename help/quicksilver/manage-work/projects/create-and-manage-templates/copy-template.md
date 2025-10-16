---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copiare un modello di progetto
description: Oltre a creare un modello di progetto da zero, puoi anche copiarne uno esistente e modificarlo.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '327'
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
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Standard</p> 
   <p>Piano</p> </td> 
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

<!--Old:

 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a template</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

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

   ![Copia casella modello](assets/copy-template-box.png)

1. Specificare un nome per il modello nel campo **Nuovo nome modello**.

   Per impostazione predefinita, Workfront imposta il nuovo nome in questo formato: `Copy of Original template name`.

1. Selezionare l&#39;opzione **Mantieni assegnazioni utente per attività e modello** se si desidera trasferire tutte le assegnazioni di attività e modelli dal modello originale al nuovo modello. Le assegnazioni delle attività del modello, il proprietario del modello e lo sponsor vengono trasferiti al modello copiato.
1. Fai clic su **Salva** per creare una copia del modello.

   Il nuovo modello viene visualizzato nell&#39;elenco dei modelli nell&#39;area Modello di Workfront.
