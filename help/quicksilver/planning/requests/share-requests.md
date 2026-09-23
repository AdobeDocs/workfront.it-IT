---
title: Condividere le richieste Planning
description: È possibile condividere una richiesta di Workfront Planning con altri utenti dopo l'invio.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 4ee702aeded88e330ec456a0e6b5cf1813bfb64e
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 5%
---
# Condividere le richieste Planning

<!--add to TOC, and miniTOC-->

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo il rilascio in anteprima, le stesse funzioni sono disponibili mensilmente nell’ambiente di produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Dopo aver sottomesso una richiesta di Planning, è possibile controllare chi la vede, chi può lavorarci e quali azioni possono intraprendere ogni persona o team. In questo modo le persone giuste vengono concentrate sulle richieste giuste e si garantisce che possano intraprendere solo le azioni appropriate al loro ruolo.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi Workfront o flusso di lavoro con un pacchetto Planning</p> 
Oppure
<p>Qualsiasi programma Workfront Planning acquistato come prodotto standalone</p> 
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
   <td>   <p>Visualizza o autorizzazioni superiori per un’area di lavoro e un tipo di record, se sei un utente di Workfront</p>  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni durante la condivisione delle richieste

* Puoi concedere le seguenti autorizzazioni agli utenti di una richiesta:

  * Visualizzazione: gli utenti possono solo visualizzare la richiesta.
  * Contribute: gli utenti possono visualizzare, modificare e commentare la richiesta.
  * Gestisci: gli utenti possono visualizzare, modificare, commentare ed eliminare la richiesta.

* I richiedenti vengono autorizzati automaticamente a gestire l’accesso alle richieste che inviano, a meno che un amministratore non abbia configurato un’impostazione predefinita diversa.

  Per informazioni, vedere [Creare il modulo di richiesta](/help/quicksilver/planning/requests/create-request-form.md).

* Gli amministratori di Workfront possono accedere a tutte le richieste e gestirle.
* Gli utenti con l’accesso Manage a un tipo di record ereditano l’accesso Manage alla forma di acquisizione di quel tipo di record e a ogni richiesta inviata tramite di esso.
* Chiunque disponga delle autorizzazioni per una richiesta può condividere la richiesta con lo stesso livello di autorizzazione o con un livello inferiore rispetto al proprio.

  Gli utenti con autorizzazioni Contribute non possono assegnare a nessun altro le autorizzazioni Manage per la richiesta.

* Persone e team diversi possono disporre di livelli di accesso diversi sulla stessa richiesta.
* Le autorizzazioni possono essere assegnate tramite più entità. Se un utente dispone delle autorizzazioni Contribute per una richiesta ma il gruppo o il ruolo dispone delle autorizzazioni View (Visualizzazione), mantiene il livello di autorizzazione più alto, ovvero Contribute.

## Condividere una richiesta

Assicurati di utilizzare la nuova esperienza di richiesta.

1. {{step1-to-requests}}
1. Trovare una richiesta di Planning e fare clic su di essa per aprirla.
1. Fai clic su **Condividi**.

   Viene visualizzata la casella **Condividi** per la richiesta selezionata.

   ![Casella di condivisione richieste](assets/requests-sharing-box.png)

1. Nel campo **Concedi l&#39;accesso a questa richiesta**, inizia a digitare il nome di un utente, un team, una mansione, un gruppo o un&#39;azienda e fai clic su di esso quando viene visualizzato nell&#39;elenco.

   Nell&#39;elenco vengono visualizzate solo le entità attive.
1. Dal menu a discesa a destra del nome di ogni entità, selezionare uno dei seguenti livelli di autorizzazione:

   * Gestione
   * Contribuisci
   * Visualizzazione
1. (Facoltativo) Per ogni livello di autorizzazione, fai clic sull&#39;icona dell&#39;autorizzazione granulare e seleziona o deseleziona le autorizzazioni granulari, ad esempio **Modifica**, **Commento**, **Condividi** o **Elimina**.

   ![Autorizzazioni granulari per le richieste](assets/granular-permissions-on-requests.png)
1. Fai clic su **Salva**.

   La richiesta viene condivisa con le entità selezionate.


