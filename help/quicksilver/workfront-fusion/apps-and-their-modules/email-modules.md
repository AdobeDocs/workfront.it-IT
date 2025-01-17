---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli e-mail
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2651'
ht-degree: 0%

---

# Moduli e-mail

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Moduli e-mail](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/email-modules.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

In uno scenario [!DNL Adobe Workfront Fusion], è possibile collegare l&#39;account di posta elettronica a più applicazioni e servizi di terze parti. Ciò consente di scaricare le e-mail tramite IMAP, inviare e-mail tramite SMTP, creare nuove bozze, spostare e copiare le e-mail da una cartella a un&#39;altra, contrassegnare le e-mail come lette o non lette ed eliminare le e-mail.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o versione successiva</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
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

## Collegare l&#39;e-mail a Workfront Fusion {#connect-your-email-to-workfront-fusion}

* [Connetti a Google](#connect-to-google)
* [Connetti ad altri servizi e-mail (SMAP)](#connect-to-other-email-services-smap)

### Connetti a [!DNL Google]

Utilizzare questa opzione per creare scenari con moduli e-mail che richiedono una connessione all&#39;account [!DNL Google]. Questo è un account con ambiti limitati.

Puoi creare una connessione al tuo account [!DNL Google] direttamente dall&#39;interno di un modulo e-mail.

1. In qualsiasi modulo e-mail, fai clic su **[!UICONTROL Aggiungi]** accanto al campo [!UICONTROL Connessione].
1. Selezionare **[!DNL Google]** come tipo di connessione.
1. Immettere un nome per la connessione.
1. (Facoltativo) Immetti l&#39;ID client [!UICONTROL [!DNL Google]] e il [!UICONTROL segreto client].
1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

### Connetti ad altri servizi e-mail (SMAP)

La connessione SMAP consente di accedere alla cassetta postale in modalità remota e di leggere o manipolare i messaggi nella cassetta postale. La connessione SMAP viene utilizzata dalla maggior parte dei moduli E-mail.

1. In qualsiasi modulo e-mail, fai clic su **[!UICONTROL Aggiungi]** accanto al campo [!UICONTROL Connessione].
1. Selezionare **[!UICONTROL Altri (SMTP)]** come tipo di connessione.
1. Immetti un **[!UICONTROL Nome]** per la connessione.
1. Seleziona il tuo **[!UICONTROL provider di posta elettronica]** dall&#39;elenco. Se il tuo provider di posta elettronica non è presente nell’elenco, seleziona Altro.
1. Immetti il tuo **[!UICONTROL indirizzo e-mail]**, **[!UICONTROL nome completo]**, il tuo **[!UICONTROL nome utente]** e la tua **[!UICONTROL password]**.
1. (Condizionale) Se il provider non è incluso nell&#39;elenco, immettere il **[!UICONTROL server SMTP]** e la **[!UICONTROL porta]** e specificare se si desidera **[!UICONTROL utilizzare una connessione sicura (TLS)]**. Per trovare queste informazioni, controllare la sezione [!UICONTROL Guida] della cassetta postale. Se non disponi di queste informazioni, contatta il provider di servizi e-mail.
1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

## [!UICONTROL E-mail] moduli e relativi campi

Quando configuri i moduli [!UICONTROL E-mail], [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati campi aggiuntivi, a seconda di fattori come il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Alcuni campi e-mail potrebbero contenere già dati, perché sono stati utilizzati in un altro modulo dello scenario. Se hai bisogno di informazioni su di loro, consulta la documentazione dell’e-mail.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>L&#39;ID e-mail univoco noto come &#39;[!UICONTROL ID e-mail (UID)]&#39; è l&#39;identificatore dell&#39;e-mail. L’ID e-mail è specifico per ciascuna cartella dell’e-mail.

* [Triggers](#triggers)
* [Azioni](#actions)
* [Iteratori](#iterators)

### Triggers

#### [!UICONTROL Controlla le e-mail]

Si attiva quando viene ricevuta una nuova e-mail per l’elaborazione in base a criteri specificati.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account di posta elettronica a [!UICONTROL Workfront Fusion], vedere <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connettere l'indirizzo di posta elettronica a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] </td> 
   <td> <p>Seleziona la cartella contenente le e-mail che desideri controllare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criteria]</p> </td> 
   <td> <p>Seleziona i criteri in base ai quali desideri guardare le e-mail:</p> 
    <ul> 
     <li>[!UICONTROL Tutte Le E-Mail]</li> 
     <li>[!UICONTROL Solo Lettura E-Mail]</li> 
     <li>[!UICONTROL Solo E-Mail Non Lette]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Indirizzo E-Mail Mittente] </td> 
   <td> <p>Immetti l’indirizzo e-mail del mittente di cui desideri guardare le e-mail.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Indirizzo E-Mail Destinatario]</td> 
   <td> <p> Inserisci l’indirizzo e-mail del destinatario di cui desideri guardare le e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Immetti l’oggetto dell’e-mail che desideri guardare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Phrase] </td> 
   <td> <p>Inserisci eventuali parole chiave per guardare solo le e-mail contenenti frasi specifiche.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contrassegna i messaggi come letti al recupero]</td> 
   <td> <p>Abilita questa opzione per contrassegnare l’e-mail non letta come letta dopo aver recuperato i dettagli.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di risultati]</td> 
   <td> <p> Il numero massimo di e-mail [!DNL Workfront Fusion] deve essere restituito durante un ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Invia un&#39;e-mail]](#send-an-email)
* [[!UICONTROL Crea bozza]](#create-a-draft)
* [[!UICONTROL Contrassegna un&#39;e-mail come già letta]](#mark-an-email-as-read)
* [[!UICONTROL Contrassegna un&#39;e-mail come non letta]](#mark-an-email-as-unread)
* [[!UICONTROL Sposta un&#39;e-mail]](#move-an-email)
* [[!UICONTROL Copia un&#39;e-mail]](#copy-an-email)
* [[!UICONTROL Eliminare un&#39;e-mail]](#delete-an-email)
* [[!UICONTROL Ricevi e-mail]](#get-emails)

#### [!UICONTROL Invia un&#39;e-mail]

Invia una nuova e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account di posta elettronica a [!DNL Workfront Fusion], vedere <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connettere l'indirizzo di posta elettronica a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salva messaggio dopo l'invio]</td> 
   <td>Una volta inviato, il messaggio e-mail verrà salvato nella cassetta postale. Abilitare questa opzione se si desidera salvare le e-mail inviate tramite [!DNL Workfront Fusion] nella cartella <i>[!UICONTROL Sent mail]</i> o in un'altra cartella della cassetta postale. Alcuni servizi di posta elettronica, ad esempio [!DNL Gmail], salvano automaticamente i messaggi inviati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL A] </td> 
   <td> <p>Aggiungi gli indirizzi e-mail a cui desideri inviare l’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Inserisci o mappa l’oggetto dell’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo di contenuto]</p> </td> 
   <td> <p>Seleziona il tipo di contenuto [!UICONTROL] per l'e-mail:</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Testo normale]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content] </td> 
   <td> <p>Immetti o mappa il contenuto dell’e-mail in formato HTML utilizzando i tag HTML o nel testo normale, a seconda di ciò che hai scelto nel campo [!UICONTROL Content Type] (Tipo di contenuto).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Allegati]</p> </td> 
   <td> <p>Aggiungi un allegato:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome file]</strong> </p> <p>Immettere il nome del file. Ad esempio, sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Dati]</strong> </p> <p>Immettere il percorso della cartella in cui caricare l'allegato.</p> </li> 
     <li> <p><strong>[!UICONTROL ID contenuto]</strong> </p> <p>Immetti l'ID di contenuto [!UICONTROL] per inserire l'allegato (immagine) nel contenuto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copia Destinatario] </td> 
   <td> <p>Inserisci o mappa uno o più indirizzi e-mail a cui desideri inviare una copia di questo messaggio e-mail. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Destinatario [!UICONTROL Blind Copy]</td> 
   <td> <p> Inserisci o mappa uno o più indirizzi e-mail ai quali desideri inviare una copia di questa e-mail senza che l’indirizzo e-mail venga visualizzato nell’e-mail.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Da] </td> 
   <td> <p>Immetti o mappa l'indirizzo e-mail (e il nome, se necessario) che viene visualizzato nel campo [!UICONTROL Da] dell'e-mail. </p> <p>Importante: utilizzare la sintassi corretta: <code>name@email.com</code> o <code>"Name" name@email.com</code>.</p> <p>Nota: in genere, [!DNL Workfront Fusion] utilizza come indirizzo del mittente l'indirizzo e-mail immesso durante la creazione della connessione. Se inserisci un altro indirizzo e-mail, potrebbe verificarsi un errore durante l’invio di un messaggio, perché il tuo account potrebbe non disporre dell’autorizzazione per inviare e-mail da un indirizzo diverso dal tuo. Esempio: <code>test@mail.com</code> o "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>Inserisci o mappa l’indirizzo e-mail visualizzato nel campo [!UICONTROL Sender] dell’e-mail.</p> <p>Suggerimento: se non si è sicuri di utilizzare questo campo o il campo Da, è consigliabile scegliere il campo Da.</p> <p>Importante: utilizzare la sintassi corretta: <code>name@email.com</code> o <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL - Risposta]</td> 
   <td> <p> Se si desidera che le risposte a questa e-mail vengano inviate a un indirizzo diverso da quello del mittente, immettere l'indirizzo e-mail a cui si desidera inviare le risposte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL In-Reply-To]</td> 
   <td> <p> Se rispondi a un’e-mail specifica, inserisci o mappa l’ID dell’e-mail a cui stai rispondendo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Riferimenti] </td> 
   <td> <p>Immetti gli ID messaggio di tutte le risposte nel thread.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Priorità [!UICONTROL]</p> </td> 
   <td> <p>Seleziona la priorità dell’e-mail:</p> 
    <ul> 
     <li>[!UICONTROL alto]</li> 
     <li>[!UICONTROL Normale]</li> 
     <li>[!UICONTROL Minimo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
   <td> <p>Aggiungi le intestazioni:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>Aggiungi la chiave. [!UICONTROL Sender], [!UICONTROL Date], [!UICONTROL To] e così via.</p> </li> 
     <li> <p><strong>[!UICONTROL Valore]</strong> </p> <p>Immetti il valore per la chiave.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea bozza]

Crea e aggiunge una nuova bozza a una cartella selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account di posta elettronica a [!UICONTROL Workfront Fusion], vedere <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connettere l'indirizzo di posta elettronica a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Seleziona la cartella in cui desideri creare la bozza di e-mail.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL A] </td> 
   <td> <p>Inserisci o mappa l’indirizzo e-mail a cui desideri inviare l’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Inserisci o mappa l’oggetto dell’e-mail.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Tipo di contenuto]</p> </td> 
   <td> <p>Seleziona il tipo di contenuto per l’e-mail:</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL testo normale]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content] </td> 
   <td> <p>Immetti o mappa il contenuto dell’e-mail in formato HTML utilizzando i tag HTML o nel testo normale, a seconda di ciò che hai scelto nel campo [!UICONTROL Content Type] (Tipo di contenuto).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Allegati]</p> </td> 
   <td> <p>Aggiungi un allegato:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome file]</strong> </p> <p>Immettere il nome del file. Ad esempio, sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Dati]</strong> </p> <p>Immettere il percorso della cartella in cui caricare l'allegato.</p> </li> 
     <li> <p><strong>[!UICONTROL ID contenuto]</strong> </p> <p>Immetti l’ID contenuto per inserire l’allegato (immagine) nel contenuto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copia Destinatario] </td> 
   <td> <p>Inserisci o mappa uno o più indirizzi e-mail a cui desideri inviare una copia di questo messaggio e-mail. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Destinatario [!UICONTROL Blind Copy]</td> 
   <td> <p> Inserisci o mappa uno o più indirizzi e-mail ai quali desideri inviare una copia di questa e-mail senza che l’indirizzo e-mail venga visualizzato nell’e-mail.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Da] </td> 
   <td> <p>Immetti o mappa l'indirizzo e-mail (e il nome, se necessario) che viene visualizzato nel campo [!UICONTROL Da] dell'e-mail. </p> <p>Importante: utilizzare la sintassi corretta: <code>name@email.com</code> o <code>"Name" name@email.com</code>.</p> <p>Nota: in genere, [!DNL Workfront Fusion] utilizza come indirizzo del mittente l'indirizzo e-mail immesso durante la creazione della connessione. Se inserisci un altro indirizzo e-mail, potrebbe verificarsi un errore durante l’invio di un messaggio, perché il tuo account potrebbe non disporre dell’autorizzazione per inviare e-mail da un indirizzo diverso dal tuo. Esempio: <code>test@mail.com</code> o "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>Inserisci o mappa l’indirizzo e-mail visualizzato nel campo [!UICONTROL Sender] dell’e-mail.</p> <p>Suggerimento: se non si è sicuri di utilizzare questo campo o il campo Da, è consigliabile scegliere il campo Da.</p> <p>Importante: utilizzare la sintassi corretta: <code>name@email.com</code> o <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL - Risposta]</td> 
   <td> <p> Se si desidera che le risposte a questa e-mail vengano inviate a un indirizzo diverso da quello di "[!UICONTROL da]", immettere l'indirizzo e-mail a cui si desidera inviare le risposte a questa e-mail.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL In-Reply-To]</td> 
   <td> <p> Se rispondi a un’e-mail specifica, inserisci o mappa l’ID dell’e-mail a cui stai rispondendo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Riferimenti] </td> 
   <td> <p>Immetti gli ID messaggio di tutte le risposte nel thread.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Priorità [!UICONTROL]</p> </td> 
   <td> <p>Seleziona la priorità dell’e-mail:</p> 
    <ul> 
     <li>[!UICONTROL alto]</li> 
     <li>[!UICONTROL Normale]</li> 
     <li>[!UICONTROL Minimo]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
   <td> <p>Aggiungi le intestazioni:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>Aggiungi la chiave. Ad esempio, Mittente, Data, A e così via.</p> </li> 
     <li> <p><strong>[!UICONTROL Valore]</strong> </p> <p>Immetti il valore per la chiave.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Contrassegna un&#39;e-mail come già letta]

Contrassegna un&#39;e-mail o una bozza in una cartella selezionata come già letta impostando il flag [!UICONTROL Leggi].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account di posta elettronica a [!UICONTROL Workfront Fusion], vedere <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connettere l'indirizzo di posta elettronica a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Seleziona la cartella dell’e-mail da contrassegnare come letta. Esempio: primario.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID e-mail (UID)]</p> </td> 
   <td> <p>Inserisci l’UID e-mail dell’e-mail che desideri contrassegnare come letta.</p> <p>È possibile ottenere l'UID dell'e-mail utilizzando il modulo [!UICONTROL E-mail] &gt;[!UICONTROL E-mail di controllo] o il modulo [!UICONTROL E-mail di ricerca].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Contrassegna un&#39;e-mail come non letta]

Contrassegna un messaggio e-mail o una bozza in una cartella selezionata come non letti impostando il flag Unread.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account di posta elettronica a [!UICONTROL Workfront Fusion], vedere <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connettere l'indirizzo di posta elettronica a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Seleziona la cartella dell’e-mail da contrassegnare come non letta. Esempio: primario.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID e-mail (UID)]</p> </td> 
   <td> <p>Inserisci l’UID e-mail dell’e-mail che desideri contrassegnare come non letta.</p> <p>È possibile ottenere l'UID dell'e-mail utilizzando il modulo [!UICONTROL E-mail] &gt;[!UICONTROL E-mail di controllo] o il modulo [!UICONTROL E-mail di ricerca].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sposta un&#39;e-mail]

Sposta un messaggio e-mail o una bozza selezionati in una cartella selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account di posta elettronica a [!UICONTROL Workfront Fusion], vedere <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connettere l'indirizzo di posta elettronica a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Folder]</td> 
   <td>Seleziona la cartella contenente l’e-mail da cui desideri spostare l’e-mail. Esempio: primario.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella di destinazione]</td> 
   <td> <p> Seleziona la cartella a cui desideri aggiungere l’e-mail. Esempio: lavoro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID e-mail (UID)]</p> </td> 
   <td> <p>Immetti l’UID e-mail dell’e-mail che desideri spostare nella cartella di destinazione.</p> <p>È possibile ottenere l'UID dell'e-mail utilizzando il modulo [!UICONTROL E-mail] &gt;[!UICONTROL E-mail di controllo] o il modulo [!UICONTROL E-mail di ricerca].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copia un&#39;e-mail]

Copia un messaggio e-mail o una bozza in una cartella selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account di posta elettronica a [!UICONTROL Workfront Fusion], vedere <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connettere l'indirizzo di posta elettronica a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Folder]</td> 
   <td>Seleziona la cartella da cui desideri copiare l’e-mail. Esempio: primario.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella di destinazione]</td> 
   <td> <p> Seleziona la cartella in cui desideri copiare l’e-mail. Esempio: lavoro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID e-mail (UID)]</p> </td> 
   <td> <p>Immetti l’UID e-mail dell’e-mail da copiare nella cartella di destinazione.</p> <p>È possibile ottenere l'UID dell'e-mail utilizzando il modulo [!UICONTROL E-mail] &gt;[!UICONTROL E-mail di controllo] o il modulo [!UICONTROL E-mail di ricerca].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un&#39;e-mail]

Rimuove un messaggio e-mail o una bozza dalla cartella selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account di posta elettronica a [!UICONTROL Workfront Fusion], vedere <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connettere l'indirizzo di posta elettronica a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Seleziona la cartella dell’e-mail da eliminare. Esempio: primario.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID e-mail (UID)]</p> </td> 
   <td> <p>Immetti l’UID e-mail dell’e-mail da eliminare.</p> <p>È possibile ottenere l'UID dell'e-mail utilizzando il modulo [!UICONTROL E-mail] &gt;[!UICONTROL E-mail di controllo] o il modulo [!UICONTROL E-mail di ricerca].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expunge]</td> 
   <td> <p>Abilita questa opzione per consentire al modulo di rimuovere definitivamente tutti i messaggi contrassegnati come [!UICONTROL Deleted] nella cassetta postale attualmente aperta.</p> <p>Nota: in [!DNL Gmail], questo comportamento è guidato dall'impostazione nella sezione [!UICONTROL Settings] &gt;[!UICONTROL Forwarding POP/IMAP in IMAP access].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ricevi e-mail]

Restituisce e-mail che corrispondono ai criteri specificati.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account di posta elettronica a [!UICONTROL Workfront Fusion], vedere <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connettere l'indirizzo di posta elettronica a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] </td> 
   <td> <p>Seleziona la cartella contenente le e-mail da recuperare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contrassegna i messaggi come letti al recupero] </td> 
   <td> <p>Abilita questa opzione se desideri contrassegnare l’e-mail non letta come letta dopo aver recuperato i dettagli.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criteria]</p> </td> 
   <td> <p>Seleziona i criteri delle e-mail che desideri recuperare:</p> 
    <ul> 
     <li>[!UICONTROL Tutte Le E-Mail]</li> 
     <li>[!UICONTROL Solo Lettura E-Mail]</li> 
     <li>[!UICONTROL Solo E-Mail Non Lette]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Indirizzo E-Mail Mittente] </td> 
   <td> <p>Inserisci o mappa l’indirizzo e-mail del mittente di cui desideri recuperare le e-mail.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Indirizzo E-Mail Destinatario]</td> 
   <td> <p> Inserisci o mappa l’indirizzo e-mail del destinatario di cui desideri recuperare le e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Da data] </td> 
   <td> <p>Inserisci o mappa la data in cui recuperare le e-mail elaborate nella data specificata o in una data successiva.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prima della data]</td> 
   <td> <p> Inserisci o mappa la data in cui recuperare le e-mail elaborate entro la data specificata.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Inserisci o mappa l’oggetto dell’e-mail che desideri recuperare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Phrase] </td> 
   <td> <p>Inserisci o mappa le parole chiave per recuperare solo le e-mail contenenti frasi specifiche.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID e-mail (UID)]</td> 
   <td> <p> Immetti l’ID e-mail (UID) dell’e-mail di cui desideri recuperare i dettagli.</p> <p>È possibile ottenere l'UID dell'e-mail utilizzando il modulo [!UICONTROL Watch Email] di [!DNL Workfront Fusion] o il modulo [!UICONTROL Search Email].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di risultati]</td> 
   <td> <p> Il numero massimo di e-mail [!DNL Workfront Fusion] deve essere restituito durante un ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Continua l'esecuzione della route anche se il modulo non restituisce alcun risultato]</td> 
   <td> <p> Seleziona questa opzione se desideri continuare a eseguire il modulo anche se non vengono restituiti risultati.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Iteratori

#### [!UICONTROL Itera Allegati]

Gli iterati hanno ricevuto gli allegati uno per uno.

Il modulo dell’iteratore e-mail consente di gestire separatamente gli allegati e-mail. Ad esempio, puoi impostare per controllare le e-mail in modo da iterare le e-mail con allegati e ricevere avvisi.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Modulo Source]</td> 
   <td> <p>Seleziona il modulo che restituisce l’e-mail con gli allegati che desideri iterare.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni sugli iteratori, vedere [Modulo iteratore in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
