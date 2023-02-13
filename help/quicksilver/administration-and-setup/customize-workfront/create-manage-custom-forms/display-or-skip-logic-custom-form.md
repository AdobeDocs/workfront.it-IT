---
title: Aggiungere logica di visualizzazione e ignorare la logica in un modulo personalizzato
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile decidere quali sezioni di un modulo personalizzato visualizzare o ignorare in base alle scelte effettuate dall’utente durante la compilazione.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
source-git-commit: 59e3b958dd81f2f068bc06c3fe439de0084f9ce4
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# Aggiungere logica di visualizzazione e ignorare la logica in un modulo personalizzato

È possibile decidere quali sezioni di un modulo personalizzato visualizzare o ignorare in base alle scelte effettuate dall’utente durante la compilazione.

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
   <td>Piano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni su come gli amministratori di Workfront concedono questo accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o configurazioni del livello di accesso si dispone, contattare l&#39;amministratore Workfront.

## Considerazioni sull’utilizzo della logica di visualizzazione e della logica di salto

* Per aggiungere logica di visualizzazione a un campo, a un widget o a un’interruzione di sezione personalizzato, è necessario posizionare almeno un campo di scelta multiplo (pulsanti di scelta, menu a discesa o caselle di controllo) prima di tale campo sul modulo.

   Per informazioni sui campi e i widget personalizzati nei moduli personalizzati, consultare [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Aggiunta o modifica di un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Non è possibile aggiungere logica di salto a un widget o a un&#39;interruzione di sezione. È possibile aggiungerlo solo a un campo di scelta multipla (pulsanti di scelta, menu a discesa o caselle di controllo).

* È possibile aggiungere logica di visualizzazione e logica di salto a un campo personalizzato tutto quanto segue è true per il campo personalizzato:

   * Si tratta di un campo a scelta multipla (pulsanti di scelta, menu a discesa o caselle di controllo)
   * È preceduto da un campo di scelta multipla
   * È seguito da un altro campo personalizzato

* Quando si copiano moduli con logica di visualizzazione o logica di salto, la logica viene copiata nel nuovo modulo personalizzato.
* Quando si crea una regola di logica di visualizzazione per un modulo personalizzato, tenere presente quanto segue

   * Per impostazione predefinita, i campi personalizzati non inclusi in un’istruzione logica di visualizzazione vengono visualizzati in un modulo personalizzato.
   * È possibile creare istruzioni logiche di visualizzazione a più campi.

* Quando si modificano gli oggetti in blocco, tutti i campi personalizzati vengono visualizzati nella casella Modifica oggetti, compresi i campi ignorati o nascosti.

## Creare un modulo personalizzato di esempio con visualizzazione e logica di esclusione

Il modo migliore per imparare ad aggiungere logica di visualizzazione e di salto a un modulo personalizzato è quello di seguire l’esempio pratico illustrato nelle due sezioni seguenti:

* [Logica di visualizzazione](#display-logic)
* [Ignora logica](#skip-logic)

### Logica di visualizzazione {#display-logic}

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Forms personalizzato** ![](assets/custom-forms-icon.png).

1. Crea il modulo personalizzato di esempio:

   1. Fai clic su **Nuovo modulo personalizzato**, quindi fai clic su **Progetto** nell’elenco a discesa.

   1. In **Titolo modulo** casella, tipo **Modulo personalizzato di esempio - Logica della visualizzazione e logica di salto per l’apprendimento**.

   1. Fai clic su **Aggiungi un campo** nell&#39;angolo in alto a sinistra.
   1. Aggiungi un campo a discesa denominato *Campo problema* facendo clic su **Elenco a discesa**, quindi digita **Campo problema** in **Etichetta** scatola.

   1. Sotto **Scelte**, aggiungere le seguenti opzioni nelle caselle di testo:

      Ricerca necessaria

      Non più ricerca

   1. Fai clic su **Salva e chiudi** nell&#39;angolo in basso a sinistra.

1. Seleziona il nuovo **Modulo personalizzato di esempio - Logica della visualizzazione e logica di salto per l’apprendimento** modulo personalizzato, quindi fai clic su **Modifica**.

1. Aggiungi un nuovo campo di testo a riga singola denominato *Altre ricerche* facendo clic su **Campo di testo a riga singola**, quindi digita **Altre ricerche** in **Etichetta** scatola.

1. Fai clic su **Aggiungi logica** vicino al lato inferiore sinistro del **Modifica modulo personalizzato** schermo.

1. Nella casella visualizzata, con la **Logica display** aprire la scheda, impostare la logica per quando **Altre ricerche** Il campo verrà visualizzato sul modulo facendo clic su **Campo problema** nel primo elenco a discesa, **Ricerca necessaria** nel secondo elenco a discesa, e **Selezionati** nel terzo menu a discesa.
1. Fai clic su **Salva** per chiudere **Logica campo** finestra, quindi fai clic su **Fine** in **Impostazioni campo** area.

   Ora, quando qualcuno seleziona **Ricerca necessaria** in **Campo problema** a discesa, **Altre ricerche** verrà visualizzato il campo .

1. Fai clic su **Anteprima** per fare in modo che la logica sia visualizzata nel modo desiderato sul modulo.
1. Fai clic su **Anteprima finale** quando scopri che la logica funziona come previsto.
1. Fai clic su **Salva e chiudi** sulla **Modifica modulo personalizzato** per salvare il modulo, quindi continuare su [Ignora logica](#skip-logic) sotto.

### Ignora logica {#skip-logic}

Ignora le funzioni logiche in modo simile alla logica di visualizzazione, ma agisce come inverso: invece di creare campi personalizzati a scelta multipla specifici da visualizzare in base a selezioni specifiche, è possibile determinare quali campi ignorare in base alle selezioni degli utenti.

Per ulteriori informazioni, continuare a utilizzare il modulo personalizzato di esempio creato nella sezione [Logica di visualizzazione](#display-logic) nel presente articolo:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Forms personalizzato**.
1. Selezionare il modulo **Modulo personalizzato di esempio - Logica della visualizzazione e logica di salto per l’apprendimento** creato nei passaggi precedenti, quindi fai clic su **Modifica**.

1. Selezionare il campo a discesa creato denominato *Campo problema*.
1. Fai clic sul pulsante **Aggiungi logica** nel **Impostazioni campo** barra laterale.

1. In **Logica campo** Assicurati che **Ignora logica** è selezionata.

1. Imposta il primo menu a discesa su **Non più ricerca** e il secondo menu a discesa **Selezionati**.

1. In **Quindi Passa a** a discesa, seleziona **Fine del modulo.**

   Ora, quando qualcuno seleziona **Non più ricerca** in **Campo problema** campo a discesa, il modulo salterà direttamente alla fine del modulo senza visualizzare il **Altre ricerche** campo .

1. Fai clic su **Salva**.
1. Fai clic su **Anteprima**  per fare in modo che la logica sia applicata nel modo desiderato.
1. Fai clic su **Fine** nella parte inferiore sinistra del modulo.
