---
title: Visualizzare e gestire i dettagli di un gruppo
description: È possibile visualizzare e modificare la pagina Dettagli gruppo per un gruppo o sottogruppo gestito.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 1%

---

# Visualizzare e gestire i dettagli di un gruppo

È possibile visualizzare e modificare la pagina Dettagli gruppo per un gruppo o sottogruppo gestito. Questa pagina include:

* Descrizione del gruppo
* I nomi del Business Leader e degli amministratori del gruppo
* Opzione che consente di rendere pubblico o privato il gruppo e i relativi sottogruppi

   <!--
  <li>An option that allows you to deactivate or reactivate a group and its subgroups.
  DRAFTED IN FLARE:
  Make this change when Callisto adds the
  <b>Is active</b>
   option to the Details pag
  </li>
  -->

Per informazioni su altri modi per gestire un gruppo, vedi [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Per informazioni su come disattivare o riattivare un gruppo, consulta [Disattivare o riattivare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

<!--
DRAFTED IN FLARE:
Delete this paragraph when Callisto adds the
<b>Is active</b>
 option to the Details pag
-->

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>È necessario essere un amministratore del gruppo o un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Visualizzare e gestire i dettagli di un gruppo

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Gruppi**.

   Nell’elenco visualizzato, puoi vedere i gruppi gestiti e tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Fai clic sul nome del gruppo di livello principale da modificare.
1. Per disattivare o riattivare il gruppo,
1. Nel menu a sinistra, fai clic su **Dettagli gruppo**, quindi effettua una delle seguenti operazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td> <p>È possibile digitare fino a 512 caratteri.</p> <p>Se il campo è vuoto, fai clic su <strong>Aggiungi</strong> per digitare una descrizione.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">È attivo</td> 
      <td> <p>(Abilitato per impostazione predefinita) Rende il gruppo attivo nell’istanza di Workfront.</p> <p>Nei campi di tipo avanti come quello mostrato di seguito, quando gli utenti normali cercano un gruppo per allegarlo a un oggetto o per condividerlo con esso, nell’elenco vengono visualizzati solo i gruppi attivi.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Per semplificare questo processo per gli utenti, puoi disattivare l’opzione È attivo per i gruppi attualmente non in uso.</p> <p>Questo campo consente di visualizzare, filtrare e raggruppare facilmente l’elenco Gruppi in base allo stato attivo o inattivo. Per informazioni sull’utilizzo di viste, filtri e raggruppamenti negli elenchi, consulta <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementi di reporting: filtri, visualizzazioni e raggruppamenti</a>.</p> <p>Per informazioni sui gruppi inattivi, consulta la sezione . <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">Considerazioni per i gruppi inattivi</a> nell'articolo <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">Eliminare o disattivare un modulo personalizzato</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accessibilità gruppo</td> 
      <td> <p>(Disponibile solo se visualizzi i Dettagli per un gruppo, non per un sottogruppo). Abilita o disabilita l’opzione <strong>Rendi privato questo gruppo e i sottogruppi</strong>.</p> <p>Per un gruppo pubblico, qualsiasi utente (all'interno o all'esterno del gruppo) con accesso per l'utente con modifica può aggiungere il gruppo al profilo di altri utenti. Non possono farlo per un gruppo privato.</p> <p>È possibile modificare questa opzione solo nel gruppo principale superiore in una gerarchia di gruppi con più di un livello. Tutti i sottogruppi del gruppo padre ereditano le relative impostazioni.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Parti interessate gruppo</td> 
      <td> 
       <ul> 
        <li><strong>Amministratori di gruppo</strong>: Aggiungi o rimuovi utenti con una licenza Planner come amministratori di gruppo per il gruppo. Inizia a digitare il nome di un utente, quindi fai clic sul nome quando viene visualizzato nel menu a discesa.</li> 
        <li><strong>Leader di business</strong>: Effettua una delle seguenti operazioni:
         <ul>
          <li>Se non hai ancora assegnato un Business Leader per il gruppo, fai clic su <strong>Aggiungi</strong>, inizia a digitare il nome dell’utente che desideri assegnare, quindi fai clic sul nome della persona quando viene visualizzato.</li>
          <li>Se il gruppo dispone già di un Business Leader e si desidera modificarlo, fare doppio clic sul nome del Business Leader esistente. Elimina il nome, inizia a digitare il nome dell'utente che desideri assegnare, quindi fai clic sul nome della persona quando viene visualizzato.</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aggiungi modulo personalizzato</td> 
      <td>Se il livello di accesso consente di gestire moduli personalizzati, aggiungere al gruppo un modulo personalizzato. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Moduli personalizzati</a>.</td> 
     </tr> 
    </tbody> 
   </table>
