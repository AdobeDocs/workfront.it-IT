---
product-area: projects
navigation-topic: financials
title: Gestire le informazioni nell'area Finanza progetto
description: È possibile visualizzare o modificare le informazioni finanziarie di un progetto accedendo all'area Finanza della sezione Dettagli progetto.
author: Lisa
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '1297'
ht-degree: 2%

---

# Gestire le informazioni nell&#39;area Finanza progetto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

È possibile visualizzare o modificare le informazioni finanziarie di un progetto accedendo all&#39;area Finanza della sezione Dettagli progetto. In quest’area è disponibile un numero limitato di campi che è possibile visualizzare o modificare. Per informazioni sulla modifica di tutte le informazioni per un progetto, vedere [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

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
   <td role="rowheader">Licenza Adobe Workfront</td>
   <td>
   <p>Nuovo: Chiaro o superiore</p>
   <p>oppure</p>
   <p>Corrente: revisione o versione successiva</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Visualizzare o accedere ai progetti e ai dati finanziari</p> <p>Modifica l'accesso a Progetti e Dati finanziari per modificare le informazioni finanziarie sul progetto</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni per un progetto o versione successiva che includono le autorizzazioni View Finance</p> <p>Consente di gestire le autorizzazioni per il progetto, tra cui Gestisci dati finanziari, per modificare le informazioni finanziarie per il progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Panoramica dell&#39;area Finanza

Quando si visualizzano o si modificano informazioni nell&#39;area Finanza, tenere presente quanto segue:

* Le informazioni finanziarie disponibili nell&#39;area Contabilità di Dettagli progetto rappresentano i valori che vengono aggregati a livello di progetto dalle attività, nonché le informazioni immesse direttamente nel progetto. Alcune informazioni finanziarie possono essere gestite sia a livello di progetto che a livello di task.
* Per poter visualizzare l&#39;area Finanza di un progetto, è necessario disporre delle autorizzazioni di visualizzazione sul progetto e accedere ai dati finanziari dal proprio livello di accesso.
* Per poter modificare le informazioni nell&#39;area Finanza, è necessario disporre delle autorizzazioni Gestione del progetto e dell&#39;accesso ai dati finanziari dal proprio livello di accesso. Tuttavia, è consigliabile che solo il proprietario del progetto possa modificare le informazioni relative a questa area.

## Visualizzare informazioni finanziarie su un progetto

1. Vai a un progetto.
1. Fai clic su **Dettagli progetto** nel pannello a sinistra.
1. Fai clic sull&#39;icona **Modifica** ![Modifica](assets/edit-icon.png) nell&#39;angolo superiore destro della sezione Dettagli, quindi fai clic su **Finanza**.

   ![Area finanza nella visualizzazione dettagli](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >A seconda del modo in cui l’amministratore di Workfront ha configurato il modello di layout, la sezione Panoramica potrebbe non essere elencata per prima, nel qual caso è compressa. Per informazioni, vedere [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Visualizzare i campi seguenti nell&#39;area Finanza del progetto:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Metodo indice prestazioni</td> 
      <td> Controlla il metodo utilizzato da Workfront per calcolare le metriche di Valore guadagnato. Può essere basato sulle ore o sui costi. <br>Per ulteriori informazioni su PIM, vedere l'articolo <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Impostare il metodo di indicizzazione delle prestazioni (PIM)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">CPI/SPI/CSI</td> 
      <td> <p>Si tratta di metriche delle prestazioni del progetto che mostrano le prestazioni del progetto in un determinato momento. I valori vengono calcolati in base al metodo dell'indice delle prestazioni.<br>Per ulteriori informazioni, vedere i seguenti articoli: </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calcola indice prestazioni costi (IPC)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Calcola indice prestazioni pianificazione (SPI) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calcola indice prestazioni programma costi</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stima al completamento</td> 
      <td> Costo totale previsto del progetto, espresso in ore se il metodo di indicizzazione delle prestazioni (PIM) è basato sulle ore e rappresentato in un valore di valuta, se il metodo di indicizzazione delle prestazioni (PIM) è basato sui costi.<br>Per ulteriori informazioni sul calcolo della stima al completamento, vedere l'articolo <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calcola stima al completamento (EAC)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Budget</td> 
      <td>Budget impostato per il progetto. Questo viene specificato manualmente dal proprietario del progetto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costi fissi</td> 
      <td>Si tratta dei costi fissi del progetto, indipendenti dalle altre attività del progetto. Vengono immesse manualmente dal proprietario del progetto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo Pianificato</td> 
      <td>Costo stimato del progetto, in base alle ore pianificate e alle tariffe associate agli assegnatari delle attività (mansioni o utenti).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo Reale</td> 
      <td>Tutti i costi derivanti dal progetto. Costo effettivo è la somma di tutti i costi effettivi: costo manodopera (in base alle ore effettive e ai tassi associati alle mansioni o agli utenti che li registrano), spese e costi fissi, che possono essere associati a un progetto o a un task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reddito Fisso</td> 
      <td>Imposta il reddito previsto in base alla programmazione del progetto. I Redditi Fissi vengono specificati manualmente dal Proprietario del Progetto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reddito Pianificato</td> 
      <td>Reddito previsto previsto basato sulle ore pianificate e sulle tariffe associate agli assegnatari delle attività (mansioni o utenti).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reddito Reale</td> 
      <td>Reddito effettivo del progetto in base alle ore effettive e alle tariffe associate agli assegnatari delle attività (mansioni o utenti).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reddito Fatturato</td> 
      <td> <p>Ricavi fatturati ai clienti o ad altre parti e registrati nelle Fatturazioni. Per ulteriori informazioni sui record di fatturazione, vedere l'articolo <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">Creare record di fatturazione</a>. </p> </td> 
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

## Modificare le informazioni finanziarie su un progetto

In qualità di proprietario del progetto, è possibile modificare le informazioni nella scheda secondaria Finanza di un progetto.

Per modificare le informazioni nella scheda secondaria Dati finanziari progetto:

1. Vai a un progetto di cui sei il proprietario.

   >[!NOTE]
   >
   >Per eseguire i passaggi seguenti, è necessario disporre delle autorizzazioni di gestione per il progetto. È inoltre consigliabile che solo il proprietario del progetto apporti modifiche alla scheda secondaria Finanza del progetto.

1. Fai clic su **Dettagli progetto** nel pannello a sinistra.
1. Fai clic sull&#39;icona **Modifica** ![Icona Modifica](assets/edit-icon.png) nell&#39;angolo superiore destro della sezione Dettagli, quindi fai clic su **Finanza**. Verrà aperta l&#39;area Finanza per la modifica.
1. Modificare qualsiasi campo disponibile per la modifica facendo clic sul campo o facendo clic su **+Aggiungi** per aggiungere informazioni a un campo vuoto.

   >[!TIP]
   >
   >I campi non sono disponibili per la modifica se vengono calcolati automaticamente da Workfront o se non si dispone di autorizzazioni di modifica su di essi.

   ![Modifica area contabilità](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. Aggiorna uno dei campi seguenti.

   >[!NOTE]
   >
   >A seconda di come l’amministratore di Workfront configura il modello di layout, i campi nella sezione Dettagli progetto potrebbero essere diversi nel tuo ambiente. Per informazioni, vedere [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Metodo indice prestazioni</td> 
      <td> <p>Controlla il metodo utilizzato da Workfront per calcolare le metriche delle prestazioni del progetto. Questa impostazione viene configurata a livello di sistema dall’amministratore, ma puoi anche modificarla a livello di progetto. Prendi in considerazione di selezionare una delle seguenti opzioni:</p> 
       <ul> 
        <li><strong>Basato su Ore:</strong>Workfront utilizza le Ore pianificate nel calcolo di CPI ed EAC del progetto e l'EAC del progetto viene visualizzato come numero, in ore. </li> 
        <li><strong>Basato su costo:</strong>Workfront utilizza il Costo manodopera pianificata per calcolare l'IPC e l'CES del progetto e l'EAC viene visualizzato come valore di valuta. Quando si seleziona questa opzione, verificare che gli assegnatari delle attività (mansioni o utenti) siano associati a tassi di costo.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stima al completamento</td> 
      <td> <p>Rappresenta il costo totale previsto del progetto o dell'attività al completamento. Questa impostazione viene configurata a livello di sistema dall’amministratore, ma puoi anche modificarla a livello di progetto. Prendi in considerazione di selezionare una delle seguenti opzioni:</p> 
       <ul> 
        <li><strong>Calcola a livello di progetto</strong>: l'EAC per l'attività padre e il progetto vengono determinati inserendo nelle formule EAC le ore effettive/il costo effettivo della manodopera. Questo calcolo include le ore effettive, i costi e le spese aggiunti direttamente all'attività o al progetto padre.</li> 
        <li><strong>Rollup da attività/ sottoattività</strong>: l'EAC per l'attività e il progetto padre viene determinato sommando l'EAC per ogni attività figlio. Questo calcolo esclude le ore effettive, i costi e le spese aggiunti direttamente all'attività o al progetto padre.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Budget</td> 
      <td>Specifica il budget per questo progetto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costi fissi</td> 
      <td>Specifica il costo fisso per questo progetto. Ciò non deve includere costi di manodopera o di spesa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reddito Fisso</td> 
      <td> <p>Specifica le entrate fisse di questo progetto. Non dovrebbero essere incluse le entrate provenienti da record di fatturazione fatturati ai partner o a terzi.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Valuta progetto</td> 
      <td> <p>Specificare una valuta per il progetto, se diversa da quella predefinita nel sistema. La valuta predefinita nel sistema è definita dall'amministratore di Workfront. Per ulteriori informazioni sull'impostazione dei tassi di cambio in Workfront, vedere l'articolo <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Impostazione dei tassi di cambio</a>.</p> </td> 
     </tr>
    </tbody> 
   </table>

1. Fai clic su **Salva modifiche**.
