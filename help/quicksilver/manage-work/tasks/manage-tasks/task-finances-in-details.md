---
product-area: projects
navigation-topic: manage-tasks
title: Gestire le finanze attività nella sezione Dettagli attività
description: Gestire le finanze attività nella sezione Dettagli attività
author: Alina
feature: Work Management
exl-id: 54ae48e5-bc8c-4e90-8fa1-0015523df4e6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 5%

---

# Gestire le finanze attività nella sezione Dettagli attività

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

Puoi visualizzare o modificare le informazioni finanziarie di un’attività accedendo all’area Panoramica della sezione Dettagli attività . È possibile visualizzare o modificare un numero limitato di campi in questa area. Per informazioni sulla modifica di tutte le informazioni finanziarie per un&#39;attività, vedere [Modifica delle attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti e attività</p> <p>Accesso ai dati finanziari o superiore</p> <p>Per modificare le informazioni finanziarie sulle attività è necessario disporre dell'accesso a Modifica dati finanziari</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza le autorizzazioni per l'attività che includono View Finance o versione successiva</p> <p>È necessario disporre delle autorizzazioni di gestione per l'attività che includono Modifica contabilità per modificare le informazioni finanziarie sulle attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Modificare le finanze delle attività nella sezione Dettagli attività

1. Passa a un progetto in cui desideri visualizzare un&#39;attività.

   >[!NOTE]
   >
   >Per trovare un’attività, è inoltre possibile cercarla e fare clic sul nome per accedere all’attività. Per ulteriori informazioni sulla ricerca di oggetti in Workfront, consulta [Ricerca in Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

1. Fai clic su **Attività** nel pannello a sinistra.
1. Fare clic sul nome di un&#39;attività che si desidera visualizzare.
1. Fai clic su **Dettagli attività**.
1. (Facoltativo) Fai clic sul pulsante **Comprimi tutto** in alto a destra della pagina Dettagli attività .

   ![](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >A seconda della modalità di configurazione del modello di layout da parte dell’amministratore di Workfront o dell’amministratore di gruppo, i campi della sezione Dettagli attività potrebbero essere ridisposti o non visualizzati. Per informazioni, consulta [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Fai clic su **Finanza** per espandere e visualizzare le informazioni finanziarie relative all&#39;attività.

   Fai clic sul pulsante **Modifica** icona ![](assets/edit-icon.png) nell&#39;angolo superiore destro della sezione Dettagli, quindi fai clic su **Finanza**.

1. Modifica i campi disponibili per la modifica facendo clic sul campo o facendo clic su **+Aggiungi** per aggiungere informazioni a un campo vuoto.
1. Rivedi o modifica le seguenti informazioni nel **Finanza** area :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipo Cst</td> 
      <td> <p>Specificare il tipo di costo per l'attività. Questo determinerà il calcolo del costo dell'attività, in base al numero di ore relative alle attività. </p> <p>Seleziona tra le seguenti opzioni: </p> 
       <ul> 
        <li> <p>Nessun Costo</p> </li> 
        <li> <p>Ore Fisse </p> </li> 
        <li> <p> Ore Utente </p> </li> 
        <li> <p> Ore Ruolo</p> </li> 
       </ul> <p>Per ulteriori informazioni sui costi di tracciamento, vedi <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Costi di tracciamento</a> . L'amministratore di Workfront o un amministratore di gruppo seleziona l'impostazione predefinita Tipo di costo per le attività nel sistema o nel gruppo. Per informazioni sull’impostazione dei valori predefiniti del progetto, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze del progetto a livello di sistema</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di Reddito</td> 
      <td> <p>Specifica il tipo di ricavi per l'attività. Questo determinerà il modo in cui vengono calcolati i Ricavi sull'attività, in base al numero di ore sulle attività. </p> <p>Seleziona tra le seguenti opzioni: </p> 
       <ul> 
        <li> <p> Non Fatturabile </p> </li> 
        <li> <p>Ore Utente </p> </li> 
        <li> <p>Ore Ruolo </p> </li> 
        <li> <p>Ore Fisse </p> </li> 
        <li> <p>Ore Utente w/Cap </p> </li> 
        <li> <p>Ore Ruolo w/Cap </p> </li> 
        <li> <p>Ore Utente più Fisso </p> </li> 
        <li> <p>Ore Ruolo più Fisso </p> </li> 
        <li> <p>Reddito Fisso </p> </li> 
       </ul> <p>Per ulteriori informazioni sul tracciamento dei ricavi, vedi<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica di fatturazione e ricavi</a> . </p> <p>L'amministratore di Workfront o l'amministratore di gruppo seleziona l'impostazione Tipo di ricavi predefinito per le attività nel sistema o nel gruppo. Per informazioni sull’impostazione dei valori predefiniti del progetto, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze del progetto a livello di sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo Pianificato</td> 
      <td> <p>Si tratta di un calcolo che mostra il costo dell'attività in base alle ore pianificate, al tipo di costo e alla tariffa oraria per gli utenti o i ruoli di lavoro. Per ulteriori informazioni sui costi di tracciamento, vedi <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Costi di tracciamento</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo effettivo</td> 
      <td> <p> Si tratta di un calcolo che mostra il costo dell'attività in base alle ore effettive, al tipo di costo e alla tariffa oraria per gli utenti o i ruoli di lavoro. Per ulteriori informazioni sui costi di tracciamento, vedi <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Costi di tracciamento</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reddito Pianificato</td> 
      <td> <p>Si tratta di un calcolo che mostra i ricavi associati all'attività in base alle ore pianificate, al tipo di ricavi e al tasso orario per gli utenti o i ruoli di lavoro. Per ulteriori informazioni sui costi di tracciamento, vedi <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Costi di tracciamento</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entrate effettive</td> 
      <td> <p>Si tratta di un calcolo che mostra i ricavi associati all'attività in base alle ore effettive, al tipo di ricavi e al tasso orario per gli utenti o i ruoli di lavoro. Per ulteriori informazioni sui costi di tracciamento, vedi <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Costi di tracciamento</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>CPI / SPI / CSI</strong> </td> 
      <td> <p>Si tratta di metriche delle prestazioni delle attività che mostrano le prestazioni dell’attività in un dato momento. I loro valori vengono calcolati in base al metodo Performance Index del progetto.<br>Per ulteriori informazioni, consulta i seguenti articoli:</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calcola indice di prestazione dei costi (CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Calcola indice delle prestazioni della pianificazione (SPI) </a> </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calcola indice prestazioni pianificazione costi (CSI)</a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stima al completamento (EAC)</td> 
      <td> <p>Questo è un calcolo che mostra il costo totale dell'attività al completamento. Per ulteriori informazioni sulla stima al completamento, vedi <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calcola Stima Al Completamento (EAC)</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condizionale) Se si modificano i campi nella sezione Finanza, fare clic su **Salva***modifiche**.
