---
title: Panoramica della sezione Cronologia
description: È possibile esaminare le modifiche apportate al record e registrate dal sistema nel pannello destro di un record in Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 3%

---

# Panoramica della sezione Cronologia

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

È possibile collaborare ai record di Adobe Workfront Planning aggiungendo commenti o risposte nel pannello destro di un record. In quest&#39;area è inoltre possibile visualizzare altre modifiche apportate al record e registrate dal sistema.

Nel pannello destro di un record vengono visualizzate le sezioni riportate di seguito.

* **Commenti**: visualizza i commenti e le risposte aggiunte dagli utenti ai record. Per ulteriori informazioni sulla gestione dei commenti nei record di Workfront Planning, vedere [Gestire i commenti ai record](/help/quicksilver/planning/records/manage-record-comments.md).
* **Cronologia**: visualizza le modifiche registrate dal sistema apportate dagli utenti ai campi record.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Prodotti</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td> 
   <td> 
<p>Uno dei seguenti piani di Workfront:</p> 
<ul><li>Seleziona</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td> <p>Standard</p>
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Visualizza o autorizzazioni superiori per un'area di lavoro <!--<span class="preview">and record type</span>--> </a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello di layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Individuare la sezione Cronologia di un record

{{step1-to-planning}}

1. Fai clic sulla scheda di un’area di lavoro.

   L&#39;area di lavoro si apre e i tipi di record vengono visualizzati sulle schede.

1. Fare clic su una scheda del tipo di record.
Viene visualizzata la pagina del tipo di record e vengono visualizzati tutti i record di quel tipo.

1. In qualsiasi visualizzazione fare clic sul nome di un record.

   Viene visualizzata la pagina del record. L’area Commenti (Comments) viene visualizzata per impostazione predefinita nel pannello di destra.
1. Fai clic sull&#39;icona **Mostra cronologia** ![Mostra icona cronologia](assets/show-history-icon.png). Tutte le modifiche apportate ai campi del record vengono visualizzate nel pannello di destra, a partire da quello più recente.
1. (Facoltativo) Fai clic sull&#39;icona **Nascondi cronologia** ![Nascondi cronologia](assets/hide-history-icon.png) per chiudere il pannello di destra.

## Considerazioni sulla sezione Cronologia

È possibile esaminare le modifiche apportate ai campi record nella sezione Cronologia del pannello di destra della pagina di un record.

![Area della cronologia nei commenti](assets/history-area-in-comments.png)

* Workfront Planning registra le seguenti informazioni nella sezione Cronologia:

   * Qualsiasi modifica apportata ai campi

   * I vecchi e i nuovi valori dei campi, quando i valori cambiano. I vecchi valori vengono visualizzati in formato barrato.

   * Nome completo dell&#39;utente che ha apportato la modifica

   * Indicatore di data e ora in cui è avvenuta la modifica.

* I campi dei tipi seguenti visualizzano sempre il valore precedente (in formato barrato) e il nuovo valore:

   * Testo
   * Paragrafo
   * Valuta
   * Data
   * Numero
   * Percentuale
   * Selezione singola

* I campi dei tipi seguenti mostrano il valore precedente in formato barrato solo se è stato rimosso almeno uno dei valori multipli:

   * Selezione multipla
   * Campi record collegati
   * Persone

  Se la modifica ha aggiunto solo valori al campo, il valore precedente non viene visualizzato e viene visualizzato solo il nuovo valore del campo.

* Nei campi di tipo casella di controllo non viene mai visualizzato il valore precedente in formato barrato. Se il campo viene modificato, viene visualizzato solo lo stato corrente al momento della modifica.

  Per ulteriori informazioni sui campi di Workfront Planning, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

* Le modifiche ai campi dei tipi seguenti non vengono visualizzate nella sezione Cronologia:

   * Campi collegati (ricerca)
   * Formula
   * Creato da
   * Data creazione
   * Ultima modifica eseguita da
   * Data ultima modifica

* Se un campo viene rimosso dal sistema, gli aggiornamenti apportati a tale campo rimangono nella sezione Cronologia. Non vi è alcuna indicazione che il campo sia stato rimosso nella sezione Cronologia di un record.
