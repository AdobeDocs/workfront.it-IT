---
product-area: projects;user-management
keywords: modifica,moduli,RTF,testo,speciale,formato,campi,personalizzato,informazioni,personalizza,oggetti
navigation-topic: work-with-custom-forms
title: Modificare le informazioni nei campi modulo personalizzati
description: È possibile modificare le informazioni di un modulo personalizzato dopo che il modulo è stato allegato a un oggetto. Per informazioni sull'aggiunta di moduli personalizzati agli oggetti, vedere Aggiungere un modulo personalizzato a un oggetto.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 4897f165a7316a52b968601b45f95f7045f63840
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 1%

---

# Modificare le informazioni nei campi modulo personalizzati

{{preview-fast-release-general}}

<!--Audited: 10/2025-->

È possibile modificare le informazioni di un modulo personalizzato dopo che il modulo è stato allegato a un oggetto. Per informazioni sull&#39;aggiunta di moduli personalizzati agli oggetti, vedere [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Pacchetto Adobe Workfront</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licenza Adobe Workfront</p> </td> 
   <td> <p>Collaboratore o versione successiva</p> 
   <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso all’oggetto per il quale si desidera modificare il modulo personalizzato</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorizzazioni oggetto</p> </td> 
   <td> 
    <ul> 
     <li> <p>Autorizzazioni Contribute o superiori per l'oggetto per il quale si desidera modificare il modulo personalizzato</p> </li> 
     <li><p>Visualizzare le autorizzazioni per i campi che si desidera modificare.</p></li> 
     <li><p>Autorizzazioni di modifica per le sezioni del modulo in cui si trovano i campi da modificare</p></li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Team or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront licenses*</p> </td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to the object for which you want to edit the custom form</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> 
    <ul> 
     <li> <p>Contribute or higher permissions on the object for which you want to edit the custom form</p> </li> 
     <li>View permissions on the fields you want to edit. For information about sharing permissions for custom fields, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/share-custom-fields.md" class="MCXref xref">Configure sharing for custom fields and widgets</a>.</li> 
     <li> <p>Edit permissions for the sections on the form where the fields you want to edit are located</p> </li> 
    </ul> <p>For information on requesting additional access for objects, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Prerequisiti

* L’amministratore di Workfront o un utente con accesso amministrativo ai moduli personalizzati deve creare moduli personalizzati nel tuo ambiente. Per ulteriori informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* A un oggetto devono essere allegati moduli personalizzati.

  Per informazioni su come applicare moduli personalizzati a un oggetto, vedere [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Modificare le informazioni in un modulo personalizzato

La modifica delle informazioni in un modulo personalizzato associato a un oggetto è simile per la maggior parte degli oggetti.

Per informazioni sugli oggetti che possono avere un modulo personalizzato, vedere [Panoramica moduli personalizzati](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. Passare a qualsiasi elenco di oggetti per i quali si desidera modificare le informazioni nel modulo personalizzato, ad eccezione di un elenco di iterazioni.
1. Seleziona uno o più oggetti nell&#39;elenco, quindi fai clic sull&#39;icona **Modifica** ![Modifica](assets/edit-icon.png) nella parte superiore dell&#39;elenco.
1. Fai clic su **Forms personalizzato** nel pannello a sinistra, all&#39;interno della casella **Modifica &lt; oggetto >**.

   Se all&#39;oggetto è allegato un modulo personalizzato, il nome del modulo verrà visualizzato come area nella sezione **Forms** personalizzato.
1. Inizia a immettere informazioni in qualsiasi campo a cui hai accesso.

   ![Casella di modifica con moduli personalizzati nel record fatturazione](assets/edit-box-with-custom-forms-on-billing-record.png)

   Se all’oggetto sono allegati più moduli personalizzati, esegui questa operazione per ogni modulo.

   A seconda del tipo di campo in cui si sta lavorando, considerare quanto segue:

   * È possibile selezionare una sola opzione per i campi pulsante di opzione.
   * Puoi selezionare una o più opzioni in un campo casella di controllo, a seconda di come il creatore del modulo ha configurato il campo.
   * Puoi selezionare una o più opzioni in un campo a discesa a selezione multipla, a seconda di come il creatore del modulo ha configurato il campo.
   * È possibile formattare i campi di testo (grassetto, corsivo o sottolineato) solo se l&#39;utente che ha creato il modulo li ha impostati come campo di testo con tipo di campo Formattazione. Impossibile formattare i campi di testo a riga singola e i campi di testo a paragrafo.
   * È possibile aggiornare l&#39;ora del giorno in un tipo di campo Data solo se l&#39;utente che ha creato il modulo lo ha incluso durante la creazione del campo.

   >[!NOTE]
   >
   ><span class="preview">I campi che consentono selezioni multiple possono limitare il numero di opzioni selezionabili. Le caselle di controllo e gli elenchi a discesa a selezione multipla sono limitati a 5000 selezioni.</span>

   Per informazioni su tutti i tipi di campo, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Fai clic su **Salva**.

   >[!IMPORTANT]
   >
   >Per salvare il modulo è necessario compilare tutti i campi obbligatori del modulo. Il nome di un campo obbligatorio è seguito da un asterisco.
   >
   >![](assets/nwe-required-custom-field.png)

   Quando qualcuno modifica i dati in un altro oggetto a cui fanno riferimento i campi personalizzati calcolati nell&#39;oggetto, le modifiche non vengono applicate automaticamente nell&#39;oggetto. Per informazioni sull&#39;aggiornamento manuale di tutti i campi personalizzati calcolati nell&#39;oggetto, vedere [Ricalcolare tutti i campi personalizzati calcolati per un oggetto](#recalculate-all-calculated-custom-fields-for-an-object) in questo articolo.

   Quando i campi dipendenti della pagina vengono modificati, i campi calcolati del modulo personalizzato vengono ricalcolati in tempo reale in modo dinamico. È possibile visualizzare il nuovo valore del campo calcolato senza salvare il modulo, ma non viene effettivamente applicato al modulo e all&#39;oggetto fino a quando non si salvano le modifiche. Ciò si applica ai campi calcolati nei moduli predefiniti e nei moduli personalizzati.

   È inoltre possibile aggiornare manualmente tutti i campi personalizzati calcolati per un oggetto quando si modifica in blocco l&#39;oggetto insieme ad altri oggetti in un elenco. Per istruzioni, vedere [Ricalcolare tutti i campi personalizzati calcolati per più oggetti in un elenco durante la modifica degli oggetti](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) in questo articolo.

1. (Condizionale) Per aggiornare i campi personalizzati per un modulo personalizzato di iterazione, procedere come segue:

   1. Passare a un&#39;iterazione.
   1. Fai clic su **Forms personalizzato** nel pannello a sinistra.
   1. Per aggiungere moduli personalizzati, inizia a digitare il nome di un modulo nel campo **Aggiungi modulo personalizzato** nell&#39;angolo superiore destro della pagina

      Oppure

      Fai clic sull&#39;icona **Modifica** nella stessa area per iniziare a modificare i campi nei moduli allegati.

      ![Modifica modulo personalizzato iterazione](assets/edit-iteration-custom-form.png)

   1. Fai clic su **Salva modifiche**.

## Ricalcola campi personalizzati per oggetti

Periodicamente, a seconda delle modifiche che potrebbero verificarsi ai moduli personalizzati o delle modifiche che si verificano sui campi a cui si fa riferimento nei campi personalizzati, i valori dei campi personalizzati calcolati potrebbero non essere più aggiornati. In questo caso, potrebbe essere necessario ricalcolare i campi personalizzati o le espressioni personalizzate per gli oggetti.

Nelle sezioni seguenti viene descritto come ricalcolare le espressioni personalizzate per gli oggetti con moduli personalizzati.

>[!NOTE]
>
>Non è possibile ricalcolare espressioni personalizzate per i gruppi.

### Ricalcolare tutti i campi personalizzati calcolati dalla pagina di un oggetto

>[!IMPORTANT]
>
>Prima di poter seguire i passaggi descritti in questa sezione, è necessario disporre di un modulo personalizzato con campi calcolati associati all&#39;oggetto.

1. Passare alla pagina principale di uno dei seguenti oggetti di cui si desidera ricalcolare i campi personalizzati:

   * Progetto
   * Attività
   * Problema
   * Portfolio
   * Programma
   * Documento

1. Fai clic sul menu **Altro** ![](assets/more-icon.png) a destra del nome dell&#39;oggetto, quindi fai clic su **Ricalcola espressioni**.

   In questo modo vengono ricalcolati tutti i campi personalizzati nel modulo dell&#39;oggetto.

### Ricalcolare tutti i campi personalizzati calcolati per più oggetti in un elenco durante la modifica degli oggetti {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

A seconda degli oggetti per i quali si desidera ricalcolare le espressioni personalizzate, è possibile eseguire questa operazione nelle aree seguenti:

* In un elenco di oggetti, dal menu Altro nella parte superiore dell&#39;elenco.
* Nella casella Modifica, quando si selezionano e si modificano più oggetti in blocco.

Per ricalcolare manualmente i campi personalizzati di più oggetti modificandoli in blocco da un elenco o da un report:

1. Consente di passare a un elenco dei tipi di oggetto seguenti i cui oggetti contengono moduli personalizzati con campi calcolati:

   * Utenti
   * Aziende
   * Record fatturazione

1. Selezionare gli oggetti di cui si desidera aggiornare i campi personalizzati calcolati.
1. Fai clic sull&#39;icona **Modifica**.
1. Fai clic su **Forms personalizzato** nel menu a sinistra, quindi seleziona **Ricalcola espressioni personalizzate**.
1. Fai clic su **Salva** o **Salva modifiche**.

   Workfront calcola tutti i campi personalizzati per tutti gli oggetti selezionati.

Per ricalcolare espressioni personalizzate da un elenco di oggetti:

1. Passare a un elenco o a un report di progetti e selezionare uno o più dei seguenti tipi di oggetti:

   * Progetti
   * Attività
   * Problemi
   * Portfolio
   * Programmi
   * Spese
1. Fai clic sul menu **Altro** ![](assets/more-icon.png), quindi fai clic su **Ricalcola espressioni personalizzate**.

![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

Workfront calcola immediatamente tutti i campi personalizzati per tutti i progetti selezionati.
Non tutti gli elenchi di tutti gli oggetti dispongono di questa funzionalità.

>[!NOTE]
>
>Durante il ricalcolo delle espressioni per più progetti, a seconda della loro complessità, si consiglia di non selezionare un numero di progetti troppo grande per garantire prestazioni ottimali.
>
>Alcuni elementi che potrebbero rendere un progetto troppo complesso potrebbero essere più dipendenze o assegnazioni o un numero elevato di campi personalizzati.

