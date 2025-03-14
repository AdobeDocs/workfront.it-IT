---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Creare una cartella collegata a Experience Manager Assets o Assets Essentials
description: In Workfront puoi creare una cartella collegata con Experience Manager Assets o Assets Essentials.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: e9c6a01e80d34bc873c9a06ae0782dc65afb2445
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# Creare una cartella collegata a Experience Manager Assets o Assets Essentials

In Workfront puoi creare una cartella collegata con Experience Manager Assets o Assets Essentials. Poiché la cartella è collegata, tutte le risorse aggiunte alla cartella verranno visualizzate automaticamente sia in Workfront che in Experience Manager. Se la risorsa si trova in una cartella collegata, non è necessario inviarla manualmente.

Se una risorsa viene eliminata o spostata da una cartella collegata all’interno di Experience Manager Assets o Assets Essentials, Workfront ne conserva una copia nell’area Progetto > Documenti.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Devi avere i seguenti:

<table>
  <tr>
   <td><strong>Piano Adobe Workfront*</strong>
   </td>
   <td>Qualsiasi
   </td>
  </tr>
  <tr>
   <td><strong>Licenze Adobe Workfront*</strong>
   </td>
   <td>Piano
   </td>
  </tr>
  <tr>
   <td><strong>Prodotto</strong>
   </td>
   <td>Devi disporre di Experience Manager Assets as a Cloud Service o Assets Essentials e devi essere aggiunto al prodotto come utente.
   </td>
  </tr>
  <tr>
   <td><strong>Autorizzazioni di Experience Manager</strong>
   </td>
   <td>Devi disporre dell’accesso in scrittura alla cartella di destinazione nell’integrazione di Experience Manager.
   </td>
  </tr>
  <tr>
   <td><strong>Configurazioni del livello di accesso</strong>
   </td>
   <td>Per configurare un’integrazione Experience Manager è necessario essere un amministratore di Workfront. Una volta configurata, gli utenti con una licenza Pianificazione possono impostare cartelle collegate su singoli progetti.
   </td>
  </tr>
</table>


*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront.

+++

## Prerequisiti

Prima di iniziare,

* L’amministratore di Workfront deve configurare un’integrazione Experience Manager. Per ulteriori informazioni, consulta [Configurare l&#39;integrazione Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configurare l&#39;integrazione Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Creare una cartella collegata

La cartella collegata viene creata nel percorso specificato dall’amministratore di Workfront al momento della configurazione dell’integrazione. Ogni integrazione può avere una sola posizione di cartella per le cartelle collegate.

Il nome della cartella collegata viene creato automaticamente in base al Portfolio, al Programma, al Progetto a cui è associato e non può essere modificato. Se il progetto non è associato a un Portfolio o a un Programma, nella cartella collegata verranno visualizzati il nome del progetto e la data di creazione.

>[!NOTE]
>
>Impossibile creare un nuovo documento o una nuova versione di una bozza all&#39;interno di una cartella collegata.


Per creare una cartella collegata:

1. Passa al progetto in cui desideri inserire la cartella.
1. Seleziona **Aggiungi nuovo**, quindi vai all&#39;integrazione di Experience Manager configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare specificamente Experience Manager Assets o Assets Essentials.

1. Selezionare **Crea cartella collegata**. Il sistema crea automaticamente una cartella in Experience Manager in base alla posizione specificata al momento della configurazione dell’integrazione.
   ![crea una cartella collegata](assets/linked-folder.png)
