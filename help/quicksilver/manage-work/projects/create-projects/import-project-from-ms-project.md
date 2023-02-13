---
product-area: projects
navigation-topic: create-projects
title: Importare un progetto da un progetto Microsoft
description: Puoi importare progetti da Microsoft Project in Adobe Workfront e gestire tutti i tuoi progetti in un’unica applicazione. Ogni volta che importi un progetto da Microsoft Project, viene creato un nuovo progetto in Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 1%

---

# Importare un progetto da un progetto Microsoft

Puoi importare progetti da Microsoft Project in Adobe Workfront e gestire tutti i tuoi progetti in un’unica applicazione. Ogni volta che importi un progetto da Microsoft Project, viene creato un nuovo progetto in Workfront.

>[!IMPORTANT]
>
>Non tutti i campi del progetto Microsoft vengono trasferiti ad Workfront.
>
>Per ulteriori informazioni sulla compatibilità dei campi tra Workfront e Microsoft Project, vedi [Mappatura dei campi del progetto Microsoft su progetti Adobe Workfront](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## Requisiti di accesso

redatto per P&amp;P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Licenza attuale: Standard </p> 
   Oppure
   <p>Licenza legacy: Pianificare </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni sull&#39;accesso ai progetti, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Concedere l’accesso ai progetti</a>. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Quando crei un progetto ricevi automaticamente le autorizzazioni Gestisci per il progetto </p> <p> Per informazioni sulle autorizzazioni del progetto, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Condivisione di un progetto in Adobe Workfront</a>.</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni sull&#39;accesso ai progetti, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Concedere l’accesso ai progetti</a>. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Quando crei un progetto ricevi automaticamente le autorizzazioni Gestisci per il progetto </p> <p> Per informazioni sulle autorizzazioni del progetto, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Condivisione di un progetto in Adobe Workfront</a>.</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creazione di un progetto da un progetto MS

Puoi creare un progetto dall’area Progetti nel menu principale o dall’area Progetti di un portfolio o di un programma.

1. Vai a Progetto Microsoft e apri un progetto da cui desideri importare in Workfront.
1. Fai clic su **File**, quindi **Salva con nome** per salvare il progetto come file .xml.

1. Accedi a Workfront.
1. Esegui una delle operazioni seguenti:

   * Fai clic sul pulsante **Menu principale** ![](assets/main-menu-icon.png), fai clic su **Progetti**, quindi espandi **Nuovo progetto**.
   * Passa a un portfolio, quindi espandi **Nuovo progetto**.
   * Vai a un programma, quindi espandi **Nuovo progetto**.
   * Gli amministratori di gruppo possono creare un progetto anche nella sezione Progetti di un gruppo gestito. Per ulteriori informazioni, consulta [Creare e modificare i progetti di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Scegli la **Importa progetto MS** opzione .

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. Fai clic su **Seleziona file**, quindi cerca il file .xml sul computer esportato da Microsoft Project.
1. Importa il file selezionato.

   Workfront avvia il processo di importazione e crea un nuovo progetto basato sul file esportato da Microsoft Project.

   Al termine del processo di importazione, vieni indirizzato alla nuova pagina del progetto che mostra una conferma del completamento dell’importazione.

   >[!NOTE]
   >
   >Workfront ha un limite di tempo di 15 minuti per il caricamento dei file. Se il caricamento del file richiede più tempo, ti consigliamo di suddividere il progetto in progetti più piccoli e importarli separatamente. Una volta importate in Workfront, sposta le attività da un progetto all’altro per combinarle in un unico progetto. Per informazioni sullo spostamento delle attività, consulta [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (Facoltativo) Continua a modificare il progetto in Workfront. Per informazioni sulla modifica dei progetti, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

   Lo stato di un nuovo progetto creato da un modello corrisponde a quello definito dall’amministratore di Workfront nell’area Preferenze progetto o da un amministratore di gruppo nell’area Preferenze progetto di gruppo. Per informazioni sulla configurazione delle preferenze del progetto, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
