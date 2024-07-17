---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Comprendere le autorizzazioni della cartella in [!DNL Workfront Proof]
description: Se un utente dispone dell'autorizzazione per visualizzare un elemento in una cartella, può anche visualizzare la cartella stessa. Tuttavia, possono visualizzare solo gli elementi nella cartella che sono stati condivisi in modo esplicito con loro.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 96162fe8-eef9-40f4-bc94-02911b970f02
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 15%

---

# Comprendere le autorizzazioni della cartella in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

Se un utente dispone dell&#39;autorizzazione per visualizzare un elemento in una cartella, può anche visualizzare la cartella stessa. Tuttavia, possono visualizzare solo gli elementi nella cartella che sono stati condivisi in modo esplicito con loro.

## Cartelle pubbliche

Se una cartella è pubblica, gli utenti dell’account (esclusi Osservatori e Utenti Light) possono visualizzarne il nome nella barra laterale a sinistra.

Il tuo profilo di autorizzazione influisce anche sui diritti di cui disponi sulle cartelle pubbliche:

| **Profilo/Azione** | **Visualizza tutti gli elementi nella cartella** | **Visualizza gli elementi condivisi in modo esplicito con loro** | **Aggiungi elementi** | **Elimina elementi** | **Aggiungi sottocartelle** | **Elimina sottocartelle** | **Modifica dettagli cartella** |
|---|---|---|---|---|---|---|---|
| **Autore** | Sì | Sì | Sì | Sì | Sì | Sì | Sì |
| **Amministratore fatturazione** | Sì | Sì | Sì | Sì | Sì | Sì | Sì |
| **Amministratore** | Sì | Sì | Sì | Sì | Sì | Sì | Sì |
| **Supervisore** | Sì | Sì | Sì | Sì | Sì | Sì | Sì |
| **Manager** | No | Sì | Sì | No | Sì | No | Sì |
| **Osservatore** | No | Sì | No | No | No | No | No |

{style="table-layout:auto"}

Se la cartella pubblica è di proprietà di un manager, quest&#39;ultimo può eliminare la cartella principale ed eventuali sottocartelle.

Per ulteriori informazioni, vedere [Profili autorizzazioni bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Cartelle private

Se una cartella è privata, gli altri utenti dello stesso account non potranno visualizzare il nome della cartella nella barra laterale a sinistra, a meno che la cartella o gli elementi nella cartella non siano stati condivisi in modo esplicito con loro o non abbiano un profilo Supervisore, Amministratore o Amministratore fatturazione:

| **Profilo/Azione** | **Visualizza tutti gli elementi nella cartella** | **Visualizza gli elementi condivisi in modo esplicito con loro** | **Aggiungi elementi** | **Elimina elementi** | **Aggiungi sottocartelle** | **Elimina sottocartelle** | **Modifica dettagli cartella** |
|---|---|---|---|---|---|---|---|
| **Autore** | Sì | Sì | Sì | Sì | Sì | Sì | Sì |
| **Amministratore fatturazione** | Sì | Sì | Sì | Sì | Sì | Sì | Sì |
| **Amministratore** | Sì | Sì | Sì | Sì | Sì | Sì | Sì |
| **Supervisore** | Sì | Sì | Sì | Sì | Sì | Sì | Sì |
| **Manager** | No | Sì | No | No | No | No | No |
| **Osservatore** | No | Sì | No | No | No | No | No |

{style="table-layout:auto"}

Se, ad esempio, si desidera che il Project Manager e i relativi team visualizzino solo cartelle specifiche, il Project Manager può impostare una cartella privata e quindi condividerla con utenti specifici.

Quando si condivide una cartella privata, è possibile decidere se si desidera che i responsabili siano in grado di creare, modificare ed eliminare gli elementi della cartella.

È possibile impostare questo valore per ogni persona singolarmente nella pagina Nuova cartella e modificarlo nella sezione [!UICONTROL Condiviso con] della pagina Dettagli cartella. Per ulteriori informazioni, vedere [Creare cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) e [Gestire le cartelle e il relativo contenuto in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

Se una cartella privata è condivisa con un osservatore o, questi disporranno dell’accesso in sola lettura a tutti gli elementi della cartella. Per ulteriori informazioni, vedere [Profili autorizzazioni bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) e [Cartelle condivise in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

>[!NOTE]
>
>* Se una cartella principale è privata, anche tutte le sottocartelle saranno private. Non è possibile avere una sottocartella pubblica in una cartella padre privata. È tuttavia possibile avere una sottocartella privata in una cartella padre pubblica.
>* Il creatore e il proprietario della cartella avranno sempre accesso alla cartella e non saranno rimovibili.
>* Solo il creatore e il proprietario della cartella privata possono eliminarla.

