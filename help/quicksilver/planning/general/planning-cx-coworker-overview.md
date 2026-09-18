---
title: Panoramica di Adobe Workfront Planning CX Coworker
description: È possibile utilizzare CX Coworker in Workfront Planning per eseguire azioni simili ai record e ad altri oggetti in Planning che vengono normalmente eseguite nell'interfaccia. I comandi dell’utente e l’esecuzione di tali comandi da parte dell’IA collaborano per garantire che le modifiche apportate dall’IA vengano riflesse accuratamente nell’ambiente.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: b529b3aded4ab92015683a0ddccd152bc2cc798c
workflow-type: tm+mt
source-wordcount: '1119'
ht-degree: 3%
---

# Panoramica di Adobe Workfront Planning CX Coworker

<!--replaced information from the AI Assistant for Planning article with CX Coworker-->

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo il rilascio in anteprima, le stesse funzioni sono disponibili mensilmente nell’ambiente di produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

CX Coworker è un&#39;interfaccia di conversazione in cui si descrive un obiettivo in linguaggio semplice e quindi pianifica, esegue e convalida il lavoro nei sistemi Workfront Planning e altri sistemi Adobe connessi prima di riportarlo per l&#39;approvazione.

CX Coworker mantiene tutte le attività di AI Assistant e aggiunge funzionalità end-to-end più potenti sia nella nuova esperienza a schermo intero che nella barra laterale destra di Workfront.

Funziona all’interno dei controlli di accesso a livello di prodotto esistenti nella tua organizzazione, consentendo agli utenti di intraprendere solo le azioni a cui sono già autorizzati in Workfront, con accesso in sola lettura per impostazione predefinita e accesso in scrittura controllato dagli amministratori di Workfront.

>[!IMPORTANT]
>
>CX Coworker non è attualmente disponibile per le organizzazioni del settore sanitario, finanziario o di altri settori con dati sensibili. L’Assistente AI è disponibile per queste organizzazioni.
>
>Per ulteriori informazioni, vedere [Panoramica dell&#39;Assistente AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).


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

## Considerazioni per CX Coworker

* Il CX Coworker deve essere abilitato per la tua organizzazione prima di essere disponibile per gli utenti della tua azienda.

  Per informazioni, vedere [Panoramica di CX Coworker](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

* Dopo che Workfront ha abilitato l’agente per l’istanza Workfront, questo è disponibile per l’amministratore principale di Workfront e può essere abilitato per la tua organizzazione. Per informazioni, vedere [Configurare le preferenze di sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

* L’amministratore di Workfront deve inoltre abilitare CX Coworker al tuo livello di accesso. Per informazioni, vedere [Creare e modificare i livelli di accesso](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* CX Coworker funziona con informazioni e oggetti presenti in Workfront o Workfront Planning e per i quali si dispone dell&#39;autorizzazione di accesso. Nella barra a destra di Planning, il pannello Collaboratore funziona nel contesto dell’area di lavoro, del tipo di record o della pagina di record aperti.

* Le azioni eseguite da CX Coworker nell&#39;area Planning si trovano nel contesto delle autorizzazioni di Workfront Planning e del livello di accesso a Workfront. Per ulteriori informazioni, consulta:

  * [Panoramica delle autorizzazioni di condivisione in Pianificazione di Adobe Workfront](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Panoramica del tipo di licenza per l’utilizzo di Pianificazione di Adobe Workfront](/help/quicksilver/planning/access/license-type-overview.md)

* Le modifiche apportate dal CX Coworker per conto dell&#39;utente vengono registrate nel pannello della cronologia del record.

* Le azioni intraprese da CX Coworker sono permanenti e potrebbero essere irreversibili. L’eliminazione di un campo, ad esempio, non può essere annullata. Rivedi tutte le azioni proposte da CX Coworker prima di accettarle.

* Durante la creazione, l’aggiornamento o l’eliminazione di un oggetto tramite CX Coworker, CX Coworker visualizza le azioni previste e richiede una conferma. Puoi quindi confermare o annullare le azioni.

## Funzionalità attualmente disponibile per CX Coworker

Attualmente, CX Coworker è disponibile nell&#39;area Planning di Workfront e utilizza una serie di competenze per accedere e manipolare le informazioni per gli oggetti Planning. Per ulteriori informazioni, vedere [CX Coworker skills](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-skills.md).

Puoi utilizzare CX Coworker per eseguire le seguenti azioni:

* Cercare i record. È possibile eseguire ricerche in base alle informazioni contenute in qualsiasi campo record.
* Creare record. Dopo la creazione del record viene visualizzato un ID con un collegamento al nuovo record. Puoi specificare i campi da aggiornare durante il processo di creazione, come date o descrizione.
* Crea record basati su un documento caricato. Workfront supporta i seguenti formati di documento per CX Coworker:

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT e la maggior parte dei formati immagine
* Aggiorna i campi per i record visualizzati sullo schermo
* Eliminare, duplicare o ripristinare record
* Collega record ad altri record
* Visualizzare la cronologia delle modifiche di un record


## Individuare CX Coworker in Workfront Planning

È possibile individuare CX Coworker nelle seguenti aree di Workfront Planning:

* La barra di navigazione principale, nell’angolo superiore destro dello schermo.
* All&#39;interno dell&#39;area dei dettagli di un record quando lo si apre in una nuova scheda.

## Accedere a CX Coworker nell&#39;area Planning


1. Accedi a Workfront, quindi fai clic sull&#39;icona **Main Menu** ![Lines main menu](assets/lines-main-menu.png) in alto a sinistra, quindi fai clic su **Planning**.

   Verrà visualizzata l&#39;area Pianificazione.

   Individua l&#39;icona **AI** ![AI](assets/ai-icon.png) nell&#39;angolo superiore destro della pagina oppure continua con i passaggi seguenti.

1. Fai clic su una **scheda dell&#39;area di lavoro**.

1. Fare clic su una **scheda del tipo di record**.

1. Fai clic su un **record** per aprire la pagina **Dettagli** del record, quindi fai clic sull&#39;opzione Apri in .

1. Fai clic sull&#39;icona **CX Coworker** nell&#39;angolo superiore destro dello schermo.

1. Nello spazio disponibile, inizia a digitare i comandi per CX Coworker, quindi al termine fai clic su Invio.

   ![Pannello CX Coworker con casella di comando vuota](assets/cx-coworker-right-rail.png)

   Ad esempio, è possibile digitare uno dei seguenti elementi:

   * Crea un nuovo record della campagna denominato Summer Sale 2026
   * Aggiorna il campo del budget nel record Campagna estiva a $75.000
   * Elimina il record della campagna denominato Old Promo
   * Ripristina la campagna che ho eliminato accidentalmente

   >[!TIP]
   >
   >Assicurarsi che l&#39;amministratore di Workfront abbia abilitato Strumenti MCP di sola scrittura nelle preferenze di sistema prima di richiedere al CX Coworker di eseguire azioni di modifica sugli oggetti.

   Durante l’elaborazione dei comandi da parte del CX Coworker viene visualizzato un indicatore visivo che imposta le aspettative relative al tempo di risposta.

   Dopo aver ricevuto una risposta corretta, segui i collegamenti forniti o osserva le modifiche a sinistra.


1. (Facoltativo) Fai clic sull&#39;icona **Espandi schermo intero** ![Espandi icona schermo intero](assets/expand-full-screen-icon.png) per aprire la finestra di chat di Coworker in una scheda del browser completa.


