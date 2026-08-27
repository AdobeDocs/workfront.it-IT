---
title: Configura regole business di tipo record
description: È possibile configurare regole business di tipo record che definiscono il modo in cui i record di quel tipo vengono gestiti in Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 914f1f8a25aa5b9e1045d2f940ed15061301c21b
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 5%

---


# Configurare le regole business di tipo record

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

È possibile configurare regole business di tipo record che definiscono il modo in cui i record di quel tipo vengono gestiti in Adobe Workfront Planning.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per eseguire i passaggi descritti in questo articolo:  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Qualsiasi Workfront o flusso di lavoro con un pacchetto Planning</p></li>
Oppure
<li><p>Qualsiasi pacchetto Planning acquistato come prodotto standalone</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Standard flusso di lavoro</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licenza Adobe Planning</p></td> 
   <td><p>Standard di pianificazione</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>È necessario aggiungere sia un flusso di lavoro che un tipo di licenza Planning al livello di accesso quando si dispone sia di un flusso di lavoro che di un pacchetto Planning</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>   <p>Gestire le autorizzazioni per un’area di lavoro e per un tipo di record</p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni durante la configurazione delle regole aziendali

* È possibile configurare le regole per la modifica o l&#39;eliminazione dei record, a seconda delle condizioni definite.

  Ad esempio, puoi creare le condizioni per richiedere che alcuni campi abbiano un valore. Se il valore non è presente in tali campi, gli utenti non possono modificare o eliminare tale record.
* Non è possibile aggiungere regole business ai tipi di record globali nelle aree di lavoro principali o secondarie.
* Non è possibile configurare regole per la creazione dei record. Tutti coloro che dispongono delle autorizzazioni Gestione per il tipo di record possono creare record.
* È possibile creare una condizione per la regola business che faccia riferimento a tutti i tipi di campo ad eccezione dei seguenti:
  * Campi formula
  * Campi di ricerca
  * Campi di riferimento

## Configurare le regole business

1. Passare a un tipo di record.
1. Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record, quindi fai clic su Regole aziendali.



