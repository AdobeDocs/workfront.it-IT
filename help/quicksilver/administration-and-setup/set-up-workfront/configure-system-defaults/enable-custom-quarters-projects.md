---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Abilita trimestri personalizzati
description: A scopo di reporting, è possibile creare trimestri personalizzati se i trimestri dell'organizzazione si basano su criteri specifici diversi dalle date del calendario, ad esempio giorni lavorativi o di acquisto.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/8kRfZ17zcgN0-hlc16wh328YGRjTlzuI3LAe-Yjj25s
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 6f64c3e6ebb8407c38ad3a1d46b2fc63b534879e
workflow-type: tm+mt
source-wordcount: 894
ht-degree: 5%

---

# Abilitare trimestri personalizzati

<!--Audited: 03/2026-->

<!--remove Production and Preview references at release-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


A scopo di reporting, è possibile creare trimestri personalizzati se i trimestri dell&#39;organizzazione si basano su criteri specifici diversi dalle date del calendario, ad esempio giorni lavorativi o di acquisto.

A seconda dei prodotti acquistati dalla società, è possibile configurare il seguente numero di trimestri nell&#39;area di configurazione di Workfront:

* I clienti che hanno acquistato solo [!DNL Workfront] possono configurare fino a otto trimestri personalizzati per il sistema [!DNL Adobe Workfront].
* I clienti che hanno acquistato [!DNL Workfront] e [!DNL Workfront Planning] possono configurare fino a 100 trimestri per il sistema [!DNL Workfront], disponibili anche in [!DNL Planning].

<div class="preview">

* I clienti che hanno acquistato [!DNL Workfront] e [!DNL Workfront Planning] possono configurare settimane personalizzate per ogni trimestre personalizzato. Le settimane personalizzate sono visibili nelle visualizzazioni della timeline [!DNL Planning].

</div>

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td><p>Licenza [!UICONTROL Workflow Standard] o [!UICONTROL Workfront Plan]</p>
       <p></p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
When we release fiscal weeks, replace the table above with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>Any Workfront or Workflow package</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>Any Planning package, including Planning as a standalone product</p>
   </div>
   </li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td>
   
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>[!UICONTROL Workflow Standard] or [!UICONTROL Workfront Plan] license</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>A [!UICONTROL Planning Standard] license, in addition to a Workfront or a Workflow license</p>
   </div>
   </li>
   </ul>
    </td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

-->


## Imposta trimestri personalizzati per il sistema [!DNL Workfront]

L’impostazione dei trimestri personalizzati varia a seconda dell’ambiente utilizzato.

### Impostare trimestri personalizzati per il sistema [!DNL Workfront] nell&#39;ambiente di produzione

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Trimestri personalizzati]**.

1. Selezionare **[!UICONTROL Abilita trimestri personalizzati]**.

1. Digita un nome per il trimestre personalizzato, ad esempio &quot;Fiscal Q1 2021&quot;.
1. Seleziona le date di inizio e fine per il trimestre personalizzato.

   ![Trimestri personalizzati](assets/custom-quarters-nwe.png)

1. (Facoltativo) Fai clic su **[!UICONTROL Aggiungi trimestre personalizzato]** per aggiungere altri trimestri personalizzati al sistema.

   >[!IMPORTANT]
   >
   > Se la tua azienda ha acquistato [!DNL Workfront Planning], non puoi salvare i trimestri personalizzati se ci sono spazi o sovrapposizioni tra i trimestri.
   >![Trimestri personalizzati con avviso di sovrapposizione](assets/custom-quarters-with-overlap-warning.png)
   >Gli spazi vuoti e le sovrapposizioni tra i trimestri sono consentiti solo per i clienti [!DNL Workfront].

1. (Facoltativo e condizionale) Se la società ha acquistato solo [!DNL Workfront], senza [!DNL Workfront Planning], crea un elemento di reporting che si riferisce ai trimestri fiscali.

   **Esempio:** Crea un filtro per un elenco di [!UICONTROL progetti] e includi la data di completamento pianificata di un progetto che fa riferimento ai trimestri personalizzati.

   ![Filtro progetti con trimestri personalizzati](assets/example-of-project-filter-with-custom-quarters.png)

   I riferimenti a &quot;Questo trimestre&quot;, &quot;Prossimo trimestre&quot; e &quot;Ultimo trimestre&quot; sono sostituiti da nuovi riferimenti ai trimestri personalizzati.

   Per informazioni sugli elementi di reporting, vedere [Elementi di reporting: filtri, visualizzazioni e raggruppamenti](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Per informazioni sulla creazione di filtri, vedere [Creare o modificare filtri in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. (Facoltativo e condizionale) Se la società ha acquistato Workfront Planning e si dispone dell&#39;accesso a [!DNL Workfront Planning], passare a una pagina del tipo di record e aprire una visualizzazione della sequenza temporale. Nella visualizzazione vengono visualizzati i nuovi trimestri personalizzati.
Per informazioni, consulta [Gestire la vista timeline](/help/quicksilver/planning/views/manage-the-timeline-view.md).

<div class="preview">

### Impostare trimestri personalizzati per il sistema [!DNL Workfront] nell&#39;ambiente di anteprima

>[!NOTE]
>
>Se l&#39;organizzazione ha acquistato un pacchetto Planning in aggiunta a un pacchetto Flusso di lavoro o se ha acquistato Workfront Planning come pacchetto standalone, è possibile configurare le settimane personalizzate, oltre ai trimestri personalizzati.
> 
>Le settimane personalizzate non sono disponibili per i rapporti e gli elenchi di Workfront.

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Trimestri personalizzati]**.

1. Selezionare **[!UICONTROL Abilita trimestri personalizzati]**.

1. Digita un nome per il trimestre personalizzato. Ad esempio, &quot;Fiscal Q1 2021&quot;.
1. Seleziona le date di inizio e fine per il trimestre personalizzato.

1. (Facoltativo) Seleziona l&#39;opzione **Avvia una nuova sequenza settimanale personalizzata**.

   Se selezionata, questa opzione imposta l&#39;inizio del trimestre personalizzato come inizio della prima settimana personalizzata del trimestre nella visualizzazione della sequenza temporale di Planning.
1. (Facoltativo) Nell&#39;area **Formato etichetta settimana personalizzato**, scegliere il **Formato** per le etichette settimana personalizzate. Scegli una tra le opzioni seguenti:

   * **W1, W2, W3 ...** . Questo è il formato predefinito.
   * **FW1, FW2, FW3 ...**
   * **Settimana1, Settimana 2, Settimana 3, ...**
   * **Personalizzato**

1. (Condizionale) Se hai selezionato **Personalizzato** per il campo **Formato**, digita una **Etichetta personalizzata** per identificare le settimane personalizzate.

   Le settimane personalizzate vengono visualizzate nelle visualizzazioni timeline di Planning.

   >[!TIP]
   >
   >Quando aggiungi un’etichetta personalizzata, puoi digitare fino a 100 caratteri.
   >
   >È possibile indicare il nome della prima settimana e le settimane successive utilizzeranno la stessa etichetta seguita da un numero sequenziale.
   >
   >Ad esempio, una **etichetta personalizzata** di &quot;Settimana fiscale&quot; aggiungerà le etichette &quot;Settimana fiscale 1, Settimana fiscale 2, Settimana fiscale 3 ...&quot; al resto delle settimane nella sequenza.

1. (Facoltativo) Fai clic su **[!UICONTROL Aggiungi trimestre personalizzato]** per aggiungere altri trimestri personalizzati al sistema.

   >[!IMPORTANT]
   >
   > Se la tua azienda ha acquistato [!DNL Workfront Planning], non puoi salvare i trimestri personalizzati se ci sono spazi o sovrapposizioni tra i trimestri.
   >![Trimestri personalizzati con avviso di sovrapposizione](assets/custom-quarters-with-overlap-warning-red-outline.png)
   >Gli spazi vuoti e le sovrapposizioni tra i trimestri sono consentiti solo per i clienti [!DNL Workfront].

1. (Facoltativo e condizionale) Per visualizzare i trimestri personalizzati in Workfront, crea un elemento di reporting che faccia riferimento ai trimestri personalizzati.

   **Esempio:** Crea un filtro per un elenco di [!UICONTROL progetti] e includi la data di completamento pianificata di un progetto che fa riferimento ai trimestri personalizzati.

   ![Filtro progetti con trimestri personalizzati](assets/example-of-project-filter-with-custom-quarters.png)

   I riferimenti a &quot;Questo trimestre&quot;, &quot;Prossimo trimestre&quot; e &quot;Ultimo trimestre&quot; sono sostituiti da nuovi riferimenti ai trimestri personalizzati.

   Per informazioni sugli elementi di reporting, vedere [Elementi di reporting: filtri, visualizzazioni e raggruppamenti](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Per informazioni sulla creazione di filtri, vedere [Creare o modificare filtri in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. (Facoltativo e condizionale) Per visualizzare i trimestri e le settimane personalizzati in Workfront Planning, passare a una pagina del tipo di record e aprire una visualizzazione della sequenza temporale. Nella visualizzazione vengono visualizzati i nuovi trimestri e settimane personalizzati.

Per informazioni, consulta [Gestire la vista timeline](/help/quicksilver/planning/views/manage-the-timeline-view.md).

</div>
