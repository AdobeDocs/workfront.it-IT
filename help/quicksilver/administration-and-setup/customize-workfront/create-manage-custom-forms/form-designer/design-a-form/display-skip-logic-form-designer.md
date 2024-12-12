---
title: Aggiungere logica di visualizzazione e salta logica a un modulo
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile decidere quali sezioni di un modulo personalizzato devono essere visualizzate o ignorate in base alle scelte effettuate da un utente durante la compilazione.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5f5dbeb5-b974-489c-8f4d-ebaa00f5e5ba
source-git-commit: 75aaa531dba8037ed75c0d6baa6d7c69ec4cfefd
workflow-type: tm+mt
source-wordcount: '1317'
ht-degree: 0%

---

# Aggiungere logica di visualizzazione e logica di salto a un modulo

È possibile decidere quali sezioni di un modulo personalizzato devono essere visualizzate o ignorate in base alle scelte effettuate da un utente durante la compilazione.

>[!NOTE]
>
>La logica si applica solo all’interno di un modulo e non può essere basata su selezioni da un modulo diverso.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">piano Adobe Workfront </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Nuovo: Standard</p>
   <p>oppure</p>
   <p>Corrente: Piano</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Accesso amministrativo ai moduli personalizzati </td> 
  </tr>  
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare e saltare le icone della logica

I moduli personalizzati visualizzano icone per indicare la logica applicata a determinati campi. Le icone di un campo nel progettista del modulo indicano che la logica viene applicata al campo.

| Icona | Posizione nel campo in Progettazione moduli | Definizione |
|--- |--- |--- |
| ![Logica di visualizzazione per il campo di destinazione](assets/display-logic-bottom-left.png) | In basso a sinistra | Il campo è il campo di destinazione per la logica di visualizzazione. Se nel modulo viene effettuata una selezione specifica, viene visualizzato questo campo. |
| ![Definisci l&#39;icona della logica di visualizzazione](assets/display-logic-bottom-right.png) | In basso a destra | Il campo definisce la logica di visualizzazione. Una selezione o un valore specifico in questo campo visualizza il campo di destinazione. |
| ![Logica di salto per il campo di destinazione](assets/skip-logic-bottom-left.png) | In basso a sinistra | Il campo è il campo di destinazione per la logica di salto. Se nel modulo viene effettuata una selezione specifica, il modulo passa a questo campo e i campi intermedi sono nascosti. |
| ![Definisci l&#39;icona per ignorare la logica](assets/skip-logic-bottom-right.png) | In basso a destra | Il campo definisce la logica di salto. Una selezione o un valore specifico in questo campo ignora altri campi e passa direttamente al campo di destinazione. |

![Icone logiche](assets/logic-icons-3.png)

Seleziona un campo a cui è applicata la logica per visualizzare le regole di logica esistenti nelle impostazioni del campo.

![Regole logiche](assets/form-designer-view-only-logic.png)

## Considerazioni per l’utilizzo della logica di visualizzazione e della logica di salto

* Per aggiungere la logica di visualizzazione a un campo personalizzato, a un widget o a un&#39;interruzione di sezione, è necessario posizionare almeno un campo a scelta multipla (pulsanti di scelta, elenco a discesa o caselle di controllo) prima di inserirlo nel modulo.
Per informazioni sui campi personalizzati e i widget nei moduli personalizzati, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Non è possibile aggiungere logica di salto a un widget o a un’interruzione di sezione. È possibile aggiungerlo solo a un campo a scelta multipla (pulsanti di scelta, menu a discesa o caselle di controllo).
* Non è possibile applicare la logica di visualizzazione o di salto per mostrare o nascondere le scelte di un campo con più opzioni. Ad esempio, non è possibile limitare le scelte visualizzate per un campo a discesa, un gruppo di caselle di controllo o un campo Pulsante di scelta in base alla logica di visualizzazione o salto di un altro campo.
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

## Aggiungere logica di visualizzazione a un modulo personalizzato

La logica di visualizzazione definisce quali campi personalizzati vengono visualizzati nel modulo quando l’utente seleziona un valore specifico in un campo a scelta multipla. La logica viene aggiunta al campo di destinazione, che viene visualizzato solo quando il valore è selezionato.

{{step-1-to-setup}}

1. Fare clic su **Forms personalizzato**.
1. Crea un nuovo modulo personalizzato o apri un modulo esistente. Per ulteriori dettagli, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
1. Aggiungi i campi al modulo in base alle esigenze. Almeno un campo a scelta multipla (pulsante di opzione, elenco a discesa o casella di controllo) deve essere posizionato prima del campo di destinazione che verrà visualizzato.
1. Seleziona il campo di destinazione e fai clic su **Aggiungi logica** in basso a sinistra nella schermata.
1. Selezionare la scheda **Logica di visualizzazione**.
1. Fai clic su **Aggiungi regola di visualizzazione** nel generatore di logica.

   ![Generatore di logica di visualizzazione](assets/custom-form-logic-builder-display-blank.png)

1. Per creare l’istruzione logica, segui i passaggi indicati di seguito nel generatore.

   1. La prima opzione consiste nel scegliere il campo di definizione. Questo è il campo con il valore di selezione che visualizza la destinazione. Deve essere un campo a scelta multipla.
   1. La seconda opzione consiste nel scegliere il valore di selezione. Sono disponibili solo i valori già definiti per quel campo.
   1. La terza opzione è **Selezionato** o **Non selezionato**. Scegliendo **Selezionato**, quando il valore è selezionato, viene visualizzato il campo di destinazione. La scelta di **Non selezionato** indica che quando nel campo di definizione viene selezionato un altro valore, viene visualizzato il campo di destinazione.
   1. Per aggiungere una regola **And** all&#39;istruzione logica, fare clic su **Aggiungi regola** direttamente sotto la regola appena creata. Segui le stesse istruzioni per generare la regola. Affinché il campo di destinazione venga visualizzato, è necessario che siano soddisfatte tutte le regole AND.

      ![Generatore di logica di visualizzazione](assets/custom-form-logic-builder-display1.png)

   1. Per aggiungere una regola **Or** all&#39;istruzione di logica, fare clic su **Aggiungi regola** nella parte inferiore del generatore di logica. Quindi, fai clic su **Aggiungi regola** all&#39;interno dell&#39;area O e segui le stesse istruzioni per generare la regola. Quando viene soddisfatta una regola Or, viene visualizzato il campo di destinazione.

1. Fai clic su **Salva** al termine della creazione dell&#39;istruzione logica.

   Le icone della logica di visualizzazione vengono aggiunte al campo di destinazione e al campo di definizione nel progettista del modulo.

## Aggiungere la logica di salto a un modulo personalizzato

La logica di salto definisce i campi modulo personalizzati che vengono saltati quando l’utente seleziona un valore specifico in un campo a scelta multipla. I campi ignorati sono nascosti nel modulo. La logica viene applicata al campo di definizione in cui viene effettuata la selezione, non ai campi saltati.

{{step-1-to-setup}}

1. Fare clic su **Forms personalizzato**.
1. Crea un nuovo modulo personalizzato o apri un modulo esistente. Per ulteriori dettagli, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
1. Aggiungi i campi al modulo in base alle esigenze. Il campo di definizione per la logica di salto deve essere un campo a scelta multipla (pulsante di scelta, elenco a discesa o casella di controllo).
1. Seleziona il campo di definizione e fai clic su **Aggiungi logica** in basso a sinistra nella schermata.
1. Selezionare la scheda **Ignora logica**.
1. Fai clic su **Aggiungi Ignora regola** nel generatore di logica.

   ![Ignora generatore di logica](assets/custom-form-logic-builder-skip-blank.png)

1. Per creare l’istruzione logica, segui i passaggi indicati di seguito nel generatore.

   1. Il campo di definizione viene visualizzato nel generatore. È il campo a cui hai selezionato la logica di salto.
   1. La prima opzione consiste nel scegliere il valore di selezione. Sono disponibili solo i valori già definiti per il campo.
   1. La seconda opzione è **Selezionato** o **Non selezionato**. La scelta di **Selezionato** implica che quando il valore è selezionato, il campo di destinazione viene visualizzato e i campi intermedi vengono ignorati. La scelta di **Non selezionato** indica che quando nel campo di definizione viene selezionato un altro valore, viene visualizzato il campo di destinazione e i campi intermedi vengono ignorati.
   1. La terza opzione è il campo di destinazione o il punto in cui passare. Selezionare un nome di campo o **Fine modulo**. Potrebbe essere necessario fare clic sulla parola &quot;vuoto&quot; prima di selezionare un&#39;opzione.

      ![Ignora generatore di logica](assets/custom-form-logic-builder-skip1.png)

   1. Per aggiungere una regola **Or** all&#39;istruzione di logica, fare clic su **Aggiungi regola** nella parte inferiore del generatore di logica. Quindi, seleziona le opzioni seguendo le stesse istruzioni per creare la regola. Quando viene soddisfatta una regola **Or**, viene visualizzato il campo di destinazione.

1. Fai clic su **Salva** al termine della creazione dell&#39;istruzione logica.

   Le icone di salto della logica vengono aggiunte al campo di destinazione e al campo di definizione nel progettista del modulo.


