---
title: Condividi campi Workfront Planning
description: È possibile condividere il campo di un record di Workfront Planning con altri utenti per garantire la collaborazione quando si utilizza Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 2d26437c69b3c36366938952d426532934f55c52
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 3%

---


# Condividere i campi di Workfront Planning

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

È possibile condividere il campo di un record di Workfront Planning con altri utenti per garantire la collaborazione quando si utilizza Adobe Workfront Planning.

La condivisione dei campi consente agli amministratori dell’area di lavoro di controllare l’accesso a un singolo campo. Ogni campo di un tipo di record dispone di una propria finestra di dialogo di condivisione in cui l&#39;accesso può essere impostato su Nessun accesso, Visualizza valori di campo o Gestisci valori di campo.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->



<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi Workfront o flusso di lavoro con un pacchetto Planning</p> 
Oppure
<p>Qualsiasi pacchetto di prodotti Workfront Planning come unità autonoma</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Qualsiasi</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Planning</p></td> 
   <td><p>Qualsiasi</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>È necessario aggiungere sia un flusso di lavoro che un tipo di licenza Planning al livello di accesso quando si dispone sia di un flusso di lavoro che di un pacchetto Planning</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td><p>Gestire le autorizzazioni per un campo per modificare i valori del campo</p>  
   <p>Contribuire o concedere autorizzazioni superiori a un tipo di record per ereditare le autorizzazioni Manage per il campo</p>  
   </td> 
  </tr>
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sulla condivisione dei campi

* Puoi condividere i campi con utenti, mansioni, gruppi, team o aziende.
* L’accesso a un campo proviene dalla combinazione delle seguenti impostazioni:

  * **Autorizzazioni ereditate**: per impostazione predefinita, un campo eredita lo stesso accesso di un utente sul tipo di record (le autorizzazioni di tipo Visualizza record concedono a un utente le autorizzazioni per visualizzare i valori dei campi; le autorizzazioni di tipo Contribute o Gestisci record concedono a un utente le autorizzazioni per gestire i valori dei campi). È possibile disattivare le autorizzazioni ereditate e concedere agli utenti un accesso al campo inferiore a quello di cui dispongono per il tipo di record.
  * **Tutti nell&#39;area di lavoro possono visualizzare** o **Solo gli invitati possono accedere alla selezione**. Puoi consentire a tutti coloro che dispongono delle autorizzazioni per l’area di lavoro di visualizzare il campo o concedere le autorizzazioni solo a singole entità.

  Se più regole si applicano alla stessa persona, questa riceve l’autorizzazione più elevata disponibile da una delle regole.

* Solo i proprietari e i responsabili dell&#39;area di lavoro possono modificare le autorizzazioni per i campi; i responsabili dell&#39;area di lavoro mantengono sempre l&#39;accesso Gestisci a tutti i campi e non possono ridurlo.
* La condivisione dei campi controlla l&#39;accesso ai valori, non alle impostazioni dei campi. Solo i responsabili del workspace possono modificare la configurazione di un campo.
* L&#39;aggiunta di un utente all&#39;elenco di condivisione di un campo non consente l&#39;accesso all&#39;area di lavoro o al tipo di record. Se non dispongono di tale accesso, un&#39;icona di avviso indica che l&#39;autorizzazione avrà effetto solo dopo essere state aggiunte al tipo di record.
* I campi di sistema (ad esempio Creato da, ID record) e i campi primari non possono avere una condivisione limitata.
* I campi con restrizioni vengono applicati ovunque venga visualizzato il campo. Ciò include tutte le visualizzazioni, le pagine dei dettagli dei record, i moduli di richiesta, le connessioni e i campi di ricerca, le dashboard di Canvas, gli strumenti API e MCP.
* I campi di ricerca ereditano le autorizzazioni del relativo campo di origine.
* Le visualizzazioni pubbliche rimangono completamente visibili e di sola lettura per chiunque possa accedervi.
* Quando si duplica un record, i valori con restrizioni non vengono copiati nei nuovi record.
* Le modifiche al valore del campo con restrizioni non vengono registrate nella cronologia di un record.
* Le modifiche delle autorizzazioni per i campi non attivano le notifiche.
* Per i tipi di record globali, le autorizzazioni del campo si applicano a tutte le aree di lavoro secondarie e non possono essere regolate localmente.


Da Claude:
Autorizzazioni aggiuntive per i campi: è possibile aggiungerlo all’articolo Panoramica per tutte le attività di condivisione?? - help/quicksilver/planning/access/sharing-permissions-overview.md

Di seguito viene illustrato il mapping tra il tipo di record e l&#39;accesso all&#39;area di lavoro e l&#39;accesso a livello di campo nel documento:

Livelli di autorizzazione del campo (solo due, più nessuno):

Nessun accesso: il campo è completamente nascosto
Visualizza i valori dei campi: può visualizzare il valore, non può modificarlo
Gestire i valori dei campi: può visualizzare e modificare

Ereditarietà predefinita dal ruolo del tipo di record

Tipo di record/accesso all’area di lavoro Autorizzazione per il campo predefinito
Visualizza i valori dei campi di visualizzazione
Valori del campo Gestione contributi
Gestisci (Workspace Manager) Gestisci valori campo (bloccato, non può essere ridotto)

Per impostazione predefinita, un campo rispecchia semplicemente il ruolo di un utente nel tipo di record: i visualizzatori sono di sola lettura, i collaboratori e i responsabili ottengono i diritti di modifica. I manager Workspace rappresentano un caso speciale: ogni volta che vengono aggiunti all’elenco di condivisione di un campo, l’opzione &quot;Gestisci valori campo&quot; è preselezionata e l’opzione &quot;Visualizza valori campo&quot; è disabilitata, in quanto il loro accesso di modifica non può mai essere rimosso.

Impostazione con caratteri jolly (fallback)
A parte l’ereditarietà, ogni campo ha un carattere jolly predefinito:

Tutti gli utenti dell&#39;area di lavoro possono visualizzare (impostazione predefinita)
Possono accedere solo le persone invitate

Calcolo dell’autorizzazione finale

Se sono abilitate le autorizzazioni ereditate: accesso di una persona = il più alto di (ereditato dal tipo di record, dal carattere jolly e dalle autorizzazioni concesse singolarmente).
Se le autorizzazioni ereditate sono disabilitate: l’accesso di una persona = il più alto tra (carattere jolly, autorizzazione concessa singolarmente) — il ruolo del tipo di record non influisce più su.
Se l’ereditarietà è disabilitata, il carattere jolly è &quot;Solo gli utenti invitati possono accedere&quot; e la persona non viene aggiunta singolarmente → non ha accesso.

Altre note sulle autorizzazioni

La concessione dell&#39;accesso individuale a un utente non consente l&#39;accesso all&#39;area di lavoro o al tipo di record, ma solo l&#39;utente rimane inattivo (con un&#39;icona di avviso) finché non viene aggiunto separatamente all&#39;area di lavoro.
Per i tipi di record globali, le autorizzazioni dei campi vengono impostate una sola volta e vengono applicate a tutte le aree di lavoro secondarie; i responsabili dell&#39;area di lavoro secondaria/team non possono sostituirle localmente.

## Condividi campi

