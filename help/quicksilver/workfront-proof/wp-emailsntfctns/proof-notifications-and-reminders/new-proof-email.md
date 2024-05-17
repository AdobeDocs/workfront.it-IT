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
>Questo articolo fa riferimento alle funzionalità del prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Bozza](../../../review-and-approve-work/proofing/proofing.md).

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

Quando crei una nuova bozza o una nuova versione di una bozza, aggiungi nuove persone a una bozza o aggiungi un flusso di lavoro a una bozza, puoi decidere di inviare un messaggio e-mail ai revisori, come spiegato in questi articoli:

* [Creare una bozza avanzata con un flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Generare bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

L’e-mail che i destinatari ricevono è denominata [!UICONTROL Nuova bozza] e-mail. Solo il creatore della bozza e gli utenti autorizzati ad aggiungere revisori a una bozza possono controllare questa e-mail. I destinatari non possono disattivarla.

L’e-mail Nuova bozza contiene:

* Il tuo messaggio personale (se scegli di includerne uno)
* Se invii sempre lo stesso messaggio personalizzato ai revisori, potrebbe essere utile salvarlo nel [!UICONTROL Impostazioni personali] sotto [!UICONTROL Valori predefiniti bozza] scheda. Per ulteriori informazioni, consulta .
* Collegamento personale alla bozza
* **[!UICONTROL Visualizza dettagli]** collegamento che ti porta al [!DNL Workfront] oggetto (ad esempio un progetto, un’attività o un problema)
* Miniatura dell’immagine della bozza
* I seguenti dettagli della bozza:

   * Nome bozza
   * Numero di versione
   * Elenco dei revisori e progressi sulla bozza
   * Un collegamento per condividere la bozza con un altro utente

     Questo consente di condividere l’URL della bozza e/o il collegamento per il download del file originale. Ciò non consente di aggiungere in modo esplicito i revisori alla bozza, ma di condividere solo l’URL della bozza pubblica e il destinatario riceverà l’accesso in sola lettura alla bozza.

     Consulta [Condividere una bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) per ulteriori informazioni.

     Se non desideri che il collegamento venga visualizzato nell’e-mail del destinatario, puoi disattivare la funzione [!UICONTROL Condivisione pubblica] impostazioni della bozza

     (Scarica il file originale e l’URL pubblico). Consulta [Gestire i dettagli della bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) per ulteriori informazioni.

## Registro attività

Invio di un [!UICONTROL Nuova bozza] l’e-mail a un revisore ha effettuato l’accesso a [!UICONTROL Attività] sezione di [!UICONTROL Dettagli bozza] pagina. Consulta  [Gestisci[!UICONTROL  Dettagli bozza] in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) per ulteriori informazioni. Puoi verificare se [!UICONTROL Nuova bozza] l’e-mail era abilitata al momento della creazione di una bozza.

![New_Verison_email_-_activity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* Se l’Autore o il Proprietario della bozza ha [!UICONTROL Bozza eseguita] e-mail disabilitate per impostazione predefinita (nelle impostazioni personali), non riceveranno alcuna [!UICONTROL Bozza effettuata] o [!UICONTROL Nuova bozza] e-mail anche se [!UICONTROL Notifica agli utenti via e-mail] nella pagina Nuova bozza. Per ulteriori informazioni, consulta .
>* Se le notifiche e-mail sono disabilitate come impostazione predefinita nel [!UICONTROL Impostazioni account] Il creatore/proprietario della bozza non riceverà alcuna [!UICONTROL Bozza effettuata] o [!UICONTROL Nuova bozza] e-mail anche se questa opzione è abilitata nelle impostazioni personali e nella [!UICONTROL Notifica] persone per e-mail è selezionata nella pagina Nuova bozza. Per ulteriori informazioni, [Il [!UICONTROL Bozza eseguita] email](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) e vedi.
>



## Abilita [!UICONTROL Nuova bozza] e-mail e includi un messaggio personalizzato

Puoi specificare se inviare un avviso e-mail ai revisori su una bozza quando la crei o quando aggiungi un utente.

* [Quando crei una bozza](#when-you-create-a-proof)
* [Quando si aggiunge un revisore a una bozza](#when-you-add-a-reviewer-to-a-proof)

### Quando crei una bozza {#when-you-create-a-proof}

Quando crei una nuova bozza in [!UICONTROL Nuova bozza] pagina, sotto **[!UICONTROL Condividi]** , puoi scegliere se inviare gli avvisi e-mail:

* Qui puoi decidere se desideri [!UICONTROL Notifica agli utenti via e-mail] (1) Se deselezioni questa opzione, nessuno dei revisori riceverà un’e-mail per informarlo che la bozza è pronta per la revisione.
* Puoi anche includere un messaggio personalizzato nella notifica e-mail (2).
* Se decidi di aggiungere un messaggio personalizzato, potrai inserire un oggetto personalizzato (3) e un messaggio nel corpo dell’e-mail (4).
* Per ignorare il messaggio personalizzato, fai clic sul collegamento (5).

  >[!NOTE]
  >
  >Se invii sempre lo stesso messaggio personalizzato ai revisori, potrebbe essere utile salvarlo nelle impostazioni Personali in [!UICONTROL Valori predefiniti bozza] scheda. Per ulteriori informazioni, consulta .

![New_Proof_page_1.png](assets/new-proof-page-1-350x186.png)

![New_Proof_page_2.png](assets/new-proof-page-2-350x283.png)

### Quando si aggiunge un revisore a una bozza {#when-you-add-a-reviewer-to-a-proof}

Puoi selezionare se la bozza verrà notificata a un nuovo revisore aggiunto a una bozza esistente (come sopra).

* Per prima cosa, aggiungi nuovi revisori facendo clic sul pulsante **[!UICONTROL Condividi questa versione]** pulsante sulla **[!UICONTROL Dettagli bozza]** pagina (1).

![Proof_Details_page_1.png](assets/proof-details-page-1-350x118.png)

* Viene visualizzata una casella in cui è possibile aggiungere nuovi revisori. Puoi quindi decidere se desideri che ricevano una notifica tramite e-mail (2) e scegliere di aggiungere un messaggio personalizzato all’e-mail (3).

![Proof_Details_page_2.png](assets/proof-details-page-2-350x174.png)

* Se scegli di aggiungere un messaggio personalizzato, la casella si espande e potrai inserire un oggetto personalizzato (4) e un testo personalizzato nel corpo dell’e-mail (5). Puoi anche ignorare il messaggio personalizzato facendo clic sul collegamento (6).

![Proof_Details_page_3.png](assets/proof-details-page-3-350x258.png)
