---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: box
title: Cartelle della casella di sincronizzazione con  [!DNL Workfront Proof]
description: È possibile sincronizzare una cartella Box con una cartella in Workfront Proof. Ogni modifica apportata ai file nella cartella Box verrà riflessa in Workfront Proof (quindi caricamento di un nuovo file, aggiunta di una nuova versione, ridenominazione di un file e così via).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d85577f5-6aa0-40a3-a6e3-45555a3124db
source-git-commit: a6c79166c50af5bfe4c0341d003052179ce78373
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# Sincronizza [!DNL Box] Cartelle Con [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

È possibile sincronizzare una cartella [!DNL Box] con una cartella in [!DNL Workfront Proof]. Ogni modifica apportata ai file nella cartella Box verrà riflessa in Workfront Proof (quindi caricamento di un nuovo file, aggiunta di una nuova versione, ridenominazione di un file e così via).

Per ulteriori informazioni sulle cartelle, vedere [Gestire le cartelle e il relativo contenuto in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

>[!NOTE]
>
>Solo gli utenti con profili di [!UICONTROL Manager] o superiori sono in grado di sincronizzare le cartelle. L&#39;utente [!DNL Box] che carica il file in una cartella sincronizzata con [!DNL Workfront Proof] sarà il proprietario della bozza creata in [!DNL Workfront Proof] (se si tratta di un utente all&#39;interno dello stesso account [!DNL Workfront Proof]). Se l&#39;utente [!DNL Box] è un utente con un account [!DNL Workfront Proof] diverso o non dispone di un account con [!DNL Workfront Proof], l&#39;utente che ha creato la sincronizzazione tra le cartelle diventerà il proprietario della bozza. Per ulteriori informazioni, vedere *&quot;Modifica dei profili utente e delle autorizzazioni&quot;*

Per sincronizzare una cartella [!DNL Box] con una cartella in [!DNL Workfront Proof]:

1. Nel tuo account [!DNL Box], vai alla pagina [!UICONTROL Tutti i file e le cartelle].
1. Fai clic sul menu **[!UICONTROL Altre opzioni]** accanto alla cartella da sincronizzare con [!DNL Workfront Proof] (1).
1. Seleziona **[!UICONTROL Altre azioni]** (2).
1. Fare clic su **[!UICONTROL Sincronizza con[!DNL Workfront Proof]]** (3).
1. Nella casella [!UICONTROL Sincronizza cartella] visualizzata (se si è connessi a [!DNL Workfront Proof]) eseguire una delle operazioni seguenti:

   * Fare clic sul nome di una cartella [!DNL Workfront Proof] per sincronizzarla con la cartella corrispondente nella casella (4).
   * Fare clic su **[!UICONTROL Nuova cartella]** per creare una nuova cartella in [!DNL Workfront Proof] (5).\

     ![cartella_sync_2.jpg](assets/folder-sync-2-350x231.jpg)Se si è scelto di creare una nuova cartella, verrà richiesto di specificare i dettagli relativi alla nuova cartella.

1. Fai clic su **[!UICONTROL Salva]**.\
   La pagina [!UICONTROL Dettagli cartella] per la cartella sincronizzata si apre in [!DNL Workfront Proof]. Questa pagina contiene informazioni sulla cartella.\
   Questa pagina consente inoltre di sospendere e disattivare la sincronizzazione. Se si sospende la sincronizzazione, la cartella non verrà più aggiornata con le modifiche di [!DNL Box], ma la sincronizzazione potrà essere ripresa in qualsiasi momento. La disattivazione della sincronizzazione comporta l&#39;interruzione della connessione tra le cartelle e la necessità di ristabilire la sincronizzazione dall&#39;account [!DNL Box].\
   La pagina [!UICONTROL Dettagli cartella] contiene le seguenti informazioni e funzioni relative alla cartella in [!DNL Box]:

   * **[!UICONTROL Pausa sincronizzazione]**: la cartella [!DNL Workfront Proof] non verrà più aggiornata con le modifiche apportate da Box. La sincronizzazione può essere ripresa in qualsiasi momento (1).
   * **[!UICONTROL Disabilita sincronizzazione cartelle]**: la connessione tra le cartelle viene persa e la sincronizzazione dovrà essere impostata nuovamente dall&#39;account [!DNL Box] (2).

   * Solo l&#39;utente che ha avviato la sincronizzazione delle cartelle può disattivarla o interromperla. Per ulteriori informazioni, vedere [Gestione cartelle e relativo contenuto in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).
   * **Vai alla cartella [!DNL Box]**: se hai condiviso l&#39;URL della cartella (nelle opzioni della cartella [!DNL Box]), questa opzione diventerà disponibile e ti porterà direttamente alla cartella [!DNL Box] (3).
   * **[!UICONTROL Dettagli sincronizzazione cartella]**: questa sezione contiene informazioni sulla cartella [!DNL Box] (4).
   * Collegamento alla cartella **[!UICONTROL [!DNL Box]]**: URL della cartella [!DNL Box] (5).
   * **[!UICONTROL Attività]:** Visualizza i registri attività della cartella [!DNL Workfront Proof]. Qui puoi controllare chi ha avviato la sincronizzazione della cartella (6).
   * ![dettagli_cartella__1_.jpg](assets/folder-details--1--350x324.jpg)

>[!NOTE]
>
>* È inoltre possibile sincronizzare la cartella [!DNL Box] dal menu [!UICONTROL Opzioni cartella].
>* Se si dispone di una pagina di accesso [!DNL Workfront Proof] con marchio personalizzato, verrà visualizzata tale pagina anziché la pagina di accesso standard [!DNL Workfront Proof]. Se hai bisogno di ulteriori informazioni, consulta gli articoli in [Branding](https://support.workfront.com/hc/en-us/sections/115000921208-Branding).
>* Se hai attivato la funzionalità [!UICONTROL Single Sign-On (SSO)] nel tuo account [!DNL Workfront Proof], verrai reindirizzato alla pagina di accesso SSO e ti verrà richiesto di immettere le credenziali di accesso SSO, ma solo se utilizzi lo stesso indirizzo e-mail per il tuo account [!DNL Box] e [!DNL Workfront Proof]. Per ulteriori informazioni, vedere [[!UICONTROL Single Sign-On] in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).
>* Se non utilizzi lo stesso indirizzo e-mail sia per l&#39;account [!DNL Box] che per l&#39;account [!DNL Workfront Proof], verrà sempre visualizzata la pagina di accesso standard di [!DNL Workfront Proof].
>


