---
title: Panoramica di Adobe Workfront Planning CX Coworker
description: È possibile utilizzare CX Coworker in Workfront Planning per eseguire azioni simili ai record e ad altri oggetti in Planning che vengono normalmente eseguite nell'interfaccia. I comandi dell’utente e l’esecuzione di tali comandi da parte dell’IA collaborano per garantire che le modifiche apportate dall’IA vengano riflesse accuratamente nell’ambiente.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: d5f36e0c8dbd9749503de25b75e70bf18b1d187b
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 5%
---

# Panoramica di Adobe Workfront Planning CX Coworker


<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo il rilascio in anteprima, le stesse funzioni sono disponibili mensilmente nell’ambiente di produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

CX Coworker è un’interfaccia di conversazione in cui descrivi un obiettivo in linguaggio semplice e quindi pianifica, esegue e convalida il lavoro in Adobe e nei sistemi connessi prima di riportarlo per l’approvazione.

CX Coworker mantiene tutte le attività di AI Assistant e aggiunge funzionalità end-to-end più potenti sia nella nuova esperienza a schermo intero che nella barra laterale destra di Workfront.

Funziona all’interno dei controlli di accesso a livello di prodotto esistenti nella tua organizzazione, consentendo agli utenti di intraprendere solo le azioni a cui sono già autorizzati in Workfront, con accesso in sola lettura per impostazione predefinita e accesso in scrittura controllato dagli amministratori di Workfront.

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
   <p>L'amministratore deve effettuare le seguenti operazioni per consentire l'accesso a CX Coworker in Planning:</p>
   <ul>
   <li><p>Aggiungere un flusso di lavoro e un tipo di licenza Planning al livello di accesso quando si dispone sia di un flusso di lavoro che di un pacchetto Planning</p></li>
   <li><p>Deseleziona l’opzione Disattiva il pannello CX Coworker in Workfront nel tuo livello di accesso. È selezionata per impostazione predefinita.</p></li></ul>
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>   <p>Gestione delle autorizzazioni per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Impostazioni di sistema</p></td> 
   <td>   <p>L'amministratore di Workfront deve selezionare gli strumenti MCP di sola lettura e di sola scrittura nell'area Preferenze di sistema di Configura. Gli strumenti MCP di sola lettura sono selezionati per impostazione predefinita.</p> 
    </td> 
  </tr> 
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considerazioni per il CX Coworker

* Il CX Coworker deve essere abilitato per la tua organizzazione prima di essere disponibile per gli utenti della tua azienda.

  Per informazioni, vedere [Panoramica di CX Coworker](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

* Dopo che Workfront ha abilitato l’agente per la tua organizzazione, questo sarà disponibile per l’amministratore Workfront principale. Per informazioni, vedere [Configurare le informazioni di base per il sistema](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

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

È possibile individuare l&#39;Assistente AI nelle seguenti aree di Workfront Planning:

* La barra di navigazione principale, nell’angolo superiore destro dello schermo.
* All&#39;interno dell&#39;area dei dettagli di un record, dopo aver aperto il record nell&#39;anteprima o dopo aver aperto la pagina del record.

## Accedere all’Assistente AI nell’area Pianificazione

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



