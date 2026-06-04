---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Creare una cartella collegata a Experience Manager Assets o Assets Essentials
description: In Workfront puoi creare una cartella collegata con Experience Manager Assets o Assets Essentials.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
TQID: https://experienceleague.adobe.com/fGs1kZQXTTMioosnBsRBKKpS3q--m5PHKYg-tHrq-b8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 409
ht-degree: 13%

---

# Creare una cartella collegata a Experience Manager Assets o Assets Essentials

In Workfront puoi creare una cartella collegata con Experience Manager Assets o Assets Essentials. Poiché la cartella è collegata, tutte le risorse aggiunte alla cartella verranno visualizzate automaticamente sia in Workfront che in Experience Manager. Se la risorsa si trova in una cartella collegata, non è necessario inviarla manualmente.

Se una risorsa viene eliminata o spostata da una cartella collegata all’interno di Experience Manager Assets o Assets Essentials, Workfront ne conserva una copia nell’area Progetto > Documenti.

>[!NOTE]
>
>Questa funzionalità non è disponibile nella nuova area Documenti.<br>
>Se la tua organizzazione utilizza l&#39;archiviazione cloud Adobe, quando accedi ai documenti in Workfront visualizzerai la nuova area Documenti. Da lì puoi aggiungere risorse da Experience Manager Assets o Assets Essentials, ma non potrai creare una cartella collegata.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table>
  <tr>
   <td><strong>Pacchetto Adobe Workfront</strong>
   </td>
   <td>Qualsiasi
   </td>
  </tr>
  <tr>
   <td><strong>Licenze Adobe Workfront</strong>
   </td>
   <td>
   <p>Standard</p>
   <p>Piano</p>
   </td>
  </tr>
  <tr>
   <td><strong>Prodotti aggiuntivi</strong>
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
   <td>Per configurare un’integrazione Experience Manager è necessario essere un amministratore di Workfront. Una volta configurata, gli utenti con una licenza Standard o Plan possono impostare cartelle collegate su singoli progetti.
   </td>
  </tr>
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
