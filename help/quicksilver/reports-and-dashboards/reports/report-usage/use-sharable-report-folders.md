---
product-area: reporting
navigation-topic: report-usage
title: Utilizzare cartelle di rapporti condivisibili
description: Utilizza cartelle di rapporti condivisibili per organizzare i rapporti creati e condividerli con altri utenti in Adobe Workfront.
author: Courtney
feature: Reports and Dashboards
exl-id: 65831f2e-9092-4e99-a86b-40df42c713bf
source-git-commit: 650d24c36c3ccee810b8918ccdf456f607b055e9
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 5%

---

# Utilizzare cartelle di rapporti condivisibili

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambiente Sandbox di anteprima.</span>

<!-- This article is linked in the UI -->

Puoi utilizzare cartelle di rapporti condivisibili per organizzare i rapporti e condividerle con altri utenti. Questa funzione è progettata per i team che gestiscono grandi volumi di rapporti e richiedono un controllo degli accessi scalabile e coerente.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
   <p>qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informazioni sulle autorizzazioni per le cartelle

Le cartelle di rapporti condivisibili utilizzano due livelli di autorizzazione:

* **Visualizza**: gli utenti possono aprire i report nella cartella, ma non possono modificare i dettagli della cartella, aggiungere o rimuovere elementi o eliminare la cartella. È possibile consentire agli utenti con l&#39;accesso in visualizzazione di condividere la cartella abilitando l&#39;impostazione **Condividi** quando si concede l&#39;accesso.
* **Gestione**: gli utenti possono modificare i dettagli della cartella e aggiungere o spostare elementi del report. Inoltre, possono gestire l’accesso ai rapporti all’interno della cartella. Puoi consentire agli utenti con l&#39;accesso Gestisci di condividere la cartella o eliminare le cartelle abilitando le impostazioni **Condividi** e **Elimina** quando concedi l&#39;accesso.

Comportamento aggiuntivo:

* Gli amministratori di sistema possono visualizzare tutte le cartelle.
* Gli altri utenti visualizzano solo le cartelle a cui hanno accesso.
* Le autorizzazioni concesse a una cartella principale si applicano a tutte le sottocartelle e a tutti i report all&#39;interno di tale struttura di cartelle.
* Gli utenti con l&#39;accesso a una sottocartella possono visualizzare le relative cartelle padre per la navigazione, ma non le cartelle di pari livello a meno che l&#39;accesso non venga concesso.

## Creare una cartella di rapporti condivisibile

Solo gli amministratori di sistema possono creare cartelle al livello superiore. Dopo aver creato una cartella condivisibile, gli utenti con accesso Gestisci possono creare sottocartelle al suo interno.

{{step1-to-reports}}

1. Attiva le **cartelle di report condivisibili**.
1. Fare clic su **Crea cartella**.
1. Immettere un nome per la cartella.
1. Fai clic su **Crea**.

![crea una cartella condivisibile](assets/add-sharable-folder.png)

## Creare una sottocartella in una cartella di rapporti condivisibile

È possibile creare fino a 3 livelli di sottocartelle in una cartella di rapporti condivisibile. Le sottocartelle ereditano le autorizzazioni dalla cartella principale, ma è anche possibile impostare autorizzazioni univoche per ogni sottocartella.

{{step1-to-reports}}

1. Individuare la cartella in cui si desidera creare una sottocartella.
1. Fai clic su **Altro** > **Aggiungi sottocartella**.
1. Immettere un nome per la sottocartella.
1. Fai clic su **Crea**.

## Condividere una cartella di rapporti con altri utenti

Quando si condivide una cartella con gli utenti, questi ereditano l&#39;accesso a tutte le sottocartelle della struttura. Gli utenti devono inoltre avere accesso a ogni rapporto, tramite le autorizzazioni per le cartelle o la condivisione diretta dei rapporti.

{{step1-to-reports}}

1. Trova la cartella da condividere.
1. Fai clic su **Altro** > **Condividi**.
1. Aggiungi utenti, team, ruoli, gruppi o aziende.
1. Scegli l&#39;accesso **Visualizza** o **Gestisci**:
   * L’accesso in visualizzazione consente agli utenti di aprire i rapporti nella cartella. Puoi anche consentire agli utenti con l&#39;accesso in visualizzazione di condividere nuovamente la cartella selezionando **Condividi** nelle impostazioni aggiuntive.
   * L&#39;accesso Gestisci consente agli utenti di modificare i dettagli della cartella e di aggiungere o rimuovere elementi. Puoi anche consentire agli utenti con l&#39;accesso Gestisci di eliminare le cartelle o condividerle selezionando **Elimina** e **Condividi** nelle impostazioni aggiuntive.
1. Fai clic su **Salva**.

   ![condividere una cartella e ottimizzare l&#39;accesso](assets/share-settings-sharable-folders.png)

## Spostare un report in una cartella condivisibile

Per spostare un report in una cartella, è necessario disporre dei diritti di **Gestione** sia per il report che per la cartella condivisibile.

{{step1-to-reports}}

1. Seleziona la casella di controllo accanto al rapporto che desideri spostare.
1. Fai clic su **Sposta nella cartella** nella barra delle azioni nella parte inferiore dello schermo.
1. Trovare la cartella in cui spostare il report, quindi fare clic su **Sposta**. La struttura del report è compressa per impostazione predefinita, pertanto potrebbe essere necessario espandere le cartelle per trovare la cartella di destinazione.

   ![sposta un report in una cartella condivisibile](assets/move-to-folder.png)

## Eliminare una cartella di rapporti condivisibile

Quando si elimina una cartella, vengono eliminate anche tutte le sottocartelle all&#39;interno della cartella. Devi avere l&#39;accesso **Gestisci** alla cartella per eliminarla. I rapporti presenti nella cartella non vengono eliminati, ma si trovano comunque nell’elenco principale dei rapporti.

Le autorizzazioni per i rapporti concesse tramite le autorizzazioni per le cartelle vengono rimosse quando la cartella viene eliminata. Le autorizzazioni per i rapporti concesse direttamente dal rapporto o ereditate da un dashboard rimangono attive.


{{step1-to-reports}}

1. Fai clic su **Altro** > **Elimina**.
1. Fai clic su **Sì, eliminalo** per confermare.


## Nuova esperienza di elenco per cartelle condivisibili

Quando accedi a cartelle condivisibili nell’area Rapporti, visualizzerai una nuova esperienza con un elenco che ti consente di visualizzare e gestire facilmente cartelle e rapporti. Per ulteriori informazioni sulla nuova esperienza di elenco, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).