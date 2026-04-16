---
title: Condividere le autorizzazioni finanziarie su un oggetto
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Il tuo amministratore Adobe Workfront può concederti l’accesso per visualizzare o modificare dati finanziari durante l’assegnazione del livello di accesso. Per ulteriori informazioni, consulta Concedere l’accesso ai dati finanziari.
author: Courtney
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: e974adc053a076a4370aa0c4ec41fea700d836be
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 17%

---

# Condividere le autorizzazioni finanziarie su un oggetto

Il tuo amministratore Adobe Workfront può concederti l’accesso per visualizzare o modificare dati finanziari durante l’assegnazione del livello di accesso. Per ulteriori informazioni, vedere [Concedere l&#39;accesso ai dati finanziari](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

Oltre al livello di accesso concesso agli utenti, è possibile concedere loro le autorizzazioni per visualizzare o gestire dati finanziari per progetti, attività o problemi specifici per i quali si dispone dell&#39;accesso alla condivisione.

Per informazioni sulle operazioni che gli utenti di ogni livello di accesso possono eseguire con i dati finanziari, vedere la sezione [Dati finanziari](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) nell&#39;articolo [Funzionalità disponibile per ogni tipo di oggetto](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Requisiti di accesso

<!--
drafted for P&P:

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
   <p>Legacy license: Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, and Financial  Data</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, and issues that include at least View Finance permissions</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Piano</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore a progetti, attività, problemi e dati finanziari</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> Visualizza autorizzazioni o versioni successive per progetti, attività e problemi che includono almeno Visualizza tariffe di fatturazione, Visualizza tariffe di costo e Visualizza autorizzazioni di contabilità generale</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Condividere un oggetto e concedere autorizzazioni finanziarie

Quando si concedono autorizzazioni finanziarie agli oggetti, tenere presente quanto segue:

* Puoi concedere autorizzazioni finanziarie a progetti, attività e problemi.
* Le autorizzazioni possono essere ereditate: se si dispone delle autorizzazioni Visualizza contabilità generale per un progetto, si ereditano automaticamente le autorizzazioni Visualizza contabilità generale per le attività e i problemi del progetto.
* La concessione di autorizzazioni per la fatturazione e le tariffe consente all&#39;utente di visualizzare o modificare le tariffe relative a tale oggetto. Le autorizzazioni per la contabilità generale consentono all&#39;utente di visualizzare o modificare i campi di contabilità generale (non correlati alla fatturazione o ai tassi di costo) sull&#39;oggetto.

Per concedere autorizzazioni finanziarie a un oggetto:

1. Passare a un&#39;attività, un progetto o un problema che si desidera condividere con altri utenti.
1. Fare clic su **Condividi** accanto al nome dell&#39;oggetto.

1. Nel campo **Concedi a `<Object name>` l&#39;accesso a** inizia a digitare il nome di un utente, un team, una mansione, un gruppo o un&#39;azienda con cui desideri condividere l&#39;oggetto.

   >[!TIP]
   >
   >Puoi condividere un oggetto solo con utenti attivi, team, ruoli o aziende.

1. Fai clic sull’elenco a discesa a destra del nome dell’utente e seleziona una delle seguenti opzioni:

   * **Visualizza**
   * **Contribuisci**
   * **Gestisci**

1. Nello stesso menu a discesa, fai clic sull’icona delle opzioni avanzate accanto al livello di autorizzazione, quindi effettua una delle seguenti operazioni:

   * Per qualsiasi livello di autorizzazione, selezionare **Visualizza tariffe di fatturazione**, **Visualizza tariffe di costo** e **Visualizza contabilità generale** in base alle esigenze.
   * Per **Gestire solo le autorizzazioni**, selezionare **Modifica tariffe di fatturazione**, **Modifica tariffe** e **Modifica contabilità generale** in base alle esigenze.

1. Fai clic su **Salva**.

## Autorizzazioni finanziarie per tutti i livelli di condivisione

Nella tabella seguente vengono visualizzate le autorizzazioni finanziarie ottenute dagli utenti quando si concedono loro le autorizzazioni Visualizza, Contribuisci o Gestisci per gli oggetti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Azioni</strong> </th> 
   <th><strong>Gestisci</strong> </th> 
   <th><strong>Contribuisci</strong> </th> 
   <th><strong>Visualizza</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Gestisci record fatturazione</td> 
   <td>✓</td> 
   <td> <p>  </p> </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Modifica tariffe di fatturazione</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Modifica tariffe di costo</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr>  
  <tr> 
   <td>Modifica dati finanziari generali</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr>
  <tr> 
   <td>Visualizza tariffe di fatturazione</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td>Visualizza tariffe di costo</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr>  
  <tr> 
   <td>Visualizza dati finanziari generale</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td>Visualizzare le informazioni per costo negli strumenti di pianificazione delle risorse</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Risorse preventivate negli strumenti di pianificazione delle risorse*</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Visualizzare le risorse negli strumenti di pianificazione delle risorse*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Richiede l&#39;accesso aggiuntivo a Gestione risorse.

Per informazioni sull&#39;accesso a Gestione risorse, vedere [Concedere l&#39;accesso a Gestione risorse](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

<!--
These rows removed from last table.

  <tr> 
   <td>Manage/ View Role Billing and Cost Rates</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Manage/ View User Billing and Cost Rates</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 

-->
