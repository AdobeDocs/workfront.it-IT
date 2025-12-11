---
title: Utilizzare Riempimento modulo basato su IA per compilare una richiesta utilizzando prompt o documenti
content-type: reference
description: È possibile utilizzare l’intelligenza artificiale per compilare automaticamente i campi della richiesta immettendo un prompt o fornendo un documento.
author: Becky
feature: Get Started with Workfront
exl-id: 4a22f9ea-c9ee-4947-8683-9989c54903b1
source-git-commit: 59aa98645583fb79a5d61a248dca535a3460956f
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 3%

---

# Utilizzare Riempimento modulo basato su IA per compilare una richiesta utilizzando prompt o documenti

>[!NOTE]
>
>Per utilizzare questa funzionalità, l’organizzazione deve soddisfare i requisiti per utilizzare l’Assistente di intelligenza artificiale di Workfront. Per informazioni dettagliate, vedere [Prerequisiti per l&#39;Assistente IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

Il riempimento del modulo AI può essere utile per compilare automaticamente i campi della richiesta in base a un prompt inserito. Può anche riempire i campi in base a testo come le e-mail o i documenti caricati. Puoi approvare o rifiutare questi suggerimenti prima di inviare la richiesta.

Il riempimento del modulo AI non sovrascrive i campi già compilati.

Gli utenti non ricevono suggerimenti di dati a cui non hanno altrimenti accesso.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Collaboratore o versione successiva</p>
   <p>Richiedi o superiore</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Issues</p>  </td> 
  </tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td><p>Accesso per aggiungere richieste a una coda di richieste</p> <p>Visualizza o autorizzazioni superiori per la richiesta esistente</p> <p>Per informazioni sulla configurazione di una coda richieste, vedere <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda richieste</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Per utilizzare il riempimento modulo AI per compilare le richieste utilizzando un prompt o un documento, **tutti** i seguenti elementi devono essere applicati:

* La tua organizzazione deve aver eseguito la migrazione ad Adobe IMS (Identity Management System)
* L’esperienza unificata di Adobe deve essere abilitata
* La tua organizzazione deve disporre di un piano Select, Prime o Ultimate Workfront
* Adobe deve disporre di un accordo Adobe Gen AI firmato su file

  Per ulteriori informazioni sulla firma del contratto, consulta [Firmare il contratto di Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) nell&#39;articolo Panoramica dell&#39;Assistente AI.
* L&#39;Assistente AI deve essere abilitato nelle impostazioni di sistema dell&#39;organizzazione. Questa funzione è gestita dall’amministratore di Workfront.

  Per ulteriori informazioni sull&#39;abilitazione dell&#39;Assistente di intelligenza artificiale nelle impostazioni di sistema, vedere [Attivare o disattivare l&#39;Assistente di intelligenza artificiale](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

## Ottieni suggerimenti da un prompt di testo

Il riempimento del modulo AI può suggerire valori di campo in base a testo come le e-mail. Si incolla in un blocco di testo e Workfront elabora il testo per suggerire i valori dei campi in base al testo.

Ad esempio, se l’e-mail include &quot;Questa è in scadenza il 1° giugno&quot; e il modulo di richiesta ha un campo per la data di scadenza, il campo Compilazione modulo AI consiglierebbe 1 giugno per tale valore di campo.

Durante la compilazione di un modulo, Workfront controlla anche le richieste precedenti per contesti simili. Ad esempio, se il prompt indica che la richiesta è per un determinato client, Workfront può individuare e immettere automaticamente l’indirizzo di fatturazione per tale client, in base alle richieste precedenti.

È possibile incollare il testo da applicare all&#39;intero modulo o a una singola sezione del modulo.

Per utilizzare i suggerimenti basati su un prompt di testo incollato:

1. Inizia a creare una richiesta.

   Per istruzioni, vedere [Creare e inviare richieste](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Per applicare il prompt di testo all&#39;intero modulo, fare clic sull&#39;icona IA ![Icona IA](assets/request-prompt-icon.png) sotto il nome del modulo.

   Oppure

   Per applicare il prompt di testo per una singola sezione, fai clic sull&#39;icona IA ![icona IA](assets/request-prompt-icon.png) accanto al nome della sezione.

1. Incollare il testo nella casella del prompt.
1. Fai clic su **Compila il modulo**.

   Workfront genera suggerimenti per il modulo.
1. Per ogni suggerimento di campo, selezionare **Accetta** o **Rifiuta** per il campo.

   ![Accetta o rifiuta suggerimento](assets/accept-reject-suggestion.png)

   Oppure

   Selezionare **Accetta tutti** o **Rifiuta tutti** nella parte superiore della pagina per accettare o rifiutare tutti i suggerimenti.

   >[!NOTE]
   >
   >Eventuali suggerimenti non rivisti verranno accettati automaticamente quando invii la richiesta.

### Esempi di prompt di testo

Questi esempi mostrano i prompt per vari modi in cui l’intelligenza artificiale può fare riferimento ad altri progetti.

#### Riferimento a una campagna cliente passata

>[!BEGINSHADEBOX]

Crea una richiesta di campagna simile a quella fatta per il lancio del secondo trimestre (società cliente), ma questa volta per la divisione Automotive. Mantenere lo stesso set di risultati finali e lo stesso profilo di pubblico.

>[!ENDSHADEBOX]

#### Basato su un progetto esistente

>[!BEGINSHADEBOX]

Utilizza la stessa configurazione adottata per l’avvio del progetto (nome progetto) la scorsa primavera. Voglio eseguire una campagna pubblicitaria digitale indirizzata allo stesso pubblico esecutivo, ma con date aggiornate per questo trimestre.

>[!ENDSHADEBOX]

#### Riutilizzo di uno stile da un risultato finale passato

>[!BEGINSHADEBOX]

Prepara una richiesta simile alla campagna di promozione estiva (società cliente) che abbiamo eseguito l’anno scorso. Concentrati sugli asset dei social media, mantieni lo spagnolo come lingua principale e regola il budget a 75.000 dollari.

>[!ENDSHADEBOX]

#### Espansione su un tipo di campagna precedente

>[!BEGINSHADEBOX]

Prendi come riferimento la campagna della serie di webinar (nome della campagna) dal primo trimestre. Voglio lo stesso flusso di lavoro di registrazione e le stesse risorse, ma questa volta l&#39;argomento è &quot;IA in Financial Planning&quot; e il pubblico è composto da giovani professionisti.

>[!ENDSHADEBOX]

#### Ripetizione di una richiesta per un prodotto diverso

>[!BEGINSHADEBOX]

Imposta una richiesta di campagna come il progetto di rebranding (società cliente) gestito da, ma sostituisci con (nuova società cliente) come cliente. Mantenere tutti i servizi forniti allineati al branding aziendale.

>[!ENDSHADEBOX]

#### Stile narrativo con riferimenti impliciti

>[!BEGINSHADEBOX]

Stiamo pianificando una campagna simile agli annunci sociali per le feste che abbiamo fatto l&#39;anno scorso. Il budget dovrebbe essere di circa 50.000, l’obiettivo è la generazione di lead e i risultati finali dovrebbero includere le risorse Instagram e TikTok.

>[!ENDSHADEBOX]


## Ottieni suggerimenti in base a un documento caricato

Il riempimento di un modulo basato sull’intelligenza artificiale può compilare una richiesta utilizzando prompt o documenti che possono suggerire valori di campo in base a un documento caricato.

Questo tipo di suggerimento controlla anche le richieste precedenti per contesti simili. Ad esempio, se il prompt indica che la richiesta è per un determinato client, Workfront può individuare e immettere automaticamente l’indirizzo di fatturazione per tale client, in base alle richieste precedenti.

### Guardrail di caricamento documenti

#### Tipi di file supportati

Sono supportati i seguenti tipi di file:

<table>
<tr style="border: 0;">
<td>
<ul>
<li>BMP</li>
<li>CSV</li>
<li>DOC</li>
<li>DOCX</li>
<li>GIF</li>
<li>JPEG</li>
</ul>
</td>
<td>
<ul>
<li>ODP</li>
<li>ODS</li>
<li>ODT</li>
<li>PDF</li>
<li>PNG</li>
<li>PPT</li>
</ul>
</td>
<td>
<ul>
<li>PPTX</li>
<li>RTF</li>
<li>TIFF</li>
<li>TXT</li>
<li>XLS</li>
<li>XLSX</li>
</ul>
</td>
</tr>
</table>

#### Dimensione file supportata

Ogni file può avere dimensioni fino a 100 MB

#### Numero di file

È possibile caricare fino a 50 file (pagine, diapositive o fogli).

>[!IMPORTANT]
>
>I documenti vengono convertiti in una serie di immagini, ognuna delle quali viene considerata un file separato.
>
>Ad esempio, è possibile caricare un PowerPoint con 50 diapositive o 5 documenti Word, ciascuno con 10 pagine.

#### Tipi di campo supportati

I tipi di campo di Workfront determinano se un determinato campo può essere compilato automaticamente.

<table>
<tr>
<td><b>Il riempimento del modulo </b><br> supportato con IA può essere compilato</td>
<td><b>Non supportato</b> <br>Il riempimento del modulo basato sull'intelligenza artificiale non viene compilato</td>
</tr>
<tr>
<td>
<ul>
<li>Testo su riga singola</li>
<li>Area di testo o paragrafo</li>
<li>Campo data</li>
<li>Casella di controllo</li>
<li>Pulsanti di scelta</li>
<li>Menu a discesa a selezione singola e multipla</li>
</ul>
</td>
<td><li>Automatico</li>
<li>Ricerca esterna</li>
<li>Ricerca interna</li>
<li>Riferimenti</li>
<li>Campi incorporati di WF Planning</li>
</ul>
</td>
</tr>
</table>

#### Altre best practice

Quando si carica un documento in AI Form Fill (Compila modulo IA), considera quanto segue:

* Il riempimento del modulo AI è attualmente ottimizzato per l’alfabeto latino.
* È consigliabile utilizzare una dimensione di testo di 8 punti o superiore.
* Il riempimento del modulo AI può presentare difficoltà con le immagini del documento, ad esempio immagini ruotate o distorte, grafici e conteggio o utilizzo di motivi spaziali sugli oggetti nelle immagini.
* Come sempre, si consiglia di verificare la precisione dei risultati prima di inviare la richiesta.

### Caricare un documento per compilare automaticamente una richiesta

È possibile caricare un documento da applicare all&#39;intero modulo o a una singola sezione del modulo.

1. Inizia a creare una richiesta.

   Per istruzioni, vedere [Creare e inviare richieste](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Per applicare il documento all&#39;intero modulo, fare clic sull&#39;icona IA ![Icona IA](assets/request-prompt-icon.png) sotto il nome del modulo.

   Oppure

   Per applicare il documento a una singola sezione, fai clic sull&#39;icona IA ![icona IA](assets/request-prompt-icon.png) accanto al nome della sezione.

1. Fai clic su **Carica file**, quindi seleziona il file dal file manager.

   Oppure

   Trascina il documento dal gestore di file nella casella **Carica file nel modulo di richiesta di compilazione automatica**.
1. Fai clic su **Compila il modulo** di **Compila la sezione**.

   Workfront genera suggerimenti per il modulo.
1. Per ogni suggerimento di campo, selezionare **Accetta** o **Rifiuta** per il campo.

   ![Accetta o rifiuta suggerimento](assets/accept-reject-suggestion.png)

   Oppure

   Selezionare **Accetta tutti** o **Rifiuta tutti** nella parte superiore della pagina per accettare o rifiutare tutti i suggerimenti.

   >[!NOTE]
   >
   >Eventuali suggerimenti non rivisti verranno accettati automaticamente quando invii la richiesta.

## Risoluzione dei problemi

Se non ricevi i suggerimenti previsti, la causa potrebbe essere una delle seguenti:

* È necessario disporre di almeno un mese di dati della richiesta nel sistema prima che possa suggerire valori di campo da richieste precedenti.
* Potresti non aver seguito i guardrail di caricamento del documento durante il caricamento di un documento da cui estrarre i suggerimenti. Per ulteriori informazioni, vedi [Guardrail di caricamento documenti](#document-upload-guardrails) in questo articolo.
