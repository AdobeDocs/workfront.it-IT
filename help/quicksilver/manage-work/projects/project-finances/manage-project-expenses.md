---
product-area: projects
navigation-topic: financials
title: Gestisci spese progetto
description: Il processo di creazione e gestione delle spese è lo stesso sia per le spese relative al progetto che per quelle relative al task. Tutte le spese aggiunte al progetto nel Business Case vengono aggiunte alla scheda Spese come spese pianificate.
author: Lisa
feature: Work Management
exl-id: 80c41b08-3618-4d6e-8d07-1736b2f824ea
TQID: https://experienceleague.adobe.com/b6lcN97EhJ4bD8w12SRE9TGLycM9Y8Si8ZSm8VBlHlA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 43ed208abe51a7172c0143fa6f838362edd913db
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 8%
---
# Gestire le spese di progetto

<!-- Audited: 6/2025 -->

Il processo di creazione e gestione delle spese è lo stesso sia per le spese relative al progetto che per quelle relative al task. Tutte le spese aggiunte al progetto nel Business Case vengono aggiunte alla scheda Spese come spese pianificate. Per ulteriori informazioni, vedere [Creare un caso di business per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

L&#39;importo totale delle spese di tutte le attività e di tutti i progetti contribuisce al costo totale del progetto. L&#39;importo pianificato delle spese contribuisce al costo pianificato del progetto e l&#39;importo effettivo delle spese contribuisce al costo effettivo del progetto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Work o successiva</p></td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Modificare l’accesso a Progetti e Attività</td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td><p>Per aggiungere spese e modificare o eliminare le spese create: Contribuisci o autorizzazioni superiori al progetto o all'attività, con autorizzazioni per Aggiungi spese.</p><p>Per visualizzare, modificare o eliminare le spese aggiunte da altri utenti: gestire le autorizzazioni per il progetto o l'attività, con le autorizzazioni per visualizzare le tariffe di costo (per la visualizzazione) o modificare le tariffe di costo (per la modifica o l'eliminazione).</p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungi spese

1. Passare al progetto o all&#39;attività per cui si desidera immettere le spese.
1. Fai clic su **Spese** nel pannello a sinistra.
1. Fai clic su **Aggiungi una spesa**. Viene visualizzata la finestra di dialogo **Aggiungi una spesa**.
1. Immettere le seguenti informazioni:

   * **Descrizione:** Immettere una descrizione della spesa.
   * **Tipo di spesa:** (obbligatorio) Selezionare la categoria che meglio descrive la spesa.
   * **Attività:** Digitare il nome dell&#39;attività a cui è associata la spesa, quindi fare clic su di essa quando viene visualizzata nell&#39;elenco a discesa.
   * **Importo pianificato:** Inserire l&#39;importo preventivato pianificato per la spesa. Questo incide sul Costo preventivato del progetto.

   * **Importo effettivo:** Immettere l&#39;importo del costo effettivo della spesa. Questo incide sul Costo Reale del progetto.

   * **Data pianificata:** Immettere la data prevista per l&#39;esecuzione della spesa. È possibile digitare la data nel campo utilizzando il formato *mm/gg/aa* oppure fare clic sull&#39;icona **Calendario** ![Icona Calendario](assets/calendar-icon.png) e selezionare la data in modo dinamico.

   * **Data pagamento:** Immettere o selezionare la data di pagamento della spesa.
   * **Fatturabile:** Selezionare questa opzione se si desidera fatturare la spesa. La classificazione di una spesa come fatturabile è importante quando si creano i record di fatturazione.
   * **Rimborsabile:** Selezionare questa opzione se la spesa deve essere rimborsata. Puoi quindi contrassegnare la spesa come rimborsata dopo che la spesa è stata rimborsata.

1. Seleziona un **modulo personalizzato** e specifica eventuali informazioni aggiuntive necessarie.

   >[!NOTE]
   >
   >È necessario creare un modulo personalizzato prima di associarlo a una spesa. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi. Per informazioni sulla creazione di moduli personalizzati, vedere l&#39;articolo [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Fai clic su **Salva**.

## Cancella Spese

1. Passare al progetto o all&#39;attività per cui si desidera eliminare una spesa.
1. Fai clic su **Spese** nel pannello a sinistra.
1. Seleziona la spesa da eliminare, quindi fai clic sull&#39;icona **Elimina** ![Elimina](assets/delete.png).
1. Nella finestra di dialogo **Elimina spesa** fare clic su **Sì, elimina**.
