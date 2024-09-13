---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Eliminare i piani nella Pianificazione scenario
description: È possibile eliminare i piani creati. Non è possibile eliminare i piani condivisi con l'utente.
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# Elimina piani in [!DNL Scenario Planner]

È possibile eliminare i piani creati. Non è possibile eliminare i piani condivisi con l&#39;utente.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] piano*</p> </td> 
   <td> <ul></li>
   <li><p>Nuovo: Ultimate </p></li>
   <p>Pianificazione scenario non disponibile per i nuovi piani Workfront Select o Workfront Prime. </p>
   <li><p>Corrente: [!UICONTROL Business] o versione successiva</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licenza*</p> </td> 
   <td> <p>Nuovo: Chiaro o superiore</p> 
   <p>Corrente: [!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td>Prodotto* </td> 
   <td> <ul><li><p>Per i nuovi piani Workfront:</p><p> Adobe Workfront</li></p>
   <li><p>Per i piani Workfront correnti: </p>
   <p>Adobe Workfront</p> <p>Pianificazione scenario Adobe Workfront</p></li></ul>

<p>Per ulteriori informazioni, vedere <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Livello di accesso </td> 
   <td> <p>Accesso di [!UICONTROL Edit] al [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorizzazioni oggetto </p> </td> 
   <td> <p>Autorizzazioni [!UICONTROL Manage] per un piano</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedere <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Richiedere accesso a un piano in [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso alla documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
>* Vengono eliminate anche tutte le informazioni relative al piano. Sono inclusi tutti gli scenari e le iniziative associati al piano, incluse informazioni su mansioni e costi. Queste informazioni non possono essere recuperate.
>* Se il piano contiene uno scenario pubblicato, i progetti collegati alle iniziative eliminate vengono mantenuti e l&#39;area [!DNL Scenario Planner] rimane nella sezione [!UICONTROL Dettagli progetto].
>
>  Per informazioni sulla pubblicazione di iniziative nei progetti, vedere [Aggiornare o creare progetti pubblicando iniziative in [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Per eliminare un piano:

{{step1-to-scenario-planner}}

Viene visualizzato un elenco di piani.

1. Fare clic sul nome di un piano per aprirlo.
1. Fai clic sul **[!UICONTROL menu Altro]** ![](assets/more-menu.png) a destra del nome del piano, quindi fai clic su **[!UICONTROL Elimina]** > **[!UICONTROL Sì, elimina]**.

   Il piano viene eliminato e si torna all&#39;elenco dei piani.

### Elimina scenari {#delete-scenarios}

>[!IMPORTANT]
>
>Quando elimini uno scenario, considera quanto segue:
>
>* Se si elimina uno scenario, vengono eliminate anche tutte le iniziative e le relative informazioni. Se vengono copiate in altri scenari, le iniziative rimangono sugli altri scenari.
>* Quando si elimina uno scenario, lo scenario successivo assume il numero dello scenario eliminato e l&#39;ordine di conteggio viene mantenuto. Ad esempio, se si elimina lo scenario 4, lo scenario 5 diventa lo scenario 4.
>* Se vengono pubblicate alcune iniziative sullo scenario, il progetto collegato all’iniziativa viene mantenuto e l’area Pianificazione scenario rimane sui progetti collegati
>* Se le iniziative pubblicate esistono in un altro scenario, rimangono in quello scenario, incluso il loro collegamento al progetto. La pubblicazione di tali iniziative da altri scenari aggiorna i progetti collegati con nuove informazioni da tali scenari.
>
>  Per informazioni sulla pubblicazione di iniziative nei progetti, vedere [Aggiornare o creare progetti pubblicando iniziative in [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Per eliminare uno scenario:

1. Passare al piano per il quale si desidera eliminare uno scenario.

   Per impostazione predefinita, viene visualizzato lo scenario Iniziale.

1. Fai clic su **[!UICONTROL Confronta scenari]**.
1. Nell&#39;angolo superiore destro della scheda dello scenario, fai clic sul menu **[!UICONTROL Altro]** ![](assets/more-menu.png), quindi fai clic su **[!UICONTROL Elimina]**.

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


