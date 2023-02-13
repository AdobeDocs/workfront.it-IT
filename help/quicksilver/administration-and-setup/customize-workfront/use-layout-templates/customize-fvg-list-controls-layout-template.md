---
title: Personalizzare filtri, visualizzazioni e gruppi utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In qualità di amministratore di Workfront, è possibile utilizzare un modello di layout per specificare quali controlli elenco visualizzare nei menu a discesa Filtra, Visualizza e Raggruppamento. Questi menu vengono visualizzati sopra gli elenchi in Workfront, ad esempio l’elenco delle attività per un progetto.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e9b61da8-2eca-4d88-969b-ae337e402540
source-git-commit: f3785c66b979cc95bf1d2d2ccacbdeefe0ef0967
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 0%

---

# Personalizzare filtri, visualizzazioni e gruppi utilizzando un modello di layout

In qualità di amministratore di Adobe Workfront, puoi utilizzare un modello di layout per specificare quali controlli elenco visualizzare nei menu a discesa Filtra, Visualizza e Raggruppamento . Questi menu vengono visualizzati sopra gli elenchi in Workfront, ad esempio l’elenco delle attività per un progetto:

![](assets/filter-view-grouping-layout-templates.png)

Per ulteriori informazioni sui modelli di layout, consulta [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Per informazioni sui modelli di layout per gruppi, consulta [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.
Per eseguirle per un gruppo, devi essere un responsabile di quel gruppo.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizzare i controlli dell’elenco Filtra, Visualizza e Raggruppamento:

1. Inizia a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Fai clic sulla freccia giù ![](assets/down-arrow-blue.png) sotto **Personalizzare ciò che gli utenti visualizzano**, quindi fai clic su **Elenchi** nel menu a discesa visualizzato.

   ![](assets/customize-what-users-see-dropdown-on-pg-adobe-branding.png)

1. Fai clic sulla freccia giù ![](assets/down-arrow-blue.png) sotto **Selezionare un elenco da personalizzare**, quindi selezionare il tipo di oggetto Workfront per il quale si desidera personalizzare i controlli dell’elenco Filtro, Visualizzazione e Raggruppamento.

   ![](assets/select-a-list-to-customize-menu-on-pg-adobe-branding.png)

   >[!NOTE]
   >
   >Se selezioni Progetti come elenco da personalizzare e disattivi Progetti in uso o Progetti di proprietà nella sezione Filtro , gli utenti non potranno più visualizzare o utilizzare il filtro:
   >
   >* Nell’elenco dei filtri che vengono visualizzati quando fanno clic sull’icona del filtro ![](assets/filter-nwepng.png) sopra un elenco:
   >   
   >  ![](assets/disable-filters-projects-im-on-or-own.png)
   >   
   >* Nell’intestazione dell’area Progetti :
   >   
   >  ![](assets/disable-filter-pills.png)

1. (Facoltativo) Per modificare il filtro, la visualizzazione o il raggruppamento predefiniti per il modello di layout, passa il puntatore del mouse sul filtro, sulla visualizzazione o sul raggruppamento, quindi fai clic su **Imposta come predefinito**.

   Le impostazioni predefinite selezionate determinano quali utenti di Filtro, Visualizzazione e Raggruppamento visualizzeranno negli elenchi in Workfront quando gli viene assegnato il modello di layout. Se non modifichi queste impostazioni predefinite, gli utenti visualizzano tutti gli elenchi come segue:

   * **Filtri**: Tutto
   * **Visualizza**: Standard (se applicabile); alcuni elenchi non dispongono di questa visualizzazione)
   * **Raggruppamento**: Niente

   È possibile nascondere le opzioni Tutto, Standard e Niente dopo aver selezionato diversi valori predefiniti (vedere il Passaggio 5), ma non è possibile eliminarli.

   È possibile eliminare qualsiasi altra opzione utilizzata come impostazione predefinita, ma prima è necessario selezionare un&#39;altra opzione predefinita.

   Per informazioni sull’eliminazione di filtri, visualizzazioni e raggruppamenti, consulta [Creare, modificare e condividere filtri, viste e raggruppamenti predefiniti](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

1. Nascondere e aggiungere controlli elenco come segue:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nascondere un controllo elenco</td> 
      <td> <p>Deselezionare o selezionare la casella accanto al controllo elenco che si desidera nascondere o visualizzare.</p> <p>Se una casella di controllo è disattivata, non è possibile nascondere tale controllo elenco. Predefinito <img src="assets/default-pill.png"> per ogni controllo elenco è disattivata perché non è possibile nascondere l'impostazione attualmente configurata come predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aggiungi un controllo elenco personalizzato</td> 
      <td> <p> 
        <ol> 
         <li value="1"> Fai clic su <strong>Aggiungi filtro</strong>, <strong>Aggiungi visualizzazione</strong>oppure <strong>Aggiungi raggruppamento</strong> nella parte inferiore dell’elenco Filtro, Visualizzazione o Raggruppamento. Nella casella visualizzata, inizia a digitare il nome di un controllo elenco personalizzato esistente creato in precedenza per l'organizzazione, quindi fai clic sul nome quando viene visualizzato.</li> 
         <li value="2"> Se si desidera impostare il nuovo controllo elenco personalizzato come filtro, visualizzazione o raggruppamento predefiniti per il modello di layout, fare clic su <strong>Imposta come predefinito</strong>. </li> 
         <li value="3"> <p>Fai clic su <strong>Aggiungi</strong> quando hai finito.</p> <p><b>NOTA</b>: <p>Gli utenti possono aggiungere controlli elenco personalizzati ai propri elenchi. Se si aggiungono controlli elenco personalizzati in un modello di layout, i controlli elenco vengono aggiunti e i relativi si spostano nella parte inferiore del pannello; il tuo non sostituisce il loro.</p> <p>Questo vale anche se si assegna l'utente a un nuovo modello di layout con controlli elenco personalizzati. </p> <p>Per informazioni sulla personalizzazione dei controlli elenco, consulta <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Panoramica sui filtri in Adobe Workfront</a>, <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Panoramica delle visualizzazioni in Adobe Workfront</a>e <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Panoramica sui raggruppamenti in Adobe Workfront</a>.</p> </p> </li> 
        </ol> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Continua a personalizzare il modello di layout.

   Oppure

   Al termine della personalizzazione, fai clic su **Salva**.

   >[!TIP]
   >
   >Puoi fare clic su Salva in qualsiasi momento per salvare l&#39;avanzamento, quindi continuare a modificare il modello in un secondo momento.
