---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Comprendere le autorizzazioni delle cartelle in [!DNL Workfront Proof]
description: Se una persona dispone dell'autorizzazione per visualizzare un elemento in una cartella, può anche vedere la cartella stessa. Tuttavia, possono visualizzare solo gli elementi nella cartella che sono stati condivisi in modo esplicito con loro.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 96162fe8-eef9-40f4-bc94-02911b970f02
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 17%

---

# Comprendere le autorizzazioni delle cartelle in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Se una persona dispone dell&#39;autorizzazione per visualizzare un elemento in una cartella, può anche vedere la cartella stessa. Tuttavia, possono visualizzare solo gli elementi nella cartella che sono stati condivisi in modo esplicito con loro.

## Cartelle pubbliche

Se una cartella è pubblica, gli utenti dell’account (esclusi Osservatori e Utenti leggeri) possono visualizzare il nome della cartella nella barra laterale sinistra.

Il tuo profilo di autorizzazione influisce anche sui diritti che hai sulle cartelle pubbliche:

| **Profilo/Azione** | **Visualizza tutti gli elementi nella cartella** | **Vedi gli elementi condivisi in modo esplicito con loro** | **Aggiungi elementi** | **Elimina elementi** | **Aggiungi sottocartelle** | **Eliminare le sottocartelle** | **Modifica dei dettagli della cartella** |
|---|---|---|---|---|---|---|---|
| **Creatore** | Sì | Sì | Sì | Sì | Sì | Sì | Sì |
| **Amministratore fatturazione** | Sì | Sì | Sì | Sì | Sì | Sì | Sì |
| **Amministratore** | Sì | Sì | Sì | Sì | Sì | Sì | Sì |
| **Supervisore** | Sì | Sì | Sì | Sì | Sì | Sì | Sì |
| **Manager** | No | Sì | Sì | No | Sì | No | Sì |
| **Osservatore** | No | Sì | No | No | No | No | No |

{style=&quot;table-layout:auto&quot;}

Se la cartella pubblica è di proprietà di un manager, può eliminare la cartella principale e tutte le sottocartelle.

Per ulteriori informazioni, consulta [Profili delle autorizzazioni di prova in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Cartelle private

Se una cartella è privata, gli altri utenti dello stesso account non potranno visualizzare il nome della cartella nella barra laterale sinistra a meno che la cartella o gli elementi della cartella non siano stati condivisi in modo esplicito con loro o abbiano un profilo di Supervisore, Amministratore o Amministratore fatturazione:

| **Profilo/Azione** | **Visualizza tutti gli elementi nella cartella** | **Vedi gli elementi condivisi in modo esplicito con loro** | **Aggiungi elementi** | **Elimina elementi** | **Aggiungi sottocartelle** | **Eliminare le sottocartelle** | **Modifica dei dettagli della cartella** |
|---|---|---|---|---|---|---|---|
| **Creatore** | Sì | Sì | Sì | Sì | Sì | Sì | Sì |
| **Amministratore fatturazione** | Sì | Sì | Sì | Sì | Sì | Sì | Sì |
| **Amministratore** | Sì | Sì | Sì | Sì | Sì | Sì | Sì |
| **Supervisore** | Sì | Sì | Sì | Sì | Sì | Sì | Sì |
| **Manager** | No | Sì | No | No | No | No | No |
| **Osservatore** | No | Sì | No | No | No | No | No |

{style=&quot;table-layout:auto&quot;}

Se, ad esempio, si desidera che Project Manager e i relativi team visualizzino solo cartelle specifiche, Project Manager può impostare una cartella privata e quindi condividere la cartella con utenti specifici.

Quando condividi una cartella privata, puoi decidere se desideri che i responsabili siano in grado di creare, modificare ed eliminare elementi della cartella.

Puoi impostare questo valore per ogni persona singolarmente nella pagina Nuova cartella e modificarlo nella [!UICONTROL Condiviso con] della pagina dei dettagli della cartella. Per ulteriori informazioni, consulta [Crea cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) e [Gestisci cartelle e relativi contenuti in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

Se una cartella privata viene condivisa con un osservatore o , avrà accesso in sola lettura a tutti gli elementi della cartella. Per ulteriori informazioni, consulta [Profili delle autorizzazioni di prova in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) e [Condividi cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

>[!NOTE]
>
>* Se una cartella principale è privata, anche tutte le sottocartelle saranno private. Non è possibile avere una sottocartella pubblica in una cartella padre privata. È tuttavia possibile avere una sottocartella privata in una cartella principale pubblica.
>* Il Creatore e il Proprietario della cartella avranno sempre accesso ad essa e non saranno rimovibili.
>* Solo il Creatore e il Proprietario della cartella privata possono eliminare la cartella.


