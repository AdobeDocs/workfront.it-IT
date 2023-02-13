---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Configura le opzioni relative alle decisioni di approvazione in [!DNL Workfront Proof]
description: Come [!DNL Workfront Proof] amministratore che utilizza un piano Select o Premium edition, puoi configurare le opzioni di approvazione nei seguenti modi per tutte le bozze create da [!DNL Workfront Proof] utenti della tua organizzazione - MODIFICA ME.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 9e1c2a4e-0641-4334-8ff9-dbb203ccbc82
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# Configura le opzioni relative alle decisioni di approvazione in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Come [!DNL Workfront Proof] amministratore che utilizza un piano Select o Premium edition, puoi configurare le opzioni di approvazione nei seguenti modi per tutte le bozze create da [!DNL Workfront Proof] utenti della tua organizzazione:

* Modificare il nome della decisione
* Modificare l’ordine delle decisioni visualizzate nel visualizzatore di bozze
* Decidi quali decisioni devono essere visualizzate

Questo articolo spiega quanto segue:

## Configurazione delle impostazioni delle decisioni

1. Fai clic su **[!UICONTROL Impostazioni account]**.
1. Apri **[!UICONTROL Decisioni]** scheda .
1. Apporta una delle seguenti modifiche:

   * Per nascondere una decisione, fai clic su **[!UICONTROL Nascondi]** a destra della decisione non è necessario.
   * Per rinominare una decisione, fare clic sul nome della decisione, modificarla, quindi fare clic all&#39;esterno della casella (o premere Invio). [!DNL Workfront Proof] aggiorna il nome della decisione su tutte le bozze esistenti nel sistema.

      >[!IMPORTANT]
      >
      >Mantenere la logica di una decisione quando la si rinomina. Ad esempio, la decisione predefinita &quot;Rifiutato&quot; può essere modificata in &quot;Nuova versione richiesta&quot;, ma non deve essere modificata in &quot;Invia a stampanti&quot;).

      Se desideri tornare al [!DNL Workfront Proof] Per impostazione predefinita, è possibile fare clic su Ripristina decisioni predefinite.

>[!NOTE]
>
>* La logica alla base delle decisioni viene utilizzata per calcolare lo stato complessivo di un flusso di lavoro di bozza in presenza di più decisioni di vari livelli.
>* Le decisioni &quot;Approvato&quot; e &quot;Approvato con le modifiche&quot; attivano la fase successiva in un flusso di lavoro automatico.
>* Se rinomini una decisione e desideri verificare la logica, puoi fare clic su **[!UICONTROL Attività]** nel pannello di navigazione a sinistra e controlla il registro attività dove le decisioni originali vengono visualizzate tra parentesi.
>
>  ![2016-12-20_1921.png](assets/2016-12-20-1921-350x132.png)>

## Creazione di motivi decisionali

I motivi decisionali sono un buon modo per acquisire ulteriori informazioni decisionali su una prova.

1. Fai clic su **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni account]**.

1. Apri **[!UICONTROL Decisioni]** scheda .
Per impostazione predefinita, tutte le decisioni sono disponibili per i responsabili delle prove, ma è possibile limitarle solo ai responsabili delle decisioni principali.
A seconda delle tue esigenze, puoi consentire la selezione di più motivi o renderlo un unico elenco di scelte. È inoltre possibile rendere obbligatori i motivi, il che significa che i revisori dovranno scegliere un motivo prima di poter salvare la loro decisione su una prova.
   ![Motivi_setup.png](assets/reasons-setup-350x121.png)

1. In **[!UICONTROL Motivi]** sezione, fai clic su **[!UICONTROL Nuovo motivo]**.
   ![New_reason.png](assets/new-reason-350x135.png)

1. Digitare un titolo per la sezione Motivi nella casella visualizzata in **[!UICONTROL Motivo]**.
1. Se si desidera includere una casella di testo, selezionare **[!UICONTROL Casella di testo Includi]**.
1. Fai clic su **[!UICONTROL Salva]**.
   ![reasons_setup_2.png](assets/reasons-setup-2-350x146.png)
Il passaggio più importante è quello di selezionare le decisioni che i motivi devono visualizzare. Se ti dimentichi di farlo, le ragioni non verranno mostrate sulle tue bozze.

1. Seleziona le caselle in **[!UICONTROL Motivi di visualizzazione]** nell’elenco delle decisioni nella parte superiore della pagina. Puoi selezionare una o più decisioni per i tuoi motivi.
   ![reasons_-_decision_selection.png](assets/reasons---decision-selection-350x150.png)

## Creazione di un messaggio di decisione post

È possibile creare un messaggio di decisione del post da visualizzare dopo che un revisore salva la sua decisione sulla bozza.

1. Fai clic su **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni account]**.

1. Apri **[!UICONTROL Decisioni]** scheda .
1. In **[!UICONTROL Invia messaggio di decisione]** sezione, fai clic su **[!UICONTROL Modifica]** alla fine del **[!UICONTROL Messaggio]** fila.
Puoi anche decidere se desideri che il messaggio venga visualizzato a tutti i decisori o se desideri limitarlo al decisore principale.
   ![post_decision_message_set_up.png](assets/post-decision-message-set-up-350x125.png)

1. In **[!UICONTROL Visualizza messaggio]** specifica le decisioni su cui deve essere visualizzato il messaggio.
Se non selezioni almeno una decisione, il messaggio non verrà visualizzato sulle bozze. Assicurati di selezionare almeno una casella in questa colonna.
   ![post_decision_message_set_up_2.png](assets/post-decision-message-set-up-2-350x151.png)
