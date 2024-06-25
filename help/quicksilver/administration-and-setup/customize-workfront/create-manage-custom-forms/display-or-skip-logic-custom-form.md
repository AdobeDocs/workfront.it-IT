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
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni sulle modalità di concessione dell'accesso da parte degli amministratori di Workfront, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Per informazioni sulle configurazioni di piano, tipo di licenza o livello di accesso disponibili, contattare l&#39;amministratore Workfront.

## Considerazioni per l’utilizzo della logica di visualizzazione e della logica di salto

* Per aggiungere la logica di visualizzazione a un campo personalizzato, a un widget o a un&#39;interruzione di sezione, è necessario posizionare almeno un campo a scelta multipla (pulsanti di scelta, elenco a discesa o caselle di controllo) prima di inserirlo nel modulo.

  Per informazioni sui campi personalizzati e i widget nei moduli personalizzati, vedi [Aggiungere un campo personalizzato a un modulo personalizzato con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Aggiungere o modificare un widget di risorse in un modulo personalizzato con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Forms personalizzato**.

1. Crea il modulo personalizzato di esempio:

   1. Clic **Nuovo modulo personalizzato**, quindi fai clic su **Progetto** nell’elenco a discesa.

   1. In **Titolo modulo** casella, digitare **Modulo personalizzato di esempio: logica di visualizzazione e logica di salto dell’apprendimento**.

   1. Clic **Aggiungi un campo** nell’angolo superiore sinistro.
   1. Aggiungi un campo a discesa denominato *Campo Issue* facendo clic su **A discesa**, quindi digita **Campo Issue** nel **Etichetta** casella.

   1. Sotto **Scelte**, aggiungi le seguenti scelte nelle caselle di testo:

      Ricerca necessaria

      Niente più ricerche

   1. Clic **Salva e chiudi** nell’angolo in basso a sinistra.

1. Seleziona il nuovo **Modulo personalizzato di esempio: logica di visualizzazione e logica di salto dell’apprendimento** modulo personalizzato, quindi fai clic su **Modifica**.

1. Aggiungi un nuovo campo di testo a riga singola denominato *Altre ricerche* facendo clic su **Campo di testo a riga singola**, quindi digita **Altre ricerche** nel **Etichetta** casella.

1. Clic **Aggiungi logica** nella parte inferiore sinistra della **Modifica modulo personalizzato** schermo.

1. Nella casella visualizzata, con **Logica di visualizzazione** , impostare la logica per quando si apre **Altre ricerche** verrà visualizzato nel modulo facendo clic su **Campo Issue** nel primo elenco a discesa, **Ricerca necessaria** nel secondo elenco a discesa, e **Selezionato** nel terzo elenco a discesa.
1. Clic **Salva** per chiudere **Logica campo** , quindi fai clic su **Fine** nel **Impostazioni campo** area.

   Ora, quando qualcuno seleziona **Ricerca necessaria** nel **Campo Issue** a discesa, il **Altre ricerche** verrà visualizzato.

1. Clic **Anteprima** per assicurarsi che la logica venga visualizzata nel modo desiderato nel modulo.
1. Clic **Fine anteprima** quando scopri che la logica funziona come previsto.
1. Clic **Salva e chiudi** il **Modifica modulo personalizzato** per salvare il modulo, quindi continuare con [Logica di salto](#skip-logic) di seguito.

### Logica di salto {#skip-logic}

Ignora funzioni logiche simili alla logica di visualizzazione, ma agiscono come l’inverso: invece di fare apparire campi personalizzati a scelta multipla specifici in base a selezioni specifiche, puoi determinare quali devono essere ignorate, in base alle selezioni degli utenti.

Per saperne di più, continua a lavorare al modulo personalizzato di esempio creato nella sezione [Logica di visualizzazione](#display-logic) in questo articolo:

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Clic **Forms personalizzato**.
1. Seleziona il modulo **Modulo personalizzato di esempio: logica di visualizzazione e logica di salto dell’apprendimento** creato nei passaggi precedenti, quindi fai clic su **Modifica**.

1. Seleziona il campo a discesa creato denominato *Campo Issue*.
1. Fai clic su **Aggiungi logica** pulsante in **Impostazioni campo** barra laterale.

1. In **Logica campo** , assicurarsi che il **Salta logica** è selezionata.

1. Impostare il primo elenco a discesa su **Niente più ricerche** e il secondo elenco a discesa per **Selezionato**.

1. In **Quindi Passa A** a discesa, seleziona **Fine del modulo.**

   Ora, quando qualcuno seleziona **Niente più ricerche** nel **Campo Issue** , il modulo salterà direttamente alla fine del modulo senza visualizzare il **Altre ricerche** campo.

1. Fai clic su **Salva**.
1. Clic **Anteprima**  per assicurarti che la logica venga applicata nel modo desiderato.
1. Clic **Fine** in basso a sinistra nel modulo.
