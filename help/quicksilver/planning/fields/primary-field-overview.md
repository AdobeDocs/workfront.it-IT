---
title: Panoramica campo primario
description: Nella vista a tabella di un tipo di record in Adobe Workfront Planning, è possibile designare un campo di testo, numero o formula a riga singola come campo principale. Il campo principale diventa il titolo dei record di quel tipo.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: fe3127ab-3f59-46a0-a747-9e9e1582265b
source-git-commit: 609396b2eb6413c8f6e84361757f00c2cc5e3ad6
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---


# Panoramica del campo primario

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Il campo principale è il campo visualizzato nella prima colonna di una vista tabella di tipo record in Adobe Workfront Planning.

Per impostazione predefinita, il campo Nome è il campo principale. È tuttavia possibile designare come campi principali dei record qualsiasi campo dei tipi seguenti:

* Campo di testo a riga singola
* Numero
* Formula

![Evidenziato un altro campo di testo come campo primario](assets/another-text-field-as-a-primary-field-highlighted.png)

Per informazioni su come designare un campo come campo principale, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

## Panoramica dei campi principali

* Le informazioni nel campo designato come primario diventano il titolo di un record.

  >[!NOTE]
  >
  >    I nomi &quot;campo primario&quot; e &quot;titolo record&quot; sono sinonimi in Workfront Planning. Quando si visualizza il record nella vista a tabella, è preferibile utilizzare il campo primario.


* Il titolo di un record viene visualizzato nelle seguenti aree:

   * Area di intestazione della pagina e della casella di anteprima del record
   * Campi record collegati
   * Viste
* Non è possibile spostare, nascondere o eliminare il campo principale nella visualizzazione tabella, a meno che non si indichi un altro campo come campo principale.
* Il campo principale è sempre bloccato e non fa parte dello scorrimento orizzontale della vista tabella.
* La modifica del campo principale nella vista tabella ha effetto sulla vista di tutti gli altri utenti che la scelgono.
* La modifica del campo principale in una vista tabella ha effetto su tutte le viste tabella del tipo di record.
* Il valore elencato nel campo principale è sempre collegato alla pagina del record.
* Se si dispone delle autorizzazioni Contribute o di livello superiore per un&#39;area di lavoro <!--<span class="preview">and record type</span>-->, è possibile modificare il valore dei campi primari, ad eccezione dei campi formula. Le formule sono calcoli che vengono aggiornati automaticamente.
