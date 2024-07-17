---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Crea e gestisci campi personalizzati in [!DNL Workfront Proof]
description: Per utilizzare questa funzione è necessario un Select o Premium [!DNL Workfront] Plan. Per ulteriori informazioni sui vari piani disponibili, vedere Piani Workfront.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: 6e6cc1db8f89b76d9903905e6ee4cf9014727ba1
workflow-type: tm+mt
source-wordcount: '1040'
ht-degree: 0%

---

# Crea e gestisci campi personalizzati in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

Per utilizzare questa funzione è necessario un piano Select o Premium [!DNL Workfront]. Per ulteriori informazioni sui vari piani disponibili, vedere [Piani Workfront](https://www.workfront.com/plans).

I campi personalizzati ti consentono di acquisire dati aggiuntivi durante la creazione di una nuova bozza, un nuovo utente o un nuovo ospite.

Ad esempio, gli utenti che creano una nuova bozza potrebbero voler includere una sezione aggiuntiva che consenta loro di acquisire un Numero OdL, un Codice reparto o un Riferimento fornitore.

>[!NOTE]
>
>* L’acquisizione di questo tipo di informazioni nella pagina Nuova bozza tramite campi personalizzati consente inoltre di ridurre la lunghezza del nome della bozza, in quanto tali dettagli non dovranno essere inclusi nel nome. Per informazioni sulla pagina Nuova bozza, vedere &quot;Creazione di bozze in [!DNL Workfront Proof]&quot;.
>
>Dopo aver utilizzato un campo personalizzato su una bozza, un utente o un contatto, non sarà più possibile eliminarlo o modificare il tipo di campo. Tuttavia, potrai nasconderlo (tramite la pagina [!UICONTROL Impostazioni campo personalizzato]) in modo che non venga utilizzato per i nuovi elementi.
>
>Se si rende nascosta una sezione di campo personalizzato, anche tutti i campi della sezione verranno nascosti, anche se i singoli campi sono impostati come visibili.

Questo articolo spiega come effettuare le seguenti operazioni:

## Creare campi personalizzati

Innanzitutto, devi impostare la sezione Campo personalizzato a cui aggiungere i campi personalizzati.

1. Fai clic su **[!UICONTROL Impostazioni]** >**[!UICONTROL Impostazioni account]**, quindi apri la scheda **[!UICONTROL Campi personalizzati]**.

1. Fare clic su **[!UICONTROL Aggiungi sezione campo personalizzato]** nel modulo appropriato (Bozza, Utenti o Contatti).
1. Digita un **Nome** per la sezione del campo personalizzato, quindi fai clic su **[!UICONTROL Salva]**.

   Ora puoi impostare campi personalizzati all’interno della sezione:

1. Fare clic sulla scheda **[!UICONTROL Impostazioni campi personalizzati]** per aggiornare la pagina.
1. Fai clic sul nome della nuova sezione del campo personalizzato per aprire la pagina **[!UICONTROL Sezione campo personalizzato]** per la nuova sezione.
1. Fai clic sul **[!UICONTROL nuovo campo personalizzato]** nell&#39;angolo superiore destro.
1. Nella pagina **[!UICONTROL Nuovo campo personalizzato]** visualizzata, specificare i dettagli per il campo personalizzato:

   | **Obbligatorio** | Workfront richiede agli utenti di completare il campo. |
   |---|---|
   | **Ricercabile** | Consente agli utenti di trovare elementi eseguendo ricerche nei dati del campo personalizzato. |
   | **Nascosto** | Nasconde il campo personalizzato nelle pagine [!UICONTROL Nuova bozza], Nuovo ospite e [!UICONTROL Nuovo utente] |

   {style="table-layout:auto"}

1. Fai clic su **[!UICONTROL Salva]**.
1. Nella pagina **Campo personalizzato** visualizzata, fare clic sulla scheda **[!UICONTROL Impostazioni campi personalizzati]** per aggiornare la pagina.

1. Apporta ulteriori modifiche alle impostazioni del campo:

   * Nascondi o scopri la sezione del campo personalizzato facendo clic sul menu **[!UICONTROL Altro]** (tre punti) a destra del nome della sezione del campo personalizzato, quindi facendo clic su **[!UICONTROL Nascondi sezione]** o **[!UICONTROL Scopri sezione]**.

   * Nascondere o rendere visibile il campo personalizzato facendo clic sul menu **[!UICONTROL Altro]** (tre punti) a destra del nome della sezione del campo personalizzato, quindi facendo clic su **[!UICONTROL Nascondi campo personalizzato]** o **[!UICONTROL Scopri campo personalizzato]**.

   * Modifica l’ordine dei campi utilizzando le frecce su/giù visualizzate a destra del nome (se sono stati aggiunti più campi in una sezione).

1. Apri la scheda **[!UICONTROL Regole di visibilità]**.\
   Le regole di visibilità consentono di determinare quali campi aggiuntivi visualizzare, in base al completamento del campo personalizzato iniziale. Ad esempio, se il campo dipendente è A e il campo Controllo è X, il campo A sarà visibile solo se il campo X è completato.

   È possibile utilizzare i valori di controllo per determinare i valori nel campo di controllo che, se selezionati, risulteranno visibili nel campo dipendente. Ad esempio, immaginate che il campo dipendente sia A e il campo di controllo sia X e che i valori di controllo in X siano solo le opzioni 1 e 2. Questo significa che il campo A sarà visibile solo se è selezionata l’opzione 1 o 2 del campo X. Ciò significa che se sono selezionate le opzioni 3 o 4 del campo X, il campo A non viene visualizzato. Apri la scheda **[!UICONTROL Regole di visibilità]**.

   >[!NOTE]
   >
   >Solo i tipi di campo personalizzati Elenco e Radio possono essere utilizzati per il campo di controllo in una regola di visibilità, mentre il campo dipendente può essere qualsiasi tipo di campo.

   Per aggiungere una regola di visibilità:

   1. Fare clic su **[!UICONTROL Nuova regola di visibilità]** per il modulo in cui si desidera aggiungere la regola.
   1. Seleziona le impostazioni desiderate per la regola, quindi fai clic su **[!UICONTROL Salva]**.

1. Apri la scheda **[!UICONTROL Regole di dipendenza]**.

   Le regole di dipendenza consentono di determinare le opzioni disponibili nel campo dipendente quando vengono selezionate determinate opzioni nel campo di controllo. Ad esempio, se il campo dipendente è &quot;B&quot; e il campo di controllo è &quot;Y&quot;, puoi impostarlo come segue:

   Se si sceglie l&#39;opzione 1 nel campo Y, vengono visualizzate solo le opzioni 1 e 2 nel campo B.

   Se si sceglie l&#39;opzione 2 nel campo Y, vengono visualizzate solo le opzioni 3 e 4 nel campo B.

   >[!NOTE]
   >
   >Per i campi dipendenti e di controllo di una regola di dipendenza è possibile utilizzare solo i tipi di campo personalizzati Elenco e Radio.

   Per aggiungere una regola di dipendenza:

   1. Fare clic su **[!UICONTROL Nuova regola di dipendenza]** per il modulo a cui si desidera aggiungere la regola.
   1. Selezionare le impostazioni desiderate per la dipendenza, quindi fare clic su **[!UICONTROL Salva]**.

## Gestire i campi personalizzati

Puoi visualizzare e modificare i dettagli della sezione del campo personalizzato o dei singoli campi personalizzati.

1. Fai clic su **[!UICONTROL Impostazioni]** >**[!UICONTROL Impostazioni account]**, quindi apri la scheda **[!UICONTROL Campi personalizzati]**.

1. Fai clic sul nome della sezione del campo personalizzato o di un singolo campo personalizzato.
1. (Condizionale) Se gestisci una sezione di campi personalizzati, apporta una delle seguenti modifiche alla pagina **[!UICONTROL Sezione di campi personalizzati]**:

   * Modifica il nome della sezione.
   * Spostala in un modulo diverso.
   * Nascondi/mostra la sezione.

1. (Condizionale) Se gestisci un campo personalizzato, apporta una delle seguenti modifiche alla pagina **[!UICONTROL Campo personalizzato]**:

   * Sposta il campo in un&#39;altra sezione.
   * Modifica il nome del campo.
   * Inserisci il testo della guida (accanto alla sezione del campo viene visualizzata un’icona con un punto interrogativo e il testo viene visualizzato al passaggio del mouse).
   * Abilita/disabilita l&#39;impostazione **[!UICONTROL Obbligatorio]** nel campo.
   * Abilita/disabilita l&#39;impostazione **[!UICONTROL Ricercabile]** nel campo.
   * Nascondi/scopri il campo.
   * Modifica il tipo di campo.
   * Imposta/modifica un valore predefinito per il campo.
   * Impostare le regole di visibilità e di dipendenza (come descritto in precedenza nei passaggi 11 e 12).
