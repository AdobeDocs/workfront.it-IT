---
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: users-workfront-proof
title: Sposta utenti tra account utilizzando  [!DNL Workfront Proof]
description: Se sei un amministratore di  [!DNL Workfront Proof]  e hai uno o più account satellite connessi al tuo account principale, puoi spostare gli utenti tra tutti questi account.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a7cf8086-8291-4a27-abd1-afd8217f1fcc
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Sposta utenti tra account utilizzando [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

Se sei un amministratore di [!DNL Workfront] Proof e hai uno o più account satellite connessi al tuo account principale, puoi spostare gli utenti tra tutti questi account.

## Spostamento di utenti tra account connessi

1. Fare clic su **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni account]**.

1. Apri la scheda **[!UICONTROL Utenti]**.
1. Fare clic sull&#39;icona **[!UICONTROL Sposta utente]** (1). ![Sposta_utente2.png](assets/move-user2-350x95.png)

1. Nella casella Sposta utente visualizzata, confermare l&#39;utente che si desidera spostare (1).
1. Selezionare un account di destinazione dall&#39;elenco degli account connessi (2).
1. Assegna l’autorizzazione profilo (3) che questo utente deve avere sul nuovo account.
1. Seleziona un utente (4) che dovrebbe diventare proprietario degli elementi che non verranno spostati.
Ciò include gli elementi che deciderai di lasciare sul vecchio account e quelli che non puoi spostare (vedi [Elementi che non possono essere spostati](https://support.workfront.com/knowledge/articles/115004087708/en-us?brand_id=662728&return_to=%2Fhc%2Fen-us%2Farticles%2F115004087708#Items-that-can&#39;t-be-moved) di seguito).

1. Seleziona le caselle di controllo se desideri spostare le bozze (5) e i file (6) insieme all’utente.
1. Crea un nome per la cartella (7) in cui tutti gli elementi spostati verranno inseriti nel nuovo account.
1. Fare clic su **[!UICONTROL Sposta utente]** (8) per avviare il processo.
   ![Sposta_utenti_pop-up.png](assets/moving-users-pop-up-350x380.png)

Se scegli di spostare l’utente senza le relative bozze e i file, questa azione verrà eseguita immediatamente. Se scegli di spostare l’utente insieme alle relative bozze e ai file, il profilo dell’utente verrà riassegnato immediatamente, ma le bozze e i file verranno visualizzati gradualmente sull’account di destinazione, in quanto questa operazione richiede tempo per trasferire i dati.

A seconda del numero di file e di bozze, il processo di spostamento può richiedere da alcuni minuti fino ad alcune ore.

>[!NOTE]
>
>Se pensi che il processo richieda più tempo del previsto o che le bozze e/o i file spostati non vengano visualizzati sul nuovo account, contatta il nostro team di supporto.

## Elementi che non possono essere spostati

### Cartelle create o di proprietà dall&#39;utente spostato

A causa della natura delle varie autorizzazioni applicate alle cartelle e al relativo contenuto (ad esempio, possono essere condivise con altri utenti e account), non è possibile spostare le strutture di cartelle con l’utente.

Se una cartella appartiene all&#39;utente spostato, la proprietà verrà trasferita all&#39;utente selezionato (4) nella finestra a comparsa &quot;Sposta utente&quot;.

>[!NOTE]
>
>Se una cartella è stata creata dall’utente spostato, questi ne resteranno l’autore e verrà trasferita solo la proprietà. La cartella rimarrà visibile all’utente spostato nella barra laterale del nuovo account. L’utente spostato disporrà comunque dell’accesso in &quot;sola lettura&quot; agli elementi inseriti all’interno di queste cartelle.

Se non si desidera che l&#39;utente spostato mantenga tali autorizzazioni o che l&#39;utente spostato non desideri visualizzare le cartelle precedenti sull&#39;account old&amp;, la soluzione consiste nell&#39;eliminare le cartelle nel modo seguente:

1. Crea una nuova cartella sul vecchio account.
1. Sposta tutti gli elementi dalle cartelle dell&#39;utente spostato a quella appena creata.
1. Elimina tutte le cartelle lasciate dall&#39;utente spostato.

### Set di versioni con proprietari diversi

Se una bozza ha poche versioni e ciascuna di esse è di proprietà di un utente diverso, le versioni di proprietà dell’utente spostato non verranno spostate. La proprietà di tali versioni verrà trasferita a un altro utente a tua scelta (4) nella casella Sposta utente. (Per ulteriori informazioni, vedere ).

>[!NOTE]
>
>Per spostare la bozza, l’utente spostato deve essere proprietario di tutte le versioni della bozza nel set.

### Gruppi

I gruppi dovranno essere ricreati dall’utente spostato sul suo nuovo account. Per ulteriori informazioni, vedere [Creare gruppi di verifica utilizzando [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/groups/create-proofing-groups.md).

### Viste personalizzate

Le visualizzazioni personalizzate personali dovranno essere ricreate dall’utente spostato sul suo nuovo account. Per ulteriori informazioni, vedere [Creare e gestire visualizzazioni personalizzate in [!DNL Workfront Proof] Bozza](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

### Campi personalizzati

I campi personalizzati non possono essere spostati e i dati dei campi personalizzati andranno persi; pertanto, assicurati di generare i rapporti sugli elementi richiesti prima dello spostamento.

### Modelli di flusso di lavoro automatizzati

I modelli di flusso di lavoro automatizzati devono essere ricreati sul nuovo account, ma le fasi verranno mantenute nelle bozze spostate create con i modelli.

### Azioni sui commenti

Le azioni sui commenti rimarranno sulle bozze, ma non sarà più possibile filtrarle. La soluzione consiste nel creare azioni corrispondenti sul nuovo account e, se necessario, contrassegnare nuovamente i commenti con le nuove azioni.
