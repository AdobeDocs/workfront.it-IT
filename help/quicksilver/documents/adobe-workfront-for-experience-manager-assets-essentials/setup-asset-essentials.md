---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configurare l’integrazione Experience Manager Assets Essentials
description: Collega il tuo lavoro con i contenuti in Experience Manager Assets Essentials - EDIT ME.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 059cfa79c57f071b3c7efd690b583099f46c99fb
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 5%

---

# Configurare l’integrazione Experience Manager Assets Essentials

Collega il tuo lavoro con i contenuti di Experience Manager Assets Essentials &#x200B;:

* &#x200B; push di risorse e metadati da Adobe Workfront a Experience Manager Assets Essentials
* Collegare le risorse da Experience Manager Assets Essentials ai tuoi progetti e attività in Workfront &#x200B;
* Facilitare i flussi di lavoro di controllo delle versioni per le risorse inviate ad Experience Manager Assets Essentials


## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table>
  <tr>
   <td><strong>piano Adobe Workfront*</strong>
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
   <td><strong>licenza di Experience Manager</strong>
   </td>
   <td>Standard
   </td>
  </tr>
  <tr>
   <td><strong>Prodotto</strong>
   </td>
   <td>È necessario disporre di Experience Manager Assets Essentials e devi essere aggiunto al prodotto come utente nell'Admin Console.
   </td>
  </tr>
  <tr>
   <td><strong>Configurazioni a livello di accesso</strong>
   </td>
   <td>Devi essere un amministratore Workfront. Per informazioni sugli amministratori di Workfront, consulta <strong>Concedere a un utente pieno accesso amministrativo</strong>.
   </td>
  </tr>
</table>


*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.


## Configurare l’integrazione

1. Fai clic sul pulsante **Menu principale** nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione**.
1. Seleziona  **Documenti** ![icona documenti](assets/document-icon.png) nel pannello a sinistra, seleziona **Integrazione Experience Manager**.
1. Seleziona **Aggiungi integrazione Experience Manager**.
1. Specifica quanto segue:

   <table>
   <tr>
      <td><strong>Nome</strong>
      </td>
      <td>Immettere il nome che gli utenti dovranno visualizzare nel pulsante Aggiungi nuovo nell'area Documenti.
      </td>
   </tr>
   <tr>
      <td><strong>URL di navigazione</strong>
      </td>
      <td>Il sistema popola automaticamente l'URL di navigazione. Questo URL viene utilizzato per collegarsi all’istanza Assets Essentials della tua organizzazione dal menu principale per un accesso rapido.
      </td>
   </tr>
   <tr>
      <td>
      <strong>Archivio Experience Manager Assets</strong>
      </td>
      <td>
      Il sistema popola automaticamente l'archivio Experience Manager associato al tuo ID organizzazione.
      </td>
   </tr>
   </table>

1. Fai clic su **Salva** o passare alla [Impostazione dei metadati (opzionale)](#set-up-metadata-optional) in questo articolo.


## Impostazione dei metadati (opzionale)

Mappa i dati oggetto Workfront ai campi degli elementi multimediali delle risorse in Experience Manager Assets. I metadati vengono mappati quando una risorsa viene trasmessa la prima volta da Workfront.


### Prerequisiti

Prima di iniziare, devi

* Configurare uno schema di metadati in Experience Manager Assets Essentials come spiegato in [Configurare la mappatura dei metadati delle risorse tra Adobe Workfront e Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
* (Facoltativo) Configura campi modulo personalizzati in Workfront. Workfront dispone di molti campi personalizzati incorporati che è possibile utilizzare. Tuttavia, puoi anche creare campi personalizzati. Per ulteriori informazioni, consulta [Creare o modificare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).


### Risorse

I metadati vengono mappati quando una risorsa viene inviata da Workfront per la prima volta. I documenti con campi incorporati o personalizzati vengono mappati automaticamente sui campi specificati al primo invio di una risorsa a Experience Manager Assets Essentials.

1. In **Campo Workfront** scegliere un campo Workfront integrato o personalizzato.
   >[!NOTE]
   >
   >È possibile mappare un singolo campo Workfront su più campi Experience Manager Assets. Non è possibile mappare più campi Workfront su un singolo campo Experience Manager Assets.
1. In **Experience Manager** scegliere un campo Experience Manager Assets.
1. Ripetere i passaggi 1 e 2 come necessario.
   ![abilitare i metadati](assets/metadata-assets-essentials.png)
1. Fai clic su **Salva** o passare alla [Imposta cartelle collegate (facoltativo)](#set-up-linked-folders-optional) in questo articolo.


## Imposta cartelle collegate (facoltativo)

{{setup-linked-folder}}
