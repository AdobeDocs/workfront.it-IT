---
title: Modifica tipi di record
description: È possibile modificare i tipi di record dopo il salvataggio. I tipi di record sono i tipi di oggetto di Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: bda3dc43828032fd5a8862b12d851c56cf9b6cbd
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the object types of Adobe Workfront Planning.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# Modifica tipi di record

{{planning-important-intro}}

I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. È possibile modificare l&#39;aspetto dei tipi di record creati dall&#39;utente o da qualsiasi altro utente. Per informazioni sulla creazione di tipi di record di Workfront Planning, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per Workfront Planning.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Prodotto</p> </td>
   <td>
   <p> Adobe Workfront</p> <p>Per collegare i tipi di record di Adobe Workfront Planning a Experience Manager Assets, è necessario disporre di una licenza Adobe Experience Manager Assets e l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Business Platform o Adobe Admin Console.</p> </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>L'organizzazione deve essere iscritta alla fase di accesso anticipato per Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>piano Adobe Workfront</p></td>
   <td>
<p>Qualsiasi</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td>
   <td>
   <p>Nuovo: Standard</p>
   <p>Corrente: Piano</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td>
   <td> <p>Nessun controllo del livello di accesso per Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestione delle autorizzazioni per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L'amministratore del Workfront o del gruppo deve aggiungere l'area Planning nel modello di layout. Per informazioni, vedere <a href="/help/quicksilver/planning/access/access-overview.md">Panoramica dell'accesso</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Modifica tipi di record

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera modificare i tipi di record.

   Oppure

   Da un workspace, espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente, cercare un workspace e selezionarlo quando viene visualizzato nell&#39;elenco.

   Viene aperto il workspace e vengono visualizzati i tipi di record.
1. Passa il puntatore del mouse sulla scheda di un tipo di record e fai clic sul menu **Altro** ![](assets/more-menu.png) nell&#39;angolo superiore destro della scheda del tipo di record, quindi fai clic su **Modifica**.

   ![](assets/more-menu-options-from-record-type-card.png)

1. Nella casella **Modifica tipo di record**, aggiornare le informazioni seguenti:

   * Se necessario, modificare il nome del tipo di record. <!--did they add a field label for this? -->
   * **Descrizione**: modificare o aggiungere una descrizione per il tipo di record con ulteriori informazioni.
   * Modificare il colore e la forma dell&#39;icona associata al tipo di record. Effettua le seguenti operazioni:
      * Selezionare un colore per identificare il tipo di record. Colore dell&#39;icona del tipo di record. Il grigio è selezionato per impostazione predefinita.
      * Seleziona un’icona dall’elenco, oppure inizia a digitare il nome di un’icona per descrivere ciò che rappresenta, quindi selezionala quando viene visualizzata. Icona del tipo di record. Per impostazione predefinita, viene selezionata un&#39;icona di file.

     ![](assets/update-record-type-box.png)

1. Fai clic su **Salva**.
1. (Facoltativo) Fai clic sulla scheda del tipo di record nell’area di lavoro per aprire la pagina del tipo di record.
1. Fai clic sul menu **Altro** a destra del nome del tipo di record, quindi fai clic su **Modifica** per aggiornare le informazioni sul tipo di record.

   >[!TIP]
   >
   >   È possibile rinominare il tipo di record nell&#39;intestazione.

   ![](assets/more-menu-options-from-record-type-page.png)

   <!--check this screen shot - not sure this is valid ???-->

1. (Facoltativo) Per modificare un altro tipo di record, espandere la freccia rivolta verso il basso a destra del nome di un tipo di record, cercare un tipo di record e selezionarlo quando viene visualizzato nell&#39;elenco.
