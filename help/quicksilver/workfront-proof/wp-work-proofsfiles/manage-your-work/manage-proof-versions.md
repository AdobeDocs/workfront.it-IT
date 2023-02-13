---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Gestione delle versioni di prova in [!DNL Workfront Proof]
description: La gestione del feedback in più versioni o revisioni di un pezzo di lavoro può essere una sfida enorme. [!DNL Workfront Proof] semplifica questo processo consentendo di creare e confrontare più versioni di una bozza.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d1bee64d-c091-40d3-a9c1-847c7f645b96
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 0%

---

# Gestione delle versioni di prova in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

La gestione del feedback in più versioni o revisioni di un pezzo di lavoro può essere una sfida enorme. [!DNL Workfront Proof] semplifica questo processo consentendo di creare e confrontare più versioni di una bozza.

Non esiste alcun limite al numero di versioni di una bozza che puoi creare. Quindi, se hai bisogno di passare attraverso molte revisioni con un cliente per ottenere un&#39;approvazione finale, tutte le versioni create possono essere visualizzate e facilmente gestite all&#39;interno di [!DNL Workfront Proof].

Le autorizzazioni sono specifiche per una versione, in modo da consentire a una persona di vedere una versione ma non un&#39;altra. Al contrario, se condividi una versione successiva con una persona, queste non potranno vedere le versioni precedenti a meno che tu non torni indietro e le aggiunga esplicitamente anche alle versioni precedenti.

Per creare una nuova versione di una bozza, è necessario disporre dei diritti di modifica sulla bozza.

Vedi [Gestisci ruoli di bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) per ottenere ulteriori informazioni su chi dispone di diritti di modifica su una bozza. Per ulteriori informazioni sulla creazione di versioni, consulta .

## Visualizzazione delle versioni di prova nel visualizzatore di correzione

Il nome completo della versione che stai visualizzando viene visualizzato in alto a sinistra nel visualizzatore di correzione. Qualsiasi altra versione della bozza verrà visualizzata solo come numero di versione.

1. Apri una bozza nel visualizzatore di bozze, come descritto in [Apertura di una bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/open-proof.md).
1. Nel visualizzatore di correzione, fai clic sul numero di versione a destra del nome della bozza.
1. Per visualizzare l&#39;altra versione, fare clic sul nome corrispondente nel menu visualizzato quando si fa clic sul numero di versione.
1. Per confrontare due versioni, fai clic sul pulsante **[!UICONTROL Confronta bozze]** icona.\
   ![Compare_Proofs_button.png](assets/compare-proofs-button.png)\
   Se sono presenti più versioni della bozza, puoi selezionare la versione da confrontare facendo clic sul numero di versione corrispondente su ciascun lato della schermata di suddivisione della modalità di confronto.

Per informazioni sulla revisione delle bozze in un visualizzatore di correzione, consulta [Rivedi una bozza](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md).

## Accesso alle versioni di prova tramite la pagina Dettagli di bozza

Puoi accedere a tutte le versioni di una bozza tramite la pagina dei dettagli della bozza .

1. Apri la pagina dei dettagli della bozza per una bozza, come descritto in [Gestisci dettagli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Fai clic sulla scheda delle schede delle versioni nella parte superiore della pagina e fai clic su **[!UICONTROL Vai alla bozza]** per aprire la versione desiderata nel visualizzatore di correzione.\
   ![Version_tabs_on_Proof_Details_page.png](assets/version-tabs-on-proof-details-page-350x205.png)

## Collegamento di versioni di prova

Se la bozza dispone di più versioni, la versione precedente della bozza è comunemente nota come bozza principale.

Se desideri modificare la bozza padre (versione precedente) in un&#39;altra bozza del tuo account o collegare una singola bozza a un&#39;altra bozza del tuo account (come nuova versione dell&#39;altra bozza), puoi farlo facilmente seguendo questi passaggi:

1. Apri la pagina dei dettagli della bozza per una bozza, come descritto in [Gestisci dettagli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Fai clic su **[!UICONTROL Altro]** > **[!UICONTROL Cambia versione precedente]**.

1. In **[!UICONTROL Cambia versione precedente]** nella casella visualizzata, selezionare la bozza da impostare come bozza principale (versione precedente).\
   Se hai bisogno di aiuto per trovare la bozza nell’elenco, puoi ordinare le colonne facendo clic sull’intestazione della colonna.

1. Fai clic su **[!UICONTROL Cambia versione precedente]** nella parte inferiore della casella per collegare le versioni.

>[!NOTE]
>
>Quando colleghi una bozza a un’altra bozza nel tuo account (come nuova versione), [!DNL Workfront Proof] blocca la bozza della versione precedente.

## Scollegamento delle versioni di bozza

Puoi scollegare la bozza che stai visualizzando dalla relativa bozza padre (versione precedente) senza collegarla a un’altra bozza nel tuo account:

1. Apri la pagina dei dettagli della bozza per una bozza, come descritto in [Gestisci dettagli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Fai clic su **[!UICONTROL Altro]** > **[!UICONTROL Rimuovi collegamento alla versione precedente]**.

   * Solo l’ultima versione può essere scollegata (disconnessa) dall’intero set di versioni. Diventerà quindi un&#39;unica prova.
   * Se devi inserire una versione tra due versioni esistenti, puoi scollegare tutte le versioni della stessa bozza e ricollegarle nell’ordine corretto.

## Informazioni sui set di versioni e i limiti delle prove

Ogni set di cinque versioni verrà conteggiato come una prova rispetto al limite di bozza totale.

Ad esempio, se carichi cinque versioni di una progettazione (inclusa la versione originale), questa viene conteggiata come un’unica bozza. Se carichi sei versioni di una progettazione, conta come due bozze. Undici versioni contano come tre prove e così via.

Per i file audiovisivi, ogni nuova versione viene conteggiata come una nuova bozza.
