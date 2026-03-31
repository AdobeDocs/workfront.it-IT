---
product-area: requests
navigation-topic: create-requests
title: Eliminare una richiesta inviata o una bozza di richiesta
description: È possibile eliminare le richieste inviate o le bozze di richieste in Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 9098ada7-0e6b-4de2-97ad-5c6e590fbba3
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 9%

---

# Eliminare una richiesta inviata o una bozza di richiesta

È possibile eliminare le richieste o le bozze di richieste inviate da Adobe Workfront o Adobe Workfront Planning oppure disporre delle autorizzazioni di gestione per.

Gli amministratori di Workfront e i responsabili dell&#39;area di lavoro di Workfront Planning possono inoltre eliminare le richieste e le bozze di richieste che non hanno creato.

Non è possibile visualizzare le richieste Planning nell’esperienza di richiesta legacy.

Questo articolo descrive come eliminare le bozze di richiesta nella nuova esperienza di richiesta. L&#39;eliminazione delle richieste Workfront e Planning o delle relative bozze è identica.

Per ulteriori informazioni, consulta:

* [Crea e invia richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md)
* [Creare richieste da bozze](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)
* [Inviare richieste di Pianificazione di Adobe Workfront per creare record](/help/quicksilver/planning/requests/submit-requests.md)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi pacchetto Workfront o flusso di lavoro</p>

<p>Qualsiasi pacchetto Workfront Planning per gestire le richieste Planning </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Collaboratore o successiva</p>
   <p>Richiedente o successiva</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Per eliminare le richieste non create, è necessario essere un amministratore di Workfront o un manager dell'area di lavoro di Planning.</p><p>Devi disporre dell'accesso in Modifica ai Problemi.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>È necessario aver creato la richiesta o la bozza per eliminarla nella nuova esperienza di richiesta oppure essere un amministratore di Workfront o un manager dell'area di lavoro di Planning per eliminare le bozze di richieste non inviate.
   </p><p>Devi disporre delle autorizzazioni di modifica per i problemi che stai eliminando.</p>  </td> 
  </tr>

</tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Elimina richieste o bozze di richieste nella nuova esperienza richiedente

È possibile eliminare richieste e bozze nelle aree seguenti:

* Nell’area Richieste di Workfront
* Nel widget Richieste personali nella Home
* Da una pagina di richiesta

I seguenti utenti possono eliminare le bozze di richiesta:

* Gli amministratori di Workfront possono eliminare le richieste e le bozze inviate da loro o da altri utenti.
* I responsabili dell&#39;area di lavoro di Workfront Planning possono eliminare le richieste e le bozze nell&#39;area di lavoro di Planning gestita.
* Gli utenti possono eliminare le richieste e le bozze che hanno inviato.

### Eliminare una richiesta o una bozza dall’area Richieste o dal widget Richieste personali nella Home

{{step1-to-requests}}

1. Per accedere al widget **Richieste personali** in **Home**:

   {{step1-to-home}}

   1. Individua il widget **Richieste personali**.

      Per ulteriori informazioni sul widget **Richieste personali**, vedere [Utilizzare il widget Richieste personali](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. Nell&#39;elenco **Richieste** o nel widget **Richieste personali** in **Home**, passa il puntatore sulla richiesta o sulla bozza da eliminare, quindi fai clic sul menu **Altro** ![Altro](assets/more-menu.png)

1. Fai clic su **Elimina**

   Oppure

   Fare clic con il pulsante destro del mouse sulla richiesta selezionata, quindi scegliere **Elimina**.

   >[!TIP]
   >
   >Se non disponi dell’accesso per la creazione di problemi, ricevi un avviso che informa che l’amministratore non ti ha consentito di creare richieste.

1. Nella finestra di dialogo visualizzata, fai clic su **Elimina**.

   La richiesta o la bozza viene eliminata.

   Le richieste eliminate vengono salvate nel Cestino e un amministratore Workfront può recuperarle per un massimo di 30 giorni. Le bozze non possono essere recuperate.

### Richieste di eliminazione in blocco da un elenco

{{step1-to-requests}}

1. Per accedere al widget **Richieste personali** in **Home**:

   {{step1-to-home}}

   1. Individua il widget **Richieste personali**.

      Per ulteriori informazioni sul widget Richieste personali, vedere [Utilizzare il widget Richieste personali](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. Nell&#39;elenco **Richieste** o nel widget **Richieste personali** fare clic sulla casella a sinistra di ogni richiesta che si desidera eliminare.
1. Nella barra blu nella parte inferiore della pagina, fai clic su **Elimina**.

   >[!NOTE]
   >
   >Se l&#39;opzione **Elimina** non è visibile nella barra blu, non si dispone dell&#39;autorizzazione per eliminare una o più richieste selezionate.

### Prerequisiti per l’eliminazione di bozze di richieste

Prima di eliminare una bozza di richiesta, è necessario effettuare le seguenti operazioni:

* Inizia a creare una richiesta. In questo modo la richiesta viene salvata automaticamente come bozza nella sezione Bozze.

  Per informazioni sulla creazione di richieste, vedere [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Eliminare le bozze di richiesta nell’esperienza di richiesta legacy

È possibile eliminare le richieste bozze dopo averle salvate come bozze se non le si ritiene più rilevanti. Non è possibile recuperare le bozze di richieste eliminate.

Non è possibile accedere alle richieste di Planning o alle relative bozze dall&#39;esperienza di richiesta legacy.

{{step1-to-requests}}

1. Fai clic su **Bozze** nel pannello a sinistra.

   In questo elenco vengono visualizzate tutte le bozze di tutte le code di richieste.

1. Selezionare una bozza nell&#39;elenco, quindi fare clic su **Elimina** nella parte superiore dell&#39;elenco.
1. Fai clic su **Sì, elimina**.

   La bozza viene eliminata e non può essere recuperata.






