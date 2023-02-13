---
product-area: resource-management
navigation-topic: resource-planning
title: Verifica la disponibilità e l’allocazione delle risorse utilizzando Adobe Workfront Resource Planner
description: È possibile visualizzare la disponibilità delle risorse e la quantità di lavoro pianificato o preventivato per i progetti nel Planner risorse. Questi valori vengono visualizzati in Ore, FTE (Full Time Equivalent) o Importi di costo e sono organizzati in colonne.
author: Alina
feature: Resource Management
exl-id: 5b3e52a6-af9b-4e68-8d6e-43a5151a2a2c
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: tm+mt
source-wordcount: '1270'
ht-degree: 4%

---

# Verifica la disponibilità e l’allocazione delle risorse utilizzando Adobe Workfront Resource Planner

È possibile visualizzare la disponibilità delle risorse e la quantità di lavoro pianificato o preventivato per i progetti nel Planner risorse. Questi valori vengono visualizzati in Ore, FTE (Full Time Equivalent) o Importi di costo e sono organizzati in colonne.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro e superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o superiore </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizza o accedi di più a quanto segue:</p> 
    <ul> 
     <li> <p>Gestione risorse</p> </li> 
     <li> <p>Dati finanziari</p> </li> 
     <li> <p>Utenti</p> </li> 
     <li> <p>Progetti</p> </li> 
    </ul> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per i progetti che desideri visualizzare nel Planner risorse</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

<!--note from the table about the license: Review or higher: 
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (waiting on Vazgen to confirm - working differenly in classic)
      </MadCap:conditionalText>
     -->

## Prerequisiti

È necessario soddisfare tutti i prerequisiti necessari per lavorare con il Planner risorse. Per ulteriori informazioni, consulta [Panoramica di Resource Planner](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

>[!IMPORTANT]
>
>Se manca uno dei prerequisiti necessari per la corretta funzionalità del Planner risorse, alcuni dei numeri potrebbero essere pari a zero oppure l&#39;orario previsto potrebbe essere disattivato.

## Disponibilità e assegnazione delle risorse

Le colonne che mostrano la disponibilità e l&#39;allocazione delle risorse cambiano a seconda della visualizzazione applicata al planner risorse. Per informazioni sulla visualizzazione delle informazioni nel Planner risorse per progetto, ruolo o utente, vedere [Panoramica sulla navigazione in planner risorse](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Quando si modifica la visualizzazione in Planner risorse, tenere presente quanto segue:

* Quando applichi la **Visualizza per progetto** o **Visualizza per ruolo** viste, puoi vedere le seguenti colonne:

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: Alina: (some of the information in this area is also covered in Calculating Costs in the RP - https://workfront.zendesk.com/hc/en-us/articles/115004186433 - update this article also, when changes here occur)
  </MadCap:conditionalText>
  -->



   * Ore disponibili, FTE o Costo
   * Ore, FTE o Costo pianificati
   * Ore, FTE o Costo preventivati
   * Ore, FTE o Varianza dei costi
   * Ore nette, FTE o Costo

* Quando applichi la **Visualizza per utente** visualizza, puoi vedere le seguenti colonne:

   * Ore disponibili o FTE
   * Orari pianificati o FTE
   * Differenza oraria o FTE
   * Percentuale allocazione ore pianificate

>[!TIP]
>
>Le informazioni non sono disponibili come Costo quando si applica il **Visualizza per utente** visualizzare il planner risorse.
>
>Per ulteriori informazioni sulla visualizzazione di ciascuna colonna, passare il mouse sul nome della colonna in cui viene visualizzato il numero.\
>![Net_hours_res_planner_mouse_over.png](assets/net-hours-res-planner-mouse-over-350x95.png)
>
>Per ulteriori informazioni sui dati visualizzati in ciascuna colonna, consulta i seguenti articoli:
>
>* [Panoramica delle informazioni su ore, FTE e costi nelle visualizzazioni Progetto e Ruolo del Planner risorse](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)
>* [Visualizza Ore disponibili, pianificate e effettive o FTE nel planner risorse quando si utilizza la visualizzazione Utente](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)
>


## Visualizza le informazioni per ora, FTE o Costo

1. Vai al Planner risorse.

   Per impostazione predefinita, le informazioni vengono visualizzate per ore nel Planner risorse.

1. Espandi il menu a discesa .\
   ![Hours_fte_or_cost_dropdown.png](assets/hours-fte-or-cost-dropdown.png)

1. Seleziona tra le seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ore</td> 
      <td>Visualizza le informazioni sulla disponibilità e sull'allocazione in ore.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">FTE</td> 
      <td> <p>Visualizza le informazioni sulla disponibilità e sull'allocazione in FTE.</p> <p>Per ulteriori informazioni sul calcolo dell’ETP nel Planner risorse, consulta <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Panoramica del calcolo delle ore e degli FTE per utenti e ruoli nel Planner risorse</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo</td> 
      <td> <p>Visualizza le informazioni sulla disponibilità e sull'allocazione in base al costo, se si visualizza il Planner risorse nelle visualizzazioni Progetto o Ruolo. Le informazioni mostrano i valori nella valuta del sistema. L’amministratore di Workfront definisce la valuta di sistema. Per ulteriori informazioni sulla configurazione della valuta del sistema in Workfront, vedi <a href="../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Imposta i tassi di cambio</a>.</p> <p><b>NOTA</b>

   Per visualizzare le informazioni sui costi nel planner risorse, è necessario associare utenti e ruoli di lavoro ai tassi di costo per ora.<br style="font-style: italic;">Per ulteriori informazioni sull&#39;associazione dei tassi di costo per ora con i ruoli di lavoro, vedere <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire ruoli di lavoro</a>.<br style="font-style: italic;">Per ulteriori informazioni sull&#39;associazione delle tariffe di costo per ora con gli utenti, consulta <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente</a>.<br style="font-style: italic;">Per ulteriori informazioni sul calcolo dei costi nel Planner risorse, vedere <a href="../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md" class="MCXref xref">Calcolare i costi nel planner risorse </a>.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Personalizza</td> 
      <td>Crea una visualizzazione personalizzata delle colonne visualizzate nel Planner risorse. Selezionare le opzioni che si desidera visualizzare nel Planner risorse, come descritto nei passaggi seguenti. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condizionale) Se hai selezionato **Personalizza**, indica le opzioni nel **Personalizzare le metriche visualizzate** per impostare la visualizzazione personalizzata.

   ![](assets/planner-customize-view-box-350x114.png)

1. In **Tipo di visualizzazione** a sinistra, seleziona una delle visualizzazioni seguenti:

   * Progetto
   * Qual
   * Utente

1. In **Visualizza gli elementi selezionati** selezionare il tipo di informazioni da visualizzare nelle colonne della visualizzazione selezionata. Nella tabella seguente sono illustrate le opzioni disponibili in ogni visualizzazione:

   | **Opzione** | Visualizzazione utente | Vista Project | Vista ruolo |
   |---|---|---|---|
   | Disponibile | ↓ | ✔ | ✔ |
   | Pianificato | ✔ | ✔ | ✔ |
   | Preventivato |   | ✔ | ✔ |
   | Varianza |   | ✔ | ✔ |
   | Net |   | ✔ | ✔ |
   | Effettivo | ✔ |   |   |
   | Differenza | ✔ |   |   |
   | Percentuale | ✔ |   |   |

1. Seleziona **Utilizzare i valori pianificati (PLN) nei calcoli NET** per utilizzare le informazioni Pianificato invece di Preventivo durante il calcolo dei valori Netto nelle visualizzazioni Progetto e Ruolo.

   Quando si seleziona questa opzione, Workfront calcola i valori netti utilizzando la formula seguente:

   ```
   Net = Available - Planned
   ```

   >[!TIP]
   >
   >**Questa opzione viene applicata solo quando si seleziona almeno un’opzione per personalizzare la visualizzazione nella sezione Visualizza elementi selezionati .**

1. Fai clic su **Salva**.

   Viene visualizzata la vista personalizzata che include le colonne selezionate.

   Nel menu a discesa Ore del planner risorse viene elencata la visualizzazione personalizzata come Personalizzata .

   >[!NOTE]
   >
   >È possibile avere una sola visualizzazione personalizzata.

   ![](assets/planner-hours-drop-down-with-custom-and-customize-option-183x281.png)

## Visualizza il grafico di allocazione utente

È possibile visualizzare in un grafico l’Allocazione pianificata degli utenti rispetto alla loro disponibilità.

Per visualizzare l’allocazione degli utenti in un grafico:

1. Vai al Planner risorse.

   Per ulteriori informazioni sull&#39;accesso al Planner risorse, vedere la [Individua il planner risorse](../../resource-mgmt/resource-planning/get-started-resource-planner.md#accessing-the-resource-planner) sezione dell&#39;articolo [Panoramica di Resource Planner](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

1. Seleziona **Visualizza per utente**.

   >[!TIP]
   >
   >È possibile visualizzare il grafico di allocazione utente solo nella visualizzazione utente.

1. Fai clic sul pulsante **Grafico di allocazione utente** icona ![RP_user_Allocation_Chart.png](assets/rp-user-allocation-chart.png) per visualizzare le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">% disponibilità senza allocazione eccessiva per tutti gli utenti</td> 
      <td>Si tratta del tempo in cui tutti gli utenti sono disponibili per il lavoro in un periodo di tempo, espresso in percentuale rispetto al tempo totale disponibile. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">% allocazione eccessiva per tutti gli utenti </td> 
      <td> <p>Si tratta del tempo in cui gli utenti vengono sovrapassegnati in un periodo di tempo, indicato come percentuale rispetto al tempo totale disponibile.</p> <p><b>NOTA</b>

   Una sovrallocazione si verifica quando le ore pianificate sono superiori alle ore disponibili. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">% sottoutilizzo per tutti gli utenti</td> 
      <td> <p>Si tratta del tempo in cui gli utenti vengono sottoutilizzati in un periodo di tempo, indicato come percentuale rispetto al tempo totale disponibile.</p> <p><b>NOTA</b>

   Il sottoutilizzo si verifica quando le ore pianificate sono inferiori alle ore disponibili. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">È presente un'allocazione eccessiva per almeno un utente durante questo periodo</td> 
      <td>Questo indica che esiste una sovrallocazione per almeno un utente in un periodo di tempo, anche se il tempo totale di tutti gli utenti non viene sovrapassegnato per il periodo di tempo.<br>È necessario scorrere l’elenco degli utenti e le ore per l’utente con sovrallocazione vengono evidenziate in rosso.</td> 
     </tr> 
    </tbody> 
   </table>

   ![RP__user_allocation_Chart_Dec._7__2017.png](assets/rp--user-allocation-chart-dec.-7--2017-350x148.png)

1. (Facoltativo) Fai clic sul pulsante **Sovrallocazione % per tutti gli utenti** nel grafico.\
   Tutti gli utenti con sovrassegnazione vengono evidenziati in rosso.
1. (Facoltativo) Fai clic sul pulsante **% sottoutilizzazione per tutti gli utenti** nel grafico.\
   Tutti gli utenti sottoutilizzati sono evidenziati in blu.

1. (Facoltativo) Fai clic sull’icona indicatore ![one_user_overallocation_marker.png](assets/one-user-overallocation-marker.png) mostra dove almeno un utente è sovrassegnato.\
   Gli utenti con sovrassegnazione vengono evidenziati in rosso.

1. (Facoltativo) Aggiorna la pagina per comprimere il grafico.
