---
title: Aggiungere logica di visualizzazione e ignorare la logica in un modulo personalizzato
description: Aggiungere logica di visualizzazione e ignorare la logica in un modulo personalizzato
draft: Probably
source-git-commit: c0722924d6621b382050a10e9aac549fc1204d72
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 0%

---

# Aggiungere logica di visualizzazione e ignorare la logica in un modulo personalizzato

È possibile utilizzare regole avanzate per rendere un modulo personalizzato dinamico e più pertinente per gli utenti che lo compilano. Quando un utente risponde in un certo modo a un campo a scelta multipla di un modulo, una regola intelligente mostra loro ciò che si desidera venga visualizzato in seguito, in base a tale risposta.

I tipi di campi a scelta multipla sono a discesa, caselle di controllo e pulsanti di scelta.

* **Logica di visualizzazione**: È possibile configurare una regola di logica di visualizzazione per il campo, il widget o la sezione che si desidera visualizzare solo dopo che l’utente ha selezionato una scelta specifica in un campo a scelta multipla precedente.

   **Esempio:** Stai creando un modulo di richiesta dei contenuti di marketing in cui gli utenti della tua organizzazione possono richiedere un nuovo logo, un aggiornamento del sito web, una brochure o altri tipi di contenuti di marketing. In base al tipo di contenuto desiderato dall’utente, è necessario richiedere loro diversi tipi di dettagli, ad esempio colori e idee di design, se hanno bisogno di un logo, o un elenco di caratteristiche del prodotto se hanno bisogno di una brochure.

   Nel campo relativo ai colori e ai dettagli di un nuovo logo, è possibile aggiungere una regola di logica di visualizzazione che visualizzi tale campo solo dopo che l’utente ha selezionato il pulsante di scelta Logo nel primo campo.

   Allo stesso modo, nel campo relativo alle funzioni del prodotto, puoi aggiungere una regola di logica di visualizzazione che visualizzi tale campo solo dopo che un utente seleziona il pulsante di scelta Brochure nel primo campo.

   ![](assets/display-logic-logo-request-350x196.png)

   È possibile configurare le regole di logica di visualizzazione per qualsiasi campo, widget o interruzione di sezione personalizzato che segue un campo a scelta multipla.

* **Ignora regola logica**: È possibile configurare questa regola per nascondere parti di un modulo di cui l’utente non ha bisogno. Quando l’utente seleziona un elemento specifico in un campo a scelta multipla precedente, la regola logica di salto li ignora fino alla fine del modulo o a un campo, widget o sezione personalizzato che si desidera vengano visualizzati.

   **Esempio:** Qualcuno utilizza il modulo di richiesta dei contenuti di marketing qui sopra per chiedere un white paper, fornito dalle vendite, non dal marketing. Per questo utente, una regola di logica di salto può nascondere la domanda che richiede i dettagli e passare a una riga di testo che li rimanda al reparto di cui hanno bisogno.

   ![](assets/skip-logic-white-paper-request-350x221.png)

   In questo caso, è possibile aggiungere un campo Testo descrittivo che fa riferimento l&#39;utente al reparto Vendite. Nel primo campo personalizzato che richiede il tipo di contenuto di marketing di cui l’utente ha bisogno, è possibile aggiungere una regola di logica di salto che visualizza solo la riga di testo quando un utente seleziona il pulsante di opzione White Paper nel primo campo.

   Questo sarebbe particolarmente utile se si aggiungono molti altri campi sui loghi, gli aggiornamenti del sito web e le brochure che questo utente non deve vedere.
Puoi applicare una regola di logica di salto solo a un campo personalizzato, non a un widget o a una sezione.

Per informazioni sui campi e i widget personalizzati nei moduli personalizzati, consultare [Aggiungere un campo personalizzato a un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Aggiunta o modifica di un widget di risorse in un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni su come gli amministratori di Workfront concedono questo accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o configurazioni del livello di accesso si dispone, contattare l&#39;amministratore Workfront.

## Creare un modulo personalizzato di esempio con visualizzazione e logica di esclusione

Il modo migliore per imparare ad aggiungere logica di visualizzazione e di salto a un modulo personalizzato è quello di seguire l’esempio pratico illustrato nelle due sezioni seguenti:

* [Logica di visualizzazione - esempio pratico](#display-logic-practical-example)
* [Ignora logica - esempio pratico](#skip-logic-practical-example)

### Logica di visualizzazione - esempio pratico {#display-logic-practical-example}

In questo esempio viene creato un modulo personalizzato con un campo pulsante di scelta a scelta multipla. Quindi, aggiungi una logica di visualizzazione che collega questo campo a un secondo campo.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, seleziona **Forms personalizzato** ![](assets/custom-forms-icon.png).

1. Fai clic su **Nuovo modulo personalizzato**, seleziona **Progetto** nella casella visualizzata, quindi selezionare **Continua**.

1. In **Titolo modulo** casella di testo, tipo **Modulo personalizzato di esempio - Logica della visualizzazione e logica di salto per l’apprendimento** per assegnare un nome al modulo.

   ![](assets/form-title-box-350x247.png)

1. Per aggiungere il primo campo al modulo:

   1. Apri **Aggiungi un campo** scheda .

      ![](assets/add-a-field-tab-350x237.png)

   1. Seleziona la **Pulsanti di scelta** tipo di campo, quindi digitare *Di quale tipo di contenuto di marketing hai bisogno?* come **Etichetta** per il campo .

   1. Sotto **Scelte**, sostituisci **Scelta 1** e **Scelta 2** con il testo seguente per creare due opzioni, gli utenti possono scegliere nel campo :

      *Aggiornamento sito Web*

      *Progettazione del logo*

1. Per aggiungere il campo personalizzato successivo e aggiungere una regola di logica di visualizzazione:

   1. Apri **Aggiungi un campo** e aggiungi un nuovo **Pulsanti di scelta** campo denominato *Di quale tipo di aggiornamento del sito web hai bisogno?*

      In seguito verranno aggiunte le opzioni per questo campo.

   1. In **Impostazioni aggiuntive** sezione , seleziona **Aggiungi logica**.

      ![](assets/add-logic-btn-350x408.png)

1. Nella casella visualizzata, con la **Logica display** apri la scheda e configura il secondo campo in modo che venga visualizzato solo per gli utenti che hanno selezionato *Progettazione sito web* nel primo campo:

   1. Nel primo menu a discesa, seleziona **Di quale tipo di contenuto di marketing hai bisogno?**
   1. Nel secondo menu a discesa, seleziona **Progettazione sito web**.
   1. Lascia il terzo menu a discesa impostato su **Selezionati**, seleziona **Salva**.

   Osserva i quadrati colorati di piccole dimensioni con una D, che indica che il secondo campo è collegato alla logica di visualizzazione alla selezione dell’utente nel primo campo:

   ![](assets/red-display-logic-indicators-350x250.png)

1. Seleziona **Anteprima** per assicurarsi che la logica funzioni nel modo desiderato sul modulo, selezionare **Anteprima finale**.

1. Fai clic su **Salva e chiudi** salvare il modulo, quindi continuare su [Ignora logica - esempio pratico](#skip-logic-practical-example) sotto.

### Ignora logica - esempio pratico {#skip-logic-practical-example}

Ignora le funzioni logiche in modo simile alla logica di visualizzazione, ma agisce come inverso: invece di visualizzare specifici campi a scelta multipla personalizzati in base alle selezioni degli utenti precedenti, è possibile determinare quali nascondere (saltato) perché non sono rilevanti per l’utente.

Per ulteriori informazioni, continuare a utilizzare il modulo personalizzato di esempio creato nella sezione [Logica di visualizzazione - esempio pratico](#display-logic-practical-example) in questo articolo.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Forms personalizzato**.
1. Fare clic sul nome del modulo **Modulo personalizzato di esempio - Logica della visualizzazione e logica di salto per l’apprendimento** creato nei passaggi precedenti, per aprirlo in modalità di modifica.
1. Selezionare il campo a discesa creato denominato *Di che tipo di sito web hai bisogno?*, aggiungi le seguenti opzioni per il campo, quindi fai clic su **Applica**:

   *E-commerce*

   *Brochure*

   *iscrizione*

1. Apri **Aggiungi un campo** creare un campo di testo con formattazione **o denominato *Qual è l&#39;obiettivo del sito web?*, quindi fai clic su **Applica**.

   In questa organizzazione, un sito di documentazione della Guida viene creato dal team di scrittura tecnica, non dal reparto Marketing. Pertanto, non sono necessarie ulteriori informazioni da parte di un utente che seleziona la documentazione della Guida nel secondo campo. Verrà creata una riga di testo (un campo di testo descrittivo) che indica loro di vedere il team di scrittura tecnica. E utilizzeremo una regola di logica di salto che salta l&#39;utente a quella riga di testo.

1. Per creare la riga di testo:

   1. Apri **Aggiungi un campo** e crea un **Campo di testo descrittivo**.

   1. Per **Etichetta**, tipo *Consulta il team di scrittura tecnica*.

   1. Per **Testo descrittivo**, tipo *Consulta il team di scrittura tecnica per la creazione della documentazione di aiuto online*.

   1. Seleziona **Applica**.

1. Per creare la regola di logica di salto:

   1. Selezionare il secondo campo a discesa, *Di che tipo di sito web hai bisogno?*
   1. In **Impostazione aggiuntiva** sezione s, seleziona **Modifica logica**.
   1. Nella casella visualizzata, apri la **Ignora logica** scheda .
   1. Imposta il primo menu a discesa su **Documentazione dell’Aiuto**, lascia il secondo menu a discesa impostato su **Selezionati** e imposta il terzo menu a discesa su **Consulta il team di scrittura tecnica**.
   1. Seleziona **Salva**.

   Osserva i piccoli quadrati della logica di salto con un S, che indicano che l’utente salterà qualcosa dopo aver selezionato una determinata scelta nel secondo campo.

   ![](assets/notice-skip-logic-squares-350x249.png)

1. Fai clic su **Anteprima**  per fare in modo che la logica sia applicata nel modo desiderato.
1. Fai clic su **Salva +Chiudi**.

Se si crea un modulo come questo, è possibile aggiungere altri campi di testo per richiedere informazioni agli utenti che selezionano E-commerce o Brochure nel secondo campo. Questi campi possono chiedere chi è il pubblico di destinazione per il sito web, qual è l’obiettivo per crearlo, qual è il budget e così via.

E, con le regole logiche, si possono creare percorsi di domanda ramificati.

Ad esempio, per gli utenti che selezionano E-commerce, puoi creare campi che pongono domande sulle foto del prodotto, descrizioni, prezzi e opzioni di pagamento. Per gli utenti che selezionano la Brochure, puoi creare campi che richiedono informazioni sul contenuto.

Un utente che ha selezionato la documentazione di aiuto non vedrà mai nessuno di questi campi aggiuntivi che sono irrilevanti per loro.

>[!TIP]
>
>È possibile aggiungere logica di visualizzazione e logica di salto a un campo personalizzato se per il campo sono soddisfatte tutte le condizioni seguenti:
>
>* Si tratta di un campo a scelta multipla (pulsanti di scelta, menu a discesa o caselle di controllo)
>* È preceduto da un campo di scelta multipla
>* È seguito da un altro campo personalizzato
>


<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Multi-field display logic statements</h2>
-->

