---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Modifica e crea tipi di rischio
description: È possibile aggiungere rischi a un progetto nella fase di pianificazione per identificare potenziali ostacoli prima dell'approvazione di qualsiasi lavoro. I rischi sono eventi possibili che potrebbero impedire il completamento del progetto nei tempi previsti o entro i limiti del budget.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 2%

---

# Modificare e creare tipi di rischio

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

È possibile aggiungere rischi a un progetto nella fase di pianificazione per identificare potenziali ostacoli prima dell&#39;approvazione di qualsiasi lavoro. I rischi sono eventi possibili che potrebbero impedire il completamento del progetto nei tempi previsti o entro i limiti del budget.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td><p>Nuovo: [!UICONTROL Standard]</p>
   Oppure
   <p>Corrente: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipi di rischi

I tipi di rischio sono etichette che è possibile utilizzare per i rischi per classificarli a scopo di reporting. Vengono creati nell&#39;area **[!UICONTROL Configurazione]** dall&#39;amministratore [!DNL Adobe Workfront]. Una volta stabiliti i tipi di rischio nell&#39;area **[!UICONTROL Configurazione]**, questi saranno universali per il sistema. Tutti i proprietari dei progetti possono utilizzare gli stessi tipi di rischio per i loro progetti.

## Modificare e creare tipi di rischio

Per impostazione predefinita, alcuni tipi di rischio sono già in [!DNL Workfront]. Per riflettere le esigenze della propria organizzazione, è possibile modificare i tipi di rischio esistenti o crearne di nuovi.

* [Modifica tipi di rischio esistenti](#edit-existing-risk-types)
* [Creare nuovi tipi di rischio](#create-new-risk-types)

### Modifica tipi di rischio esistenti {#edit-existing-risk-types}

{{step-1-to-setup}}

1. Fare clic su **[!UICONTROL Tipi di rischio]**.
1. Seleziona il tipo di rischio da modificare.
1. Fai clic su **[!UICONTROL Modifica]**.
1. (Facoltativo) Modificare il nome e la descrizione del tipo di rischio.

   I campi **[!UICONTROL Nome]** e **[!UICONTROL Descrizione]** contengono un limite di 50 caratteri.

1. Fai clic su **[!UICONTROL Salva modifiche].**

### Creare nuovi tipi di rischio {#create-new-risk-types}

È possibile creare nuovi tipi di rischio, oltre a quelli predefiniti, per riflettere le esigenze della propria organizzazione.

Per creare un nuovo tipo di rischio:

{{step-1-to-setup}}

1. Fare clic su **[!UICONTROL Tipi di rischio]**.
1. Fare clic su **[!UICONTROL Nuovo tipo di rischio]**.
1. Digitare un **[!UICONTROL Nome]** (obbligatorio) e una **[!UICONTROL Descrizione]** (facoltativo) per il tipo di rischio.

   I campi **[!UICONTROL Nome]** e **[!UICONTROL Descrizione]** contengono un limite di 50 caratteri.

1. Fare clic su **[!UICONTROL Crea tipo di rischio]**. Se hai utilizzato la modifica in linea per aggiungere il tipo di rischio, al termine fai clic su **[!UICONTROL Invio]**.

   >[!NOTE]
   >
   >Se devi modificare un tipo di rischio personalizzato, consulta la sezione [[!UICONTROL Modifica tipi di rischio esistenti]](#edit-existing-risk-types) in questo articolo.

## Allega rischi con tipi di rischio ai progetti

I tipi di rischio possono essere utilizzati per etichettare i rischi aggiunti ai progetti. Per ulteriori informazioni su come aggiungere rischi ai progetti, vedere [Creare e modificare rischi nei progetti](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
