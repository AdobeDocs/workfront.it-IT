---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli e-mail
description: In una [!DNL Adobe Workfront Fusion] In questo caso, è possibile collegare il tuo account Email a più applicazioni e servizi di terze parti. Questo consente di scaricare e-mail tramite IMAP, inviare e-mail tramite SMTP, creare nuove bozze, spostare e copiare e-mail da una cartella a un'altra, contrassegnare e-mail come lette o non lette ed eliminare le e-mail.
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2613'
ht-degree: 0%

---

# Moduli e-mail

In una [!DNL Adobe Workfront Fusion] In questo caso, è possibile collegare il tuo account Email a più applicazioni e servizi di terze parti. Questo consente di scaricare e-mail tramite IMAP, inviare e-mail tramite SMTP, creare nuove bozze, spostare e copiare e-mail da una cartella a un&#39;altra, contrassegnare e-mail come lette o non lette ed eliminare le e-mail.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o superiore</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Collegare l&#39;e-mail a Workfront Fusion {#connect-your-email-to-workfront-fusion}

* [Connessione a Google](#connect-to-google)
* [Connessione ad altri servizi e-mail (SMAP)](#connect-to-other-email-services-smap)

### Connetti a [!DNL Google]

Utilizza questa opzione per creare scenari con moduli e-mail che richiedono una connessione al tuo [!DNL Google] conto. Questo è un account con ambito limitato.

Puoi creare una connessione al tuo [!DNL Google] account direttamente da un modulo Email.

1. In qualsiasi modulo Email, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo .
1. Seleziona **[!DNL Google]** come tipo di connessione.
1. Immettere un nome per la connessione.
1. (Facoltativo) Inserisci il tuo [!UICONTROL [!DNL Google] ID client] e [!UICONTROL Segreto client].
1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo .

### Connessione ad altri servizi e-mail (SMAP)

La connessione SMAP consente di accedere alla cassetta postale in remoto e di leggere o manipolare i messaggi nella cassetta postale. La connessione SMAP viene utilizzata dalla maggior parte dei moduli e-mail.

1. In qualsiasi modulo Email, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo .
1. Seleziona **[!UICONTROL Altro (SMTP)]** come tipo di connessione.
1. Inserisci un **[!UICONTROL Nome]** per la connessione.
1. Seleziona la tua **[!UICONTROL Fornitore e-mail]** dall&#39;elenco. Se il provider di posta elettronica non è presente nell’elenco, selezionare Altro.
1. Inserisci il tuo **[!UICONTROL Indirizzo e-mail]**, **[!UICONTROL Nome completo]**, il **[!UICONTROL Nome utente]** e le **[!UICONTROL Password]**.
1. (Condizionale) Se il provider non è presente nell’elenco, immetti il **[!UICONTROL Server SMTP]** e **[!UICONTROL Porta]** e specifica se desideri **[!UICONTROL Utilizzare una connessione sicura (TLS)]**. Per trovare queste informazioni, controlla il [!UICONTROL Aiuto] sezione per la cassetta postale. Se non disponi di queste informazioni, contatta il provider di servizi e-mail.
1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo .

## [!UICONTROL E-mail] moduli e relativi campi

Quando si configura [!UICONTROL E-mail] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati campi aggiuntivi, a seconda di fattori come il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Alcuni campi e-mail potrebbero contenere già dati, in quanto sono stati utilizzati in un altro modulo dello scenario. Se hai bisogno di informazioni, consulta la documentazione della guida e-mail .

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>ID e-mail univoco noto come &quot;[!UICONTROL ID e-mail (UID)]&#39; è l&#39;identificatore dell&#39;e-mail. L’ID e-mail è specifico per ciascuna cartella dell’e-mail.

* [Triggers](#triggers)
* [Azioni](#actions)
* [Iteratori](#iterators)

### Triggers

#### [!UICONTROL Guarda le e-mail]

Viene attivato quando viene ricevuta una nuova e-mail per l’elaborazione in base a criteri specifici.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account e-mail a [!UICONTROL Workfront Fusion], vedi <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Collega il tuo messaggio e-mail a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella] </td> 
   <td> <p>Seleziona la cartella che contiene le e-mail che desideri controllare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Criteri di [!UICONTROL]</p> </td> 
   <td> <p>Seleziona i criteri in base ai quali desideri visualizzare le e-mail:</p> 
    <ul> 
     <li>[!UICONTROL Tutte Le E-Mail]</li> 
     <li>[!UICONTROL Leggi e-mail]</li> 
     <li>[!UICONTROL Solo e-mail non lette]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Indirizzo e-mail mittente] </td> 
   <td> <p>Immetti l’indirizzo e-mail del mittente di cui desideri visualizzare le e-mail.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Indirizzo e-mail destinatario]</td> 
   <td> <p> Immetti l’indirizzo e-mail del destinatario di cui desideri visualizzare le e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Inserisci l’oggetto dell’e-mail che desideri visualizzare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Frase] </td> 
   <td> <p>Immetti qualsiasi parola chiave per guardare solo le e-mail contenenti frasi specifiche.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Segna i messaggi letti al momento del recupero]</td> 
   <td> <p>Abilita questa opzione per contrassegnare l’e-mail non letta come letta dopo il recupero dei dettagli.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di risultati]</td> 
   <td> <p> Numero massimo di e-mail [!DNL Workfront Fusion] dovrebbe essere restituito durante un ciclo di esecuzione di uno scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Invia un messaggio e-mail]](#send-an-email)
* [[!UICONTROL Creare una bozza]](#create-a-draft)
* [[!UICONTROL Contrassegna e-mail come letto]](#mark-an-email-as-read)
* [[!UICONTROL Contrassegna e-mail come non letto]](#mark-an-email-as-unread)
* [[!UICONTROL Sposta un’e-mail]](#move-an-email)
* [[!UICONTROL Copiare un messaggio e-mail]](#copy-an-email)
* [[!UICONTROL Eliminare un messaggio e-mail]](#delete-an-email)
* [[!UICONTROL Ottieni e-mail]](#get-emails)
* [[!UICONTROL Invia un&#39;e-mail]](#send-me-an-email)

#### [!UICONTROL Invia un messaggio e-mail]

Invia un nuovo messaggio e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account e-mail a [!DNL Workfront Fusion], vedi <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Collega il tuo messaggio e-mail a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salva messaggio dopo l’invio]</td> 
   <td>Dopo l’invio del messaggio e-mail, questo verrà salvato nella tua casella di posta. Abilita questa opzione se desideri salvare le e-mail inviate utilizzando [!DNL Workfront Fusion] al <i>[!UICONTROL Posta inviata]</i> cartella o altra cartella nella cassetta postale. Alcuni servizi e-mail, ad esempio [!DNL Gmail], salva automaticamente i messaggi inviati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL A] </td> 
   <td> <p>Aggiungi gli indirizzi e-mail a cui desideri inviare il messaggio e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Immetti o mappa l’oggetto dell’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
   <td> <p>Seleziona il tipo di contenuto per l’e-mail:</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Plaintext]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content] </td> 
   <td> <p>Inserisci o mappa il contenuto dell’e-mail in formato HTML utilizzando i tag HTML o nel testo normale, a seconda di ciò che hai scelto nel campo [!UICONTROL Content Type] (Tipo di contenuto).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Allegati]</p> </td> 
   <td> <p>Aggiungi un allegato:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Immettere il nome del file. Ad esempio, sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Immettere il percorso della cartella in cui caricare l'allegato.</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>Inserisci l’ [!UICONTROL content ID] per inserire l’allegato (immagine) nel contenuto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copia destinatario] </td> 
   <td> <p>Immetti o mappa uno o più indirizzi e-mail a cui desideri inviare una copia di questo messaggio e-mail. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destinatario copia cieca]</td> 
   <td> <p> Immetti o mappa uno o più indirizzi e-mail a cui desideri inviare una copia di questo messaggio e-mail senza che l’indirizzo e-mail venga visualizzato nell’e-mail.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL DA] </td> 
   <td> <p>Immetti o mappa l’indirizzo e-mail (e il nome, se necessario) visualizzato nel campo [!UICONTROL Da] nell’e-mail. </p> <p>Importante: Utilizza la sintassi corretta: <code>name@email.com</code> o <code>"Name" name@email.com</code>.</p> <p>Nota: Normalmente, [!DNL Workfront Fusion] utilizza l’indirizzo e-mail immesso al momento della creazione della connessione come indirizzo del mittente. Se immetti un altro indirizzo e-mail, potrebbe verificarsi un errore durante l’invio di un messaggio, perché il tuo account potrebbe non disporre dell’autorizzazione per l’invio di e-mail da un indirizzo diverso dal tuo. Ad esempio <code>test@mail.com</code> o "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>Immetti o mappa l’indirizzo e-mail visualizzato nel campo [!UICONTROL Sender] nell’e-mail.</p> <p>Suggerimento: Se non sei sicuro se utilizzare questo campo o il campo Da, ti consigliamo di scegliere il campo Da.</p> <p>Importante: Utilizza la sintassi corretta: <code>name@email.com</code> o <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Risposta [!UICONTROL]</td> 
   <td> <p> Se desideri che le risposte a questa e-mail vengano inviate a un indirizzo diverso da quello "Da", inserisci l’indirizzo e-mail in cui desideri ricevere le risposte a questa e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL In-Reply-To]</td> 
   <td> <p> Se rispondi a un’e-mail specifica, immetti o mappa l’ID dell’e-mail a cui stai rispondendo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Riferimenti </td> 
   <td> <p>Immetti gli ID del messaggio di tutte le risposte nel thread.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Priority]</p> </td> 
   <td> <p>Seleziona la priorità dell’e-mail:</p> 
    <ul> 
     <li>[!UICONTROL High]</li> 
     <li>[!UICONTROL Normale]</li> 
     <li>[!UICONTROL Bassa]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
   <td> <p>Aggiungi le intestazioni:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>Aggiungi la chiave. Ad esempio, [!UICONTROL Sender], [!UICONTROL Date], [!UICONTROL To] e così via.</p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Immetti il valore della chiave.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare una bozza]

Crea e aggiunge una nuova bozza a una cartella selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account e-mail a [!UICONTROL Workfront Fusion], vedi <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Collega il tuo messaggio e-mail a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella]</td> 
   <td>Seleziona la cartella in cui desideri creare la bozza dell’e-mail.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL A] </td> 
   <td> <p>Immetti o mappa l’indirizzo e-mail a cui desideri inviare l’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Immetti o mappa l’oggetto dell’e-mail.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
   <td> <p>Seleziona il tipo di contenuto dell’e-mail:</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Testo normale]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content] </td> 
   <td> <p>Inserisci o mappa il contenuto dell’e-mail in formato HTML utilizzando i tag HTML o nel testo normale, a seconda di ciò che hai scelto nel campo [!UICONTROL Content Type] (Tipo di contenuto).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Allegati]</p> </td> 
   <td> <p>Aggiungi un allegato:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Immettere il nome del file. Ad esempio, sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Immettere il percorso della cartella in cui caricare l'allegato.</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>Immetti l’ID contenuto per inserire l’allegato (immagine) nel contenuto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copia destinatario] </td> 
   <td> <p>Immetti o mappa uno o più indirizzi e-mail a cui desideri inviare una copia di questo messaggio e-mail. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destinatario copia cieca]</td> 
   <td> <p> Immetti o mappa uno o più indirizzi e-mail a cui desideri inviare una copia di questo messaggio e-mail senza che l’indirizzo e-mail venga visualizzato nell’e-mail.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL DA] </td> 
   <td> <p>Immetti o mappa l’indirizzo e-mail (e il nome, se necessario) visualizzato nel campo [!UICONTROL Da] nell’e-mail. </p> <p>Importante: Utilizza la sintassi corretta: <code>name@email.com</code> o <code>"Name" name@email.com</code>.</p> <p>Nota: Normalmente, [!DNL Workfront Fusion] utilizza l’indirizzo e-mail immesso al momento della creazione della connessione come indirizzo del mittente. Se immetti un altro indirizzo e-mail, potrebbe verificarsi un errore durante l’invio di un messaggio, perché il tuo account potrebbe non disporre dell’autorizzazione per l’invio di e-mail da un indirizzo diverso dal tuo. Ad esempio <code>test@mail.com</code> o "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>Immetti o mappa l’indirizzo e-mail visualizzato nel campo [!UICONTROL Sender] nell’e-mail.</p> <p>Suggerimento: Se non sei sicuro se utilizzare questo campo o il campo Da, ti consigliamo di scegliere il campo Da.</p> <p>Importante: Utilizza la sintassi corretta: <code>name@email.com</code> o <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Risposta [!UICONTROL]</td> 
   <td> <p> Se desideri che le risposte a questa e-mail vengano inviate a un indirizzo diverso da quello "[!UICONTROL da]", inserisci l’indirizzo e-mail in cui desideri ricevere le risposte a questa e-mail.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL In-Reply-To]</td> 
   <td> <p> Se rispondi a un’e-mail specifica, immetti o mappa l’ID dell’e-mail a cui stai rispondendo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Riferimenti </td> 
   <td> <p>Immetti gli ID del messaggio di tutte le risposte nel thread.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Priority]</p> </td> 
   <td> <p>Seleziona la priorità dell’e-mail:</p> 
    <ul> 
     <li>[!UICONTROL High]</li> 
     <li>[!UICONTROL Normale]</li> 
     <li>[!UICONTROL Bassa]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
   <td> <p>Aggiungi le intestazioni:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>Aggiungi la chiave. Ad esempio, Mittente, Data, A e così via.</p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Immetti il valore della chiave.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Contrassegna e-mail come letto]

Contrassegna un messaggio e-mail o una bozza in una cartella selezionata come letto impostando [!UICONTROL Leggi] bandiera.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account e-mail a [!UICONTROL Workfront Fusion], vedi <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Collega il tuo messaggio e-mail a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella]</td> 
   <td>Seleziona la cartella dell’e-mail da contrassegnare come già letta. Esempio: Principale.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID e-mail (UID)</p> </td> 
   <td> <p>Immetti l’ID e-mail dell’e-mail da contrassegnare come letto.</p> <p>Puoi ottenere l’UID dell’e-mail utilizzando il modulo [!UICONTROL Email] &gt;[!UICONTROL Watch Email] o [!UICONTROL Search Email] .</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Contrassegna e-mail come non letto]

Contrassegna un messaggio e-mail o una bozza di una cartella selezionata come non letta impostando il flag Non letto .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account e-mail a [!UICONTROL Workfront Fusion], vedi <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Collega il tuo messaggio e-mail a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella]</td> 
   <td>Seleziona la cartella dell’e-mail da contrassegnare come non letta. Esempio: Principale.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID e-mail (UID)</p> </td> 
   <td> <p>Immetti l’ID e-mail dell’e-mail da contrassegnare come non letto.</p> <p>Puoi ottenere l’UID dell’e-mail utilizzando il modulo [!UICONTROL Email] &gt;[!UICONTROL Watch Email] o [!UICONTROL Search Email] .</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sposta un’e-mail]

Sposta un messaggio e-mail o una bozza selezionati in una cartella selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account e-mail a [!UICONTROL Workfront Fusion], vedi <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Collega il tuo messaggio e-mail a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella di origine]</td> 
   <td>Seleziona la cartella contenente l’e-mail da cui vuoi spostare l’e-mail. Esempio: Principale.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella di destinazione]</td> 
   <td> <p> Seleziona la cartella alla quale desideri aggiungere il messaggio e-mail. Esempio: Lavoro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID e-mail (UID)</p> </td> 
   <td> <p>Immetti l’ID e-mail dell’e-mail che desideri spostare nella cartella di destinazione.</p> <p>Puoi ottenere l’UID dell’e-mail utilizzando il modulo [!UICONTROL Email] &gt;[!UICONTROL Watch Email] o [!UICONTROL Search Email] .</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiare un messaggio e-mail]

Copia un’e-mail o una bozza in una cartella selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account e-mail a [!UICONTROL Workfront Fusion], vedi <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Collega il tuo messaggio e-mail a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella di origine]</td> 
   <td>Seleziona la cartella da cui copiare l’e-mail. Esempio: Principale.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella di destinazione]</td> 
   <td> <p> Seleziona la cartella in cui copiare il messaggio e-mail. Esempio: Lavoro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID e-mail (UID)</p> </td> 
   <td> <p>Immetti l’ID e-mail dell’e-mail da copiare nella cartella di destinazione.</p> <p>Puoi ottenere l’UID dell’e-mail utilizzando il modulo [!UICONTROL Email] &gt;[!UICONTROL Watch Email] o [!UICONTROL Search Email] .</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un messaggio e-mail]

Rimuove un messaggio e-mail o una bozza dalla cartella selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account e-mail a [!UICONTROL Workfront Fusion], vedi <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Collega il tuo messaggio e-mail a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella]</td> 
   <td>Seleziona la cartella dell’e-mail da eliminare. Esempio: Principale.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID e-mail (UID)</p> </td> 
   <td> <p>Immetti l’ID e-mail dell’e-mail da eliminare.</p> <p>Puoi ottenere l’UID dell’e-mail utilizzando il modulo [!UICONTROL Email] &gt;[!UICONTROL Watch Email] o [!UICONTROL Search Email] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expunge]</td> 
   <td> <p>Abilita questa opzione per consentire al modulo di rimuovere definitivamente tutti i messaggi contrassegnati come eliminati nella cassetta postale attualmente aperta.</p> <p>Nota: In [!DNL Gmail], questo comportamento è determinato dalle impostazioni nella sezione [!UICONTROL Settings] &gt;[!UICONTROL Forwarding POP/IMAP in IMAP access] (Accesso IMAP) .</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni e-mail]

Restituisce e-mail che corrispondono ai criteri specificati.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account e-mail a [!UICONTROL Workfront Fusion], vedi <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Collega il tuo messaggio e-mail a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella] </td> 
   <td> <p>Seleziona la cartella che contiene le e-mail che desideri recuperare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Segna i messaggi letti al momento del recupero] </td> 
   <td> <p>Abilita questa opzione se desideri contrassegnare l’e-mail non letta come letta dopo il recupero dei dettagli.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Criteri di [!UICONTROL]</p> </td> 
   <td> <p>Seleziona i criteri delle e-mail da recuperare:</p> 
    <ul> 
     <li>[!UICONTROL Tutte Le E-Mail]</li> 
     <li>[!UICONTROL Leggi e-mail]</li> 
     <li>[!UICONTROL Solo e-mail non lette]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Indirizzo e-mail mittente] </td> 
   <td> <p>Immetti o mappa l’indirizzo e-mail del mittente di cui desideri recuperare le e-mail.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Indirizzo e-mail destinatario]</td> 
   <td> <p> Immetti o mappa l’indirizzo e-mail del destinatario di cui desideri recuperare le e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Da data] </td> 
   <td> <p>Immetti o mappa la data per recuperare le e-mail elaborate alla data specificata o dopo tale data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prima della data]</td> 
   <td> <p> Immetti o mappa la data per recuperare le e-mail elaborate alla data specificata o prima di essa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Immetti o mappa l’oggetto dell’e-mail che desideri recuperare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Frase] </td> 
   <td> <p>Immetti o mappa qualsiasi parola chiave per recuperare solo le e-mail contenenti frasi specifiche.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID e-mail (UID)</td> 
   <td> <p> Immetti l’ID e-mail (UID) dell’e-mail di cui desideri recuperare i dettagli.</p> <p>Puoi ottenere l’UID dell’e-mail utilizzando [!DNL Workfront Fusion]Modulo 's[!UICONTROL Watch Email] o modulo [!UICONTROL Search Email].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di risultati]</td> 
   <td> <p> Numero massimo di e-mail [!DNL Workfront Fusion] dovrebbe essere restituito durante un ciclo di esecuzione di uno scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Continua l’esecuzione del percorso anche se il modulo non restituisce risultati]</td> 
   <td> <p> Seleziona se desideri continuare a eseguire il modulo anche se non vengono restituiti risultati.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Invia un&#39;e-mail]

Invia una nuova e-mail al tuo indirizzo e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Immetti o mappa l’oggetto dell’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content] </td> 
   <td> <p>Inserisci il corpo dell’e-mail.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Iteratori

#### [!UICONTROL Itera allegati]

Itera gli allegati ricevuti uno ad uno.

Il modulo di iteratore e-mail consente di gestire gli allegati e-mail separatamente. Ad esempio, puoi impostare l’opzione per guardare le e-mail per eseguire l’iterazione delle e-mail con gli allegati e ricevere gli avvisi.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Modulo di origine]</td> 
   <td> <p>Seleziona il modulo che invia l’e-mail con gli allegati che desideri eseguire.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni sugli iteratori, vedi [Modulo iteratore in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
