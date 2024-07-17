---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Visualizzare lo stato e l'avanzamento di una bozza in [!DNL Workfront Proof]
description: L’avanzamento della bozza indica il lavoro svolto su una bozza dal momento in cui la si invia ai revisori al momento in cui prendono una decisione sulla bozza.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 8fd85595-1403-490e-9d52-2ba5b01457b7
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 0%

---

# Visualizzare lo stato e l&#39;avanzamento di una bozza in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

## Informazioni sull’avanzamento della bozza

L’avanzamento della bozza indica il lavoro svolto su una bozza dal momento in cui la si invia ai revisori al momento in cui prendono una decisione sulla bozza.

* [Icone di avanzamento](#progress-icons)
* [Livelli di avanzamento bozza](#levels-of-proof-progress)

### Icone di avanzamento {#progress-icons}

Le icone di avanzamento, S, O, C e D, vengono visualizzate nella barra di avanzamento per indicare lo stato della bozza.

![proof_edit_existing_progress.png](assets/proof-edit-existing-progress-350x78.png)

Indicano le seguenti informazioni su una bozza:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Icona avanzamento</strong> </p> </td> 
   <td> <p><strong>Descrizione</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt="proof_progress_sent_icon.png"> </p> </td> 
   <td> <p><strong>Inviato</strong>. La bozza è stata inviata ai revisori.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-opened-icon.png" alt="proof_progress_open_icon.png"> </p> <p> </p> </td> 
   <td> <p><strong>Aperto</strong>. Un revisore ha aperto la pagina Dettagli bozza o ha aperto la bozza nel visualizzatore di bozze.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-comment-icon.png" alt="proof_progress_comment_icon.png"> </p> </td> 
   <td> <p><strong>Commenti</strong>. I revisori (utenti che possono fare commenti) hanno fatto commenti sulla bozza.</p> <p>Se per la bozza non è stato designato alcun revisore, l’icona non viene visualizzata.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt="proof_progress_decision_icon.png"> </p> </td> 
   <td> <p><strong>Decisione</strong>. Un revisore ha preso una decisione sulla bozza.</p> <p>Se per la bozza non è designato alcun approvatore (responsabili delle decisioni), questa icona non viene visualizzata. </p> </td> 
  </tr> 
 </tbody> 
</table>

Queste icone possono essere visualizzate nei seguenti colori per indicare alcune informazioni sull’avanzamento della bozza:

* **Verde**. Completato.
* **Bianco**. Non completato.
* **Arancione**. Non completo e scadenza inferiore a 24 ore.
* **Rosso**. Non completo e scaduto il termine.

### Livelli di avanzamento bozza {#levels-of-proof-progress}

Workfront Proof utilizza le icone di avanzamento per monitorare l’avanzamento di una bozza a ciascuno dei seguenti livelli:

* Per ogni revisore, in base all’attività della persona nella bozza.
* Per ogni fase, in base all’avanzamento del revisore sulla fase che è più indietro nel processo di verifica. Per ulteriori informazioni, vedere [Panoramica delle fasi automatizzate del flusso di lavoro](../../../review-and-approve-work/proofing/proofing-overview/stages.md).
* Per la bozza, in base all’avanzamento della fase (gruppo di revisori) che è la più indietro nel processo di bozza.

Per un esempio di come [!DNL Workfront Proof] determina l&#39;avanzamento utilizzando il revisore o la fase più indietro, si supponga che tre revisori su una bozza debbano prendere una decisione. Se due di loro hanno preso la loro decisione, ma il terzo no, l&#39;indicatore di avanzamento della prova non mostra la D in verde a causa della decisione in sospeso.

Se l&#39;impostazione [!UICONTROL Primary Decision Maker] è selezionata in una bozza e il decisore principale invia una decisione, la D nella barra di avanzamento della bozza diventa verde per tutti i revisori perché non sono necessarie altre decisioni.

Analogamente, se per una bozza è selezionata l&#39;impostazione [!UICONTROL Solo una decisione richiesta] e un revisore invia una decisione, la D nella barra di avanzamento della bozza diventa verde per tutti i revisori perché non sono necessarie altre decisioni.

## Informazioni sullo stato delle bozze

Lo stato della bozza visualizza lo stato delle decisioni necessarie per la bozza.

![modifica_bozza_stato_esistente.png](assets/proof-edit-existing-status-350x78.png)\
Le opzioni di stato standard sono:

* In Attesa
* Approvato
* Approvato con modifiche
* Modifiche richieste
* Non pertinente

Se nel tuo account sono configurate decisioni personalizzate, le opzioni di stato riflettono le impostazioni di decisione personalizzate.

Lo stato della bozza è determinato dal partecipante che si trova nel &quot;caso peggiore&quot;. Si supponga, ad esempio, di avere tre decisioni sulla bozza: due hanno lo stato **Accettato** e uno ha lo stato **Rifiutato**. La decisione del &quot;caso peggiore&quot; di Rifiutato sovrascrive le altre decisioni e lo stato complessivo della bozza viene visualizzato come **Rifiutato**.

## Visualizzazione dello stato e dell&#39;avanzamento {#viewing-progress-and-status}

Puoi visualizzare l’avanzamento e lo stato di bozze, fasi e revisori in ogni fase.

* [Riepilogo bozza](#proof-summary)
* [Menu Azioni stage](#stage-actions-menu)
* [Nella sezione [!UICONTROL Riepilogo] è inoltre possibile accedere ai menu delle azioni del revisore, purché si disponga dei diritti di modifica per la bozza. Per ulteriori informazioni, consulta Profili delle autorizzazioni di bozza in Workfront Proof e Gestione dei ruoli di bozza in Workfront Proof. Il menu [!UICONTROL Azioni revisore] (1) viene visualizzato quando si passa il puntatore del mouse sui dettagli del revisore e si consente di:](#in-the-summary-section-you-can-also-access-the-reviewer-actions-menus-provided-you-have-edit-rights-on-the-proof-for-more-information-see-proof-permissions-profiles-in-workfront-proof-and-manage-proof-roles-in-workfront-proof-the-reviewer-actions-menu-1-appears-when-you-hover-over-the-reviewer-s-details-and-allows-you-to)
* [Menu Azioni bozza](#proof-actions-menu)

### Riepilogo bozza {#proof-summary}

Ogni bozza nella cartella dispone di un riepilogo espandibile che consente di visualizzarne e modificarne rapidamente i dettagli.

Per espandere o comprimere il riepilogo:

1. Fai clic sulla freccia a sinistra della bozza nel dashboard o in una visualizzazione a elenco.

![Riepilogo_espandibile.png](assets/summary-expandable-350x68.png)

Il riepilogo include quanto segue:

* Flusso di lavoro (2)
* Versione (3)
* Cartella (4)
* Stato (5)\
   ![riepilogo_2.png](assets/summary-2-350x160.png)

Nel riepilogo, puoi visualizzare e modificare i seguenti dettagli della bozza:

* Avanzamento bozza (1)
* Stato di avanzamento di ciascuna fase (2)
* Termine fissato per la fase (3)
* Dettagli revisore:

   * Numero di commenti e risposte di ciascun revisore (4)
   * Avanzamento di ciascun revisore (5)
   * Decisione (se una decisione contiene firme elettroniche, accanto alla decisione che lo indica viene visualizzata un’icona). 6)
   * Ruolo nella bozza (7)
   * Impostazioni degli avvisi e-mail (8)

>[!NOTE]
>
>La possibilità di modificare i dettagli della bozza dipende dai tuoi diritti sulla bozza (vedi [Profili di autorizzazione bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) e [Gestione ruoli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![summary_details_3.png](assets/summary-details-3-350x160.png)

### Menu [!UICONTROL Azioni fase]  {#stage-actions-menu}

Ogni fase del flusso di lavoro dispone di un menu separato che consente di eseguire azioni in blocco correlate ai revisori in quella fase.

Il menu [!UICONTROL Azioni stage] viene visualizzato quando passi il cursore del mouse sulla sezione Stage (1) e consente di:

* [!UICONTROL Messaggio tutto] (2)
* [!UICONTROL Condividi] (3)
* [!UICONTROL Elimina fase] (4)

>[!NOTE]
>
>La disponibilità di queste opzioni dipende dai diritti sulla bozza (vedi [Profili di autorizzazione bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) e [Gestione ruoli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![Stage_actions_menu.png](assets/stage-actions-menu-350x161.png)

Nella sezione Riepilogo è inoltre possibile accedere ai menu delle azioni del revisore, purché si disponga dei diritti di modifica sulla bozza. Per ulteriori informazioni, vedere [Profili autorizzazioni bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) e [Gestione ruoli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md). Il menu Azioni revisore (1) viene visualizzato quando si passa il puntatore del mouse sui dettagli del revisore e consente di:

* Invia un messaggio al revisore (2)
* Modifica i dettagli del revisore (3): consente di modificare il nome visualizzato, il ruolo della bozza e l’avviso e-mail per quel revisore
* Rendi loro il proprietario della bozza (4)
* Diventare il principale responsabile delle decisioni (5)
* Rimuovi dalla bozza (6)

>[!NOTE]
>
>La visibilità di queste opzioni dipende dai diritti sulla bozza (vedi [Profili di autorizzazione bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) e [Gestione ruoli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![Reviewer_actions_menu.png](assets/reviewer-actions-menu-350x135.png)

### Menu Azioni bozza {#proof-actions-menu}

Ogni bozza dispone anche di un menu (1) che consente di eseguire le azioni seguenti:

* Puoi accedere alla pagina dei dettagli della bozza (2)
* Condividi la bozza con altri utenti (3)
* Invia un messaggio ai revisori (4)
* Crea una nuova versione della bozza (5)
* Copia la bozza (6)
* Scarica il file originale (7)
* Condividere collegamenti bozza (8)
* Stampa commenti (9)
* Richiedi un riepilogo Excel della bozza (10)
* Blocca la bozza (11)
* Elimina la bozza (12)

![Menu_azioni_bozza__1_.png](assets/proof-actions-menu--1--350x158.png)

>[!NOTE]
>
>La disponibilità di queste opzioni dipende dai diritti sulla bozza (vedi [Profili di autorizzazione bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) e [Gestione ruoli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

Per informazioni sulla visualizzazione dello stato e dell&#39;avanzamento della bozza in [!DNL Workfront], vedere [Visualizzazione dello stato e dell&#39;avanzamento](#viewing-progress-and-status).

Per informazioni sull&#39;avanzamento e lo stato della visualizzazione nel Visualizzatore bozze desktop, vedere [Rivedere un flusso di lavoro nel visualizzatore bozze](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-workflow.md).
