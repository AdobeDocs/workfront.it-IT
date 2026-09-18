---
title: Panoramica dell’Assistente di Adobe Workfront Planning AI
description: È possibile utilizzare l’assistente AI per generare, aggiornare o rimuovere record in base al contesto della pagina e alla struttura dei record correnti. I comandi dell’utente e l’esecuzione di tali comandi da parte dell’IA collaborano per garantire che le modifiche apportate dall’IA vengano riflesse accuratamente nell’ambiente.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/3I5y7eTZml-nkAiAYnBFuaw72DyXgNG12D-EVYVourA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: b529b3aded4ab92015683a0ddccd152bc2cc798c
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 6%
---
# Panoramica dell’Assistente IA di pianificazione di Adobe Workfront



<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo il rilascio in anteprima, le stesse funzioni sono disponibili mensilmente nell’ambiente di produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>



{{planning-important-intro}}

È possibile utilizzare l&#39;Assistente AI per apportare modifiche o aggiornamenti ai record e ad altri oggetti in Adobe Workfront Planning in base al contesto della pagina corrente.

I comandi dell’utente e l’esecuzione di tali comandi da parte dell’IA collaborano per garantire che le modifiche apportate dall’IA vengano riflesse accuratamente nell’ambiente.

>[!IMPORTANT]
>
><span class="preview">In alcune organizzazioni, l&#39;Assistente AI è stato sostituito da CX Coworker. Per informazioni, vedere [Panoramica di Adobe Workfront Planning CX Coworker](/help/quicksilver/planning/general/planning-cx-coworker-overview.md).</span>

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacchetti Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi Workfront o flusso di lavoro con un pacchetto Planning</p>
Oppure
<p>Qualsiasi pacchetto Planning acquistato come prodotto standalone</p>
   </td> </tr>
 <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
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
     <p>Per consentire l’accesso all’Assistente AI, l’amministratore deve effettuare le seguenti operazioni:</p>
   <ul>
   <li><p>Aggiungere un flusso di lavoro e un tipo di licenza Planning al livello di accesso quando si dispone sia di un flusso di lavoro che di un pacchetto Planning</p></li>
   <li><p>Deseleziona l’opzione Disattiva l’impostazione Assistente di intelligenza artificiale di Workfront nel tuo livello di accesso</p></li></ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>   <p>Gestione delle autorizzazioni per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Impostazioni di sistema</p></td> 
   <td>   <p>L’amministratore di Workfront deve selezionare l’impostazione Abilita AI nell’area Preferenze di sistema di Configura e firmare l’AI per accedere all’Assistente AI</p>  
    </td> 
  </tr> 
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considerazioni sull’Assistente AI

* L’Assistente AI deve essere abilitato per la tua organizzazione prima che sia disponibile per gli utenti della tua azienda.

  Per informazioni, vedere [Panoramica dell&#39;Assistente AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

* Dopo che Workfront ha abilitato l’agente per la tua organizzazione, questo sarà disponibile per l’amministratore Workfront principale. Per informazioni, vedere [Configurare le preferenze di sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

* L’amministratore di Workfront deve abilitare l’Assistente AI per tutti gli altri utenti. Per ulteriori informazioni, consulta [Abilitare o disabilitare l’Assistente IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* L’Assistente AI funziona nel contesto di ogni pagina. Le richieste inviate per l&#39;Assistente AI devono fare riferimento alla funzionalità disponibile nella pagina aperta.

* Le azioni eseguite dall&#39;Assistente IA nell&#39;area Planning si trovano nel contesto delle autorizzazioni di Workfront Planning e del livello di accesso a Workfront. Per ulteriori informazioni, consulta:

  * [Panoramica delle autorizzazioni di condivisione in Pianificazione di Adobe Workfront](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Panoramica del tipo di licenza per l’utilizzo di Pianificazione di Adobe Workfront](/help/quicksilver/planning/access/license-type-overview.md)

* Le modifiche apportate dall&#39;Assistente AI per conto dell&#39;utente vengono tracciate nel pannello della cronologia del record.

* Le azioni eseguite dall’assistente di intelligenza artificiale sono permanenti e potrebbero essere irreversibili. L’eliminazione di un campo, ad esempio, non può essere annullata. Rivedi tutte le azioni proposte dall’Assistente AI prima di accettarle.

* Durante la creazione, l’aggiornamento o l’eliminazione di un oggetto tramite l’Assistente IA, l’Assistente AI visualizza le azioni previste e richiede una conferma. Puoi quindi confermare o annullare le azioni.

## Funzionalità attualmente disponibile per l’Assistente IA

Attualmente, l’Assistente AI è disponibile nell’area Planning di Workfront per le seguenti pagine:

* Pagina Workspace
* Pagina tipo di record
* Pagina record

In questo momento, puoi utilizzare l’Assistente IA per eseguire le seguenti azioni:

* Cercare i record. È possibile eseguire ricerche in base alle informazioni contenute in qualsiasi campo record.
* Creare record. Dopo la creazione del record viene visualizzato un ID con un collegamento al nuovo record. Puoi specificare i campi da aggiornare durante il processo di creazione, come date o descrizione.
* Crea record basati su un documento caricato. Workfront supporta i seguenti formati di documento per l’Assistente IA:

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT e la maggior parte dei formati immagine
* Aggiorna i campi per i record visualizzati sullo schermo
* Eliminare i record
* Ripristina i record appena eliminati


## Individuare l&#39;Assistente IA in Workfront Planning

>[!NOTE]
>
><span class="preview">Se l&#39;organizzazione ha ricevuto l&#39;accesso a CX Coworker, l&#39;individuazione di CX Coworker è simile all&#39;individuazione dell&#39;Assistente AI. Per informazioni, vedere [Panoramica di Adobe Workfront Planning CX Coworker](/help/quicksilver/planning/general/planning-cx-coworker-overview.md).</span>


È possibile individuare l&#39;Assistente AI nelle seguenti aree di Workfront Planning:

* La barra di navigazione principale, nell’angolo superiore destro dello schermo.
* All&#39;interno dell&#39;area dei dettagli di un record, dopo aver aperto il record nell&#39;anteprima o dopo aver aperto la pagina del record.

### Accedere all’Assistente AI nell’area Pianificazione

1. Accedi a Workfront, quindi fai clic sull&#39;icona **Main Menu** ![Lines main menu](assets/lines-main-menu.png) in alto a sinistra, quindi fai clic su **Planning**.

   Verrà visualizzata l&#39;area Pianificazione.

1. Fai clic su una **scheda dell&#39;area di lavoro**.

1. (Facoltativo) Fai clic su una **scheda del tipo di record**.

1. (Facoltativo) Fai clic su un **record** per aprire la pagina **Dettagli** del record.

1. Fare clic sull&#39;icona **Assistente AI** nell&#39;angolo superiore destro dello schermo nella barra di navigazione globale o nell&#39;angolo superiore destro dell&#39;anteprima o della pagina del record.

   ![Icona Assistente IA](assets/ai-assistant-icon-highlighted.png)

1. Nello spazio disponibile, inizia a digitare i comandi per l’Assistente AI, quindi al termine fai clic su Invio.

   ![Pannello Assistente IA con casella di comando vuota](assets/ai-assistant-panel-with-empty-command-box.png)

   Ad esempio, è possibile digitare uno dei seguenti elementi:

   * Crea una campagna con data di inizio 4 luglio e data di fine 30 luglio
   * Aggiorna il campo Descrizione del record Campagna estiva con data da determinare
   * Elimina l&#39;ultimo record
   * Ripristina il record

   Viene visualizzato un indicatore visivo mentre l’Assistente AI elabora i comandi, impostando le aspettative per il tempo di risposta.

   Dopo aver ricevuto una risposta corretta, segui i collegamenti forniti o osserva le modifiche a sinistra.



