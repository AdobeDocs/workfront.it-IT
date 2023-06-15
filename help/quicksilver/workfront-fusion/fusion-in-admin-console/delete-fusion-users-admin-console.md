---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Eliminare gli utenti tramite Adobe Admin Console
description: Puoi rimuovere un utente solo da Adobe Workfront Fusion, lasciando l’accesso a qualsiasi altro profilo di prodotto di Adobe, oppure puoi rimuovere completamente l’utente da Adobe Admin Console.
author: Becky
feature: Workfront Fusion
exl-id: 0d989134-46c0-4637-b465-6fbe04258b8a
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Elimina utenti tramite [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>La funzionalità di questo articolo è disponibile solo se l’istanza di [!DNL Adobe Workfront Fusion] è stato acquisito in [!DNL Adobe Business Platform].
>
>Per un elenco di procedure che differiscono in base al fatto che la tua organizzazione sia stata caricata su [!DNL Adobe Business Platform], vedi [Differenze di amministrazione basate sulla piattaforma ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

È possibile rimuovere un utente da [!DNL Adobe Workfront Fusion] solo, lasciando accesso a qualsiasi altro [!DNL Adobe] profili di prodotto, oppure puoi rimuovere l’utente dal [!DNL Adobe Admin Console] interamente.

## Eliminare un utente in [!DNL Adobe Workfront Fusion]

Per eliminare un utente in [!DNL Adobe Workfront Fusion], è necessario disattivare l&#39;utente tramite [!DNL Adobe Admin Console].

Un utente viene disattivato dalla [!DNL Adobe Admin Console] quando si verifica una delle condizioni seguenti:

* L’utente viene spostato da un prodotto o profilo di prodotto e non viene assegnato ad alcun altro prodotto o profilo di prodotto.
* L’utente viene rimosso da un gruppo collegato a un profilo di prodotto e non viene incluso in alcun altro gruppo collegato a un profilo di prodotto.
* L’utente viene rimosso da un profilo di prodotto e non viene assegnato a un altro profilo di prodotto.
* L’utente viene eliminato o disattivato nell’organizzazione che include Workfront Fusion.

  Per istruzioni, consulta la sezione &quot;Rimuovere gli utenti&quot; in [Gestire gli utenti singolarmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html).

In entrata [!DNL Workfront Fusion], la disattivazione influisce sull’utente in uno dei seguenti modi:

* Se l’utente fa parte di una sola organizzazione, viene disattivato.
* Se l’utente fa parte di più organizzazioni, viene rimosso da quella in cui è stato modificato nel [!DNL Adobe Admin Console].
* Per altre considerazioni durante l’eliminazione di un utente in [!DNL Workfront Fusion], vedi [Considerazioni durante l’eliminazione di un utente in [!DNL Workfront Fusion]](../../workfront-fusion/organizations/manage-fusion-users.md#consider)
