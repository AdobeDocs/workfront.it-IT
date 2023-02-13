---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Eliminare gli utenti tramite Adobe Admin Console
description: È possibile rimuovere un utente solo da Adobe Workfront Fusion, lasciando accesso a qualsiasi altro profilo di prodotto di Adobe, oppure è possibile rimuovere l'utente completamente da Adobe Admin Console.
author: Becky
feature: Workfront Fusion
exl-id: 0d989134-46c0-4637-b465-6fbe04258b8a
hidefromtoc: true
source-git-commit: 137165deb0c0e9172224e810c82bc651bb0adfc0
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Elimina gli utenti tramite [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>La funzionalità di questo articolo è disponibile solo se l’istanza di [!DNL Adobe Workfront Fusion] è stato integrato nel [!DNL Adobe Business Platform].
>
>Per un elenco delle procedure che variano a seconda che l&#39;organizzazione sia stata integrata o meno nel [!DNL Adobe Business Platform], vedi [Differenze di amministrazione basate su piattaforma ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

È possibile rimuovere un utente da [!DNL Adobe Workfront Fusion] solo lasciando accesso a qualsiasi altro [!DNL Adobe] i profili di prodotto, oppure puoi rimuovere l’utente dal [!DNL Adobe Admin Console] interamente.

## Elimina un utente in [!DNL Adobe Workfront Fusion]

Per eliminare un utente in [!DNL Adobe Workfront Fusion], devi disattivare l’utente tramite la [!DNL Adobe Admin Console].

Un utente è disattivato dal [!DNL Adobe Admin Console] quando si applica uno dei seguenti casi:

* L’utente viene spostato da un prodotto o un profilo di prodotto e non viene assegnato ad alcun altro prodotto o profilo di prodotto.
* L’utente viene rimosso da un gruppo collegato a un profilo di prodotto e non è incluso in nessun altro gruppo collegato a un profilo di prodotto.
* L’utente viene rimosso da un profilo di prodotto e non viene assegnato a un altro profilo di prodotto.
* L&#39;utente viene eliminato o disattivato nell&#39;organizzazione che include Workfront Fusion.

   Per istruzioni, consulta la sezione &quot;Rimuovi utenti&quot; in [Gestire gli utenti individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html).

In [!DNL Workfront Fusion], la disattivazione interessa l’utente in uno dei seguenti modi:

* Se l’utente si trova in una sola organizzazione, viene disattivato.
* Se l&#39;utente si trova in più di un&#39;organizzazione, l&#39;utente viene rimosso dall&#39;organizzazione in cui l&#39;utente è stato modificato in nel [!DNL Adobe Admin Console].
* Per altre considerazioni sull&#39;eliminazione di un utente in [!DNL Workfront Fusion], vedi [Considerazioni sull’eliminazione di un utente in [!DNL Workfront Fusion]](../../workfront-fusion/organizations/manage-fusion-users.md#consider)
