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
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 2%

---

# Modificare e creare tipi di rischio

<!--Audited: 03/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Adobe Workfront dispone di una serie di tipi di rischio predefiniti che è possibile associare ai progetti nella fase di pianificazione per identificare potenziali ostacoli prima dell’approvazione di qualsiasi lavoro.

I rischi sono eventi possibili che potrebbero impedire il completamento del progetto nei tempi previsti o entro i limiti del budget.

Oltre ai tipi di rischio predefiniti, è possibile aggiungere un nuovo tipo di rischio in base alle esigenze dell&#39;organizzazione.

È possibile associare i tipi di rischio ai rischi del progetto per identificare il tipo di rischio che può presentare un progetto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipi di rischio

I tipi di rischio sono etichette che è possibile utilizzare per i rischi per classificarli a scopo di reporting.

In qualità di amministratore [!DNL Workfront], puoi creare [!UICONTROL Tipi di rischio] nell&#39;area [!UICONTROL **Configurazione**].

Dopo aver impostato i tipi di rischio, questi sono universali per il sistema.

Tutti i proprietari dei progetti possono utilizzare gli stessi tipi di rischio per i loro progetti.

## Modificare e creare tipi di rischio

Per impostazione predefinita, alcuni tipi di rischio sono già in [!DNL Workfront].


Per aumentare il numero di tipi di rischio nell’istanza di Workfront, puoi effettuare le seguenti operazioni:

* [Modifica tipi di rischio esistenti](#edit-existing-risk-types)
* [Creare tipi di rischio](#create-risk-types)

### Modifica tipi di rischio esistenti {#edit-existing-risk-types}

{{step-1-to-setup}}

1. Fare clic su **[!UICONTROL Tipi di rischio]**.
1. Seleziona il tipo di rischio da modificare.
1. Fai clic sull&#39;icona **[!UICONTROL Modifica]** ![Modifica](assets/edit-icon.png).

   Viene visualizzata la casella [!UICONTROL **Modifica tipo di rischio**].

   ![Modifica casella tipo di rischio](assets/edit-risk-type-box.png)

   >[!TIP]
   >
   >È possibile modificare le informazioni sul tipo di rischio in linea quando si fa doppio clic sul nome o sulla descrizione di un tipo di rischio in un elenco di tipi di rischio.

1. (Facoltativo) Modificare il nome e la descrizione del tipo di rischio.

   I campi **[!UICONTROL Nome]** e **[!UICONTROL Descrizione]** contengono un limite di 50 caratteri.

1. Fai clic su **[!UICONTROL Salva modifiche].**

1. (Facoltativo) Per eliminare un tipo di rischio, selezionalo nell&#39;elenco, quindi fai clic sull&#39;icona [!UICONTROL **Elimina**] ![Elimina icona](assets/delete.png), quindi fai clic su [!UICONTROL **Sì, Elimina**]. Il tipo di rischio viene eliminato e non può essere recuperato.

1. (Facoltativo) Per esportare un elenco di tipi di rischio, fare clic sull&#39;icona [!UICONTROL **Esporta**] ![Icona Esporta](assets/export-icon.png). Puoi esportare i seguenti tipi di file:

   * PDF
   * Excel
   * Excel (xlsx)
   * Delimitato in tabella

   >[!TIP]
   >
   >   È innanzitutto possibile selezionare un numero limitato di tipi di rischio e quindi esportarli per un elenco più piccolo.

### Creare tipi di rischio {#create-risk-types}

È possibile creare tipi di rischio, oltre a quelli predefiniti.

{{step-1-to-setup}}

1. Fare clic su **[!UICONTROL Tipi di rischio]**.

1. Fai clic su **[!UICONTROL Nuovo tipo di rischio]** per aprire la casella [!UICONTROL **Nuovo tipo di rischio**]

   Oppure

   Fare clic su [!UICONTROL **Aggiungi altri tipi di rischio**] nell&#39;angolo inferiore sinistro dell&#39;elenco dei tipi di rischio per aggiungere i tipi di rischio in linea.

   Viene visualizzata la casella **Nuovo tipo di rischio**.

   ![Casella nuovo tipo di rischio](assets/new-risk-type-box.png)

1. Aggiungi un **[!UICONTROL Nome]** (obbligatorio) e una **[!UICONTROL Descrizione]** (facoltativo) per il tipo di rischio.

   I campi **[!UICONTROL Nome]** e **[!UICONTROL Descrizione]** contengono un limite di 50 caratteri.

1. Fai clic su **[!UICONTROL Crea tipo di rischio]**,

   Oppure, se hai usato la modifica in linea per aggiungere il tuo tipo di rischio, al termine fai clic su **[!UICONTROL Invio]**.

   >[!TIP]
   >
   >Per modificare un tipo di rischio personalizzato, vedere la sezione [[!UICONTROL Modifica tipi di rischio esistenti]](#edit-existing-risk-types) in questo articolo.

## Allega rischi con tipi di rischio ai progetti

Puoi utilizzare i tipi di rischio per etichettare i rischi aggiunti ai progetti.

Per ulteriori informazioni su come aggiungere rischi ai progetti, vedere [Creare e modificare rischi nei progetti](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
