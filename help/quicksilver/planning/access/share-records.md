---
title: Condividi record
description: Puoi condividere i record utilizzando il pulsante Condividi per aumentare la collaborazione in Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 0964ad24535bf43a23c740cd63abcf8fea705b8d
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 2%

---


<!--update metadata with real information at release-->

# Condividere i record

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

È possibile modificare le autorizzazioni delle persone per singoli record di un tipo di record. O

È possibile condividere un record di Adobe Workfront Planning nei modi seguenti:

* Condividere un collegamento al record.

  Per ulteriori informazioni, vedere [Condividere record utilizzando un collegamento](/help/quicksilver/planning/records/share-records.md).

* Condividere tutti i record di un&#39;area di lavoro con altri utenti condividendo l&#39;area di lavoro e il tipo di record.

  Per ulteriori informazioni, consulta i seguenti articoli:

   * [Condividere un’area di lavoro](/help/quicksilver/planning/access/share-workspaces.md)

   * [Condividere un tipo di record](/help/quicksilver/planning/access/share-record-types.md)

* Condividi un record utilizzando l&#39;opzione **Condividi**.

  Questo articolo descrive come condividere un record con altri utenti utilizzando l&#39;opzione **Condividi**.

>[!IMPORTANT]
>
>Gli utenti con accesso a un&#39;area di lavoro ottengono automaticamente almeno le autorizzazioni di visualizzazione per tutti i record dell&#39;area di lavoro.
>La condivisione delle visualizzazioni non concede agli utenti le autorizzazioni per i record. Solo le aree di lavoro condivise possono concedere agli utenti le autorizzazioni per tipi di record e record.
>
>Per informazioni generali sulla condivisione di oggetti in Workfront Planning, vedere anche [Panoramica sulle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).


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
<p>Qualsiasi pacchetto Workfront e Planning</p> 
Oppure
<p>Qualsiasi pacchetto di Workflow e Planning</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Qualsiasi</p> 
   <p><b>NOTA</b></p>
   <p>Solo le persone con una licenza Standard possono ottenere le autorizzazioni di gestione per i record. Tutte le altre licenze possono disporre solo delle autorizzazioni di visualizzazione e l’opzione Gestisci non è attiva.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>  <p>Gestire le autorizzazioni per un'area di lavoro, un tipo di record e il record</p>  
   <p><b>IMPORTANTE</b></p>
   <p>Solo gli utenti con le autorizzazioni di gestione di un'area di lavoro possono condividere un record</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> Agli utenti con una licenza Light o Contributor deve essere assegnato un modello di layout che includa Planning.
   <p>Per impostazione predefinita, le aree Pianificazione sono attivate dagli utenti standard e dagli amministratori di sistema.</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni durante la condivisione dei record

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

* Puoi condividere i record con le seguenti entità: persone, gruppi, team, aziende o mansioni.
* Per impostazione predefinita, quando si condivide un&#39;area di lavoro con gli utenti, questi ultimi ricevono anche le stesse autorizzazioni per i record nell&#39;area di lavoro.
* Quando rimuovi un’entità da un’area di lavoro, tutte le autorizzazioni di condivisione vengono rimosse dai tipi di record e da tutti i record in essa contenuti.
* L’accesso di un utente al record è determinato dalla combinazione delle tre impostazioni seguenti:

   * Le relative autorizzazioni ereditate dal tipo di record e dall’area di lavoro
   * Autorizzazioni aggiunte singolarmente nella finestra di dialogo di condivisione dei record
   * Le seguenti autorizzazioni:

      * **Tutti nell&#39;area di lavoro possono visualizzare**: in questo modo il record sarà visualizzabile da tutti gli utenti nell&#39;area di lavoro <!-- is this OK to say "workspace? should it be "record"??-->
      * **Solo le persone invitate possono accedere**: questa opzione è selezionata per impostazione predefinita e consente di limitare l&#39;accesso al record a persone specifiche.

* È possibile concedere a un record i livelli di autorizzazione seguenti:

   * Visualizzazione
   * Gestione

* Per impostazione predefinita, quando si condivide un record con un utente, questi vengono aggiunti con la stessa autorizzazione disponibile per il tipo di record.

  Ad esempio:

   * Se dispongono delle autorizzazioni di visualizzazione per il tipo di record, ottengono le autorizzazioni di visualizzazione per il record
   * Se dispongono delle autorizzazioni Contribuisci o Gestisci per il tipo di record, ottengono le autorizzazioni Gestione per il record

* In qualità di responsabile dell&#39;area di lavoro, puoi condividere un record con un utente che non fa parte dell&#39;area di lavoro. In questo caso, accanto all’entità aggiunta viene visualizzato un avviso per informare che non hanno accesso all’area di lavoro. È possibile accettare di aggiungere l&#39;utente sia al record che all&#39;area di lavoro oppure negare l&#39;aggiunta di tali utenti all&#39;area di lavoro, rimuovendoli anche dal record.

* Quando si condivide un record con utenti che dispongono delle autorizzazioni di gestione per l&#39;area di lavoro, per impostazione predefinita tali utenti ottengono anche le autorizzazioni di gestione per il record. L’autorizzazione Visualizzazione è disabilitata.

* Se non disponi delle autorizzazioni necessarie per aggiungere persone all’area di lavoro, visualizzerai e aggiungerai solo utenti, team, gruppi, ruoli e aziende già aggiunti all’area di lavoro. Non è possibile aggiungere altre entità che non fanno già parte dell&#39;area di lavoro.

* È possibile disabilitare le autorizzazioni ereditate per un singolo record, nel qual caso è possibile assegnare loro le autorizzazioni singolarmente oppure ottenere le autorizzazioni se appartengono all&#39;opzione &quot;Tutti nell&#39;area di lavoro&quot;. <!-- is this OK to say "workspace? should it be "record"??-->

* Se più autorizzazioni di condivisione si applicano allo stesso utente, quest&#39;ultimo riceve l&#39;autorizzazione più elevata.

  Ad esempio, se un record è condiviso con un utente con autorizzazioni di visualizzazione e il relativo gruppo con l&#39;accesso Gestisci, ottengono le autorizzazioni di gestione per il record.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Se un campo formula o un campo di ricerca di un record connesso è basato su un campo di un record per il quale non si dispone di autorizzazioni, verrà visualizzato il calcolo corretto per i fattori del record ai quali non è possibile accedere in altro modo.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Condividere le autorizzazioni dei record

