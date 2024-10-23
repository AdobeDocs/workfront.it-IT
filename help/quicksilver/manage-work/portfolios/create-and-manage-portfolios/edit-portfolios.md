---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Modifica i Portfolio
description: Puoi modificare le informazioni sui portfolio che hai creato o che altri utenti hanno creato se li hanno condivisi con te. Questo articolo descrive come cercare, trovare e modificare un portfolio, se si dispone delle autorizzazioni necessarie.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 0a2e18c3-1722-4fc6-8442-19e80eca9d47
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1009'
ht-degree: 1%

---

# Modificare i portfolio

Puoi modificare le informazioni sui portfolio che hai creato o che altri utenti hanno creato se li hanno condivisi con te.

Puoi modificare un [!UICONTROL portfolio] nella pagina del portfolio oppure puoi modificare i portfolio in un elenco.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td> <p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] licenze*</td> 
   <td> <p>Nuovo: Standard</p>
   <p>Corrente: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso</td> 
   <td> <p>Accesso a [!UICONTROL Edit] ai Portfoli</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni [!UICONTROL Manage] per un portfolio</p>
   <p> Gestisci le autorizzazioni per i progetti nel portfolio per aggiungerli o rimuoverli dal portfolio</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modificare i portfolio

{{step1-to-portfolios}}

1. Fai clic sul nome di un portfolio per aprirlo.
1. (Facoltativo) Per modificare informazioni limitate sul portfolio, fai clic su **[!UICONTROL Dettagli Portfolio]** nel pannello a sinistra.

   ![](assets/portfolio-details-tab-nwe-350x163.png)

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the note below will also be true for Edit Portfolio box)</p>
   -->

   >[!NOTE]
   >
   >A seconda della modalità di modifica del modello di layout da parte dell&#39;amministratore di [!DNL Workfront] o del gruppo, i campi nell&#39;area [!UICONTROL Dettagli Portfolio] potrebbero essere ridisposti o non essere visualizzati. Per informazioni, vedere [Personalizzare la visualizzazione [!UICONTROL Dettagli] utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Per modificare le informazioni nella sezione [!UICONTROL Dettagli], eseguire le operazioni seguenti:

   1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Comprimi tutto]** nell&#39;angolo superiore destro per comprimere tutte le aree.
   1. (Facoltativo e condizionale) Quando un&#39;area è compressa, fare clic sulla **freccia rivolta a destra** ![](assets/right-pointing-arrow.png) accanto a ogni area per espandere l&#39;area che si desidera modificare.
   1. Per informazioni sui campi visibili nella sezione [!UICONTROL Dettagli Portfolio], continuare a modificare il portfolio nella casella [!UICONTROL Modifica Portfolio] come descritto di seguito.
   1. (Facoltativo) Se non sono presenti moduli personalizzati allegati al portfolio, inizia a digitare il nome di un modulo nel campo **[!UICONTROL Aggiungi modulo personalizzato]**, selezionalo quando viene visualizzato nell&#39;elenco, quindi fai clic su **[!UICONTROL Salva modifiche]**.
   1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Esporta]** ![](assets/export.png) per esportare le informazioni [!UICONTROL Panoramica] e moduli personalizzati in un file PDF, quindi fai clic su **[!UICONTROL Esporta]**. Selezionare una delle opzioni seguenti:

      * Seleziona tutto (viene visualizzato solo se è allegato almeno un modulo personalizzato)
      * Panoramica
      * Nome di uno o più moduli personalizzati

      Il file PDF viene scaricato nel computer.

      ![](assets/export-portfolio-details-box-with-export-button-350x368.png)

      Per ulteriori informazioni, vedere [Esportare moduli personalizzati e dettagli oggetto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).


1. Per modificare tutte le informazioni su uno o più portfolio, effettuare una delle seguenti operazioni:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might have to be split in two sections if the single edit and the bulk edit won't come at the same time for portfolios)</p>
   -->

   * Fai clic sul menu **[!UICONTROL Altro]** accanto al nome del portfolio, quindi **[!UICONTROL Modifica].**

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will change in NWE with a new Edit Portfolio UI)</p>   
     -->

   * Vai a un elenco di portfolio e seleziona uno o più portfolio da modificare, quindi fai clic sull&#39;icona **[!UICONTROL Modifica]** ![](assets/edit-icon.png) nella parte superiore dell&#39;elenco.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to split into another section when they release the new [!UICONTROL Edit Portfolio] UI)</p>   
     -->
   Viene visualizzata la finestra di dialogo **[!UICONTROL Modifica Portfolio]**.

   ![](assets/edit-portfolio-box-classic-350x224.png)

   Tutti i campi portfolio sono disponibili nella casella [!UICONTROL Modifica Portfolio] e sono raggruppati per le aree elencate nel pannello sinistro.

1. Prendere in considerazione la possibilità di specificare informazioni in una delle sezioni seguenti:

   * [[!UICONTROL Panoramica]](#overview)
   * [Moduli personalizzati](#Custom%C2%A0F)
   * [Commento](#comment)

### [!UICONTROL Panoramica] {#overview}

1. Inizia a modificare un portfolio come descritto in precedenza.
1. Fai clic su **[!UICONTROL Panoramica]** e specifica i campi seguenti:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: note below is drafted: drafted till they release new Edit Portfolio boxes)</p>
   -->

   <!--
   <note type="note">
   Depending on how your Workfront administrator or Group administrator sets up our Layout Template, the fields in the Edit Portfolio box might be rearranged or not display. For information, see
   <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md" class="MCXref xref">Customize the Details view using a layout template</a>.
   </note>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Aggiorna il nome del portfolio. </p> <p>Suggerimento: questa opzione non è disponibile se hai selezionato più di un portfolio. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td> <p>Digitare una descrizione per il Portfolio per indicare l'elemento univoco. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Gestione Portfoli]</td> 
      <td> <p>Inizia a digitare il nome di un utente che desideri indicare come gestore del portfolio, quindi selezionalo quando viene visualizzato nell’elenco. Corrisponde al proprietario del Portfolio [!UICONTROL]. Questa è la persona che può supervisionare il lavoro definito nei progetti del portfolio e può approvare il Business Case.</p> <p>Importante: quando si designa un utente come manager di Portfolio, questi ottiene automaticamente le autorizzazioni [!UICONTROL Manage] per il portfolio, i programmi e i progetti in esso contenuti. </p> <p>Suggerimento: puoi aggiornare rapidamente il gestore portfolio nell’intestazione del portfolio. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Group]</td> 
      <td> <p>Aggiungi il nome di un singolo gruppo se il gruppo è associato al portfolio o se ne ha la responsabilità di completarlo. </p> <p>Suggerimento  <p>Quando si accede al campo [!UICONTROL Group] dalla pagina [!UICONTROL Portfolio Details], eseguire le operazioni seguenti: </p> <p>Per assicurarsi di selezionare il gruppo corretto, posizionare il puntatore del mouse su di esso e fare clic sull'icona [!UICONTROL information] <img src="assets/info-icon.png"> visualizzata accanto ad esso. In questo modo viene visualizzata una descrizione del gruppo contenente informazioni sul gruppo stesso, ad esempio la gerarchia dei gruppi al di sopra del gruppo e i relativi amministratori.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> <p>Questa opzione non è disponibile nella casella [!UICONTROL Modifica Portfolio]. </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Allineamento Scorecard]</p> </td> 
      <td> <p>Selezionare la scorecard di allineamento che si desidera utilizzare dall'elenco a discesa. Una scorecard viene utilizzata per misurare il livello di allineamento di un progetto con i criteri stabiliti di un Portfolio, che spesso riflettono la missione, i valori e gli obiettivi strategici di un’organizzazione. Per ulteriori informazioni, vedere <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Applicare una scorecard a un progetto e generare un punteggio di allineamento</a> e <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">Creare una scorecard</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL È Attivo]</td> 
      <td> <p> Seleziona questa casella di controllo se desideri che il portfolio sia attivo. Altri utenti possono trovare portfolio attivi e allegarli ai progetti durante la creazione o la modifica di progetti. I portfolio inattivi non possono essere allegati ai progetti. Questa opzione è attivata per impostazione predefinita.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Salva modifiche]** o continua a modificare le sezioni seguenti.

### Moduli personalizzati

1. Inizia a modificare il portfolio come descritto in precedenza.
1. Fai clic sul menu a discesa **[!UICONTROL Aggiungi Forms]** per selezionare un modulo personalizzato e aggiungerlo al portfolio.

   È necessario creare moduli personalizzati del portfolio prima che siano disponibili per l’aggiunta.

   >[!NOTE]
   >
   >A seconda di come l&#39;amministratore di [!DNL Workfront] ha impostato le autorizzazioni per le sezioni nel modulo personalizzato, non tutti possono visualizzare o modificare gli stessi campi in un determinato modulo personalizzato. Le autorizzazioni per modificare i campi all’interno di una sezione di un modulo personalizzato dipendono dalle autorizzazioni di cui disponi sul portfolio stesso. Per informazioni sull&#39;impostazione delle autorizzazioni per le sezioni di un modulo personalizzato, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Aggiorna i campi nei moduli personalizzati, quindi fai clic su **[!UICONTROL Salva modifiche]** o continua con la sezione seguente.

### Commento {#comment}

1. Inizia a modificare un portfolio come descritto in precedenza.
1. Fai clic su **[!UICONTROL Commento]**.

   ![](assets/comment-box-edit-portfolio-classic-350x227.png)

1. Aggiungi un commento in **[!UICONTROL Pubblica un aggiornamento per il campo portfolio]**.
1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Persone]** per aggiungere un utente o un team al commento.
1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Blocca]** per bloccare il commento e renderlo privato solo per gli utenti della tua azienda.
1. Fai clic su **[!UICONTROL Salva modifiche]**.
