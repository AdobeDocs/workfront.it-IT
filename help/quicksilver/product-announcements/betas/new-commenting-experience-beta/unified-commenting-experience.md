---
product-area: betas
navigation-topic: new-commenting-experience-beta
title: Nuova esperienza di commento
description: È attualmente in fase di sviluppo un aggiornamento dell’esperienza di aggiunta di commenti in Adobe Workfront. Questo aggiornamento include una nuova interfaccia, nuove funzioni e prestazioni migliorate nella sezione Aggiornamenti di alcuni oggetti selezionati.
author: Alina
feature: Product Announcements
role: User
exl-id: f750b35b-8021-4cc1-81d6-e1ece2530438
source-git-commit: 5d6e9788ccbae7a8970cff56558233a57ceee1ab
workflow-type: tm+mt
source-wordcount: '1377'
ht-degree: 1%

---

# Nuova esperienza di commento

<!--take out legacy, preview, prod references from below-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti.  </span>

<span class="preview">Per informazioni sulla pianificazione della versione corrente, consulta [Panoramica sulla versione del secondo trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

<!--

After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases.

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  -->

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono alle funzioni rilasciate nella nuova esperienza di commento.
>
>Il programma beta per la nuova esperienza di commento è iniziato ad aprile 2023 ed è terminato a ottobre 2023. Il programma beta per la nuova esperienza di commento si è chiuso con la versione di ottobre 2023.
>
>A partire da ottobre 2023, tutte le nuove funzioni per la nuova esperienza di commento vengono rilasciate a tutti i clienti. Per ulteriori informazioni, consulta la pagina con la panoramica della versione corrente per ciascuna versione.

<!--An update to the commenting experience in Adobe Workfront is currently in development. This update includes a new interface, new features, and improved performance in the Updates section of select objects. 

The new commenting experience will slowly become available for all the objects with an Updates section in Workfront, and later it will expand to other Adobe Experience Cloud applications.-->

<!--For additional resources for the new commenting experience, also see the following articles:

* [New commenting experience release activity](../new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md)
* [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md)
-->

## Funzioni

La nuova esperienza di aggiunta di commenti include miglioramenti e modifiche alla sezione Aggiornamenti degli oggetti di Adobe Workfront.

Tra i miglioramenti inclusi nella nuova esperienza di commento, ci sono i seguenti:

* Prestazioni ed esperienza utente migliorate
* Separazione dei commenti degli utenti dagli aggiornamenti delle attività di sistema
* Indicatore in tempo reale quando vengono aggiunti nuovi commenti a un oggetto
* Modifica di commenti dopo l’invio

Le seguenti funzioni sono state rimosse o diventeranno obsolete nella nuova esperienza:

* Commento su un aggiornamento del sistema. I commenti aggiunti in passato agli aggiornamenti di sistema sono stati importati come commenti di sola lettura nella nuova scheda Attività di sistema.
* Possibilità di modificare lo stato, la condizione, la data di conferma e la percentuale di completamento durante il commento di attività e problemi.

  In alternativa, è consigliabile aggiungere questi campi nel pannello Riepilogo delle attività e dei problemi, per accedervi facilmente da elenchi, Home, Workfront Balancer o una scheda orario.
* Possibilità di modificare il modulo personalizzato
* Le informazioni &quot;per conto di &lt; nome utente >&quot; quando un amministratore di Workfront o di gruppo effettua l’accesso come altro utente e aggiunge un commento per suo conto sono state originariamente rimosse. È stato ripristinato il 19 ottobre 2023.
* L’opzione &quot;Richiedi approvazione&quot; quando si applicano tag alle persone durante l’aggiunta di un commento a un documento.
* Quando si modifica la casella del profilo di un utente, l’impostazione &quot;Mostra percentuale di completamento all’aggiornamento dello stato&quot; viene rimossa. È stata rimossa la funzionalità di aggiornamento della percentuale di completamento di un’attività o di un problema.


<!--removed this note on November 28, 2023, when this limitation was removed: 

>[!NOTE]
>
>The objects listed below have only the comments and system updates starting with January 1, 2019 available in the new commenting experience.  
>
>You can view comments and system updates on these objects prior to January 1, 2019 when viewing the Updates section in the current experience:
>
>* Issues
>* Projects
>* Tasks
>* Documents

For more information, see the [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md). 
-->

La tabella seguente illustra le funzioni che saranno disponibili nella nuova esperienza di commento e la loro disponibilità nelle aree in cui sono supportate:

<table>
  <tr>
   <td><strong>Funzionalità </strong>
   </td>
   <td><strong>Esiste nella vecchia esperienza di commento </strong>
   </td>
   <td><strong>Esiste nella nuova esperienza di commento </strong>
   </td>
   <td><strong>Verrà introdotta nella nuova esperienza di commento </strong>
   </td>
   <td><strong>Quando verrà introdotta nella nuova esperienza di commento </strong>
   </td>
   <td><strong>Nella ricerca </strong>
   </td>
  </tr>
  <tr>
   <td>Creare/leggere/rispondere/eliminare commenti 
   </td>
   <td>✓ 
  </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Testo formattato (escluse citazioni ed emoticon)
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Testo formattato (emoji)
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Testo formattato (virgolette)
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 2° trimestre 2023
   </td>
   <td> 
   </td>
  </tr>
  <tr>
<tr>
   <td> Commenti offerta
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 2° trimestre 2023
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Reagisce ai commenti (come) 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Allega immagini ai commenti 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Assegnare tag alle persone nei commenti 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Rimuovi partecipanti thread
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>


<tr>
   <td>Assegna automaticamente tag a tutti i partecipanti del thread
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Commenti privati a un’azienda 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Annullare la pubblicazione di un commento 
   </td>
   <td>✓ 
   </td>
   <td>Sostituito con modifica commento 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Disattiva aggiornamenti di sistema 
   </td>
   <td>✓ 
   </td>
   <td>Sostituito con la scheda Attività 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Modifica commenti 
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Salvataggio delle bozze dei commenti quando si esce dalla pagina 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Visualizzare nuovi commenti in tempo reale (include la visualizzazione quando un commento viene eliminato)
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Registra ore 
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
    <tr>
   <td>Copia link thread 
   </td>
   <td>✓ 
   </td>
   <td> Sostituito con il collegamento Copia
   </td>
   <td> 
   </td>
   <td>2° trimestre 2023 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Copia collegamento commento 
   </td>
   <td>✓ 
   </td>
   <td> Sostituito con il collegamento Copia
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Testo commento preventivo 
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td>2° trimestre 2023 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Copia corpo del testo 
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
    <tr>
   <td>Cerca nei commenti 
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>1° trimestre 2024 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Copiare e incollare immagini in un commento
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>1° trimestre 2024 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Trascinare le immagini in un commento
   </td>
   <td> ✓
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>1° trimestre 2024 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Modifica modulo personalizzato 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Possibilità di modificare lo stato, la condizione e la data del commit durante l'inserimento di commenti 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>
   </td>
  </tr>
<tr>
   <td>Rispondi agli aggiornamenti di sistema 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
<tr>
   <td>Visualizza "per conto di" quando si aggiungono commenti connessi come altro utente
   </td>
   <td> ✓
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Possibilità per il proprietario del progetto di modificare la data di completamento pianificata di un'attività quando la data di commit viene modificata dalla sezione Aggiornamenti
   </td>
   <td> ✓
   </td>
   <td> Potrebbe essere rilasciato in una data successiva
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> ✓
   </td>
  </tr>
</table>

## Timeline di rilascio

>[!IMPORTANT]
>
>Per informazioni sulle funzioni rilasciate alla nuova esperienza di commento durante l’intervallo di tempo beta, consulta [Nuova attività di commento della versione dell’esperienza beta](../../betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md).
>
>Per ulteriori informazioni sulla gestione degli aggiornamenti per gli oggetti Workfront, vedere [Aggiorna lavoro](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


Di seguito è riportata una timeline pianificata con le tappe principali per il rilascio della nuova esperienza di commento nell’ambiente di produzione. Oltre alle tappe indicate di seguito, continueremo a migliorare l’esperienza di aggiunta dei commenti con miglioramenti di minore entità.

Per informazioni sulle funzioni rilasciate per la nuova esperienza di commento dopo la chiusura del periodo beta, consulta la pagina di panoramica della versione corrente.

Di seguito è riportata una timeline pianificata per il rilascio della nuova esperienza di commento:

* Con la versione 23.2 (6 aprile 2023):
   * Avvia l’esperienza di commento Beta per i problemi
   * Rilascia la nuova esperienza di commento per gli obiettivi (come unica esperienza)
* Con la versione 23.3 (20 luglio 2023):
   * Avvia l&#39;esperienza di commento beta per progetti, attività e documenti.
   * Rilascia la nuova esperienza di commento per le schede nell’area Schede (come unica esperienza)
* Durante il rilascio del quarto trimestre 2023 (rilascio limitato, disponibile solo per i clienti che scelgono il rilascio rapido):
   * Rilascia la nuova esperienza di commento per modelli, attività modello, programmi, portfolio, team, utenti e schede orario (come unica esperienza)
   * Aggiorna l’esperienza di aggiunta di commenti Beta per progetti, attività, problemi e documenti, affinché diventi l’opzione predefinita. L’etichetta &quot;Beta&quot; viene rimossa.
* Con la versione del quarto trimestre 2023 (23.10) (26 ottobre 2023)
   * Rilascia a tutti i clienti la nuova esperienza di aggiunta di commenti per modelli, attività modello, programmi, portfolio, team, utenti e schede orario (come unica esperienza).
   * Imposta come predefinita la nuova esperienza di aggiunta di commenti per progetti, attività, problemi e documenti.

  >[!IMPORTANT]
  >
  >    In questo modo si conclude la fase beta della nuova esperienza di commento.

   * Rendi tutte le funzioni rilasciate per la nuova esperienza di commento che inizia con questa data parte delle regolari versioni mensili e trimestrali correnti.
* Fine del 2023:
   * Mantieni l’esperienza di commento legacy come opzione secondaria per i seguenti oggetti: progetti, attività, problemi e documenti. La nuova esperienza di aggiunta di commenti è l’opzione predefinita per tutti gli utenti di questi oggetti.
   * Rendi la nuova esperienza di commento l’unica esperienza per tutti gli altri oggetti.

  >[!NOTE]
  >
  >    Le iterazioni continueranno a presentare l’esperienza di commento legacy. La nuova esperienza di aggiunta di commenti non sarà disponibile per le iterazioni.

* Con la versione del secondo trimestre 2024 (11 aprile 2024):

   * Rimuovi l’opzione per tornare al flusso di commenti legacy e rendere il nuovo flusso di commenti l’unica esperienza per tutti gli oggetti, ad eccezione delle iterazioni.

## Individua la nuova esperienza di commento

<!--info for April 11: make this commented out text live and hide everything else underneath it, all the way to the end of the article: 

>[!IMPORTANT]
>
>The new commenting experience is available in all Workfront environments on all objects with the exception of Iterations. 
>
>The legacy commenting experience has been removed from all environments for Projects, Tasks, Issues, and Documents. 

For information about accessing the Updates section of Workfront objects, see [Updates section overview](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md). 

-->

La nuova esperienza di aggiunta di commenti è attualmente disponibile per tutti i clienti e per tutti gli ambienti.

A seconda degli oggetti per i quali accedi all’esperienza di commento, per la sezione Aggiornamenti potresti visualizzare le seguenti funzionalità:

* Sia la nuova esperienza di commento che quella legacy per i seguenti oggetti:

   * Progetto
   * Attività (incluse le storie)
   * Problema
   * Documento

     >[!NOTE]
     >
     ><span class="preview">L’esperienza di commento legacy è stata rimossa dall’ambiente di anteprima dal 1° aprile 2024. </span>

* Solo la nuova esperienza di commento per gli oggetti elencati di seguito. Non è possibile abilitare l’esperienza di commento legacy per questi oggetti:

   * Obiettivo

  >[!NOTE]
  >
  >Per accedere a quest’area di Workfront è necessaria un’ulteriore licenza per Adobe Workfront Goals. Per ulteriori informazioni, consulta [Requisiti per l’utilizzo degli obiettivi di Workfront](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * Scheda su una bacheca
   * Team
   * Modello
   * Attività modello
   * Scheda orario
   * Programma
   * Portfolio
   * Utente

* Solo l’esperienza di commento legacy per i seguenti oggetti:

   * Iterazioni

     Non è disponibile alcuna opzione per abilitare la nuova esperienza di commento per le iterazioni. Per le iterazioni è disponibile solo l’esperienza di commento legacy.


<!--before August 17: 

The new commenting experience is currently supported for the following objects:


* When enabling the Beta experience in the Updates section for 

    * Issues, projects, tasks, and documents

    For more information about managing updates for Workfront objects, see [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

* By default, as the only commenting experience for

    * Goals, cards on a board

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

-->

<!--Depending on the environment you access the commenting experience you can do one of the following: 

* Enable the commenting experience Beta in the Production environment
* <span class="preview">Enable the legacy commenting experience in the Preview  environment </span>
-->

Per abilitare l’opzione di esperienza con commenti per progetti, attività, problemi e documenti:

1. (Condizionale) Nell’ambiente di produzione, passa a un oggetto per il quale desideri attivare la nuova esperienza di commento, quindi fai clic su **Aggiornamenti** nel pannello a sinistra.
1. (Condizionale) Se è disabilitato, abilita **Nuovo commento** nell’angolo superiore destro dell’area Aggiornamenti per abilitarla. Questa opzione deve essere attivata per impostazione predefinita.
   <span class="preview">L’opzione Nuovo commento è stata rimossa dall’ambiente di anteprima.</span>

   ![](assets/new-commenting-toggle-off-highlighted.png)

1. Inizia a digitare un aggiornamento in **Commenti** scheda. La scheda Commenti è la scheda predefinita all’apertura della nuova esperienza

   Oppure

   Fai clic su  **Attività di sistema** per visualizzare gli aggiornamenti dell’attività generati da Workfront.

1. (Facoltativo) Per disattivare la nuova esperienza di commento e tornare ai commenti precedenti, deseleziona la **Nuovo commento** opzione.

