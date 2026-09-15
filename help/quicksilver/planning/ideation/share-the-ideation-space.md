---
title: Condividere uno spazio delle idee con altri
description: Adobe Workfront Planning ora offre una funzionalità aggiuntiva da ideare prima di avviare le campagne. Sfrutta la potenza dell’intelligenza artificiale per creare e collaborare alle idee con altri prima che diventino record di pianificazione.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: ff8ec4e7f5f9ffefcfc6eeea7e37443bcd1f55d2
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 2%
---

# Condividere uno spazio delle idee con altri

<!--add to TOC and miniTOC-->

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambito del programma **Ideation Space Beta**. </span>

<span class="preview">Per ulteriori informazioni, vedere [Introduzione allo spazio ideazione per Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

<!--
Some of this information is also duplicated in the section for Ideation space permissions in the Access needed to use Ideation space article
-->

Le autorizzazioni per i record di Workfront Planning vengono trasferite nello spazio di ideazione di un record.

Inoltre, puoi assegnare ad altri utenti le autorizzazioni per utilizzare lo spazio delle idee e aggiungervi idee.

Considera i seguenti aspetti:

* I creatori di idee hanno sempre i permessi editor per le proprie idee.

* È necessario disporre delle autorizzazioni di editor per uno spazio di ideazione per creare resoconti brevi ed esportarli in altre applicazioni.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

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
   </td> 
    <!--
    <tr> 
    <td role="rowheader"><p>Additional products</p></td> 
    <td><ul>
    <li><p>Adobe GenStudio for Performance Marketing</p></li>
    <li><p>Adobe Customer Journey Analytics</p></li>
    </ul>
    </td> 
    </tr> 
    -->
  <tr> 
   <td role="rowheader"><p>Licenza flusso di lavoro Adobe</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licenza Adobe Planning</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> 
   <ul>
   <li><p>È necessario aggiungere sia un flusso di lavoro che un tipo di licenza Planning al livello di accesso quando si dispone sia di un flusso di lavoro che di un pacchetto Planning</p>   </li>
   <li><p>L’impostazione Disattiva spazio ideazione nel livello di accesso deve essere deselezionata</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td> <p>Autorizzazioni Contribute o superiori per l'area di lavoro e il tipo di record in cui si desidera aggiungere record </p>
      <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
      <p>Visualizzare le autorizzazioni per gli oggetti Workfront per aggiungerli alle descrizioni <!--not sure if this is available--></p>
      <p>Autorizzazioni dell’editor per lo spazio ideazione per creare resoconti</p>
   </td> 
  </tr>  
  <!--
    <tr> 
    <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
    <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
    <li>GenStudio System Manager to access Activations and Events</li></ul>
    For information, see <a href="https://experienceleague.adobe.com/it/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
    </p>
    </td> 
    </tr> 
    -->
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

## Condivisione di uno spazio delle idee

1. Accedere allo spazio Ideazione di un record Planning.

   Per informazioni, vedere uno degli articoli seguenti:

   * [Crea record di Planning dalle descrizioni dello spazio ideazione](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)
   * [Creare slip nello spazio ideazione](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md)

1. Fai clic su **Condividi** nell&#39;angolo superiore destro, quindi sull&#39;icona **Impostazioni** ![Impostazioni](assets/setting-icon.png) nell&#39;angolo superiore destro della casella **Condividi documento**.
1. Nell&#39;elenco Chi dispone dell&#39;accesso, scegliere una delle opzioni seguenti:

   * **Accesso consentito solo agli invitati**

     Devi aggiungere singoli utenti allo spazio Ideazione e assegnare loro un livello di autorizzazione.
   * **Tutti gli utenti di &lt; ambiente Workfront della tua azienda > possono aggiungere commenti**

     Tutti gli utenti dell&#39;organizzazione che dispongono di un flusso di lavoro e di una licenza Planning nel proprio livello di accesso possono trovare e commentare l&#39;idea.
   * **Chiunque abbia il collegamento può commentare**

     Chiunque condivida un collegamento all’idea può commentare l’idea, incluse le persone esterne alla tua organizzazione.

1. Fai clic su **Copia collegamento** per generare un collegamento all&#39;ideazione e condividerlo con altri utenti. Il collegamento viene aggiunto agli Appunti.
1. Fare clic sulla freccia indietro nella casella Impostazioni per tornare alla condivisione.
1. (Condizionale) Se hai selezionato di condividere lo spazio delle idee con persone specifiche, inizia a digitare il loro nome o indirizzo e-mail, quindi seleziona uno dei seguenti livelli di autorizzazione:

   | Autorizzazione per spazio ideazione | Funzionalità |
   |---|---|
   | **Editor** | Può modificare, scaricare e condividere lo spazio delle idee |
   | **Commento** | Può visualizzare e commentare lo spazio delle ideazioni |
   | **Visualizzatore** | Può visualizzare lo spazio delle ideazioni |

1. (Facoltativo) Includi un messaggio con l&#39;assegnazione, quindi fai clic su **Invita**.

   Gli utenti invitati ricevono una notifica e-mail relativa all’assegnazione delle autorizzazioni.

1. Fare clic sull&#39;icona **X** per chiudere la casella **Condividi documento**.











