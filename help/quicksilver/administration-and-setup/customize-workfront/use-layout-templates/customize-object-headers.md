---
title: Personalizzare le intestazioni degli oggetti utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In qualità di amministratore di Adobe Workfront o di amministratore di gruppo, puoi utilizzare un modello di layout per configurare i campi che gli utenti visualizzano nell’intestazione dell’oggetto quando aprono la pagina di un oggetto.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: 9507e04be7cdd33658b4958f3030b0d3359a9ef1
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 3%

---

# Personalizzare le intestazioni degli oggetti utilizzando un modello di layout

{{preview-fast-release-general}}

In qualità di amministratore di Adobe Workfront o di amministratore di gruppo, puoi utilizzare un modello di layout per configurare i campi che gli utenti visualizzano nell’intestazione dell’oggetto quando aprono la pagina di un oggetto.

>[!IMPORTANT]
>
>La personalizzazione delle intestazioni degli oggetti è attualmente disponibile per progetti, attività e problemi.

![Campi intestazione oggetto](assets/object-header-fields.png)

Per informazioni sulla creazione di modelli di layout, vedere [Creare e gestire modelli di layout](../use-layout-templates/create-and-manage-layout-templates.md).

Per informazioni sui modelli di layout per i gruppi, vedere [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Dopo aver configurato un modello di layout, è necessario assegnarlo agli utenti affinché le modifiche apportate siano visibili agli altri utenti. Per informazioni sull&#39;assegnazione di un modello di layout agli utenti, vedere [Assegnare gli utenti a un modello di layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.</p>
        <p>Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizzare le intestazioni degli oggetti

1. Iniziare a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Nel menu a discesa **Personalizza gli utenti**, seleziona **Progetti**, **Attività** o **Problemi**.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. Nella sezione [!UICONTROL Campi intestazione], passa il puntatore del mouse sui campi correnti ed effettua una delle seguenti operazioni:
   * Fai clic sull&#39;icona **x** per rimuovere un campo

     Oppure

   * Fai clic sull&#39;icona **grab** e tieni premuto per trascinare il campo in una nuova posizione.

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![I campi intestazione oggetto nascondono e spostano le icone](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. È possibile avere fino a cinque campi nell&#39;intestazione di un oggetto.
Se sono già stati selezionati cinque campi, è necessario rimuovere un campo prima di poterne aggiungere uno nuovo.
1. Nella casella **Aggiungi campo** digitare il nome di un campo personalizzato o di un campo Workfront nativo che si desidera aggiungere, quindi selezionarlo quando viene visualizzato nell&#39;elenco. Il campo viene aggiunto a destra della casella Aggiungi campo e verrà visualizzato come primo campo nell&#39;angolo superiore destro dell&#39;intestazione dell&#39;oggetto.

   >[!TIP]
   >
   >* È possibile aggiungere qualsiasi campo personalizzato o qualsiasi campo nativo disponibile nell&#39;area Panoramica della sezione Dettagli di un oggetto. Ad esempio, solo i problemi hanno il campo Severity (Gravità) e tale campo non è disponibile per l’aggiunta a progetti o attività.
   >
   >* Quando aggiungi il campo &quot;Risolto da&quot; all’intestazione di un problema, il campo diventa &quot;Risolto da un problema, un’attività o un progetto&quot;, quando al problema è associato un oggetto di risoluzione.

   ![Aggiungi campo all&#39;intestazione](assets/add-field-to-header-in-lt-list.png)

1. (Facoltativo) Trascina i campi in un ordine diverso.

1. <span class="preview">Nell&#39;ambiente di anteprima: continuare a personalizzare il modello di layout. Puoi fare clic su **Applica** in qualsiasi momento per salvare i tuoi progressi.</span>

   <span class="preview">O</span>

   <span class="preview">Se hai completato la personalizzazione, fai clic su **Salva e chiudi**.</span>

1. Nell’ambiente di produzione: continua a personalizzare il modello di layout.

   Oppure

   Se hai completato la personalizzazione, fai clic su **Salva**.

   >[!TIP]
   >
   >Puoi fare clic su **Salva** in qualsiasi momento per salvare l&#39;avanzamento, quindi continuare a modificare il modello in un secondo momento.
