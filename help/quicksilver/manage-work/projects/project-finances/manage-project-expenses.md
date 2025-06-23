---
product-area: projects
navigation-topic: financials
title: Gestisci spese progetto
description: Il processo di creazione e gestione delle spese è lo stesso sia per le spese relative al progetto che per quelle relative al task. Tutte le spese aggiunte al progetto nel Business Case vengono aggiunte alla scheda Spese come spese pianificate.
author: Lisa
feature: Work Management
exl-id: 80c41b08-3618-4d6e-8d07-1736b2f824ea
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 1%

---

# Gestisci spese progetto

<!-- Audited: 6/2025 -->

Il processo di creazione e gestione delle spese è lo stesso sia per le spese relative al progetto che per quelle relative al task. Tutte le spese aggiunte al progetto nel Business Case vengono aggiunte alla scheda Spese come spese pianificate. Per ulteriori informazioni, vedere [Creare un caso di business per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

L&#39;importo totale delle spese di tutte le attività e di tutti i progetti contribuisce al costo totale del progetto. L&#39;importo pianificato delle spese contribuisce al costo pianificato del progetto e l&#39;importo effettivo delle spese contribuisce al costo effettivo del progetto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Nuovo: Standard</p>
   <p>Corrente: Lavoro o versione successiva</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Modifica accesso a progetti e dati finanziari</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Contribuire o accedere ad autorizzazioni superiori per il progetto con autorizzazioni di visualizzazione o gestione delle finanze</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungi spese

1. Passare al progetto o all&#39;attività per cui si desidera immettere le spese.
1. Fai clic su **Spese** nel pannello a sinistra.
1. Fai clic su **Aggiungi una spesa**. Viene visualizzata la finestra di dialogo **Aggiungi una spesa**.
1. Aggiorna quanto segue:

   * **Descrizione:** Immettere una descrizione della spesa.
   * **Tipo di spesa:** (obbligatorio) Selezionare la categoria che meglio descrive la spesa.
   * **Attività:** Digitare il nome dell&#39;attività a cui è associata la spesa, quindi fare clic su di essa quando viene visualizzata nell&#39;elenco a discesa.
   * **Importo pianificato:** Inserire l&#39;importo preventivato pianificato per la spesa. Questo incide sul Costo preventivato del progetto.

   * **Importo effettivo:** Immettere l&#39;importo del costo effettivo della spesa. Questo incide sul Costo Reale del progetto.

   * **Data pianificata:** Immettere la data prevista per l&#39;esecuzione della spesa. È possibile digitare la data nel campo utilizzando il formato *mm/gg/aa* oppure fare clic sull&#39;icona **Calendario**  ![Icona Calendario](assets/calendar-icon.png) e selezionare la data in modo dinamico.

   * **Data pagamento:** Immettere o selezionare la data di pagamento della spesa.
   * **Fatturabile:** Selezionare questa opzione se si desidera fatturare la spesa. La classificazione di una spesa come fatturabile è importante quando si creano i record di fatturazione.
   * **Rimborsabile:** Selezionare questa opzione se la spesa deve essere rimborsata. Puoi quindi contrassegnare la spesa come rimborsata dopo che la spesa è stata rimborsata.

1. Seleziona un **modulo personalizzato** e specifica eventuali informazioni aggiuntive necessarie.

   >[!NOTE]
   >
   >È necessario creare un modulo personalizzato prima di associarlo a una spesa. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi. Per informazioni sulla creazione di moduli personalizzati, vedere l&#39;articolo [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Fai clic su **Salva modifiche**.

## Cancella Spese

1. Vai al progetto per il quale desideri eliminare una spesa.
1. Fai clic su **Spese** nel pannello a sinistra.
1. Seleziona la spesa da eliminare, quindi fai clic sull&#39;icona **Elimina** ![Elimina](assets/delete.png).
1. Nella finestra di dialogo **Elimina spesa** fare clic su **Sì, elimina**.