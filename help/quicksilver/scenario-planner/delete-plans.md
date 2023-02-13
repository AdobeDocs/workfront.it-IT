---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Eliminare i piani nel planner dello scenario
description: È possibile eliminare i piani creati. Non è possibile eliminare i piani condivisi con te.
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---

# Elimina i piani nel [!DNL Scenario Planner]

È possibile eliminare i piani creati. Non è possibile eliminare i piani condivisi con te.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> piano*</b> </p> </td> 
   <td>[!UICONTROL Business] o superiore</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licenza*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td><b>Prodotto</b> </td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alla funzionalità descritta in questo articolo.</p> <p>Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedi <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurazioni a livello di accesso*</strong> </td> 
   <td> <p>Accesso o superiore a [!DNL Scenario Planner]</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Autorizzazioni di gestione per un piano</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedi <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Richiedi l'accesso a un piano nel [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Elimina piani

>[!IMPORTANT]
>
>Non è possibile recuperare i piani eliminati.

È possibile eliminare un piano oppure uno scenario in un piano.

* [Elimina piani](#delete-plans)
* [Elimina scenari](#delete-scenarios)

### Elimina piani

>[!IMPORTANT]
>
>Quando si eliminano i piani, tenere presente quanto segue:
>
>* Vengono inoltre eliminate tutte le informazioni relative al piano. Ciò include tutti gli scenari e le iniziative associati al piano, comprese le informazioni sui ruoli e i costi del lavoro. Queste informazioni non possono essere recuperate.
>* Se il piano contiene uno scenario pubblicato, i progetti collegati alle iniziative eliminate vengono mantenuti e la [!DNL Scenario Planner] la zona rimane [!UICONTROL Dettagli progetto] sezione .
>
>  Per informazioni sulla pubblicazione di iniziative in progetti, consulta [Aggiornare o creare progetti pubblicando iniziative nel [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Per eliminare un piano:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png), quindi fai clic su [!UICONTROL Scenari].

   Viene visualizzato un elenco di piani.

1. Fare clic sul nome di un piano per aprirlo.
1. Fai clic sul pulsante **[!UICONTROL Menu Altro]** ![](assets/more-menu.png) a destra del nome del piano, quindi fare clic su **[!UICONTROL Elimina]** > **[!UICONTROL Sì, eliminalo]**.

   Il piano viene eliminato e si torna all&#39;elenco dei piani.

### Elimina scenari {#delete-scenarios}

>[!IMPORTANT]
>
>Quando si elimina uno scenario, tenere presente quanto segue:
>
>* L’eliminazione di uno scenario comporta l’eliminazione di tutte le iniziative e delle relative informazioni dallo scenario. Se vengono copiati in altri scenari, le iniziative rimangono sugli altri scenari.
>* Quando si elimina uno scenario, lo scenario successivo assume il numero dello scenario eliminato e l&#39;ordine di conteggio viene mantenuto. Ad esempio, se elimini lo Scenario 4, lo Scenario 5 diventa lo Scenario 4.
>* Se vengono pubblicate alcune iniziative sullo scenario, il progetto collegato all&#39;iniziativa viene mantenuto e l&#39;area Planner scenario rimane sui progetti collegati
>* Se le iniziative pubblicate esistono in un altro scenario, rimangono su tale scenario, compreso il loro collegamento al progetto. La pubblicazione di tali iniziative dagli altri scenari aggiorna i progetti collegati con nuove informazioni provenienti da tali scenari.
>
>  Per informazioni sulla pubblicazione di iniziative in progetti, consulta [Aggiornare o creare progetti pubblicando iniziative nel [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Per eliminare uno scenario:

1. Passare al piano per il quale si desidera eliminare uno scenario.

   Per impostazione predefinita, viene visualizzato lo scenario Iniziale .

1. Fai clic su **[!UICONTROL Confronto degli scenari]**.
1. Nell’angolo in alto a destra della scheda dello scenario, fai clic su **[!UICONTROL Altro]** menu ![](assets/more-menu.png), quindi fai clic su **[!UICONTROL Elimina]**.

   Lo scenario viene eliminato.

1. Fai clic su **[!UICONTROL Salva piano]** per salvare le modifiche.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete initiatives</h2>
<p>(NOTE: moved this section to its own article about deleting initiatives) </p> <note type="important">
<p>Consider the following when deleting initiatives:</p>
<ul>
<li>Deleting an initiative deletes the job roles and cost information from the initiative.</li>
<li><span>When you delete an initiative that is published to a project, the initiative is removed from the scenario but the Scenario Planner area remains in the Project Details section.</span> </li>
<li> <p>If the initiative you delete is the only published initiative on the scenario, the indicator that the plan has been published is also removed. </p> <p>For information about publishing initiatives to projects, see <a href="../scenario-planner/publish-scenarios-update-projects.md" class="MCXref xref">Update or create projects by publishing initiatives in the Scenario Planner</a>.</p> </li>
</ul>
</note>
<p>To delete an initiative:</p>
<ol>
<li value="1"> <p> <p>Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png">, then click Scenarios.</p> </p> <p>A list of plans displays. </p> </li>
<li value="2">Click the name of a plan to open it, then locate the initiative you want to delete.</li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/more-menu.png"> to the right of the initiative name, then click <strong>Delete</strong> > <strong>Yes, delete it</strong>. </p> <p>The initiative is deleted. </p> </li>
<li value="4">Click <strong>Save Plan</strong> to save your changes. </li>
</ol>
</div>
-->


