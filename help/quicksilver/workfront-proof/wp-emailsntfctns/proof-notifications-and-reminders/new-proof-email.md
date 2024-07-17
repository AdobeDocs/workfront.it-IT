---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: E-mail nuova bozza
description: Rendi questo articolo più efficace per la PiW.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d879b1c6-e862-4653-aa93-90ad92170951
source-git-commit: 1030d4110fd5dabb3b5751387585cc66968c2326
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# E-mail nuova bozza

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

Quando crei una nuova bozza o una nuova versione di una bozza, aggiungi nuove persone a una bozza o aggiungi un flusso di lavoro a una bozza, puoi decidere di inviare un messaggio e-mail ai revisori, come spiegato in questi articoli:

* [Creare una bozza avanzata con un flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Genera bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

L&#39;e-mail che i destinatari ricevono è denominata [!UICONTROL New Proof]. Solo il creatore della bozza e gli utenti autorizzati ad aggiungere revisori a una bozza possono controllare questa e-mail. I destinatari non possono disattivarla.

L’e-mail Nuova bozza contiene:

* Il tuo messaggio personale (se scegli di includerne uno)
* Se invii sempre lo stesso messaggio personalizzato ai revisori, potrebbe essere opportuno salvarlo nelle [!UICONTROL Impostazioni personali] nella scheda [!UICONTROL Impostazioni predefinite bozza]. Per ulteriori informazioni, consulta .
* Collegamento personale alla bozza
* **[!UICONTROL Visualizza dettagli]** collegamento che ti porta all&#39;oggetto [!DNL Workfront] associato (ad esempio un progetto, un&#39;attività o un problema)
* Miniatura dell’immagine della bozza
* I seguenti dettagli della bozza:

   * Nome bozza
   * Numero di versione
   * Elenco dei revisori e progressi sulla bozza
   * Un collegamento per condividere la bozza con un altro utente

     Questo consente di condividere l’URL della bozza e/o il collegamento per il download del file originale. Ciò non consente di aggiungere in modo esplicito i revisori alla bozza, ma di condividere solo l’URL della bozza pubblica e il destinatario riceverà l’accesso in sola lettura alla bozza.

     Per ulteriori informazioni, vedere [Condividi bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

     Se non vuoi che questo collegamento venga visualizzato nell&#39;e-mail del destinatario, puoi disabilitare le impostazioni [!UICONTROL Condivisione pubblica] nella bozza

     (Scarica il file originale e l’URL pubblico). Per ulteriori informazioni, consulta [Gestione dettagli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

## Registro attività

L&#39;invio di un&#39;e-mail di [!UICONTROL Nuova bozza] a un revisore è registrato nella sezione [!UICONTROL Attività] della pagina [!UICONTROL Dettagli bozza]. Per ulteriori informazioni, vedi [Gestisci[!UICONTROL  dettagli bozza] in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md). Puoi verificare se l&#39;e-mail [!UICONTROL New Proof] è stata abilitata al momento della creazione di una bozza.

![New_Verison_email_-_activity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* Se il creatore o il proprietario della bozza ha disabilitato [!UICONTROL Proof Made] email per impostazione predefinita (nelle impostazioni personali), non riceverà alcuna [!UICONTROL Proof made] o [!UICONTROL New proof] email anche se nella pagina New proof è selezionata la casella [!UICONTROL Notify people by email] (Notifica agli utenti tramite posta elettronica). Per ulteriori informazioni, consulta .
>* Se le notifiche e-mail sono disabilitate come impostazione predefinita nelle [!UICONTROL Impostazioni account], il creatore/proprietario della bozza non riceverà alcuna e-mail di [!UICONTROL bozza creata] o [!UICONTROL Nuova bozza], anche se questa è abilitata nelle impostazioni personali e la casella [!UICONTROL Notifica] persone tramite e-mail è selezionata nella pagina Nuova bozza. Per ulteriori informazioni, [L&#39;e-mail [!UICONTROL Proof Made]](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) e vedere .
>



## Abilita l&#39;e-mail [!UICONTROL New Proof] e includi un messaggio personalizzato

Puoi specificare se inviare un avviso e-mail ai revisori su una bozza quando la crei o quando aggiungi un utente.

* [Quando crei una bozza](#when-you-create-a-proof)
* [Quando si aggiunge un revisore a una bozza](#when-you-add-a-reviewer-to-a-proof)

### Quando crei una bozza {#when-you-create-a-proof}

Quando crei una nuova bozza nella pagina [!UICONTROL Nuova bozza], nella sezione **[!UICONTROL Condividi]** puoi scegliere se inviare gli avvisi e-mail:

* Qui puoi decidere se desideri [!UICONTROL inviare una notifica via e-mail] (1). Se deselezioni questa opzione, nessuno dei revisori riceverà un’e-mail per informarlo che la bozza è pronta per la revisione.
* Puoi anche includere un messaggio personalizzato nella notifica e-mail (2).
* Se decidi di aggiungere un messaggio personalizzato, potrai inserire un oggetto personalizzato (3) e un messaggio nel corpo dell’e-mail (4).
* Per ignorare il messaggio personalizzato, fai clic sul collegamento (5).

  >[!NOTE]
  >
  >Se invii sempre lo stesso messaggio personalizzato ai revisori, potrebbe essere opportuno salvarlo nelle impostazioni Personali nella scheda [!UICONTROL Impostazioni predefinite bozza]. Per ulteriori informazioni, consulta .

![Nuova_pagina_bozza_1.png](assets/new-proof-page-1-350x186.png)

![Nuova_pagina_bozza_2.png](assets/new-proof-page-2-350x283.png)

### Quando si aggiunge un revisore a una bozza {#when-you-add-a-reviewer-to-a-proof}

Puoi selezionare se la bozza verrà notificata a un nuovo revisore aggiunto a una bozza esistente (come sopra).

* Per aggiungere nuovi revisori, fare clic sul pulsante **[!UICONTROL Condividi questa versione]** nella pagina **[!UICONTROL Dettagli bozza]** (1).

![Dettagli_bozza_pagina_1.png](assets/proof-details-page-1-350x118.png)

* Viene visualizzata una casella in cui è possibile aggiungere nuovi revisori. Puoi quindi decidere se desideri che ricevano una notifica tramite e-mail (2) e scegliere di aggiungere un messaggio personalizzato all’e-mail (3).

![Dettagli_bozza_pagina_2.png](assets/proof-details-page-2-350x174.png)

* Se scegli di aggiungere un messaggio personalizzato, la casella si espande e potrai inserire un oggetto personalizzato (4) e un testo personalizzato nel corpo dell’e-mail (5). Puoi anche ignorare il messaggio personalizzato facendo clic sul collegamento (6).

![Dettagli_bozza_pagina_3.png](assets/proof-details-page-3-350x258.png)
