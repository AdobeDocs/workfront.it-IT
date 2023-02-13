---
title: Personalizzare le intestazioni degli oggetti utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In qualità di amministratore di Adobe Workfront o di amministratore di gruppo , è possibile utilizzare un modello di layout per configurare i campi visualizzati dall’utente nell’intestazione dell’oggetto all’apertura della pagina di un oggetto.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: a1ffec0d8a50ff7f025ff23370afa746cf0d6d3f
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Personalizzare le intestazioni degli oggetti utilizzando un modello di layout

In qualità di amministratore di Adobe Workfront o di amministratore di gruppo, è possibile utilizzare un modello di layout per configurare i campi visualizzati dall’utente nell’intestazione dell’oggetto all’apertura della pagina di un oggetto.

>[!IMPORTANT]
>
>La personalizzazione delle intestazioni degli oggetti è attualmente disponibile per progetti, attività e problemi.


Per informazioni sui modelli di layout per gruppi, consulta [Creare e modificare i modelli di layout di un gruppo](../../manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

![](assets/object-header-fields.png)

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:


<table>
  <tr>
   <td><strong>piano Adobe Workfront</strong>
   </td>
   <td>Qualsiasi
   </td>
  </tr>
  <tr>
   <td><strong>Licenza Adobe Workfront</strong>
   </td>
   <td>Piano
   </td>
  </tr>
  <tr>
   <td><strong>Configurazioni a livello di accesso</strong>
   </td>
   <td>Devi essere un amministratore di Workfront o di gruppo.
<p>
   </td>
  </tr>
</table>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta [Creare o modificare livelli di accesso personalizzati](../../add-users/configure-and-grant-access/create-modify-access-levels.md).

## Personalizzare le intestazioni degli oggetti

1. Inizia a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. In **Personalizzare ciò che gli utenti visualizzano** menu a discesa, seleziona **Progetti**, **Attività** o **Problemi**.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. In [!UICONTROL Campi di intestazione] passare il mouse sui campi visualizzati ed effettuare una delle seguenti operazioni:
   * Fai clic sul pulsante **x** icona per rimuovere un campo

      Oppure

   * Fai clic e tieni premuto il pulsante **afferrare** per trascinare il campo in una nuova posizione.

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. Nell’intestazione di un oggetto possono essere presenti fino a cinque campi.
Se sono già stati selezionati cinque campi, è necessario rimuovere un campo prima di poterne aggiungere uno nuovo.
1. In **Aggiungi campo** iniziare a digitare il nome di un campo Workfront non modificabile che si desidera aggiungere, quindi selezionarlo quando viene visualizzato nell’elenco. Il campo viene aggiunto all’immediata destra della casella Aggiungi campo e viene visualizzato come primo campo nell’angolo superiore sinistro dell’intestazione dell’oggetto.

   >[!TIP]
   >
   >* È possibile aggiungere solo campi che vengono visualizzati nell’area Panoramica della sezione Dettagli dell’oggetto e che non sono modificabili. I campi non modificabili sono campi che gli utenti non possono modificare manualmente. Vengono calcolati automaticamente da Workfront.
   >
   >* È possibile aggiungere campi modificabili che fanno già parte delle intestazioni predefinite (ad esempio, Proprietario progetto, Stato, Percentuale completamento, Assegnazioni).
   >
   >* Quando aggiungi il campo &quot;Risolto da&quot; all&#39;intestazione di un problema, il campo diventa &quot;Risoluzione del problema, attività o progetto&quot;, quando è presente un oggetto di risoluzione associato al problema.



   ![](assets/add-field-to-header-in-lt-list.png)


1. (Facoltativo) Trascina e rilascia i campi aggiunti in un ordine diverso.

1. Continua a personalizzare il modello di layout.

   Oppure

   Al termine della personalizzazione, fai clic su **Salva**.

   >[!TIP]
   >
   >Puoi fare clic su Salva in qualsiasi momento per salvare l&#39;avanzamento, quindi continuare a modificare il modello in un secondo momento.
