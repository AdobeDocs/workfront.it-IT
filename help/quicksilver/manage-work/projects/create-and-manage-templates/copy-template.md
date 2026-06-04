---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copiare un modello di progetto
description: Oltre a creare un modello di progetto da zero, puoi anche copiarne uno esistente e modificarlo.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/6d0OXEaAdH-569LF5nuQ8wcJd-Iq7KYz8os3IOyx0yA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 327
ht-degree: 12%

---

# Copiare un modello di progetto

<!--Audited: 5/2025-->

Oltre a creare un modello di progetto da zero, puoi anche copiarne uno esistente e modificarlo in Adobe Workfront.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

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
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td><p>Standard</p> 
   <p>Piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso ai modelli</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Visualizza o autorizzazioni superiori per un modello</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

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
</table>
-->

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
1. Fai clic sul menu **Altro** ![Icona Altro](assets/more-icon.png) a destra del nome del modello nell&#39;intestazione, quindi fai clic su **Copia**.

   Viene visualizzata la casella **Copia modello**.

   ![Copia casella modello](assets/copy-template-box.png)

1. Specificare un nome per il modello nel campo **Nuovo nome modello**.

   Per impostazione predefinita, Workfront imposta il nuovo nome in questo formato: `Copy of Original template name`.

1. Selezionare l&#39;opzione **Mantieni assegnazioni utente per attività e modello** se si desidera trasferire tutte le assegnazioni di attività e modelli dal modello originale al nuovo modello. Le assegnazioni delle attività del modello, il proprietario del modello e lo sponsor vengono trasferiti al modello copiato.
1. Fai clic su **Salva** per creare una copia del modello.

   Il nuovo modello viene visualizzato nell&#39;elenco dei modelli nell&#39;area Modello di Workfront.
