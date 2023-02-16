---
product-area: projects
navigation-topic: manage-projects
title: Copiare un progetto
description: Puoi copiare un progetto anziché crearne uno da zero. Puoi copiare un solo progetto alla volta. Non è possibile copiare i progetti in blocco.
author: Alina
feature: Work Management
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 95c999a72020ce825f3a8377662c71e35a194d80
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 5%

---

# Copiare un progetto

<span class="preview">Le informazioni evidenziate in questa pagina fanno riferimento a funzionalità non ancora disponibili al pubblico. È disponibile solo nell’ambiente Anteprima.</span>

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

Puoi copiare un progetto anziché crearne uno da zero. Puoi copiare un solo progetto alla volta. Non è possibile copiare i progetti in blocco.

>[!IMPORTANT]
>
>I seguenti elementi non vengono mai copiati da un progetto esistente a uno nuovo:
>
>* Problemi
>* Tariffe di fatturazione
>* Record fatturazione
>* Note
>* Ore
>* predecessori tra progetti
>* <span class="preview">Ore preventivate</span>
>
>I seguenti elementi vengono sempre copiati da un progetto esistente a uno nuovo:
>
>* Attività
>* Modello
>* Rischi
>* Informazioni sulla configurazione della coda
>* Portfolio e programma
>* Scorecard
>* Informazioni predefinite attività (processo di approvazione predefinito attività, Forms personalizzato predefinito attività)
>


## Requisiti di accesso

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>View permissions or higher to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td> <p>Licenza Adobe Workfront*</p> </td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurazioni a livello di accesso*</strong> </td> 
   <td> <p>Modifica l’accesso a Progetti con la possibilità di creare <span>e copia</span> progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Visualizza autorizzazioni o versioni successive al progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Copiare un singolo progetto

Copiare alcune informazioni dal progetto originale al nuovo progetto viene copiato anche. È inoltre possibile specificare quali elementi non devono essere copiati nel nuovo progetto durante il processo di copia.

Per copiare un progetto:

1. Passa al progetto da copiare e fai clic sul pulsante **Altro** icona ![](assets/qs-more-menu.png) a destra del nome del progetto

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Oppure

   Passa a un elenco o a un rapporto di progetto e seleziona un progetto, quindi fai clic sul pulsante **Altro** icona ![](assets/qs-more-menu.png) in cima all&#39;elenco.

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. Fai clic su **Copia**.

1. Aggiorna il nome del nuovo progetto.

   Per impostazione predefinita, il nuovo nome è **Copia di `<Original project name>`.**

   ![](assets/copy-project-box-nwe-350x276.png)

1. Seleziona la **Stato** per il nuovo progetto.

   Per impostazione predefinita, la **Stato** corrisponde a quello del progetto originale.

1. (Facoltativo) Deseleziona gli elementi che non desideri copiare nel nuovo progetto. La tabella seguente descrive cosa accade quando deselezioni gli elementi:


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Seleziona tutto</td> 
      <td> <p>Seleziona tutte le opzioni e cancella tutti i campi e gli oggetti elencati dal nuovo progetto.</p> <p><b>SUGGERIMENTO</b>

   Deselezionare <strong>Seleziona tutto</strong> deseleziona tutti gli elementi. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Assegnazioni</td> 
      <td>Rimuove tutte le assegnazioni di progetto e task</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Avanzamento</td> 
      <td>Rimuove l’avanzamento di tutte le attività e vengono visualizzate come nuove. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dati personalizzati</td> 
      <td> <p>Rimuove le informazioni dal modulo personalizzato sul progetto, nonché quelle sui moduli personalizzati associati agli elementi seguenti:</p> 
       <ul> 
        <li>Attività</li> 
        <li>Spese</li> 
        <li> Documenti</li> 
       </ul> <p><b>NOTA</b>

   I moduli personalizzati rimangono allegati alle attività, alle spese, ai documenti e al progetto, ma le informazioni contenute nei campi personalizzati dei moduli non vengono copiate nel nuovo progetto. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Documenti</td> 
      <td> <p>Rimuove tutti gli elementi presenti nella scheda documenti, incluse le versioni del documento, i documenti collegati e le cartelle.</p> <p>Per impostazione predefinita, le bozze dei documenti e le approvazioni non possono essere copiate in un altro progetto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tutti i predecessori</td> 
      <td> <p>Rimuove tutte le relazioni precedenti tra le attività del progetto. </p> <p><b>SUGGERIMENTO</b>

   I predecessori tra progetti non vengono mai trasferiti al nuovo progetto, indipendentemente dal fatto che sia selezionato o meno. </p> </td>
   </tr>

<tr> 
      <td role="rowheader"><span class="preview">Ore preventivate</span></td> 
      <td> <p><span class="preview">Rimuove dal progetto copiato le ore previste nell'area di pianificazione delle risorse del Business Case del progetto. <span class="preview"></p>

<b>NOTA</b>

<span class="preview">Le ore inserite in budget utilizzando il Planner scenario non vengono mai copiate nel nuovo progetto perché il nuovo progetto non è collegato a un&#39;iniziativa nel Planner scenario. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">Risorse di budget nel caso aziendale utilizzando il Planner scenario</a></span>
</tr></td>
    <tr> 
      <td role="rowheader">Informazione Finanziaria</td> 
      <td> <p>Rimuove le informazioni nelle seguenti aree: </p> 
       <ul> 
        <li>Sottoscheda Finanziamento del progetto</li> 
        <li> Vantaggio pianificato nel caso aziendale</li> 
        <li>Informazioni finanziarie da tutte le attività<br></li> 
       </ul> <p>Per ulteriori informazioni sulla sottoscheda Finanza progetto, consulta <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Gestire le informazioni nell'area di finanziamento del progetto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processo di approvazione</td> 
      <td>Rimuove tutte le approvazioni associate alle attività o al progetto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche promemoria</td> 
      <td> Rimuove le notifiche dei promemoria associate alle attività o al progetto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spese</td> 
      <td>Rimuove le spese associate alle attività o al progetto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autorizzazioni</td> 
      <td> Rimuove le autorizzazioni per tutti gli utenti sulle attività o sul progetto.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Copia** per creare una copia del progetto.

   Viene creato un nuovo progetto simile a quello copiato.

   È possibile iniziare a apportare modifiche al nuovo progetto copiato, ad esempio rivedere le assegnazioni delle attività o regolare le timeline.
