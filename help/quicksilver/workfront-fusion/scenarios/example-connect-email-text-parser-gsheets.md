---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: "Esempio di scenario Adobe Workfront Fusion: connettere e-mail, parser di testo e fogli di Google"
description: Questo scenario consente di creare un registro di tutti i messaggi e-mail e di assegnarvi tag per ulteriori azioni in un foglio di calcolo. Acquisisce il corpo di un’e-mail in due tabelle separate in un foglio di calcolo utilizzando Espressioni regolari (Regex) come pattern di ricerca. Il primo modello cerca una frase, mentre il secondo cerca la stessa frase e un indirizzo e-mail.
author: Becky
feature: Workfront Fusion
exl-id: ebcfa3b9-3207-441c-9ce5-9af696c0119d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 0%

---

# Esempio di scenario [!DNL Adobe Workfront Fusion]: Connect email, [!UICONTROL Text Parser] e [!DNL Google Sheets]

Questo scenario consente di creare un registro di tutti i messaggi e-mail e di assegnarvi tag per ulteriori azioni in un foglio di calcolo. Acquisisce il corpo di un’e-mail in due tabelle separate in un foglio di calcolo utilizzando Espressioni regolari (Regex) come pattern di ricerca. Il primo modello cerca una frase, mentre il secondo cerca la stessa frase e un indirizzo e-mail.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!DNL Pro] o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Questo tutorial richiede una conoscenza di base delle espressioni regolari. Per informazioni su Regex, visita [https://regexone.com](https://regexone.com/).

Aggiungi il primo modulo e configuralo

1. Cerca e-mail e scegli **[!UICONTROL Controlla le e-mail]** come attivatore.

   >[!NOTE]
   >
   >È possibile connettere un account [!DNL Google] utilizzando il modulo Email, ma è anche possibile utilizzare un modulo [!DNL Gmail].

1. Connettere un account [!DNL Google] o qualsiasi altro client di posta elettronica basato su IMAP (ad esempio [!DNL Outlook]).
1. Una volta effettuata la connessione, selezionare una cartella di cui si desidera controllare le e-mail in arrivo, ad esempio [!UICONTROL Posta in arrivo].
1. In [!UICONTROL Criteri], scegli **[!UICONTROL Tutte le e-mail]** (o restringi la selezione per leggere o non leggere le e-mail).

   Puoi anche scegliere di contrassegnare le e-mail recuperate come lette o non lette.

1. Imposta [!UICONTROL Numero massimo di risultati] su 1.

   ![](assets/save-max-as-1-350x304.png)

   Puoi modificarlo in base al volume di messaggi che ricevi. Tuttavia, si consiglia di impostare un valore basso ed eseguire lo scenario più spesso.

1. Fai clic su **[!UICONTROL Mostra impostazioni avanzate]** in basso.

   ![](assets/show-adv-settings-350x332.png)

1. Filtra le e-mail in base al [!UICONTROL indirizzo mittente], [!UICONTROL oggetto] e [!UICONTROL frase].

   Questo ti consente di guardare solo le e-mail pertinenti. In questo esempio, è stato aggiunto solo un filtro Oggetto e sono stati lasciati vuoti gli altri 2.

   >[!NOTE]
   >
   >Aggiungeremo un router per cercare frasi in un messaggio e-mail utilizzando l&#39;iteratore [!UICONTROL Match Pattern] e un&#39;espressione regolare (Regex) come modello di ricerca. Questo ci permette anche di creare uno scenario multiutility.

1. Al termine della configurazione e quando ti viene richiesto di specificare dove iniziare a guardare le e-mail, fai clic su **[!DNL From now on]**.

   ![](assets/from-now-on-350x236.png)

1. Continua con [Cerca [!UICONTROL Controllo flusso] e aggiungi [!UICONTROL Router]](#search-for-flow-control-and-add-a-router)

## Cerca [!UICONTROL Controllo flusso] e aggiungi [!UICONTROL Router]

1. Aggiungere un router dopo qualsiasi modulo per dividere o duplicare i dati prima di inviarli al modulo successivo.

   In questo caso, è stato utilizzato un [!UICONTROL Router] per inviare il testo del corpo dell&#39;e-mail a 2 tabelle separate in un [!DNL Google Sheet].

   ![](assets/search-for-flow-control-350x220.png)

## Utilizza il modulo [!UICONTROL Parser di testo]

1. Aggiungi un trasformatore [!UICONTROL Match Pattern] per cercare una frase in un messaggio e-mail.

   Cercheremo la frase &quot;[!UICONTROL text parser module]&quot; in tutte le e-mail in arrivo per acquisire il corpo del testo e il nome del mittente di quelli che corrispondono a tale frase.

   1. Scrivere il motivo come espressione regolare:

      text\sparser\smodule

   1. (Facoltativo) Utilizzate una qualsiasi delle altre opzioni della serie.

      ![](assets/pattern-350x318.png)

      La funzione Multiriga è utile se il testo contiene più righe e se è necessario cercare il motivo in ogni riga. Per questo tutorial è necessario cercare il pattern nell’intero testo del corpo dell’e-mail, pertanto non lo selezioneremo.

   1. Nel campo [!UICONTROL Testo], fare clic sull&#39;attributo **Contenuto testo** nell&#39;elenco.

      ![](assets/text-content-350x264.png)

      Questo è l’attributo che memorizza il testo del corpo dell’e-mail in cui cercheremo il modello.

1. Aggiungi un altro [!UICONTROL Match Pattern] che cerca la stessa frase e un indirizzo e-mail.

   Questa funzione è particolarmente utile se disponi di account cliente con più utenti. Per risparmiare tempo, puoi clonare il modulo [!UICONTROL Parser di testo] appena creato e collegarlo al router.

   ![](assets/clone.png)

1. Modificate il modello come indicato di seguito:

   text\sparser\smodule.+\s([\w.-]+@[\w.-]+)

   ![](assets/text-parser-350x202.png)

   Questo modello cerca la frase &quot;[!UICONTROL text parser module]&quot; e un indirizzo e-mail come john.doe@gmail.com e restituisce solo l&#39;indirizzo e-mail.

   >[!NOTE]
   >
   >È importante scrivere il proprio regex in conformità con le specifiche degli indirizzi e-mail che si accettano, ma quello di cui sopra si occupa della maggior parte degli indirizzi e-mail standard.

   * Se desideri cercare solo l’indirizzo e-mail, puoi utilizzare il codice regex seguente:

     ([\w.-]+@[\w.-]+)

   * Puoi anche cercare solo i numeri di telefono utilizzando il codice regex seguente:

     ^[+]?\(?(\d{1,3})\)?[\s-]?\(?(\d{3})\)?[\s-]?\d{3}[\s-]?\d{3,4}
Il modello di cui sopra copre i formati più comuni in cui è scritto un numero di telefono.

   Per verificare i tuoi pattern, ti consigliamo di utilizzare [[!DNL https://regex101.com]](https://regex101.com/) con [!DNL javascript] come aroma.

   Il resto della configurazione rimane invariato rispetto a quella precedente.

## Aggiungi i moduli [!DNL Google Sheets]

Per [!DNL Sheets], è innanzitutto necessario creare un foglio di calcolo con le intestazioni richieste.

1. Crea un foglio di calcolo con le colonne sotto le quali desideri acquisire i dati utente. Puoi anche usare un file esistente.

   Ad esempio, creane una denominata &quot;Dati e-mail: ticket di supporto&quot; con le colonne Nome mittente, E-mail mittente e Contenuto e-mail. Denomina il foglio di lavoro &quot;contiene: modulo parser di testo&quot;.

1. Aggiungi il modulo [!UICONTROL Fogli Google] con **[!UICONTROL Aggiungi una riga]** come azione.

   ![](assets/add-a-row-350x174.png)

1. Connetti il tuo account [!DNL Google] (se non lo hai già fatto). Scegliere il file creato in precedenza, quindi scegliere il foglio di lavoro in cui acquisire i dati.

   La configurazione deve essere simile alla seguente:

   ![](assets/connect-google-acct-350x279.png)

1. Mappa gli attributi nei campi pertinenti (colonne) per completare la configurazione del modulo.

   ![](assets/map-attributes-350x282.png)

1. Clona il modulo appena creato e collegalo al secondo modulo [!UICONTROL Text Parser].

   1. Passare al foglio di calcolo, duplicare il foglio di lavoro creato in precedenza e assegnare un nome.

      Ad esempio, assegna al nome &quot;contiene: modulo parser di testo e e-mail&quot;.

   1. Aggiungi un’altra colonna per memorizzare l’indirizzo e-mail contenuto nel corpo dell’e-mail.

      Ad esempio, denominalo &quot;Indirizzo e-mail condiviso&quot;.

   1. Fare clic sul modulo [!DNL Google Sheets] clonato per configurare la configurazione.
   1. Sostituire il foglio di lavoro con quello appena creato.
   1. Mappa l&#39;output del modulo [!UICONTROL Match Pattern] ($1) alla colonna in cui desideri memorizzare l&#39;indirizzo e-mail (indirizzo e-mail condiviso).

      ![](assets/map-the-output.png)

      ![](assets/sender-name-350x411.png)

   1. Fai clic su **[!UICONTROL OK]**, salva lo scenario e esegui un test.

      Dovrai inviare due e-mail separate all’indirizzo e-mail connesso come segue:

      * Contenente la frase &quot;[!UICONTROL modulo parser di testo]&quot; (e nessun indirizzo e-mail)

        ![](assets/text-parser-module-350x103.png)

      * contenente la frase precedente e un indirizzo e-mail

        ![](assets/above-phrase-and-email-350x106.png)

        Se nella configurazione non sono presenti errori, il primo foglio di lavoro acquisirà tutte le e-mail contenenti la frase &quot;[!UICONTROL text parser module]&quot;, mentre il secondo foglio di lavoro acquisirà solo quelle contenenti la frase &quot;[!UICONTROL text parser module]&quot; e un indirizzo e-mail. Fai riferimento alle schermate seguenti.

        Scheda Lavoro 1:

        ![](assets/worksheet-1-350x57.png)

        Scheda Lavoro 2:

        ![](assets/worksheet-2-350x41.png)

## Risorse

* [Esercitazioni gratuite](https://regexone.com/) per informazioni sulle espressioni regolari
* [Informazioni sulla corrispondenza dei numeri di telefono](https://regexone.com/problem/matching_phone_numbers) con Regex
* [Scopri la corrispondenza e-mail](https://regexone.com/problem/matching_emails) con Regex
* [Verifica le espressioni regolari](https://regex101.com/)
