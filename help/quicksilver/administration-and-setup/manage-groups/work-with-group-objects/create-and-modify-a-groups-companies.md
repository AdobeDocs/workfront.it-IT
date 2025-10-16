---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Creare e modificare le società di un gruppo
description: Quando visualizzi un gruppo che gestisci nell’area Gruppi, puoi visualizzare e lavorare con le aziende associate al gruppo e ai relativi sottogruppi.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: 1554c067afcc548c7f7abd03dbc3a49404e3c89c
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Creare e modificare le società di un gruppo

Quando visualizzi un gruppo che gestisci nell’area Gruppi, puoi visualizzare e lavorare con le aziende associate al gruppo e ai relativi sottogruppi.

Se ci sono gruppi al di sopra del gruppo, gli amministratori possono eseguire queste operazioni anche per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

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

## Dall’area Gruppi puoi visualizzare, lavorare con il tuo gruppo e crearne altre

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![Gruppi](assets/groups-icon.png).

1. Fare clic sul nome del gruppo per il quale si desidera creare o modificare le società.
1. Nel pannello a sinistra, fai clic su **Aziende** per elencare le aziende associate al gruppo ed eventuali sottogruppi.
1. (Facoltativo) Per aggiungere una società, fai clic su **Aggiungi società**, quindi configura la società utilizzando le opzioni elencate di seguito. Al termine, fare clic su **Crea società**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sezione Informazioni di base</td> 
      <td> 
       <ul> 
        <li> <p><b>Nome società</b>: digitare un nome per la società.</p> </li> 
        <li> <p><b>È attivo</b>: quando questa opzione è abilitata, gli utenti possono trovare la società e allegarla ai progetti che creano e modificano. Una società inattiva non può essere collegata a progetti. Questa opzione è attivata per impostazione predefinita.</p> </li> 
        <li> <p><b>Questa è la società principale</b>: assegna la società come società principale della tua organizzazione. L’azienda principale in genere rappresenta l’account Workfront dove lavora la maggior parte degli utenti.</p> <p>Modificando i livelli di accesso, è possibile limitare la visualizzazione ad altri utenti:</p> 
         <ul> 
          <li>Solo nella società principale</li> 
          <li> <p>Nella società associata e nella società principale</p> <p>Per informazioni sulle funzionalità aziendali principali nei livelli di accesso degli utenti, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> <p>È possibile designare una sola o nessuna società come società principale, ma non è possibile designare più società come società principali. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Gruppo</b>: se è presente un gruppo che conduce affari con la società, è possibile aggiungere il nome del gruppo qui. Questo è utile per gli amministratori di gruppi che devono segnalare e gestire tutte le aziende con cui i loro gruppi intrattengono rapporti commerciali.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Il sistema compila il campo <strong>Gruppo</strong> per la nuova società con il gruppo che stai visualizzando.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Se disponi di accesso amministrativo per le aziende nel tuo livello di accesso, puoi rimuovere il gruppo dalla società e assegnarne uno diverso, oppure lasciare la società senza un gruppo.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Se non hai accesso amministrativo alle aziende, è necessario il campo <strong>Gruppo</strong> e puoi selezionare solo i gruppi che gestisci o eventuali sottogruppi in tali gruppi.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Per informazioni sull'accesso amministrativo alle aziende, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Concedere agli utenti l'accesso amministrativo ad alcune aree</a>.</p> </li> 
        <li> <p><b>Membri società</b>: aggiungi utenti esistenti alla società. In questo modo, si associano questi utenti a questa azienda.</p> <p>Non esiste un limite al numero di utenti associati a una società, ma un utente non può essere associato a più società.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Sezione Forms personalizzata</td> 
      <td> <p>Se sono presenti campi che si desidera aggiungere alla società e che non sono disponibili in Workfront, è possibile creare un modulo personalizzato e associarlo alla società. Per allegare il modulo alla società, selezionarlo dal menu a discesa. Nel menu a discesa sono elencate solo le società attive. Per informazioni sulla creazione di moduli personalizzati, vedere <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Creare un modulo personalizzato</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Se disponi di accesso amministrativo per le aziende nel tuo livello di accesso, puoi anche fare clic su Aggiungi altre aziende nella parte inferiore dell’elenco. In questo modo viene aggiunta una riga in cui è possibile configurare rapidamente la nuova società.

1. (Facoltativo) Per modificare o eliminare società, selezionare almeno una società, quindi utilizzare i pulsanti della barra degli strumenti per modificare ![icona Modifica](assets/edit-icon.png) o eliminare ![icona Elimina](assets/delete.png).

   Per informazioni sulla modifica di una società, vedere la sezione [Creare o modificare una società in Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) nell&#39;articolo [Creare e modificare società](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Facoltativo) Per esportare l&#39;elenco di società, fare clic sull&#39;icona Esporta ![icona Esporta](assets/export.png), quindi selezionare il formato di file desiderato per l&#39;elenco esportato.
