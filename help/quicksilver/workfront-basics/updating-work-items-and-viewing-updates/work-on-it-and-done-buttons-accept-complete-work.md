---
content-type: o
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Panoramica del pulsante Lavoraci e Fine
description: Quando ti viene assegnata un’attività o un problema, puoi utilizzare un pulsante contestuale che cambia nome e funzione in base al tuo coinvolgimento con l’elemento di lavoro.
author: Lisa and Alina
feature: Get Started with Workfront
role: User
exl-id: cfda6702-1a9a-4645-b031-8b2f201ac0af
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 1%

---

# Panoramica del pulsante Lavoraci e Fine

Quando ti viene assegnata un’attività o un problema, puoi utilizzare un pulsante contestuale che cambia nome e funzione in base al tuo coinvolgimento con l’elemento di lavoro.

Utilizzando il pulsante contestuale per accettare o completare gli elementi di lavoro, puoi consentire ad Adobe Workfront di aggiornare diversi campi sugli elementi senza doverli aggiornare manualmente.

I pulsanti Lavoraci e Fine sono visibili agli utenti che dispongono di:

* Una licenza Standard (nuova) o una licenza Pianificazione o Lavoro (corrente)
* Accesso limitato o superiore alle modifiche per l’attività o il problema

>[!NOTE]
>
>Il pulsante Done (Fine) viene visualizzato come Mark as done (Contrassegna come completato) in tutte le aree di Workfront.

## Lavoraci e nomi dei pulsanti Fine

A seconda dell’area di Workfront da cui accedi all’attività o al problema, il pulsante Lavoraci o Fine può modificare i nomi, come descritto nei seguenti scenari:

* Quando l’attività o il problema viene assegnato per la prima volta e lo stato è Nuovo, il pulsante viene visualizzato come Lavoraci.

  ![](assets/nwe-work-on-it-button.png)

  >[!TIP]
  >
  >È possibile sostituire il pulsante Lavoraci con un pulsante Avvia. Per informazioni sulla sostituzione del pulsante Lavoraci con un pulsante Start, vedere [Sostituire il pulsante Lavoraci con un pulsante Start](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md) .

* Dopo aver fatto clic su Accetta lavoro, il pulsante diventa Contrassegna come completato. Per informazioni su dove è possibile accedere al pulsante Lavoraci, vedere la sezione [Individuare il pulsante Lavoraci e completati](#locate-the-work-on-it-and-done-button) in questo articolo.

  ![](assets/nwe-mark-as-done-button-350x122.png)


<!--If you are not the only one assigned to the task or issue and you are accessing your work item from the My Work widget in the Home area, the button changes to Done with my part.

  ![](assets/home-left-done-with-my-part-button-350x184.png)-->

## Individuare il pulsante Lavoraci e Fine {#locate-the-work-on-it-and-done-button}

Puoi individuare il pulsante Lavoraci e Fine nelle seguenti aree di Workfront:

* Area Home nel widget Il mio lavoro

  Per informazioni su come contrassegnare un elemento come completato nell&#39;area Home, vedere [Contrassegnare un elemento come completato nell&#39;area Home](../../workfront-basics/using-home/using-the-home-area/mark-item-done-in-home.md).

* Nell’intestazione dell’attività o del problema

  Per informazioni sulle intestazioni degli oggetti, vedere [Nuove intestazioni degli oggetti](../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

* Nel pannello Riepilogo dell’attività o del problema

  Per informazioni sull&#39;utilizzo del pannello Riepilogo, vedere [Panoramica di riepilogo](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

## Panoramica dei campi che vengono aggiornati automaticamente quando si fa clic sui pulsanti Lavoraci o Fine

I pulsanti Lavoraci e Fine consentono a Workfront di aggiornare automaticamente le informazioni sull&#39;elemento di lavoro assegnato.

* [Pulsante Lavoraci](#work-on-it-button)
* [Pulsante Start](#start-button)
* [Pulsante Fine](#the-done-button)

### Pulsante Lavoraci {#work-on-it-button}

Quando fai clic su Lavoraci, vengono aggiornati anche i seguenti elementi:

* Aggiornamenti dello stato di assegnazione da Richiesto a In esecuzione

  >[!TIP]
  >
  >Il campo Stato assegnazione è visibile solo nei report e negli elenchi. Per informazioni sul campo Stato assegnazione, vedere il [Glossario della terminologia di Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Conferma data

  Per informazioni sulla data del commit, vedere [Panoramica sulla data del commit](../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

### Pulsante Start {#start-button}

Se si dispone dell&#39;accesso per modificare i team, è possibile sostituire il pulsante Lavoraci con un pulsante Avvia per un team. Quando gli utenti con quel team come team predefinito fanno clic sul pulsante Start sugli elementi a cui sono assegnati, i campi aggiuntivi sugli elementi di lavoro si aggiornano automaticamente. Per informazioni sulla sostituzione del pulsante Lavoraci con un pulsante Start, vedere [Sostituire il pulsante Lavoraci con un pulsante Start](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

Oltre ai campi che vengono aggiornati quando si fa clic sul pulsante Lavoraci, quando si fa clic sul pulsante Start i campi seguenti vengono aggiornati automaticamente per un&#39;attività o un problema:

* Stato
* Data di inizio effettiva

  Per informazioni sulla data di inizio effettiva, vedere [Panoramica sulla data di inizio effettiva del progetto](../../manage-work/projects/planning-a-project/project-actual-start-date.md).

* Data di completamento effettiva se il pulsante Inizio è associato a uno stato che equivale a Completo o Chiuso.

  Per informazioni sulla data di completamento effettiva, vedere [Panoramica della data di completamento effettiva del progetto](../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

>[!NOTE]
>
>Facendo clic sul pulsante Annulla, l&#39;elemento di lavoro torna allo stato originale ed elimina la data di inizio effettiva.
>
>Il pulsante Annulla non è disponibile nelle seguenti aree:
>
>* Richieste team
>* Intestazione attività
>

### Pulsante Fine {#the-done-button}

Se si dispone dell&#39;accesso per modificare i team, è possibile configurare il pulsante Fine per un team in modo da aggiornare gli stati di attività o problemi quando si contrassegna un elemento come completato. Quando gli utenti con quel team come team predefinito fanno clic sul pulsante Contrassegna come completato sui loro elementi, i seguenti campi si aggiornano automaticamente su un’attività o un problema:

* Stato
* Stato assegnazione aggiornato da In corso a Fine
* Data di completamento effettiva

Per informazioni sulla configurazione del pulsante Fine per un team, vedere gli articoli seguenti:

* [Configura il pulsante Fine per le attività](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)
* [Configura il pulsante Fine per i problemi](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)
