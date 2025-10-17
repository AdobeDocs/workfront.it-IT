---
title: Visualizzare e gestire i dettagli di un gruppo
description: È possibile visualizzare e modificare la pagina Dettagli gruppo per un gruppo o un sottogruppo gestito dall'utente.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 1%

---

# Visualizzare e gestire i dettagli di un gruppo

È possibile visualizzare e modificare la pagina Dettagli gruppo per un gruppo o un sottogruppo gestito dall&#39;utente. Questa pagina include:

* Descrizione del gruppo
* I nomi del Business Leader e degli amministratori di gruppi
* Opzione che consente di rendere il gruppo e i relativi sottogruppi pubblici o privati

Per informazioni su altre modalità di gestione di un gruppo, vedere [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Per informazioni su come disattivare o riattivare un gruppo, vedere [Disattivare o riattivare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Devi essere un amministratore di gruppo del gruppo o un amministratore di sistema.</td>
  </tr>
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare e gestire i dettagli di un gruppo

{{step-1-to-setup}}

1. Fai clic su **Gruppi**.

   Nell’elenco visualizzato puoi visualizzare i gruppi che gestisci, insieme a tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Fare clic sul nome del gruppo di primo livello da modificare.
1. Se si desidera disattivare o riattivare il gruppo,
1. Nel menu a sinistra, fare clic su **Dettagli gruppo**, quindi eseguire una delle operazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td> <p>È possibile digitare fino a 512 caratteri.</p> <p>Se il campo è vuoto, fare clic su <strong>Aggiungi</strong> per digitare una descrizione.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">È attivo</td> 
      <td> <p>(Abilitato per impostazione predefinita) Attiva il gruppo nell’istanza di Workfront.</p> <p>Nei campi di completamento automatico come quello mostrato di seguito, quando gli utenti normali cercano un gruppo per allegarlo a un oggetto o per condividerlo con esso, nell’elenco vengono visualizzati solo i gruppi attivi.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Per semplificare questa operazione per gli utenti, è possibile disattivare l'opzione È attivo per i gruppi attualmente non in uso.</p> <p>Questo campo consente di visualizzare, filtrare e raggruppare facilmente l’elenco Gruppi in base allo stato attivo o inattivo. Per informazioni sull'utilizzo di viste, filtri e raggruppamenti negli elenchi, vedere <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementi di reporting: filtri, viste e raggruppamenti</a>.</p> <p>Per informazioni sui gruppi inattivi, vedere la sezione <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">Considerazioni sui gruppi inattivi</a> nell'articolo <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">Eliminare o disattivare un modulo personalizzato</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accessibilità gruppo</td> 
      <td> <p>(Disponibile solo se si visualizzano i dettagli di un gruppo e non di un sottogruppo). Abilita o disabilita l'opzione <strong>Rendi privato il gruppo e i sottogruppi</strong>.</p> <p>Per un gruppo pubblico, qualsiasi utente (interno o esterno al gruppo) con accesso di modifica utente può aggiungere il gruppo al profilo di altri utenti. Non possono farlo per un gruppo privato.</p> <p>È possibile modificare questa opzione solo sul gruppo padre superiore in una gerarchia di gruppi con più livelli. Tutti i sottogruppi del gruppo padre ereditano l'impostazione.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Parti interessate gruppo</td> 
      <td> 
       <ul> 
        <li><strong>Amministratori di gruppi</strong>: aggiungi o rimuovi utenti con una licenza Planner come amministratori di gruppi per il gruppo. Inizia a digitare il nome di un utente, quindi fai clic sul nome quando viene visualizzato nel menu a discesa.</li> 
        <li><strong>Business Leader</strong>: eseguire una delle operazioni seguenti:
         <ul>
          <li>Se non hai ancora assegnato un Business Leader al gruppo, fai clic su <strong>Aggiungi</strong>, inizia a digitare il nome dell'utente che desideri assegnare, quindi fai clic sul nome della persona quando viene visualizzato.</li>
          <li>Se il gruppo dispone già di un Business Leader e si desidera modificarlo, fare doppio clic sul nome del Business Leader esistente. Elimina il nome, inizia a digitare il nome dell'utente che desideri assegnare, quindi fai clic sul nome della persona quando viene visualizzato.</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aggiungi modulo personalizzato</td> 
      <td>Se il tuo livello di accesso ti consente di gestire i moduli personalizzati, aggiungi un modulo personalizzato al gruppo. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Moduli personalizzati</a>.</td> 
     </tr> 
    </tbody> 
   </table>
