---
content-type: o
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Panoramica dei pulsanti "Work On It and Done"
description: Quando si è assegnati a un'attività o a un problema, è possibile utilizzare un pulsante contestuale che cambia nomi e funzioni a seconda del coinvolgimento con l'elemento di lavoro.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: cfda6702-1a9a-4645-b031-8b2f201ac0af
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 0%

---

# Panoramica dei pulsanti &quot;Work On It and Done&quot;

Quando si è assegnati a un&#39;attività o a un problema, è possibile utilizzare un pulsante contestuale che cambia nomi e funzioni a seconda del coinvolgimento con l&#39;elemento di lavoro.

Utilizzando il pulsante contestuale per accettare o completare elementi di lavoro, è possibile consentire ad Adobe Workfront di aggiornare diversi campi sugli elementi senza doverli aggiornare manualmente.

## Utilizzare i nomi dei pulsanti Fine

A seconda dell’area di Workfront da cui si accede all’attività o al problema, il pulsante Work On It o Done può modificare i nomi, come descritto nei seguenti scenari: 

* Quando l&#39;attività o il problema viene assegnato per la prima volta e lo stato è Nuovo, il pulsante viene visualizzato come Lavoro.

   ![](assets/nwe-work-on-it-button.png)

   >[!TIP]
   >
   >È possibile sostituire il pulsante Lavora su di esso con un pulsante Start. Per informazioni sulla sostituzione del pulsante Work On It con un pulsante Start, vedere  [Sostituire il pulsante Work On It con un pulsante Start](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md) .

* Dopo aver fatto clic su Lavora su accetta, il pulsante diventa Contrassegna come completato o Fine , a seconda di dove in Workfront accedi all’attività o al problema da cui. Per informazioni su dove è possibile accedere al pulsante Lavora su di esso, vedere la sezione [Individua il pulsante Lavora su di esso e Fine](#locate-the-work-on-it-and-done-button) in questo articolo.

   ![](assets/nwe-mark-as-done-button-350x122.png)

* Se non sei l&#39;unico assegnato all&#39;attività o al problema e accedi all&#39;elemento di lavoro dall&#39;Elenco lavori nell&#39;area Home, il pulsante diventa Fine con la mia parte.

   ![](assets/home-left-done-with-my-part-button-350x184.png)

## Individua il pulsante Lavora su di esso e Fine {#locate-the-work-on-it-and-done-button}

È possibile individuare il pulsante Lavoro su di esso e Fine nelle seguenti aree di Workfront:

* Area Home, sia nell’Elenco lavori che nel pannello dei dettagli

   Per informazioni sulla marcatura di un elemento come Fatto nell&#39;area Home, vedere [Contrassegna un elemento come Fatto nell&#39;area Home](../../workfront-basics/using-home/using-the-home-area/mark-item-done-in-home.md).

* Nell’intestazione dell’attività o del problema

   Per informazioni sulle intestazioni dell&#39;oggetto, vedere [Nuove intestazioni oggetto](../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

* Nel pannello Attività o Riepilogo del problema in un elenco o nel servizio di bilanciamento del carico di lavoro

   Per informazioni sull’utilizzo del pannello Riepilogo, consulta [Panoramica di riepilogo](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

## Panoramica dei campi che si aggiornano automaticamente quando si fa clic sul pulsante Lavora su e Fine

L’utilizzo dei pulsanti Lavora su e Fine consente a Workfront di aggiornare automaticamente le informazioni sull’elemento di lavoro assegnato.

* [Pulsante Su](#work-on-it-button)
* [Pulsante Start](#start-button)
* [Pulsante Fine](#the-done-button)

### Pulsante Su {#work-on-it-button}

Quando fai clic su Lavora su di esso, vengono aggiornati anche i seguenti elementi:

* Aggiornamenti dello stato di assegnazione da Richiesto a Lavoro

   >[!TIP]
   >
   >Il campo Stato assegnazione è visibile solo nei rapporti e negli elenchi. Per informazioni sul campo Stato assegnazione, vedere la [Glossario della terminologia di Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Data del commit

   Per informazioni sulla data di commit, vedi [Panoramica sulla data del commit](../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

### Pulsante Start {#start-button}

Se hai accesso per modificare i team, puoi sostituire il pulsante Lavora su di esso con un pulsante Start per un team. Quando gli utenti con quel team come team principale fanno clic sul pulsante Start sugli elementi a cui sono assegnati, i campi aggiuntivi sugli elementi di lavoro vengono aggiornati automaticamente. Per informazioni sulla sostituzione del pulsante Work On It con un pulsante Start, vedere [Sostituire il pulsante Work On It con un pulsante Start](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

Oltre ai campi che vengono aggiornati quando si fa clic sul pulsante Attivato, i campi seguenti vengono aggiornati automaticamente su un&#39;attività o su un problema quando si fa clic sul pulsante Avvia:

* Stato
* Data di inizio effettiva

   Per informazioni sulla data di inizio effettiva, vedi [Panoramica della data di inizio effettiva del progetto](../../manage-work/projects/planning-a-project/project-actual-start-date.md).

* Data completamento effettiva se il pulsante Start è associato a uno stato che corrisponde a Completo o Chiuso.

   Per informazioni sulla data di completamento effettiva, vedere [Panoramica della data di completamento effettivo del progetto](../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

>[!NOTE]
>
>Facendo clic sul pulsante Annulla, l&#39;elemento di lavoro viene ripristinato allo stato originale ed è eliminata la data di inizio effettiva.
>
>Il pulsante Annulla non è disponibile nelle seguenti aree:
>
>* Richieste del team
>* Intestazione attività
>


### Pulsante Fine {#the-done-button}

Se si dispone dell&#39;accesso per modificare i team, è possibile configurare il pulsante Fine per un team per aggiornare l&#39;attività o gli stati di problema quando si contrassegna un elemento come completato. Quando gli utenti con quel team come team principale fanno clic sul pulsante Fine sui loro elementi, i campi seguenti vengono aggiornati automaticamente su un&#39;attività o un problema:

* Stato
* Aggiornamenti dello stato dell&#39;assegnazione da Lavoro a Fine
* Data completamento effettivo

Per informazioni sulla configurazione del pulsante Fine per un team, vedere i seguenti articoli:

* [Configura il pulsante Fine per le attività](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)
* [Configura il pulsante Fine per i problemi](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)
