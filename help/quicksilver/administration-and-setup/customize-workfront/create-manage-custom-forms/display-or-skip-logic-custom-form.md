---
title: Aggiungere logica di visualizzazione e logica di salto a un modulo personalizzato con il generatore di moduli legacy
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile decidere quali sezioni di un modulo personalizzato devono essere visualizzate o ignorate in base alle scelte effettuate da un utente durante la compilazione.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '969'
ht-degree: 0%

---

# Aggiungere logica di visualizzazione e logica di salto a un modulo personalizzato con il generatore di moduli legacy

{{form-designer-default}}

È possibile decidere quali sezioni di un modulo personalizzato devono essere visualizzate o ignorate in base alle scelte effettuate da un utente durante la compilazione.

>[!NOTE]
>
>La logica si applica solo all’interno di un modulo e non può essere basata su selezioni da un modulo diverso.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni su come gli amministratori di Workfront concedono questo accesso, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo ad alcune aree</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Per informazioni sulle configurazioni del piano, del tipo di licenza o del livello di accesso disponibili, contattare l&#39;amministratore Workfront.

## Considerazioni per l’utilizzo della logica di visualizzazione e della logica di salto

* Per aggiungere la logica di visualizzazione a un campo personalizzato, a un widget o a un&#39;interruzione di sezione, è necessario posizionare almeno un campo a scelta multipla (pulsanti di scelta, elenco a discesa o caselle di controllo) prima di inserirlo nel modulo.

  Per informazioni sui campi personalizzati e i widget nei moduli personalizzati, consulta [Aggiungere un campo personalizzato a un modulo personalizzato con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Aggiungere o modificare un widget di risorse in un modulo personalizzato con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Non è possibile aggiungere logica di salto a un widget o a un’interruzione di sezione. È possibile aggiungerlo solo a un campo a scelta multipla (pulsanti di scelta, menu a discesa o caselle di controllo).

* È possibile aggiungere logica di visualizzazione e logica di salto a un campo personalizzato se si verificano tutte le condizioni seguenti relative al campo personalizzato:

   * È un campo a scelta multipla (pulsanti di scelta, menu a discesa o caselle di controllo)
   * È preceduto da un campo a scelta multipla
   * È seguito da un altro campo personalizzato

* Quando si copiano i moduli con la logica di visualizzazione o salta, la logica viene copiata nel nuovo modulo personalizzato.
* Durante la modifica di oggetti in blocco, tutti i campi personalizzati vengono visualizzati nella casella Modifica oggetti, inclusi i campi ignorati o nascosti.
* Quando crei una regola di logica di visualizzazione per un modulo personalizzato, tieni presente quanto segue:

   * Per impostazione predefinita, i campi personalizzati non inclusi in un’istruzione di logica di visualizzazione vengono visualizzati in un modulo personalizzato.
   * Puoi creare istruzioni logiche di visualizzazione a più campi.
   * Se a tutti i campi di un’interruzione di sezione è applicata una logica di visualizzazione e questi sono tutti nascosti come risultato della logica, l’intera sezione sarà nascosta nel modulo personalizzato.

## Creare un modulo personalizzato di esempio con logica di visualizzazione e salto

Il modo migliore per imparare ad aggiungere logica di visualizzazione e salto a un modulo personalizzato consiste nell’esempio pratico illustrato nelle due sezioni seguenti:

### Logica di visualizzazione {#display-logic}

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Forms personalizzato**.

1. Crea il modulo personalizzato di esempio:

   1. Fai clic su **Nuovo modulo personalizzato**, quindi su **Progetto** nell&#39;elenco a discesa.

   1. Nella casella **Titolo modulo**, digita **Modulo personalizzato di esempio - Logica di visualizzazione apprendimento e logica di salto**.

   1. Fai clic su **Aggiungi un campo** nell&#39;angolo superiore sinistro.
   1. Aggiungi un campo a discesa denominato *Campo problema* facendo clic su **Elenco**, quindi digitando **Campo problema** nella casella **Etichetta**.

   1. In **Scelte**, aggiungi le seguenti scelte nelle caselle di testo:

      Ricerca necessaria

      Niente più ricerche

   1. Fai clic su **Salva + Chiudi** nell&#39;angolo in basso a sinistra.

1. Seleziona il nuovo modulo personalizzato **Esempio - Logica di visualizzazione apprendimento e logica di salto**, quindi fai clic su **Modifica**.

1. Aggiungi un nuovo campo di testo a riga singola denominato *Altre ricerche* facendo clic su **Campo di testo a riga singola**, quindi digitando **Altre ricerche** nella casella **Etichetta**.

1. Fare clic su **Aggiungi logica** nella parte inferiore sinistra della schermata **Modifica modulo personalizzato**.

1. Nella casella visualizzata, con la scheda **Logica di visualizzazione** aperta, impostare la logica per la visualizzazione del campo **Altre ricerche** nel modulo facendo clic sul campo **Problema** nel primo elenco a discesa, sul campo **Ricerche necessarie** nel secondo elenco a discesa e sul campo **Selezionato** nel terzo.
1. Fai clic su **Salva** per chiudere la finestra **Logica campo**, quindi fai clic su **Fine** nell&#39;area **Impostazioni campo**.

   Ora, quando qualcuno seleziona **Ricerche necessarie** nel menu a discesa **Campo problema**, verrà visualizzato il campo **Altre ricerche**.

1. Fare clic su **Anteprima** per verificare che la logica sia visualizzata nel modo desiderato nel modulo.
1. Fare clic su **Fine anteprima** quando si rileva che la logica funziona come previsto.
1. Fai clic su **Salva + Chiudi** nella finestra **Modifica modulo personalizzato** per salvare il modulo, quindi continua con [Ignora logica](#skip-logic) di seguito.

### Logica di salto {#skip-logic}

Ignora funzioni logiche simili alla logica di visualizzazione, ma agiscono come l’inverso: invece di fare apparire campi personalizzati a scelta multipla specifici in base a selezioni specifiche, puoi determinare quali devono essere ignorate, in base alle selezioni degli utenti.

Per saperne di più, continua a lavorare sul modulo personalizzato di esempio creato nella sezione [Logica di visualizzazione](#display-logic) in questo articolo:

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fare clic su **Forms personalizzato**.
1. Seleziona il modulo **Modulo personalizzato di esempio - Logica di visualizzazione di apprendimento e logica di salto** creato nei passaggi precedenti, quindi fai clic su **Modifica**.

1. Selezionare il campo a discesa creato denominato *Campo problema*.
1. Fai clic sul pulsante **Aggiungi logica** nella barra laterale **Impostazioni campo**.

1. Nella casella **Logica campo**, accertati che sia selezionata la scheda **Salta logica**.

1. Imposta il primo elenco a discesa su **Non effettuare altre ricerche** e il secondo su **Selezionati**.

1. Nel menu a discesa **Quindi vai a**, seleziona **Fine modulo.**

   Ora, quando qualcuno seleziona **Non effettuare altre ricerche** nel campo a discesa **Campo problema**, il modulo salterà direttamente alla fine del modulo senza visualizzare il campo **Altre ricerche**.

1. Fai clic su **Salva**.
1. Fai clic su **Anteprima** per assicurarti che la logica venga applicata nel modo desiderato.
1. Fai clic su **Fine** in basso a sinistra nel modulo.
