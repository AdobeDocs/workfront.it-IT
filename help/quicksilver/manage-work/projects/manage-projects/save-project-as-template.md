---
product-area: projects;templates
navigation-topic: manage-projects
title: Salvare un progetto come modello
description: Salva un progetto come modelloSalva come modello" a livello di progetto, in modo che gli utenti lo vedano nell’interfaccia utente; c'è un altro articolo a cui questo link è più approfondito (passo per passo). Questa funzionalità deve rimanere nelle aree dei progetti E dei modelli.)"
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 1%

---

# Salvare un progetto come modello

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

Se decidi che un progetto si ripeterà in futuro, puoi creare un modello da quel progetto esistente. A questo punto, è possibile utilizzare nuovamente il modello per creare progetti futuri che potrebbero contenere informazioni simili o condividere la stessa timeline o assegnazioni con il progetto esistente.

## Requisiti di accesso

<!--drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or 
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you save the project as a template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modificare l’accesso ai modelli</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare o concedere autorizzazioni superiori a un progetto </p> <p>Ottieni le autorizzazioni Gestisci per il modello dopo aver salvato il progetto come modello</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Salvare un progetto come modello

1. Passa al progetto da salvare come modello.
1. Fai clic sul pulsante **Altro** menu ![](assets/qs-more-icon-on-an-object.png), quindi **Salva come modello**.
1. Specifica le seguenti informazioni per il modello:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td>Specifica un nome per il modello.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Fornisci una descrizione del modello.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">È attivo</td> 
      <td> <p>Seleziona tra le seguenti opzioni:</p> 
       <ul> 
        <li> <p><strong>Sì</strong>: Altri utenti possono trovare il modello e allegarlo ai progetti.</p> </li> 
        <li><strong>No</strong>: Altri utenti non possono trovare il modello e non possono allegarlo ai progetti.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Moduli personalizzati</td> 
      <td>Utilizzare l’elenco a discesa per selezionare i moduli personalizzati da allegare al modello. Se al progetto sono già stati associati moduli personalizzati, vengono visualizzati tutti i campi dati di tali moduli personalizzati.<br>È possibile includere fino a 10 moduli personalizzati in un singolo modello.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Gestione Forms** per rimuovere o riordinare i moduli. Per informazioni su come rimuovere e riordinare i moduli personalizzati nel modello, vedere [Moduli personalizzati](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![](assets/save-as-template-first-step-350x159.png)

1. Fai clic su **Passaggio successivo.**
1. In **Opzioni** , seleziona la casella di controllo accanto alle informazioni che desideri cancellare dal modello.

   ![](assets/save-as-template-options-step-350x109.png)

1. Fai clic su **Passaggio successivo.**
1. In **Escludi** seleziona le attività da escludere dal progetto.

   ![](assets/save-as-template-exclude-350x205.png)

1. Fai clic su **Finisci e salva modello.**

   Il modello viene ora visualizzato nell’elenco dei modelli disponibili e può essere allegato a un progetto esistente o utilizzato per crearne uno nuovo.
