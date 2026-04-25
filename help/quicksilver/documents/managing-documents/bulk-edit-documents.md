---
content-type: reference
product-area: documents
navigation-topic: documents-navigation-topic
title: Modificare documenti in blocco
description: Puoi modificare più documenti contemporaneamente nell’area Documenti.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: e8badce6-86f5-416c-a238-f9b7f19cdd2d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 76%

---

# Modificare documenti in blocco

Puoi modificare la descrizione, aggiungere moduli personalizzati e modificarli in più documenti contemporaneamente.

## Considerazioni durante la modifica di moduli personalizzati

Durante la modifica in blocco di moduli personalizzati nei documenti, tieni presente quanto segue:

* Le informazioni che modifichi in tutti i documenti selezionati sovrascrivono quelle esistenti nei singoli documenti.
* Quando selezioni documenti che hanno valori diversi per lo stesso campo, il campo mostra l’indicatore “Valori multipli”. I campi costituiti da caselle di controllo, pulsanti di scelta e interruttori mostrano l’indicatore “Valori multipli” accanto.
* Quando aggiorni un’opzione in un campo con più opzioni (ad esempio un campo visualizzato come un set di interruttori o caselle di controllo), tutte le altre devono corrispondere nei documenti selezionati.

>[!BEGINSHADEBOX]

**Esempio**
È possibile che sia disponibile un modulo personalizzato con un campo casella di controllo con tre caselle di controllo (Opzione 1, Opzione 2 e Opzione 3) e che l&#39;Opzione 1 sia deselezionata per tutti i documenti selezionati e che le Opzioni 2 e 3 siano selezionate per alcuni documenti e deselezionate per altri documenti selezionati. Se desideri selezionare l’Opzione 1 per tutti i documenti, prima di salvare le modifiche è necessario che anche le opzioni 2 e 3 corrispondano per tutti i progetti selezionati. Quindi è necessario selezionarle o deselezionarle in modo che corrispondano a tutti i progetti selezionati. Se non modifichi alcuna opzione, puoi salvare il campo così com’è e i documenti manterranno la selezione corrente per tutte le opzioni.

>[!ENDSHADEBOX]

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi pacchetto Workfront per gestire i documenti utilizzando lo storage Workfront legacy</p>
<p>Qualsiasi pacchetto di flusso di lavoro per gestire i documenti utilizzando lo storage aziendale Adobe</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td><p>Collaboratore o successiva</p> 
   <p>Richiedente o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso in modifica ai documenti</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Accesso in gestione al documento</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modificare documenti in blocco nell&#39;area documenti legacy

Se la tua organizzazione utilizza un sistema di archiviazione Workfront legacy, quando accedi ai documenti in Workfront visualizzerai l’area documenti legacy. Per ulteriori informazioni sull&#39;archiviazione Workfront, vedere [Differenze tra l&#39;archiviazione aziendale Adobe e l&#39;archiviazione Workfront legacy](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage).

Per modificare i documenti in blocco:

1. Passa alla scheda Documenti di un progetto o all’area Documenti dal menu principale.
1. Premi Ctrl o Comando sulla tastiera e seleziona i documenti che desideri modificare.
1. Fai clic sull’icona Modifica ![icona Modifica](assets/edit-icon.png).
   ![posizione dell’icona Modifica sulla pagina](assets/edit-multiple-documents.png)
1. (Facoltativo) Aggiungi o modifica la **Descrizione**. Se la descrizione di ciascun documento è diversa, nella casella della descrizione verrà visualizzato _Valori multipli_. Puoi aggiungere la stessa descrizione per tutti i documenti, ma non puoi modificare le descrizioni dei singoli documenti durante la modifica in blocco.
1. Apporta le seguenti modifiche tramite i moduli personalizzati:

   <table>
    <tr>
    <td><strong>Aggiungere i moduli</strong></td>
    <td>Nella <strong>casella Aggiungi modulo personalizzato</strong> puoi scegliere tra moduli allegati e moduli da aggiungere. I moduli allegati sono presenti in alcuni dei documenti selezionati, ma non in tutti. Un modulo associato a tutti i documenti selezionati viene visualizzato automaticamente nella finestra di modifica.  </td>
    </tr>
    <tr>
    <td><strong>Modificare i moduli</strong></td>
    <td>Modifica qualsiasi modulo personalizzato associato. Le informazioni modificate sovrascrivono quelle esistenti nei singoli documenti. I campi con valori diversi nei documenti vengono visualizzati come “Valori multipli”. </td>
    </tr>
    <tr>
    <td><strong>Ridisporre i moduli</strong></td>
    <td>Fai clic sul modulo personalizzato e trascinalo per ridisporlo.</td>
    </tr>
    </table>
1. Fai clic su **Salva**.

## Modificare i documenti in blocco nell&#39;area nuovi documenti


Se l&#39;organizzazione utilizza l&#39;archiviazione aziendale, quando si accede ai documenti in Workfront verrà visualizzata la nuova area documenti. Per ulteriori informazioni sull&#39;archiviazione aziendale, vedere [Panoramica sull&#39;archiviazione aziendale di Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Per modificare i documenti in blocco:

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti**.
1. Premi Ctrl o Comando sulla tastiera e seleziona i documenti che desideri modificare.
1. Fai clic su Modifica nella parte inferiore della pagina.
   ![modifica più documenti](assets/bulk-edit-documents.png)
1. (Facoltativo) Aggiungi o modifica la **Descrizione**. Se la descrizione di ciascun documento è diversa, nella casella della descrizione verrà visualizzato _Valori multipli_. Puoi aggiungere la stessa descrizione per tutti i documenti, ma non puoi modificare le descrizioni dei singoli documenti durante la modifica in blocco.
1. Apporta le seguenti modifiche tramite i moduli personalizzati:

   <table>
    <tr>
    <td><strong>Aggiungere i moduli</strong></td>
    <td>Nella sezione <strong>Modulo personalizzato</strong> è possibile aggiungere un nuovo modulo personalizzato ai documenti selezionati. I moduli personalizzati allegati a tutti i documenti selezionati vengono visualizzati nella sezione <strong>Moduli personalizzati in comune</strong>.  </td>
    </tr>
    <tr>
    <td><strong>Modificare i moduli</strong></td>
    <td>Modifica qualsiasi modulo personalizzato associato. Le informazioni modificate sovrascrivono quelle esistenti nei singoli documenti. I campi con valori diversi nei documenti vengono visualizzati come “Valori multipli”. </td>
    </tr>
    </table>
1. Fai clic su **Salva**.

## Modificare documenti in blocco in un rapporto di documenti

1. Accedi a un rapporto di documenti esistente.
oppure
Creare un report di documenti come descritto in [Creare un report personalizzato](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Seleziona i documenti che desideri modificare.
1. Fai clic sull’icona Modifica ![icona Modifica](assets/edit-icon.png).
1. (Facoltativo) Aggiungi o modifica la **Descrizione**. Se la descrizione di ciascun documento è diversa, nella casella della descrizione verrà visualizzato _Valori multipli_. Puoi aggiungere la stessa descrizione per tutti i documenti, ma non puoi modificare le descrizioni dei singoli documenti durante la modifica in blocco.
1. Apporta le seguenti modifiche tramite i moduli personalizzati:

   <table>
    <tr>
    <td><strong>Aggiungere i moduli</strong></td>
    <td>Nella <strong>casella Aggiungi modulo personalizzato</strong> puoi scegliere tra moduli allegati e moduli da aggiungere. I moduli allegati sono presenti in alcuni dei documenti selezionati, ma non in tutti. Un modulo associato a tutti i documenti selezionati viene visualizzato automaticamente nella finestra di modifica.  </td>
    </tr>
    <tr>
    <td><strong>Modificare i moduli</strong></td>
    <td>Modifica qualsiasi modulo personalizzato associato. Le informazioni modificate sovrascrivono quelle esistenti nei singoli documenti. I campi con valori diversi nei documenti vengono visualizzati come “Valori multipli”. </td>
    </tr>
    <tr>
    <td><strong>Ridisporre i moduli</strong></td>
    <td>Fai clic sul modulo personalizzato e trascinalo per ridisporlo.</td>
    </tr>
    </table>
1. Fai clic su **Salva**.
