---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Abilitare l’archiviazione cloud Adobe per la tua organizzazione
description: Puoi abilitare l’archiviazione cloud di Adobe per la tua organizzazione per utilizzare una soluzione di archiviazione unificata per tutti i prodotti Adobe.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 48b581c7-a21a-45de-95c5-eafb0713b42e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7fc5fe2f2692841a8663740441f70be0c82c4073
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 7%

---

# Abilitare l’archiviazione cloud Adobe per la tua organizzazione

Adobe Cloud Storage è una soluzione di archiviazione unificata per tutti i prodotti Adobe. Si tratta di una soluzione di archiviazione basata su cloud che funge da archivio centrale per le risorse tra i prodotti aziendali Adobe.

L’archiviazione cloud di Adobe è abilitata per impostazione predefinita per i nuovi clienti e può essere abilitata per i clienti esistenti al momento del rinnovo del contratto.

Per ulteriori informazioni sull&#39;archiviazione cloud Adobe, consulta [Panoramica sull&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi pacchetto flusso di lavoro</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td><p>Standard</p> <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Devi essere un amministratore di Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Abilitare l’archiviazione cloud Adobe per la tua organizzazione

Per abilitare l’archiviazione cloud Adobe per la tua organizzazione:

{{step-1-to-setup}}

1. Seleziona **Sistema** nel menu di navigazione a sinistra, quindi seleziona **Preferenze**.
1. Scorri verso il basso fino alla sezione **Preferenze di archiviazione**.
1. Nel menu a discesa Predefinito, seleziona **Adobe Cloud Storage**.
1. (Facoltativo) Se desideri utilizzare una combinazione di archiviazione cloud Adobe e archiviazione Workfront legacy, seleziona la casella di controllo **Consenti all&#39;utente di selezionare il provider di archiviazione**.

   >[!NOTE]
   >
   >L’attivazione di questa opzione consente agli utenti di selezionare il provider di archiviazione al momento della creazione di un nuovo progetto. L’archiviazione cloud di Adobe è etichettata come &quot;Nuovo progetto&quot; in quanto è il provider di archiviazione predefinito. Lo storage Workfront legacy è etichettato come &quot;Progetto legacy&quot;.
   >
   >![nuove opzioni progetto e progetto legacy](assets/new-esm-project.png)

1. Nel menu a discesa Si applica a, scegliere una delle seguenti opzioni:

   - **Intera organizzazione**: questa opzione applica il provider di archiviazione predefinito all&#39;intero ambiente Workfront. Ogni volta che un utente crea un nuovo progetto, viene utilizzato il provider di archiviazione predefinito.
   - **Gruppi specifici**: questa opzione applica il provider di archiviazione predefinito solo a gruppi specifici all&#39;interno dell&#39;organizzazione. Ogni volta che un utente nei gruppi specificati crea un nuovo progetto, verrà utilizzato il provider di archiviazione predefinito

1. Fai clic su **Salva**.

   >[!NOTE]
   >
   >I progetti esistenti mantengono il modello di archiviazione con cui sono stati creati. Ad esempio, i progetti che utilizzano l’archiviazione cloud di Adobe continuano a utilizzare l’archiviazione cloud di Adobe dopo aver modificato la preferenza di archiviazione predefinita.

## Archiviazione cloud Adobe in ambienti sandbox

L&#39;archiviazione cloud di Adobe è disponibile in [!DNL Workfront] ambienti sandbox, che consentono di testare la funzionalità descritta in questo articolo prima di implementarla in produzione. Tuttavia, il visualizzatore Frame.io non è disponibile in sandbox, pertanto l’esperienza completa di revisione e approvazione unificata deve essere convalidata in produzione.

Se disponi di una sandbox di aggiornamento personalizzata, devi aggiornarla dopo l’aggiornamento a una versione di Workfront che supporta l’archiviazione cloud di Adobe. L’aggiornamento consente alla sandbox di accedere alla funzionalità di archiviazione cloud di Adobe e di iniziare a testarla. Per ulteriori informazioni, vedere [L&#39;ambiente Sandbox di aggiornamento personalizzato [!DNL Adobe Workfront] &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).
