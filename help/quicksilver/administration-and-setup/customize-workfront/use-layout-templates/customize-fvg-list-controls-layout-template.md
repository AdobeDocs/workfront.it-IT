---
title: Personalizzare filtri, viste e raggruppamenti utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In qualità di amministratore di Workfront, è possibile utilizzare un modello di layout per specificare quali controlli elenco visualizzare nei menu a discesa Filtro, Visualizza e Raggruppamento. Questi menu vengono visualizzati sopra gli elenchi in Workfront, ad esempio l’elenco delle attività di un progetto.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: e9b61da8-2eca-4d88-969b-ae337e402540
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout

In qualità di amministratore di Adobe Workfront, puoi utilizzare un modello di layout per specificare quali controlli elenco visualizzare nei menu a discesa Filtro, Visualizza e Raggruppamento. Questi menu vengono visualizzati sopra gli elenchi in Workfront, ad esempio l’elenco delle attività di un progetto:

![](assets/filter-view-grouping-layout-templates.png)

Per ulteriori informazioni sui modelli di layout, vedere [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Per informazioni sui modelli di layout per i gruppi, vedere [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Dopo aver configurato un modello di layout, è necessario assegnarlo agli utenti affinché le modifiche apportate siano visibili agli altri utenti. Per informazioni sull&#39;assegnazione di un modello di layout agli utenti, vedere [Assegnare gli utenti a un modello di layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td><p>Nuovo: Standard</p>
  <p> Corrente: Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.
Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizzare i controlli Filtro, Visualizza e Raggruppamento:

1. Iniziare a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Fai clic sulla freccia rivolta verso il basso ![](assets/down-arrow-blue.png) in **Personalizza gli elementi visualizzati dagli utenti**, quindi fai clic su **Elenchi** nel menu a discesa visualizzato.

   ![](assets/customize-what-users-see-dropdown-on-pg-adobe-branding.png)

1. Fare clic sulla freccia rivolta verso il basso ![](assets/down-arrow-blue.png) in **Selezionare un elenco da personalizzare**, quindi selezionare il tipo di oggetto Workfront per il quale si desidera personalizzare i controlli Filtro, Visualizza e Raggruppamento.

   ![](assets/select-a-list-to-customize-menu-on-pg-adobe-branding.png)

   >[!NOTE]
   >
   >Se selezioni Progetti come elenco da personalizzare e poi disabiliti Progetti in cui sono o Progetti di cui sono proprietario nella sezione Filtro, gli utenti non vedranno più o non potranno utilizzare quel filtro:
   >
   >* Nell&#39;elenco di filtri visualizzato quando si fa clic sull&#39;icona del filtro ![](assets/filter-nwepng.png) sopra un elenco:
   >   
   >  ![](assets/disable-filters-projects-im-on-or-own.png)
   >   
   >* Nell’intestazione dell’area Progetti:
   >   
   >  ![](assets/disable-filter-pills.png)

1. (Facoltativo) Se desideri modificare il filtro, la visualizzazione o il raggruppamento predefiniti per il modello di layout, passa il puntatore del mouse sul filtro, sulla visualizzazione o sul raggruppamento, quindi fai clic su **Imposta come predefinito**.

   Le impostazioni predefinite scelte determinano gli utenti di Filtro, Visualizzazione e Raggruppamento da visualizzare negli elenchi in Workfront quando il modello di layout viene loro assegnato. Se non si modificano queste impostazioni predefinite, gli utenti visualizzeranno tutti gli elenchi come segue:

   * **Filtri**: Tutti
   * **Visualizzazione**: Standard (se applicabile; alcuni elenchi non dispongono di questa visualizzazione)
   * **Raggruppamento**: Niente

   È possibile nascondere le opzioni Tutto, Standard e Niente dopo aver selezionato diversi valori predefiniti (vedere il passaggio 5), ma non è possibile eliminarli.

   È possibile eliminare qualsiasi altra opzione utilizzata come impostazione predefinita, ma è necessario selezionare prima un&#39;impostazione predefinita diversa.

   Per informazioni sull&#39;eliminazione di filtri, viste e raggruppamenti, vedere [Creare, modificare e condividere filtri, viste e raggruppamenti predefiniti](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

1. Nascondere e aggiungere i controlli elenco nel modo seguente:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nascondere un controllo elenco</td> 
      <td> <p>Deselezionare o selezionare la casella accanto al controllo elenco che si desidera nascondere o visualizzare.</p> <p>Se una casella di controllo è disattivata, non è possibile nasconderla. L'impostazione predefinita <img src="assets/default-pill.png"> per ogni controllo elenco è disabilitata perché non è possibile nascondere l'impostazione attualmente configurata come predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aggiungere un controllo elenco personalizzato</td> 
      <td> <p> 
        <ol> 
         <li value="1"> Fare clic su <strong>Aggiungi filtro</strong>, <strong>Aggiungi visualizzazione</strong> o <strong>Aggiungi raggruppamento</strong> nella parte inferiore dell'elenco Filtro, Visualizzazione o Raggruppamento. Nella casella visualizzata, iniziare a digitare il nome di un controllo elenco personalizzato esistente creato in precedenza per l'organizzazione, quindi fare clic sul nome quando viene visualizzato.</li> 
         <li value="2"> Se si desidera impostare il nuovo controllo elenco personalizzato come filtro, visualizzazione o raggruppamento predefinito per il modello di layout, fare clic su <strong>Imposta come predefinito</strong>. </li> 
         <li value="3"> <p>Al termine, fai clic su <strong>Aggiungi</strong>.</p> <p><b>NOTA</b>: <p>Gli utenti possono aggiungere controlli elenco personalizzati ai propri elenchi. Se si aggiungono controlli elenco personalizzati in un modello di layout, i controlli elenco vengono aggiunti e spostati nella parte inferiore del pannello, senza sostituirli.</p> <p>Questo vale anche se si assegna l'utente a un nuovo modello di layout con controlli elenco personalizzati. </p> <p>Per informazioni sulla personalizzazione dei controlli elenco, vedere <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Panoramica filtri</a>, <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Panoramica visualizzazioni in Adobe Workfront</a> e <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Panoramica raggruppamenti in Adobe Workfront</a>.</p> </p> </li> 
        </ol> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Continuate a personalizzare il modello di layout.

   Oppure

   Se hai completato la personalizzazione, fai clic su **Salva**.

   >[!TIP]
   >
   >Puoi fare clic su Salva in qualsiasi momento per salvare l’avanzamento, quindi continuare a modificare il modello in un secondo momento.
