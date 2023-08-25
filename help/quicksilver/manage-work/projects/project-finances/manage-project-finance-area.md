---
product-area: projects
navigation-topic: financials
title: Gestire le informazioni nell'area Finanza progetto
description: Gestire le informazioni nell'area Finanza progetto
author: Alina
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: 647788221b4acff1cfd5e0ce14d5b99cf90ceee0
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Gestire le informazioni nell&#39;area Finanza progetto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

È possibile visualizzare o modificare le informazioni finanziarie di un progetto accedendo all&#39;area Finanza della sezione Dettagli progetto. In quest’area è disponibile un numero limitato di campi che è possibile visualizzare o modificare. Per informazioni sulla modifica di tutte le informazioni di un progetto, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Visualizzare o accedere ai progetti e ai dati finanziari</p> <p>Modifica l'accesso a Progetti e Dati finanziari per modificare le informazioni finanziarie sul progetto</p> <p><b>NOTA</b></p>
   <p> Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni per un progetto o versione successiva che includono le autorizzazioni View Finance</p> <p>Consente di gestire le autorizzazioni per il progetto, tra cui Gestisci dati finanziari, per modificare le informazioni finanziarie per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Panoramica dell&#39;area Finanza

Quando si visualizzano o si modificano informazioni nell&#39;area Finanza, tenere presente quanto segue:

* Le informazioni finanziarie disponibili nell&#39;area Contabilità di Dettagli progetto rappresentano i valori che vengono aggregati a livello di progetto dalle attività, nonché le informazioni immesse direttamente nel progetto. Alcune informazioni finanziarie possono essere gestite sia a livello di progetto che a livello di task.
* Per poter visualizzare l&#39;area Finanza di un progetto, è necessario disporre delle autorizzazioni di visualizzazione sul progetto e accedere ai dati finanziari dal proprio livello di accesso.
* Per poter modificare le informazioni nell&#39;area Finanza, è necessario disporre delle autorizzazioni Gestione del progetto e dell&#39;accesso ai dati finanziari dal proprio livello di accesso. Tuttavia, è consigliabile che solo il proprietario del progetto possa modificare le informazioni relative a questa area.

## Visualizzare informazioni finanziarie su un progetto

1. Vai a un progetto.
1. Clic **Dettagli progetto** nel pannello a sinistra.
1. Fai clic su **Modifica** icona ![](assets/edit-icon.png) nell’angolo superiore destro della sezione Dettagli, quindi fai clic su **Finanza**.

   ![](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >A seconda del modo in cui l’amministratore di Workfront ha configurato il modello di layout, la sezione Panoramica potrebbe non essere elencata per prima, nel qual caso è compressa. Per informazioni, consulta [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Visualizzare i campi seguenti nell&#39;area Finanza del progetto:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Metodo di indice performance</td> 
      <td> Controlla il metodo utilizzato da Workfront per calcolare le metriche di Valore guadagnato. Può essere basato sulle ore o sui costi. <br>Per ulteriori informazioni sulla protezione PIM, vedere l'articolo <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Impostare il metodo PIM (Performance Index Method)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">CPI / SPI / CSI</td> 
      <td> <p>Si tratta di metriche delle prestazioni del progetto che mostrano le prestazioni del progetto in un determinato momento. I valori vengono calcolati in base al metodo dell'indice delle prestazioni.<br>Per ulteriori informazioni, consulta i seguenti articoli: </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calcola indice prestazioni costi (IPC)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Calcola indice prestazioni Schedule (SPI) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calcola indice prestazioni programma costi (CSI)</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stima al completamento</td> 
      <td> Costo totale previsto del progetto, espresso in ore se il metodo di indicizzazione delle prestazioni (PIM) è basato sulle ore e rappresentato in un valore di valuta, se il metodo di indicizzazione delle prestazioni (PIM) è basato sui costi.<br>Per ulteriori informazioni sul calcolo della stima al completamento, vedere l'articolo <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calcola stima al completamento (EAC)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bdg</td> 
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
      <td> <p>Ricavi fatturati ai clienti o ad altre parti e registrati nelle Fatturazioni. Per ulteriori informazioni sui record di fatturazione, consulta l’articolo <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">Crea record fatturazione</a>. </p> </td> 
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

1. Clic **Dettagli progetto** nel pannello a sinistra.
1. Fai clic su **Modifica** icona ![](assets/edit-icon.png) nell’angolo superiore destro della sezione Dettagli, quindi fai clic su **Finanza** . Verrà aperta l&#39;area Finanza per la modifica.
1. Modificare qualsiasi campo disponibile per la modifica facendo clic sul campo o facendo clic su **+Aggiungi** per aggiungere informazioni a un campo vuoto.

   >[!TIP]
   >
   >I campi non sono disponibili per la modifica se vengono calcolati automaticamente da Workfront o se non si dispone di autorizzazioni di modifica su di essi.

   ![](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. Aggiorna uno dei campi seguenti.

   >[!NOTE]
   >
   >A seconda di come l’amministratore di Workfront configura il modello di layout, i campi nella sezione Dettagli progetto potrebbero essere diversi nel tuo ambiente. Per informazioni, consulta [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Metodo di indice performance</td> 
      <td> <p>Controlla il metodo utilizzato da Workfront per calcolare le metriche delle prestazioni del progetto. Questa impostazione viene configurata a livello di sistema dall’amministratore, ma puoi anche modificarla a livello di progetto. Prendi in considerazione di selezionare una delle seguenti opzioni:</p> 
       <ul> 
        <li><strong>Basato su Ore:</strong>Workfront utilizza le ore pianificate per calcolare l’IPC e l’CES del progetto, e l’CES del progetto viene visualizzato come un numero, in ore. </li> 
        <li><strong>Basato su Costo:</strong>Workfront utilizza il Costo manodopera pianificata per calcolare l'IPC e l'CES del progetto e l'CES viene visualizzato come valore di valuta. Quando si seleziona questa opzione, verificare che gli assegnatari delle attività (mansioni o utenti) siano associati a tassi di costo.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stima al completamento</td> 
      <td> <p>Rappresenta il costo totale previsto del progetto o dell'attività al completamento. Questa impostazione viene configurata a livello di sistema dall’amministratore, ma puoi anche modificarla a livello di progetto. Prendi in considerazione di selezionare una delle seguenti opzioni:</p> 
       <ul> 
        <li><strong>Calcola a livello di progetto</strong>: il costo effettivo della manodopera per l'attività e il progetto padre viene determinato inserendo il costo effettivo ore/manodopera nelle formule EAC. Questo calcolo include le ore effettive, i costi e le spese aggiunti direttamente all'attività o al progetto padre.</li> 
        <li><strong>Esegui il rollup da attività/sottoattività</strong>: l’EAC per l’attività e il progetto principali viene determinato sommando l’EAC per ogni attività secondaria. Questo calcolo esclude le ore effettive, i costi e le spese aggiunti direttamente all'attività o al progetto padre.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bdg</td> 
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
      <td> <p>Specificare una valuta per il progetto, se diversa da quella predefinita nel sistema. La valuta predefinita nel sistema è definita dall'amministratore di Workfront. Per ulteriori informazioni sull'impostazione dei tassi di cambio in Workfront, vedere l'articolo <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Imposta tassi di cambio</a>.</p> </td> 
     </tr>
    </tbody> 
   </table>

1. Clic **Salva modifiche**.
