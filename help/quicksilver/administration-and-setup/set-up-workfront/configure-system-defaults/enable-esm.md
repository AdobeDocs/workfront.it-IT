---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Abilitare l’archiviazione cloud Adobe per la tua organizzazione
description: Puoi abilitare l’archiviazione cloud di Adobe per la tua organizzazione per utilizzare una soluzione di archiviazione unificata per tutti i prodotti Adobe.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 5%

---
# Abilitare l’archiviazione cloud Adobe per la tua organizzazione

Adobe Cloud Storage è una soluzione di archiviazione unificata basata su cloud che funge da archivio centrale per le risorse tra i prodotti aziendali Adobe. Questo articolo descrive come abilitare l’archiviazione cloud di Adobe come opzione di archiviazione predefinita per l’intera organizzazione o per gruppi specifici.

Questa è la singola azione che attiva la nuova esperienza: una volta abilitata, i nuovi progetti utilizzano l’archiviazione cloud Adobe, che include il visualizzatore Frame.io e le approvazioni unificate. Non cambia nulla finché non scegli di abilitare l’archiviazione cloud Adobe.

Poiché controlli la tempistica, puoi testare l’esperienza, aggiornare gli scenari di Workfront Fusion e pianificare le modifiche da apportare ai rapporti prima che qualcuno vi lavori. Per ulteriori informazioni sulle differenze e su come pianificare il rollout, consulta [Passare a Workfront nell&#39;archivio cloud Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Funzionamento delle approvazioni con l’archiviazione cloud Adobe

L’archiviazione cloud di Adobe determina il servizio di approvazione utilizzato da un progetto. Il passaggio a una versione di Workfront che supporta l’archiviazione cloud di Adobe non comporta il passaggio automatico dell’intera organizzazione alle approvazioni unificate. Il servizio di approvazione dipende invece dal modello di storage di ciascun progetto:

* Per impostazione predefinita, i **progetti Adobe per l&#39;archiviazione cloud** utilizzano le approvazioni unificate, con revisione e approvazione nel visualizzatore Frame.io.
* **I progetti di archiviazione legacy di Workfront** mantengono il servizio di approvazione già in uso. A seconda dell’organizzazione, potrebbe trattarsi di approvazioni unificate o di approvazioni di documenti legacy.

Per ulteriori informazioni sull&#39;esperienza di revisione e approvazione sull&#39;archiviazione cloud Adobe, consulta [Passare a Workfront sull&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

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

   * **Intera organizzazione**: questa opzione applica il provider di archiviazione predefinito all&#39;intero ambiente Workfront. Ogni volta che un utente crea un nuovo progetto, viene utilizzato il provider di archiviazione predefinito.
   * **Gruppi specifici**: questa opzione applica il provider di archiviazione predefinito solo a gruppi specifici all&#39;interno dell&#39;organizzazione. Ogni volta che un utente nei gruppi specificati crea un nuovo progetto, verrà utilizzato il provider di archiviazione predefinito.

     ![gruppi di preferenze di archiviazione](assets/configure-storage-preference.png)

1. Fai clic su **Salva**.

   >[!NOTE]
   >
   >I progetti esistenti mantengono il modello di archiviazione con cui sono stati creati. Ad esempio, i progetti che utilizzano l’archiviazione cloud di Adobe continuano a utilizzare l’archiviazione cloud di Adobe dopo aver modificato la preferenza di archiviazione predefinita.



## Archiviazione cloud Adobe in ambienti sandbox

L&#39;archiviazione cloud di Adobe è disponibile in [!DNL Workfront] ambienti sandbox, che consentono di testare la funzionalità descritta in questo articolo prima di implementarla in produzione. Tuttavia, il visualizzatore Frame.io non è disponibile in sandbox, pertanto l’esperienza completa di revisione e approvazione unificata deve essere convalidata in produzione.

Se disponi di una sandbox di aggiornamento personalizzata, devi aggiornarla dopo l’aggiornamento a una versione di Workfront che supporta l’archiviazione cloud di Adobe. L’aggiornamento consente alla sandbox di accedere alla funzionalità di archiviazione cloud di Adobe e di iniziare a testarla. Per ulteriori informazioni, vedere [L&#39;ambiente Sandbox di aggiornamento personalizzato [!DNL Adobe Workfront] ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).
