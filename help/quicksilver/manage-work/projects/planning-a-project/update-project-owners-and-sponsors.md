---
product-area: projects
navigation-topic: plan-a-project
title: Aggiorna proprietari e sponsor del progetto
description: Quando crei un progetto in Adobe Workfront, l’utente viene automaticamente impostato come Proprietario del progetto. Puoi aggiornare questo campo con un altro utente. Puoi anche aggiornare il campo Sponsor progetto di un progetto.
author: Alina
feature: Work Management
exl-id: 10421cab-237a-49a5-bb5b-5be510dc4c46
source-git-commit: 4cdebe4890b775a097469e7d7035a38397b71094
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Aggiorna proprietari e sponsor del progetto

Quando crei un progetto in Adobe Workfront, l’utente viene automaticamente impostato come Proprietario del progetto. Puoi aggiornare questo campo con un altro utente. Puoi anche aggiornare il campo Sponsor progetto di un progetto.

Per informazioni sui proprietari e gli sponsor dei progetti, vedi [Panoramica dei proprietari e degli sponsor dei progetti](../../../manage-work/projects/planning-a-project/project-owners-and-sponsors.md).

>[!TIP]
>
>Puoi identificare un proprietario e uno sponsor per un modello. Quando crei un progetto da tale modello, il proprietario del modello diventa il proprietario del progetto e lo sponsor del modello diventa lo sponsor del progetto.
>
>Se il modello non dispone di un Proprietario, l’utente che crea il progetto dal modello diventa il Proprietario del progetto.
>
>Per informazioni sulla modifica dei modelli, consulta [Modificare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Requisiti di accesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> <p>  </p> </td> 
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
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Edit permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Modificare le autorizzazioni per un progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Aggiornare il proprietario di un progetto

Quando aggiungi un utente come proprietario del progetto, Workfront assegna automaticamente le autorizzazioni necessarie per visualizzare il progetto.

1. Vai al progetto che desideri aggiornare.
1. Clic **Dettagli progetto** nel pannello a sinistra.
1. Fai clic su **Modifica** icona ![](assets/qs-edit-icon.png) nell’angolo superiore destro dell’area Project Details (Dettagli progetto), fai clic su  **Panoramica**.

1. Specifica il nome di un utente per **Proprietario progetto** campo.

   Solo gli utenti attivi possono essere specificati come Proprietari del progetto.

1. Clic  **Salva modifiche**.

   Il Proprietario del progetto viene aggiornato nell’intestazione del progetto e nell’area Dettagli progetto.

![](assets/project-stakeholders-owner-highlighted-nwe-350x149.png)

## Aggiornare lo sponsor di un progetto

Quando aggiungi un utente come sponsor del progetto di un progetto, Workfront assegna automaticamente a tale utente le autorizzazioni per visualizzare il progetto.

>[!TIP]
>
>Se l&#39;utente aggiunto come sponsor del progetto è un amministratore di sistema, non viene aggiunto all&#39;elenco Condivisione del progetto.

1. Vai al progetto che desideri aggiornare.
1. Clic **Dettagli progetto** nel pannello a sinistra.
1. Fai clic su **Modifica** icona ![](assets/qs-edit-icon.png) nell’angolo superiore destro dell’area Project Details (Dettagli progetto), fai clic su  **Panoramica**.

1. Specifica il nome di un utente per **Sponsor Progetto** campo.

   Solo gli utenti attivi possono essere specificati come sponsor del progetto.

1. Clic  **Salva modifiche**.

   Lo sponsor del progetto viene aggiornato nella sezione Project Details (Dettagli progetto).

   ![](assets/project-stakeholders-sponsor-highlighted-nwe-350x147.png)
