---
content-type: reference
product-area: documents
navigation-topic: documents-navigation-topic
title: Modifica documenti in blocco
description: È possibile modificare più documenti contemporaneamente nell'area Documenti.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: e8badce6-86f5-416c-a238-f9b7f19cdd2d
source-git-commit: 486b672a67c62b86f3306c9375a286895c2fae01
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 0%

---

# Modifica documenti in blocco

È possibile modificare la descrizione, aggiungere moduli personalizzati e modificare i moduli personalizzati in più documenti contemporaneamente.

## Considerazioni durante la modifica di moduli personalizzati

Quando si modificano in blocco moduli personalizzati per documenti, tenere presente quanto segue:

* Le informazioni che si stanno modificando in tutti i documenti selezionati sovrascrivono quelle esistenti nei singoli documenti.
* Quando si selezionano documenti con valori diversi per lo stesso campo, nel campo viene visualizzato un indicatore &quot;Più valori&quot;. I campi costituiti da caselle di controllo, pulsanti di scelta e interruttori dispongono accanto di un indicatore &quot;Più valori&quot;.
* Quando si aggiorna un&#39;opzione in un campo con più opzioni, ad esempio un campo visualizzato come un insieme di interruttori o caselle di controllo, tutte le altre opzioni devono corrispondere tra i documenti selezionati.

>[!BEGINSHADEBOX]

**Esempio**
È possibile che sia disponibile un modulo personalizzato con un campo casella di controllo con tre caselle di controllo (Opzione 1, Opzione 2 e Opzione 3) e che l&#39;Opzione 1 sia deselezionata per tutti i documenti selezionati e che le Opzioni 2 e 3 siano selezionate per alcuni documenti e deselezionate per altri documenti selezionati. Se si desidera selezionare l&#39;opzione 1 per tutti i documenti, prima di salvare le modifiche è necessario far corrispondere le opzioni 2 e 3 per tutti i progetti selezionati. Devi quindi selezionarli o deselezionarli in modo che corrispondano a tutti i progetti selezionati. Se non si modifica alcuna opzione, è possibile salvare il campo così com&#39;è e i documenti mantengono la selezione corrente per tutte le opzioni.

>[!ENDSHADEBOX]

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td><p> Nuovo: Collaboratore o versione successiva</p> 
   <p> Corrente: richiesta o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire l’accesso al documento</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

+++

## Modifica documenti in blocco

Per modificare documenti in blocco:

1. Passa alla scheda Documenti di un progetto o all’area Documenti dal menu principale.
1. Premere Ctrl o Comando sulla tastiera e selezionare i documenti da modificare.
1. Fai clic sull&#39;icona Modifica ![icona Modifica](assets/edit-icon.png).
   ![modifica posizione icona a pagina](assets/edit-multiple-documents.png)
1. (Facoltativo) Aggiungi o modifica la **Descrizione**. Se la descrizione di ogni documento è diversa, nella casella di descrizione verranno visualizzati _Più valori_. È possibile aggiungere la stessa descrizione per tutti i documenti, ma non è possibile modificare le descrizioni di singoli documenti durante la modifica in blocco.
1. Apporta le seguenti modifiche ai moduli personalizzati:

   <table>
    <tr>
    <td><strong>Aggiungi moduli</strong></td>
    <td>Nella <strong>casella Aggiungi modulo personalizzato</strong> è possibile scegliere tra Moduli allegati e moduli da aggiungere. I moduli allegati si trovano su alcuni dei documenti selezionati, ma non su tutti. Un modulo allegato a tutti i documenti selezionati viene visualizzato automaticamente nella finestra di modifica.  </td>
    </tr>
    <tr>
    <td><strong>Modifica moduli</strong></td>
    <td>Modifica eventuali moduli personalizzati allegati. Le informazioni modificate sovrascrivono quelle esistenti nei singoli documenti. I campi con valori diversi nei documenti vengono visualizzati come "Più valori". </td>
    </tr>
    <tr>
    <td><strong>Ridisponi moduli</strong></td>
    <td>Fai clic su e trascina il modulo personalizzato per ridisporlo.</td>
    </tr>
    </table>
1. Fai clic su **Salva**.


## Modificare documenti in blocco in un report Documento

1. Passare a un report documento esistente.
o
Creare un report di documenti come descritto in [Creare un report personalizzato](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Selezionare i documenti da modificare.
1. Fai clic sull&#39;icona Modifica ![icona Modifica](assets/edit-icon.png).
   ![modifica posizione icona a pagina](assets/edit-multiple-documents.png)
1. (Facoltativo) Aggiungi o modifica la **Descrizione**. Se la descrizione di ogni documento è diversa, nella casella di descrizione verranno visualizzati _Più valori_. È possibile aggiungere la stessa descrizione per tutti i documenti, ma non è possibile modificare le descrizioni di singoli documenti durante la modifica in blocco.
1. Apporta le seguenti modifiche ai moduli personalizzati:

   <table>
    <tr>
    <td><strong>Aggiungi moduli</strong></td>
    <td>Nella <strong>casella Aggiungi modulo personalizzato</strong> è possibile scegliere tra Moduli allegati e moduli da aggiungere. I moduli allegati si trovano su alcuni dei documenti selezionati, ma non su tutti. Un modulo allegato a tutti i documenti selezionati viene visualizzato automaticamente nella finestra di modifica.  </td>
    </tr>
    <tr>
    <td><strong>Modifica moduli</strong></td>
    <td>Modifica eventuali moduli personalizzati allegati. Le informazioni modificate sovrascrivono quelle esistenti nei singoli documenti. I campi con valori diversi nei documenti vengono visualizzati come "Più valori". </td>
    </tr>
    <tr>
    <td><strong>Ridisponi moduli</strong></td>
    <td>Fai clic su e trascina il modulo personalizzato per ridisporlo.</td>
    </tr>
    </table>
1. Fai clic su **Salva**.
