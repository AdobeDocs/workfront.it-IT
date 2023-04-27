---
product-area: projects
navigation-topic: financials
title: Gestire le informazioni nell'area di finanziamento del progetto
description: Gestire le informazioni nell'area di finanziamento del progetto
author: Alina
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: d8c274d2153836647367c263cad8d786402cbe7f
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 2%

---

# Gestire le informazioni nell&#39;area di finanziamento del progetto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

È possibile visualizzare o modificare le informazioni finanziarie di un progetto accedendo all&#39;area Finanza della sezione Dettagli progetto. È possibile visualizzare o modificare un numero limitato di campi in questa area. Per informazioni sulla modifica di tutte le informazioni per un progetto, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

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
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizza o un accesso più elevato a progetti e dati finanziari</p> <p>Modifica l’accesso a Progetti e dati finanziari per modificare le informazioni finanziarie sul progetto</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza le autorizzazioni per un progetto o una versione successiva che includono le autorizzazioni di View Finance</p> <p>Consente di gestire le autorizzazioni per il progetto che includono Gestisci contabilità per modificare le informazioni finanziarie per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Panoramica dell&#39;area Finanza

Quando si visualizzano o si modificano le informazioni nell&#39;area Contabilità:

* Le informazioni finanziarie disponibili nell&#39;area Finanza di Dettagli progetto rappresentano i valori che si estendono a livello di progetto dalle attività, nonché le informazioni inserite direttamente nel progetto. Alcune informazioni finanziarie possono essere gestite sia a livello di progetto che a livello di attività.
* Per poter visualizzare l&#39;area Finanza in un progetto, è necessario disporre delle autorizzazioni di visualizzazione per il progetto e dell&#39;accesso ai dati finanziari dal livello di accesso.
* Per poter modificare le informazioni sull&#39;area Finanza , è necessario disporre delle autorizzazioni Gestisci sul progetto e dell&#39;accesso a Dati finanziari dal livello di accesso. Tuttavia, consigliamo solo al proprietario del progetto di modificare le informazioni su questa area .

## Visualizza informazioni finanziarie su un progetto

1. Vai a un progetto.
1. Fai clic su **Dettagli progetto** nel pannello a sinistra.
1. Fai clic sul pulsante **Modifica** icona ![](assets/edit-icon.png) nell&#39;angolo superiore destro della sezione Dettagli, quindi fai clic su **Finanza**.

   ![](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >A seconda della configurazione del modello di layout da parte dell’amministratore di Workfront, la sezione Panoramica potrebbe non essere elencata per prima, nel qual caso viene compressa. Per informazioni, consulta [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Visualizzare i campi seguenti nell&#39;area Finanza del progetto:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Metodo Indicizzazione Performance</td> 
      <td> Controlla il metodo utilizzato da Workfront per calcolare le metriche del valore generato. Può essere basato su ore o su costi. <br>Per ulteriori informazioni sul PIM, consulta l’articolo <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Impostare il metodo Performance Index (PIM)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">CPI / SPI / CSI</td> 
      <td> <p>Si tratta di metriche delle prestazioni del progetto che mostrano le prestazioni del progetto in un dato momento. I loro valori vengono calcolati in base al metodo Performance Index.<br>Per ulteriori informazioni, consulta i seguenti articoli: </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calcola indice di prestazione dei costi (CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Calcola indice delle prestazioni della pianificazione (SPI) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calcola indice prestazioni pianificazione costi (CSI)</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stima al completamento</td> 
      <td> Costo totale previsto del progetto, rappresentato in ore se il metodo dell'indice delle prestazioni (PIM) è basato su ore e viene rappresentato in un valore in valuta se il metodo dell'indice delle prestazioni (PIM) è basato sui costi.<br>Per ulteriori informazioni sul calcolo della stima al completamento, consulta l’articolo <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calcola Stima Al Completamento (EAC)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bdg</td> 
      <td>Questo è il budget impostato per il progetto. Questo è specificato manualmente dal proprietario del progetto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo Fisso</td> 
      <td>Si tratta dei costi fissi del progetto, indipendentemente da altre attività del progetto. Vengono immessi manualmente dal proprietario del progetto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo Pianificato</td> 
      <td>Il costo stimato del progetto, in base alle ore pianificate e ai tassi associati alle assegnazioni delle attività (ruoli o utenti).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo Reale</td> 
      <td>Tutti i costi relativi al progetto. Il costo effettivo è la somma di tutti i costi effettivi: costo della manodopera (in base alle ore effettive e ai tassi associati ai ruoli o agli utenti che li registrano), spese e costi fissi, che possono essere associati a un progetto o a un task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reddito Fisso</td> 
      <td>Imposta il reddito previsto in base alla pianificazione del progetto. I ricavi fissi vengono specificati manualmente dal proprietario del progetto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reddito Pianificato</td> 
      <td>Entrate previste in base alle ore pianificate e ai tassi associati alle assegnazioni delle attività (ruoli o utenti).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reddito Reale</td> 
      <td>Entrate effettive del progetto in base alle ore effettive e ai tassi associati agli assegnatari delle attività (ruoli o utenti).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reddito Fatturato</td> 
      <td> <p>Ricavi fatturati ai clienti o ad altre parti che vengono acquisiti nei record di fatturazione. Per ulteriori informazioni sui record di fatturazione, consulta l’articolo <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">Creazione di record di fatturazione</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
    </tbody> 
   </table>

## Modifica delle informazioni finanziarie su un progetto

In qualità di proprietario del progetto, è possibile modificare le informazioni nella sottoscheda Finanza di un progetto.

Per modificare le informazioni nella sottoscheda Finanza progetto:

1. Passa a un progetto di cui sei il proprietario.

   >[!NOTE]
   >
   >Per eseguire i passaggi seguenti, è necessario disporre delle autorizzazioni di gestione per il progetto. È inoltre consigliabile che solo il proprietario del progetto apporti modifiche alla sottoscheda Finanza del progetto.

1. Fai clic su **Dettagli progetto** nel pannello a sinistra.
1. Fai clic sul pulsante **Modifica** icona ![](assets/edit-icon.png) nell&#39;angolo superiore destro della sezione Dettagli, quindi fai clic su **Finanza** . Viene aperta l&#39;area Finanza per la modifica.
1. Modifica i campi disponibili per la modifica facendo clic sul campo o facendo clic su **+Aggiungi** per aggiungere informazioni a un campo vuoto.

   >[!TIP]
   >
   >I campi non sono disponibili per la modifica se vengono calcolati automaticamente da Workfront o se non si dispone delle autorizzazioni di modifica.

   ![](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. Aggiorna uno dei campi seguenti.

   >[!NOTE]
   >
   >A seconda della configurazione del modello di layout da parte dell’amministratore di Workfront, i campi nella sezione Dettagli progetto potrebbero essere diversi nell’ambiente in uso. Per informazioni, consulta [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Metodo Indicizzazione Performance</td> 
      <td> <p>Controlla il metodo utilizzato da Workfront per calcolare le metriche delle prestazioni del progetto. Questa impostazione viene configurata a livello di sistema dall’amministratore, ma puoi anche modificarla a livello di progetto. Scegli una delle seguenti opzioni:</p> 
       <ul> 
        <li><strong>Basato su ora:</strong>Workfront utilizza le ore pianificate per calcolare l’IPC e l’EAC del progetto e l’EAC del progetto viene visualizzato come numero, in ore. </li> 
        <li><strong>Basato sui costi:</strong>Workfront utilizza il costo del lavoro pianificato per calcolare l’IPC e l’EAC del progetto, e l’EAC viene visualizzato come valore di valuta. Quando si seleziona questa opzione, assicurarsi che le assegnatarie dell'attività (ruoli o utenti) siano associate alle tariffe di costo.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stima al completamento</td> 
      <td> <p>Rappresenta il costo totale previsto del progetto o dell'attività al completamento. Questa impostazione viene configurata a livello di sistema dall’amministratore, ma puoi anche modificarla a livello di progetto. Scegli una delle seguenti opzioni:</p> 
       <ul> 
        <li><strong>Calcola a livello di progetto</strong>: L'EAC per l'attività e il progetto padre viene determinato inserendo le ore effettive/il costo effettivo del lavoro nelle formule EAC. Questo calcolo include le ore/costi effettivi e le spese aggiunte direttamente all'attività o al progetto padre.</li> 
        <li><strong>Eseguire il rollup da attività/sottoattività</strong>: L'EAC per l'attività e il progetto padre viene determinato sommando l'EAC per ogni attività figlio. Questo calcolo esclude le ore/i costi effettivi e le spese aggiunte direttamente all'attività o al progetto padre.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bdg</td> 
      <td>Specifica il budget per il progetto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo Fisso</td> 
      <td>Specifica il costo fisso per il progetto. Ciò non dovrebbe includere i costi di manodopera o di spesa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reddito Fisso</td> 
      <td> <p>Specifica i ricavi fissi del progetto. Ciò non dovrebbe includere i ricavi provenienti da qualsiasi record di fatturazione fatturati a partner o terze parti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Valuta progetto</td> 
      <td> <p>Specificare una valuta per il progetto, se è diversa dalla valuta predefinita nel sistema. La valuta predefinita nel sistema è definita dall’amministratore Workfront. Per ulteriori informazioni sull'impostazione dei tassi di cambio in Workfront, consulta l'articolo <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Imposta i tassi di cambio</a>.</p> </td> 
     </tr>
    </tbody> 
   </table>

1. Fai clic su **Salva modifiche**.
