---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Messaggio di errore: C'è un piccolo problema. Tale campo viene utilizzato in una configurazione a più moduli"
description: Quando si modifica un calcolo in un campo personalizzato calcolato su un modulo personalizzato e viene visualizzato un messaggio di errore che indica che il campo è utilizzato in una configurazione a più moduli, è necessario sostituire il campo con un nuovo campo contenente il calcolo che si desidera utilizzare.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 0%

---

# Messaggio di errore: C&#39;è un piccolo problema. Tale campo viene utilizzato in una configurazione a più moduli

## Problema

Quando si modifica un calcolo in un campo personalizzato calcolato in un modulo personalizzato, [!DNL Adobe Workfront] potrebbe essere visualizzato il seguente avviso:

Si è verificato un piccolo problema

[Il campo] viene utilizzato in una configurazione a più moduli; se desideri modificare questa formula, devi rimuovere questo campo e sostituirlo con uno nuovo contenente il calcolo desiderato.

## Causa

Almeno due moduli personalizzati contenenti il campo personalizzato calcolato che si sta tentando di modificare sono collegati a un singolo oggetto nel [!DNL Workfront] istanza.

**Esempio:** I moduli A e B personalizzati sono entrambi associati alla stessa attività. Entrambi i moduli contengono un campo personalizzato calcolato denominato Profitto. L&#39;errore si verifica quando si tenta di modificare il calcolo nel campo Profitto del modulo personalizzato A.

Non è possibile modificare il calcolo per il campo personalizzato in uno dei moduli perché ciò sarebbe in conflitto con la formula nello stesso campo nell’altro modulo.
Per risolvere questo conflitto, è necessario trovare l’oggetto a cui sono collegati i più moduli con lo stesso campo personalizzato calcolato, quindi eseguire una delle operazioni seguenti:

* Rimuovere uno dei moduli dall’oggetto.
* Modificare il calcolo in base alle esigenze, ma farlo in tutti i moduli personalizzati associati all’oggetto.
* In tutti i moduli personalizzati associati all’oggetto, aggiungere un nuovo campo personalizzato calcolato contenente il calcolo necessario e contrassegnare il vecchio campo personalizzato calcolato come obsoleto.

Questo articolo spiega come trovare l&#39;oggetto e quindi risolvere il problema in uno di questi tre modi.

## Trova l’oggetto a cui sono allegati i moduli personalizzati {#find-the-object-where-the-custom-forms-are-attached}

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Utenti]** ![](assets/users-icon-in-main-menu.png).

1. Fai clic su **[!UICONTROL Forms personalizzato]** > **[!UICONTROL Campi]**.
1. Applica la **[!UICONTROL Elenco campi]** visualizzare per trovare il campo calcolato che si sta tentando di modificare e prendere nota di ogni modulo personalizzato in cui viene utilizzato (ad esempio modulo 1, modulo 2, modulo 3).
1. Fai clic su **[!UICONTROL Forms]**, quindi applica il **[!UICONTROL Elenco moduli]** visualizza.
1. Fai clic sul pulsante **[!UICONTROL Filtro]** elenco a discesa, quindi **[!UICONTROL Nuovo filtro]**.

1. Fai clic su **[!UICONTROL Aggiungere una regola filtro]**, quindi inizia a digitare &quot;nome modulo personalizzato&quot; e seleziona questo valore quando viene visualizzato nell’elenco.
1. Seleziona **[!UICONTROL Uguale]** per il modificatore di filtro, inizia a digitare il nome di ciascun modulo di cui hai effettuato una nota nel passaggio 1, quindi selezionalo quando viene visualizzato.

   **Esempio:** Il Nome Del Modulo Personalizzato È Uguale Al Modulo 1, Modulo 2, Modulo 3.

1. Fai clic su **[!UICONTROL Salva filtro]**, quindi denomina il nuovo filtro e fai clic su **[!UICONTROL Salva filtro]**.

1. Nell’elenco dei moduli, prendere nota del tipo di oggetto del filtro, ad esempio Attività o Problema, visualizzato nella **[!UICONTROL Tipo]** colonna.
1. Per ogni modulo personalizzato trovato nel passaggio 1, creare un nuovo campo personalizzato Casella di selezione con un singolo valore predefinito di Sì.

   **Esempio:** Campo 1 nel modulo 1 = Sì, Campo 2 nel modulo 2 = Sì, Campo 3 nel modulo 3 = Sì. Ciò significa che il campo personalizzato calcolato esiste nel modulo 1 oppure il campo personalizzato calcolato esiste nel modulo 2 e così via.

1. In **[!UICONTROL Icona Ricerca]** ![](assets/search-icon.png) nell’angolo superiore destro dello schermo, fai clic su **[!UICONTROL Ricerca avanzata]**.
1. Fai clic sull’oggetto del modulo personalizzato (ad esempio Problema), quindi fai clic su **[!UICONTROL Filtrare i risultati]**, quindi fai clic su **[!UICONTROL Aggiungere un filtro]**.
1. Inizia a digitare il nome di un campo Casella di selezione nel **[!UICONTROL Inizia a digitare il nome del campo]** e selezionalo quando viene visualizzato nell’elenco, quindi seleziona **[!UICONTROL Uguale]** e tipo **[!UICONTROL Sì]** (senza virgolette) nella casella seguente.

   **Esempio:** Campo 1 Uguale a (distinzione maiuscole/minuscole) Sì.

1. Fai clic su **[!UICONTROL Aggiungere un filtro]** e aggiungi tutti i campi casella di controllo alla ricerca avanzata.

   Cerca ogni possibile combinazione.

   **Esempio:** Crea diversi filtri con le combinazioni trovate, come elencato di seguito. È necessario trovare oggetti con più moduli personalizzati allegati che contengono gli stessi campi calcolati. È possibile trovare i seguenti scenari:

   * Campo 1= Sì + Campo 2 = Sì + Campo 3 = Sì (nessun oggetto, ad esempio)
   * Campo 1= Sì + Campo 2 = Sì (nessun oggetto, ad esempio)
   * Campo 1= Sì + Campo 3 = Sì (ad esempio, due oggetti)

   Ciò significa che il campo calcolato esiste sia nel modulo 1 che nel modulo 3, in quanto su questi oggetti esistono i campi corrispondenti della casella di controllo (campo 1 e campo 3).

   Campo 2 = Sì + Campo 3 = Sì (nessun oggetto, ad esempio)

1. Procedi a una delle seguenti sezioni del presente articolo:

   * [Rimuovi uno dei moduli personalizzati dall’oggetto e modifica il calcolo in tale area](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [Apportare modifiche identiche nel calcolo in tutti i moduli personalizzati allegati](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [Aggiungere un nuovo campo calcolato contenente il calcolo modificato a uno o tutti i moduli personalizzati allegati](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## Rimuovi uno dei moduli personalizzati dall’oggetto e modifica il calcolo in tale area {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. Trova l’oggetto a cui sono allegati i moduli personalizzati, come spiegato in [Trova l’oggetto a cui sono allegati i moduli personalizzati](#find-the-object-where-the-custom-forms-are-attached) in questo articolo, quindi apri l’oggetto .
1. Rimuovere uno dei moduli personalizzati dall’oggetto, quindi salvare l’oggetto.

   >[!NOTE]
   >
   >Per aggiungere i campi dal modulo rimosso dall’oggetto, potrebbe essere necessario modificare il modulo personalizzato che rimane allegato all’oggetto. In questo modo è possibile conservare le informazioni sui dati personalizzati dell’oggetto.

1. Nel modulo personalizzato rimosso, modificare il calcolo per il campo personalizzato che si stava tentando di aggiornare originariamente, quindi fare clic su **[!UICONTROL Salva]**.

   Questa volta, [!DNL Workfront] Non deve trovarsi in un conflitto.

1. (Facoltativo) Rimuovere i campi casella di controllo dai moduli personalizzati o eliminarli [!DNL Workfront].

## Apportare modifiche identiche nel calcolo in tutti i moduli personalizzati allegati {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>I dati vengono persi negli oggetti in cui il modulo personalizzato è già allegato quando si seguono questi passaggi. Tuttavia, se il campo calcolato fa riferimento a campi statici e non a campi calcolati, è possibile utilizzare [!UICONTROL Ricalcola espressioni personalizzate] opzione sull&#39;oggetto per ripristinare i dati persi

1. Trova l’oggetto a cui sono allegati i moduli personalizzati, come spiegato in [Trova l’oggetto a cui sono allegati i moduli personalizzati](#find-the-object-where-the-custom-forms-are-attached) in questo articolo.
1. Rimuovere il campo da tutti i moduli personalizzati associati all’oggetto, quindi salvare i moduli.

1. Aggiungi nuovamente ai moduli personalizzati il campo personalizzato contenente il nuovo calcolo.

   >[!IMPORTANT]
   >
   >I calcoli devono essere identici in tutti i moduli personalizzati allegati.

1. (Facoltativo) Rimuovere i campi casella di controllo dai moduli o eliminarli [!DNL Workfront].

## Aggiungere un nuovo campo calcolato contenente il calcolo modificato a uno o tutti i moduli personalizzati allegati {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

Per evitare di perdere dati nel campo personalizzato calcolato esistente o se è necessario eseguire il calcolo modificato solo in uno dei moduli personalizzati associati all’oggetto trovato:

1. Trova l’oggetto a cui sono allegati i moduli personalizzati, come spiegato in [Trova l’oggetto a cui sono allegati i moduli personalizzati](#find-the-object-where-the-custom-forms-are-attached) in questo articolo.
1. Aggiungere un nuovo campo personalizzato calcolato contenente il calcolo necessario a uno o tutti i moduli.
1. Rinomina il vecchio campo personalizzato calcolato **Obsoleto**.

   In tutti i moduli associati all’oggetto, questo modulo personalizzato calcolato in precedenza conserva i dati storici associati, ma l’utente smette di utilizzarlo.

   >[!IMPORTANT]
   >
   >È possibile fare riferimento al campo precedente in altri campi personalizzati calcolati, pertanto è necessario aggiornare i calcoli dopo aver modificato il nome.

1. (Facoltativo) Rimuovere i campi Casella di controllo dai moduli o eliminarli da Workfront.

<!--
<blockquote data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Problem</h2>
<p>You get the following error while editing a calculated Custom Field on a custom form: </p>
<p><em>"<Name of custom field> field is used in a multi-form configuration, if you would like to change this formula you will need to remove this field and replace it with a new one containing the desired calculation."</em> </p>
<h2>Cause</h2>
<p>The error occurs because the following setup exists: currently you have at least one object in your system that has multiple custom forms attached. The calculated field you are editing exists on multiple forms attached to these objects.</p>
<p>You cannot have the same calculated field with different calculations on the same object. For this reason, the system does not allow you to make a change which will result in calculations being different.</p>
<p><a href="../../Resources/Images/Admin and setup/Tips, Tricks, and Troubleshooting/Calculated_field_error.png" class="MCXref xref" xrefformat="{para}"><img src="assets/calculated-field-error.png" alt="" width="542" height="272"></a> </p>
<p>For example, you have a task with custom forms A and B attached to it. Both forms contain the same calculated field, Field 1. You encounter this error when you try to edit the calculation for Field 1 on custom form A. </p>
<h2>Solution</h2>
<p>Remove the field from the custom form and replace it with a new one containing the desired calculation.  </p>
<p>To understand what custom forms are attached to objects, you can build a report for those objects and reference the Category Name field in the view of the report.<br>For more information about referencing custom forms in reports, see the "Referencing Custom Forms in a Report View (Column)" section in <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/reference-custom-form-report.md" class="MCXref xref" xrefformat="{para}">Reference a custom form in a report</a>.</p>
<p>To understand what custom form contains a Custom Field, see the "Accessing Custom Forms and Fields" section in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md" class="MCXref xref" xrefformat="{para}">Custom forms overview</a>.</p>
<p>For more information about creating a custom form and adding or removing fields from it, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Create or edit a custom form</a>.</p>
</blockquote>
-->
