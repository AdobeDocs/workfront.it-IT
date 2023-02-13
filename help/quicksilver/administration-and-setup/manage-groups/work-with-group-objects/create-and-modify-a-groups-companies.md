---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Creare e modificare le aziende di un gruppo
description: Quando visualizzi un gruppo gestito nell’area Gruppi, puoi visualizzare e lavorare con le aziende associate al gruppo e a uno qualsiasi dei relativi sottogruppi.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# Creare e modificare le aziende di un gruppo

Quando visualizzi un gruppo gestito nell’area Gruppi, puoi visualizzare e lavorare con le aziende associate al gruppo e a uno qualsiasi dei relativi sottogruppi.

Se ci sono gruppi al di sopra del gruppo, i loro amministratori possono fare queste cose anche per il tuo gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

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
   <td> <p>Piano </p> <p>È necessario essere un amministratore del gruppo o un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Amministratori di gruppo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Visualizza, lavora con e crea aziende per il gruppo dall&#39;area Gruppi

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Fai clic sul nome del gruppo per il quale desideri creare o modificare le aziende.
1. Nel pannello a sinistra, fai clic su **Aziende** per elencare le società associate al gruppo ed eventuali sottogruppi.
1. (Facoltativo) Per aggiungere una società, fai clic su **Aggiungi società**, quindi configura l’azienda utilizzando le opzioni elencate di seguito. Al termine, fai clic su **Crea società**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sezione Informazioni di base</td> 
      <td> 
       <ul> 
        <li> <p><b>Nome dell'azienda</b>: Digita un nome per la società.</p> </li> 
        <li> <p><b>È attivo</b>: Quando questa opzione è abilitata, gli utenti possono trovare l’azienda e allegarla ai progetti creati e modificati. Impossibile allegare ai progetti un'azienda inattiva. Questa opzione è attivata per impostazione predefinita.</p> </li> 
        <li> <p><b>Questa è l'azienda principale</b>: Assegna l'azienda come azienda principale dell'organizzazione. L’azienda principale rappresenta in genere il tuo account Workfront in cui la maggior parte degli utenti lavora.</p> <p>Modificando i rispettivi livelli di accesso, puoi limitare gli utenti alla visualizzazione di altri utenti:</p> 
         <ul> 
          <li>Solo nella loro azienda primaria</li> 
          <li> <p>Nella società associata e nella società principale</p> <p>Per informazioni sulla funzionalità principale dell'azienda nei livelli di accesso degli utenti, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> <p>Puoi avere una sola o nessuna società designata come società primaria, ma non puoi avere più aziende designate come società primarie. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Gruppo</b>: Se c'è un gruppo che conduce affari con l'azienda, è possibile aggiungere il nome del gruppo qui. Questo è utile per gli amministratori dei gruppi che devono creare rapporti e gestire tutte le aziende con cui i loro gruppi svolgono attività commerciali.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Il sistema riempie il <strong>Gruppo</strong> campo per la nuova società con il gruppo che stai visualizzando.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Se disponi di accesso amministrativo alle aziende nel livello di accesso, puoi rimuovere il gruppo dalla società e assegnarne uno diverso o lasciare la società senza un gruppo.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Se non hai accesso amministrativo alle aziende, la <strong>Gruppo</strong> Il campo è obbligatorio ed è possibile selezionare solo i gruppi gestiti o qualsiasi sottogruppo in tali gruppi.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Per informazioni sull'accesso amministrativo alle aziende, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> </li> 
        <li> <p><b>Membri dell'azienda</b>: Aggiungi utenti esistenti alla società. In questo modo, associ questi utenti a questa azienda.</p> <p>Non vi è alcun limite al numero di utenti che si associano a una società, ma un utente non può essere associato a più di una società.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sezione Tassi di fatturazione</td> 
      <td> <p>Puoi sovrascrivere i tassi di fatturazione associati ai ruoli del lavoro a livello aziendale. Per informazioni sulla creazione di ruoli di lavoro e sull'associazione di questi con i tassi di fatturazione, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" data-mc-variable-override="">Creare e gestire ruoli di lavoro</a>.</p> <p>Per ulteriori informazioni sull'override delle tariffe di fatturazione a livello aziendale, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md" class="MCXref xref" data-mc-variable-override="">Escludere i tassi di fatturazione dei ruoli di lavoro a livello aziendale</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sezione Forms personalizzata</td> 
      <td> <p>Se esistono campi che si desidera aggiungere alla società che non sono disponibili in Workfront, è possibile creare un modulo personalizzato e associarlo alla società. Puoi allegare il modulo alla tua azienda selezionandolo dal menu a discesa. Solo le società attive sono elencate nel menu a discesa. Per informazioni sulla creazione di Custom Forms, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare un modulo personalizzato</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Se disponi di accesso amministrativo alle aziende nel livello di accesso, puoi anche fare clic su Aggiungi altre società in fondo all’elenco. In questo modo viene aggiunta una riga in cui è possibile configurare rapidamente la nuova azienda.

1. (Facoltativo) Per modificare o eliminare le aziende, seleziona almeno una società, quindi utilizza i pulsanti della barra degli strumenti per modificare ![](assets/edit-icon.png) o eliminare ![](assets/delete.png) .

   Per informazioni sulla modifica di un&#39;azienda, consulta la sezione . [Creare o modificare un’azienda in Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) nell&#39;articolo [Creare e modificare aziende](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Facoltativo) Per esportare l’elenco delle aziende, fai clic sull’icona Esporta ![](assets/export.png), quindi selezionare il formato di file desiderato per l’elenco esportato.
