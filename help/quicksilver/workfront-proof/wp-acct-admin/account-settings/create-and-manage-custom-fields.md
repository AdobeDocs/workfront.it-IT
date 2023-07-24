---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Creare e gestire campi personalizzati in [!DNL Workfront Proof]
description: A Select o Premium [!DNL Workfront] Per utilizzare questa funzione è necessario un piano. Per ulteriori informazioni sui vari piani disponibili, vedere Piani Workfront.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: 6e6cc1db8f89b76d9903905e6ee4cf9014727ba1
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 0%

---

# Creare e gestire campi personalizzati in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità del prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Bozza](../../../review-and-approve-work/proofing/proofing.md).

A Select o Premium [!DNL Workfront] Per utilizzare questa funzione è necessario un piano. Per ulteriori informazioni sui vari piani disponibili, vedere [Piani Workfront](https://www.workfront.com/plans).

I campi personalizzati ti consentono di acquisire dati aggiuntivi durante la creazione di una nuova bozza, un nuovo utente o un nuovo ospite.

Ad esempio, gli utenti che creano una nuova bozza potrebbero voler includere una sezione aggiuntiva che consenta loro di acquisire un Numero OdL, un Codice reparto o un Riferimento fornitore.

>[!NOTE]
>
>* L’acquisizione di questo tipo di informazioni nella pagina Nuova bozza tramite campi personalizzati consente inoltre di ridurre la lunghezza del nome della bozza, in quanto tali dettagli non dovranno essere inclusi nel nome. Per informazioni sulla pagina Nuova bozza, consulta &quot;Creazione di bozze in [!DNL Workfront Proof].&quot;
>
>Dopo aver utilizzato un campo personalizzato su una bozza, un utente o un contatto, non sarà più possibile eliminarlo o modificare il tipo di campo. Tuttavia, potrai nasconderlo (tramite il [!UICONTROL Impostazioni campo personalizzato] ) in modo che non venga utilizzato per i nuovi elementi.
>
>Se si rende nascosta una sezione di campo personalizzato, anche tutti i campi della sezione verranno nascosti, anche se i singoli campi sono impostati come visibili.

Questo articolo spiega come effettuare le seguenti operazioni:

## Creare campi personalizzati

Innanzitutto, devi impostare la sezione Campo personalizzato a cui aggiungere i campi personalizzati.

1. Clic **[!UICONTROL Impostazioni]** >**[!UICONTROL Impostazioni account]**, quindi aprire **[!UICONTROL Campi personalizzati]** scheda.

1. Clic **[!UICONTROL Aggiungi sezione campo personalizzato]** nel modulo appropriato (Bozza, Utenti o Contatti).
1. Digita un **Nome** per la sezione campo personalizzato, quindi fai clic su **[!UICONTROL Salva]**.

   Ora puoi impostare campi personalizzati all’interno della sezione:

1. Fai clic su **[!UICONTROL Impostazioni campi personalizzati]** per aggiornare la pagina.
1. Fai clic sul nome della nuova sezione del campo personalizzato per aprire **[!UICONTROL Campo personalizzato] sezione** per la nuova sezione.
1. Fai clic su **[!UICONTROL Nuovo campo personalizzato]** vicino all’angolo superiore destro.
1. In **[!UICONTROL Nuovo campo personalizzato]** pagina visualizzata, specifica i dettagli del campo personalizzato:

   | **Obbligatorio** | Workfront richiede agli utenti di completare il campo. |
   |---|---|
   | **Ricercabile** | Consente agli utenti di trovare elementi eseguendo ricerche nei dati del campo personalizzato. |
   | **Nascosta** | Nasconde il campo personalizzato sul [!UICONTROL Nuova bozza], Nuovo ospite e [!UICONTROL Nuovo utente] pagine |

   {style="table-layout:auto"}

1. Fai clic su **[!UICONTROL Salva]**.
1. In **Campo personalizzato** pagina visualizzata, fai clic su **[!UICONTROL Impostazioni campi personalizzati]** per aggiornare la pagina.

1. Apporta ulteriori modifiche alle impostazioni del campo:

   * Per nascondere o rendere visibile la sezione del campo personalizzato, fare clic sul pulsante **[!UICONTROL Altro]** (tre punti) a destra del nome della sezione del campo personalizzato, quindi facendo clic su **[!UICONTROL Nascondi sezione]** o **[!UICONTROL Mostra sezione]**.

   * Per nascondere o rendere visibile un campo personalizzato, fare clic sul pulsante **[!UICONTROL Altro]** (tre punti) a destra del nome della sezione del campo personalizzato, quindi facendo clic su **[!UICONTROL Nascondi campo personalizzato]** o **[!UICONTROL Mostra campo personalizzato]**.

   * Modifica l’ordine dei campi utilizzando le frecce su/giù visualizzate a destra del nome (se sono stati aggiunti più campi in una sezione).

1. Apri **[!UICONTROL Regole di visibilità]** scheda.\
   Le regole di visibilità consentono di determinare quali campi aggiuntivi visualizzare, in base al completamento del campo personalizzato iniziale. Ad esempio, se il campo dipendente è A e il campo Controllo è X, il campo A sarà visibile solo se il campo X è completato.

   È possibile utilizzare i valori di controllo per determinare i valori nel campo di controllo che, se selezionati, risulteranno visibili nel campo dipendente. Ad esempio, immaginate che il campo dipendente sia A e il campo di controllo sia X e che i valori di controllo in X siano solo le opzioni 1 e 2. Questo significa che il campo A sarà visibile solo se è selezionata l’opzione 1 o 2 del campo X. Ciò significa che se sono selezionate le opzioni 3 o 4 del campo X, il campo A non viene visualizzato. Apri **[!UICONTROL Regole di visibilità]** scheda.

   >[!NOTE]
   >
   >Solo i tipi di campo personalizzati Elenco e Radio possono essere utilizzati per il campo di controllo in una regola di visibilità, mentre il campo dipendente può essere qualsiasi tipo di campo.

   Per aggiungere una regola di visibilità:

   1. Clic **[!UICONTROL Nuova regola di visibilità]** per il modulo in cui desideri aggiungere la regola.
   1. Seleziona le impostazioni desiderate per la regola, quindi fai clic su **[!UICONTROL Salva]**.

1. Apri **[!UICONTROL Regole di dipendenza]** scheda.

   Le regole di dipendenza consentono di determinare le opzioni disponibili nel campo dipendente quando vengono selezionate determinate opzioni nel campo di controllo. Ad esempio, se il campo dipendente è &quot;B&quot; e il campo di controllo è &quot;Y&quot;, puoi impostarlo come segue:

   Se si sceglie l&#39;opzione 1 nel campo Y, vengono visualizzate solo le opzioni 1 e 2 nel campo B.

   Se si sceglie l&#39;opzione 2 nel campo Y, vengono visualizzate solo le opzioni 3 e 4 nel campo B.

   >[!NOTE]
   >
   >Per i campi dipendenti e di controllo di una regola di dipendenza è possibile utilizzare solo i tipi di campo personalizzati Elenco e Radio.

   Per aggiungere una regola di dipendenza:

   1. Clic **[!UICONTROL Nuova regola di dipendenza]** per il modulo a cui desideri aggiungere la regola.
   1. Selezionare le impostazioni desiderate per la dipendenza, quindi fare clic su **[!UICONTROL Salva]**.

## Gestire i campi personalizzati

Puoi visualizzare e modificare i dettagli della sezione del campo personalizzato o dei singoli campi personalizzati.

1. Clic **[!UICONTROL Impostazioni]** >**[!UICONTROL Impostazioni account]**, quindi aprire **[!UICONTROL Campi personalizzati]** scheda.

1. Fai clic sul nome della sezione del campo personalizzato o di un singolo campo personalizzato.
1. (Condizionale) Se gestisci una sezione di campi personalizzati, apporta una delle seguenti modifiche alla sezione **[!UICONTROL Sezione campo personalizzato]** pagina:

   * Modifica il nome della sezione.
   * Spostala in un modulo diverso.
   * Nascondi/mostra la sezione.

1. (Condizionale) Se gestisci un campo personalizzato, apporta una delle seguenti modifiche al **[!UICONTROL Campo personalizzato]** pagina:

   * Sposta il campo in un&#39;altra sezione.
   * Modifica il nome del campo.
   * Inserisci il testo della guida (accanto alla sezione del campo viene visualizzata un’icona con un punto interrogativo e il testo viene visualizzato al passaggio del mouse).
   * Attiva/disattiva il **[!UICONTROL Obbligatorio]** sul campo.
   * Attiva/disattiva il **[!UICONTROL Ricercabile]** sul campo.
   * Nascondi/scopri il campo.
   * Modifica il tipo di campo.
   * Imposta/modifica un valore predefinito per il campo.
   * Impostare le regole di visibilità e di dipendenza (come descritto in precedenza nei passaggi 11 e 12).
