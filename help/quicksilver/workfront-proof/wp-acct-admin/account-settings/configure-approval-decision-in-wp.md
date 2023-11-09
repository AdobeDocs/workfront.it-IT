---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Configurare le opzioni di decisione di approvazione in [!DNL Workfront Proof]
description: Puoi configurare le opzioni di decisione di approvazione per tutte le bozze create da [!DNL Workfront Proof] utenti dell’organizzazione.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 9e1c2a4e-0641-4334-8ff9-dbb203ccbc82
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# Configurare le opzioni di decisione di approvazione in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità del prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Bozza](../../../review-and-approve-work/proofing/proofing.md).

As a [!DNL Workfront Proof] tramite un piano Select o Premium edition, è possibile configurare le opzioni di decisione di approvazione nei modi seguenti per tutte le bozze create da [!DNL Workfront Proof] utenti dell’organizzazione:

* Modifica il nome della decisione
* Modifica l&#39;ordine delle decisioni visualizzate nel visualizzatore di bozze
* Decidere quali decisioni visualizzare

Questo articolo spiega quanto segue:

## Configurazione delle impostazioni delle decisioni

1. Clic **[!UICONTROL Impostazioni account]**.
1. Apri **[!UICONTROL Decisioni]** scheda.
1. Effettua una delle seguenti modifiche:

   * Per nascondere una decisione, fai clic su **[!UICONTROL Nascondi]** a destra della decisione non è necessario.
   * Per rinominare una decisione, fai clic sul nome della decisione, modificalo, quindi fai clic all’esterno della casella (oppure premi Invio). [!DNL Workfront Proof] aggiorna il nome della decisione su tutte le bozze esistenti nel sistema.

     >[!IMPORTANT]
     >
     >Quando lo rinomini, mantieni la logica per una decisione. Ad esempio, la decisione predefinita &quot;Rifiutato&quot; può essere modificata in &quot;Nuova versione richiesta&quot;, ma non in &quot;Invia a stampanti&quot;).

     Se desideri tornare al [!DNL Workfront Proof] impostazioni predefinite, puoi fare clic su Ripristina decisioni predefinite.

>[!NOTE]
>
>* La logica alla base delle decisioni viene utilizzata per calcolare lo stato complessivo di un flusso di lavoro di una bozza in presenza di più decisioni di vari livelli.
>* Le decisioni &quot;Approvato&quot; e &quot;Approvato con modifiche&quot; attivano la fase successiva in un flusso di lavoro automatico.
>* Se rinomini una decisione e desideri verificare la logica, puoi fare clic su **[!UICONTROL Attività]** nel pannello di navigazione a sinistra e controlla il registro attività in cui sono visualizzate le decisioni originali tra parentesi.
>
>  ![2016-12-20_1921,png](assets/2016-12-20-1921-350x132.png)>

## Creazione di motivi di decisione

I motivi decisionali sono un buon modo per acquisire informazioni aggiuntive sulla decisione relative a una bozza.

1. Clic **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni account]**.

1. Apri **[!UICONTROL Decisioni]** scheda.
Per impostazione predefinita, i motivi sono disponibili per tutti i responsabili decisionali nelle bozze, ma puoi limitarli ai soli responsabili decisionali principali.
A seconda delle tue esigenze, puoi consentire la selezione di più motivi o impostarla come elenco di scelta singolo. Puoi anche rendere i motivi obbligatori, il che significa che i revisori dovranno scegliere un motivo prima di poter salvare la decisione su una bozza.
   ![Reasons_setup.png](assets/reasons-setup-350x121.png)

1. In **[!UICONTROL Motivi]** , fare clic su **[!UICONTROL Nuovo motivo]**.
   ![Nuovo_motivo.png](assets/new-reason-350x135.png)

1. Digita un titolo per la sezione dei motivi nella casella visualizzata in **[!UICONTROL Motivo]**.
1. Se si desidera includere una casella di testo, selezionare **[!UICONTROL Casella di testo da includere]**.
1. Fai clic su **[!UICONTROL Salva]**.
   ![reason_setup_2.png](assets/reasons-setup-2-350x146.png)
Il passaggio più importante è selezionare le decisioni sulle quali devono essere visualizzate le motivazioni. Se dimentichi di farlo, i motivi non saranno mostrati sulle tue bozze.

1. Seleziona le caselle in **[!UICONTROL Motivi di visualizzazione]** nell’elenco delle decisioni nella parte superiore della pagina. Puoi selezionare una o più decisioni per i tuoi motivi.
   ![reason_decision_selection.png](assets/reasons---decision-selection-350x150.png)

## Creazione di un messaggio di post decisione

Puoi creare un messaggio di post decisione da visualizzare dopo che un revisore ha salvato la sua decisione sulla bozza.

1. Clic **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni account]**.

1. Apri **[!UICONTROL Decisioni]** scheda.
1. In **[!UICONTROL Pubblica messaggio di decisione]** , fare clic su **[!UICONTROL Modifica]** alla fine del **[!UICONTROL Messaggio]** riga.
Puoi anche decidere se desideri che il messaggio venga visualizzato a tutti i decision maker o se desideri limitarlo al principale decision maker.
   ![post_decision_message_set_png](assets/post-decision-message-set-up-350x125.png)

1. In **[!UICONTROL Visualizza messaggio]** , specifica le decisioni su cui deve essere visualizzato questo messaggio.
Se non selezioni almeno una decisione, il messaggio non verrà visualizzato sulle bozze. Assicurati di selezionare almeno una casella in questa colonna.
   ![post_decision_message_set_2.png](assets/post-decision-message-set-up-2-350x151.png)
