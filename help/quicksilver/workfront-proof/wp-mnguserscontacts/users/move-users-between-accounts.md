---
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: users-workfront-proof
title: Sposta gli utenti tra gli account tramite [!DNL Workfront Proof]
description: Se sei un [!DNL Workfront Proof] amministratore e disponi di uno o più account satellitari collegati al tuo account principale, puoi spostare gli utenti tra tutti questi account.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a7cf8086-8291-4a27-abd1-afd8217f1fcc
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 0%

---

# Sposta gli utenti tra gli account tramite [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Se sei un [!DNL Workfront] L&#39;amministratore di prova e uno o più account satellitari collegati al tuo account principale, puoi spostare gli utenti tra tutti questi account.

## Spostamento di utenti tra account collegati

1. Fai clic su **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni account]**.

1. Apri **[!UICONTROL Utenti]** scheda .
1. Fai clic sul pulsante **[!UICONTROL Sposta utente]** icona (1). ![Move_user2.png](assets/move-user2-350x95.png)

1. Nella casella Sposta utente visualizzata, confermare l&#39;utente che si desidera spostare (1).
1. Selezionare un account di destinazione dall&#39;elenco degli account connessi (2).
1. Assegna l&#39;autorizzazione profilo (3) che questo utente deve avere sul nuovo account.
1. Seleziona un utente (4) che deve assumersi la proprietà degli elementi che non verranno spostati.
Ciò include gli elementi che deciderai di lasciare sul vecchio account e quelli che non possono essere spostati (vedi [Elementi che non possono essere spostati](https://support.workfront.com/knowledge/articles/115004087708/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004087708#Items-that-can&#39;t-be-moved) qui sotto).

1. Se desideri spostare le bozze (5) e i file (6) insieme all’utente, seleziona le caselle di controllo.
1. Crea un nome per la cartella (7) in cui verranno inseriti tutti gli elementi spostati sul nuovo account.
1. Fai clic su **[!UICONTROL Sposta utente]** (8) avviare il processo.
   ![Moving_users_pop-up.png](assets/moving-users-pop-up-350x380.png)

Se scegli di spostare l’utente senza le relative bozze e file, questa azione verrà eseguita immediatamente. Se scegli di spostare l’utente insieme alle relative bozze e file, il profilo dell’utente verrà riassegnato immediatamente, ma le bozze e i file verranno visualizzati gradualmente sull’account di destinazione in quanto questa operazione richiede tempo per trasferire i dati.

A seconda del numero di file e di prove in movimento il processo può richiedere qualcosa da pochi minuti a poche ore.

>[!NOTE]
>
>Se pensi che il processo richieda più tempo del previsto o che le bozze e/o i file spostati non vengano visualizzati sul nuovo account, contatta il nostro team di assistenza.

## Elementi che non possono essere spostati

### Cartelle create o possedute dall&#39;utente spostato

A causa della natura di varie autorizzazioni applicate alle cartelle e al relativo contenuto (ad esempio, possono essere condivise con altri utenti e account) non è possibile spostare le strutture di cartelle con l&#39;utente.

Se una cartella è di proprietà dell&#39;utente spostato, la proprietà verrà trasferita all&#39;utente selezionato (4) nella finestra a comparsa &quot;Sposta utente&quot;.

>[!NOTE]
>
>Se una cartella è stata creata dall’utente spostato, rimarrà il suo creatore, verrà trasferita solo la proprietà. La cartella rimarrà visibile all’utente spostato nella barra laterale del nuovo account. L&#39;utente spostato avrà ancora accesso in sola lettura agli elementi inseriti all&#39;interno di queste cartelle.

Se non desideri che l&#39;utente spostato mantenga tali autorizzazioni o che l&#39;utente spostato non desideri vedere le vecchie cartelle sul vecchio account, la soluzione qui sarebbe quella di eliminare le cartelle come segue:

1. Crea una nuova cartella sul vecchio account.
1. Sposta tutti gli elementi dalle cartelle dell&#39;utente spostato a quello appena creato.
1. Elimina tutte le cartelle lasciate dall&#39;utente spostato.

### Set di versioni con proprietari diversi

Se una bozza ha alcune versioni e ciascuna di esse è di proprietà di un utente diverso, le versioni di proprietà dell’utente spostato non verranno spostate. La proprietà di tali versioni verrà trasferita a un altro utente secondo la tua scelta (4) nella casella Sposta utente. (Per ulteriori informazioni, consulta .)

>[!NOTE]
>
>Per spostare la bozza, un utente spostato deve possedere tutte le versioni di bozza del set.

### Gruppi

I gruppi dovranno essere ricreati dall&#39;utente spostato sul nuovo account. Per ulteriori informazioni, consulta [Creare gruppi di correzione utilizzando [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/groups/create-proofing-groups.md).

### Viste personalizzate

Le visualizzazioni personalizzate personali dovranno essere ricreate dall’utente spostato sul nuovo account. Per ulteriori informazioni, consulta [Creare e gestire visualizzazioni personalizzate in [!DNL Workfront Proof] Prova](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

### Campi personalizzati

Non è possibile spostare i campi personalizzati e i dati dei campi personalizzati andranno persi; assicurati quindi di generare i rapporti sugli elementi richiesti prima dello spostamento.

### Modelli di flusso di lavoro automatizzati

I modelli di flusso di lavoro automatizzati devono essere ricreati nel nuovo account, ma le fasi verranno mantenute nelle bozze spostate create con i modelli.

### Azioni sui commenti

Le azioni sui commenti rimarranno sulle bozze, ma non sarà più possibile filtrarle. La soluzione consisterebbe nel creare azioni corrispondenti sul nuovo account e contrassegnare i commenti con le nuove azioni, se necessario.
