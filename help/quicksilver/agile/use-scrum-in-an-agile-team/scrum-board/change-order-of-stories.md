---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Modificare l’ordine delle storie sulla bacheca Scrum
description: L'ordine in cui le storie vengono visualizzate sulla bacheca delle storie non indica la priorità. Tuttavia, può influenzare la priorità percepita rendendo le storie più visibili. Per impostazione predefinita, i brani vengono visualizzati in ordine alfabetico in ogni colonna [!UICONTROL status] dello storyboard.
author: Courtney
feature: Agile
exl-id: 326d78e0-06de-4b98-8fa6-102e0fd89d76
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/Vy3r2L1yuMPvMesRxEohYAgA6geAlKYIRsstLp1kpt8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
    internal-label: Agile
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 9%
---
# Cambia l&#39;ordine delle storie sulla bacheca [!UICONTROL Scrum]

L&#39;ordine in cui le storie vengono visualizzate sulla bacheca delle storie non indica la priorità. Tuttavia, può influenzare la priorità percepita rendendo le storie più visibili. La priorità è definita nel backlog e quando le storie vengono portate sulla bacheca delle storie non hanno una priorità impostata perché verranno lavorate durante l&#39;intervallo di tempo dell&#39;iterazione. Se le storie vengono restituite al backlog, puoi riordinarle per mostrare la priorità.

Per impostazione predefinita, i brani vengono visualizzati in ordine alfabetico all&#39;interno di ogni colonna di stato sullo storyboard. Le storie con corsie sono mostrate nella parte superiore della bacheca delle storie e le storie senza corsie sono mostrate separatamente sotto qualsiasi corsia.

Quando riordinate le colonne sullo storyboard, tutte le modifiche apportate vengono salvate nell&#39;iterazione o nel progetto, pertanto le modifiche vengono mantenute alla successiva visualizzazione dello storyboard da parte di un altro utente. Le modifiche apportate non vengono ripristinate quando si cancella la cache del browser.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

Per eseguire i passaggi descritti in questo articolo, devi disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> <p>Nuovo: [!UICONTROL Standard]</p> 
   oppure
   <p>Corrente: [!UICONTROL Work] o versione successiva</p> </td> 
  </tr>
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modificare l’ordine delle storie in un’iterazione

{{step1-to-team}}

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.

1. Passare all&#39;iterazione o al progetto contenente le storie che si desidera riordinare.
1. Trascinare una storycard o una corsia nella posizione verticale desiderata all&#39;interno di una colonna di stato sulla bacheca delle storie.

## Modificare l&#39;ordine delle storie in un progetto

A differenza delle iterazioni Agile, non è possibile modificare l’ordine delle storie quando si visualizza un progetto in una visualizzazione Agile. Per modificare l&#39;ordine delle storie di un progetto, è necessario visualizzare il progetto in una visualizzazione standard.

Per informazioni su come modificare la visualizzazione del progetto, vedere [[!UICONTROL Gestione di un progetto] nella visualizzazione [!UICONTROL Agile]](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md). Invece di selezionare una vista Agile, selezionate una vista standard.
