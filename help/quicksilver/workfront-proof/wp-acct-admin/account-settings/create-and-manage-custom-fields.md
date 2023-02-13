---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Crea e gestisci campi personalizzati in [!DNL Workfront Proof]
description: A Select o Premium [!DNL Workfront] Per utilizzare questa funzione è necessario pianificare. Per ulteriori informazioni sui vari piani disponibili, consulta Piani Workfront .
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 0%

---

# Crea e gestisci campi personalizzati in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

A Select o Premium [!DNL Workfront] Per utilizzare questa funzione è necessario pianificare. Per ulteriori informazioni sui vari piani disponibili, vedi [Piani Workfront](https://www.workfront.com/plans).

I campi personalizzati ti consentono di acquisire dati aggiuntivi durante la creazione di una nuova bozza, un nuovo utente o un nuovo ospite.

Ad esempio, gli utenti che creano una nuova bozza possono voler includere una sezione aggiuntiva che consenta loro di acquisire un numero di OdL, un codice reparto o un riferimento fornitore.

>[!NOTE]
>
>* L’acquisizione di questo tipo di informazioni nella pagina Nuova bozza tramite campi personalizzati consente inoltre di ridurre la lunghezza del nome della bozza, in quanto questi dettagli non dovranno essere inclusi nel nome. Per informazioni sulla pagina Nuova bozza, consulta &quot;Creazione di bozze in [!DNL Workfront Proof].&quot;
>
>Una volta utilizzato un campo personalizzato su una bozza, un utente o un contatto, non potrai eliminarlo o modificarlo. Tuttavia, potrai nasconderlo (tramite il [!UICONTROL Impostazioni campo personalizzato] in modo che non venga utilizzato per i nuovi elementi.
>
>Se si rende nascosta una sezione campo personalizzata, anche tutti i campi all’interno della sezione verranno nascosti se i singoli campi sono impostati come visibili.

Questo articolo spiega come effettuare le seguenti operazioni:

## Creazione di campi personalizzati

Innanzitutto, devi impostare la sezione Campo personalizzato a cui aggiungere campi personalizzati.

1. Fai clic su **[!UICONTROL Impostazioni]** >**[!UICONTROL Impostazioni account]**, quindi apri la **[!UICONTROL Campi personalizzati]** scheda .

1. Fai clic su **[!UICONTROL Aggiungi sezione campo personalizzato]** nel modulo pertinente (Proof, Users o Contatti).
1. Tipo a **Nome** per la sezione campo personalizzato, fai clic su **[!UICONTROL Salva]**.

   Ora puoi impostare campi personalizzati all’interno della sezione :

1. Fai clic sul pulsante **[!UICONTROL Impostazioni dei campi personalizzati]** per aggiornare la pagina.
1. Fai clic sul nome della nuova sezione del campo personalizzato per aprire la **[!UICONTROL Campo personalizzato] sezione** per la nuova sezione.
1. Fai clic sul pulsante **[!UICONTROL Nuovo campo personalizzato]** nell&#39;angolo in alto a destra.
1. In **[!UICONTROL Nuovo campo personalizzato]** pagina visualizzata, specifica i dettagli del campo personalizzato:

   | **Obbligatorio** | Workfront richiede agli utenti di completare il campo. |
   |---|---|
   | **Ricerca** | Consente agli utenti di trovare gli elementi ricercando nei dati del campo personalizzato. |
   | **Nascosta** | Nasconde il campo personalizzato nella [!UICONTROL Nuova prova], nuovo ospite, e [!UICONTROL Nuovo utente] pagine |

   {style=&quot;table-layout:auto&quot;}

1. Fai clic su **[!UICONTROL Salva]**.
1. In **Campo personalizzato** nella pagina visualizzata, fai clic sul pulsante **[!UICONTROL Impostazioni dei campi personalizzati]** per aggiornare la pagina.

1. Apporta ulteriori modifiche alle impostazioni del campo:

   * Per nascondere o visualizzare la sezione del campo personalizzato, fai clic sul pulsante **[!UICONTROL Altro]** (tre punti) a destra del nome della sezione campo personalizzato, quindi fare clic su **[!UICONTROL Nascondi sezione]** o **[!UICONTROL Mostra sezione]**.

   * Per nascondere o visualizzare il campo personalizzato, fai clic sul pulsante **[!UICONTROL Altro]** (tre punti) a destra del nome della sezione campo personalizzato, quindi fare clic su **[!UICONTROL Nascondi campo personalizzato]** o **[!UICONTROL Mostra campo personalizzato]**.

   * Modificare l’ordine dei campi utilizzando le frecce verso l’alto o il basso visualizzate a destra dei loro nomi (se sono stati aggiunti più campi in una sezione).

1. Apri **[!UICONTROL Regole di visibilità]** scheda .\
   Le regole di visibilità consentono di determinare quali campi aggiuntivi vengono visualizzati, in base al completamento del campo Personalizzato iniziale. Ad esempio, se il campo dipendente è A e il campo Controllo è X, significa che il campo A sarà visibile solo se il campo X è completato.

   È possibile utilizzare i valori di controllo per determinare i valori nel campo di controllo che, se selezionati, renderanno visibile il campo dipendente. Ad esempio, supponiamo che il campo dipendente sia A e il campo di controllo sia X e che i valori di controllo in X siano solo le opzioni 1 e 2. Ciò significa che il campo A sarà visibile solo se è selezionata l’opzione 1 o 2 del campo X. Ciò significa che se sono selezionate le opzioni 3 o 4 del campo X, il campo A non viene visualizzato. Apri **[!UICONTROL Regole di visibilità]** scheda .

   Per aggiungere una regola di visibilità:

   1. Fai clic su **[!UICONTROL Nuova regola di visibilità]** per il modulo in cui desideri aggiungere la regola.
   1. Seleziona le impostazioni desiderate per la regola, quindi fai clic su **[!UICONTROL Salva]**.

1. Apri **[!UICONTROL Regole di dipendenza]** scheda .

   Le regole di dipendenza consentono di determinare le opzioni disponibili nel campo dipendente quando determinate opzioni sono selezionate nel campo di controllo. Ad esempio, se il campo dipendente è &quot;B&quot; e il campo di controllo è &quot;Y&quot;, è possibile impostarlo come segue:

   Se è selezionata l’opzione 1 nel campo Y, vengono visualizzate solo le opzioni 1 e 2 nel campo B.

   Se è selezionata l’opzione 2 nel campo Y, vengono visualizzate solo le opzioni 3 e 4 nel campo B.

   Per aggiungere una regola di dipendenza:

   1. Fai clic su **[!UICONTROL Nuova regola di dipendenza]** per il modulo che desideri aggiungere la regola.
   1. Selezionare le impostazioni desiderate per la dipendenza, quindi fare clic su **[!UICONTROL Salva]**.

## Gestire i campi personalizzati

Puoi visualizzare e modificare i dettagli della sezione Campo personalizzato o dei singoli campi Personalizzato.

1. Fai clic su **[!UICONTROL Impostazioni]** >**[!UICONTROL Impostazioni account]**, quindi apri la **[!UICONTROL Campi personalizzati]** scheda .

1. Fai clic sul nome della sezione del campo personalizzato o di un singolo campo personalizzato.
1. (Condizionale) Se gestisci una sezione di campi personalizzati, apporta una delle seguenti modifiche nella sezione **[!UICONTROL Sezione campo personalizzato]** pagina:

   * Modifica il nome della sezione.
   * Spostalo in un modulo diverso.
   * Nascondere/mostrare la sezione.

1. (Condizionale) Se gestisci un campo personalizzato, apporta una delle seguenti modifiche al **[!UICONTROL Campo personalizzato]** pagina:

   * Sposta il campo in una sezione diversa.
   * Modificare il nome del campo.
   * Testo della guida di input (accanto alla sezione del campo viene visualizzata un’icona con un punto interrogativo e il testo viene visualizzato al passaggio del mouse).
   * Attiva/disattiva la **[!UICONTROL Obbligatorio]** sul campo.
   * Attiva/disattiva la **[!UICONTROL Ricerca]** sul campo.
   * Nascondere/rendere visibile il campo.
   * Modifica il tipo di campo.
   * Imposta/modifica un valore predefinito per il campo.
   * Imposta le regole di visibilità e dipendenza (come descritto sopra nei passaggi 11 e 12).
