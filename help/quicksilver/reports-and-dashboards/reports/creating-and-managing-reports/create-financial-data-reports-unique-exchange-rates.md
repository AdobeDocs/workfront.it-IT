---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Creazione di report di dati finanziari con tassi di cambio univoci
description: Se in Adobe Workfront sono stati configurati più tassi di cambio, è possibile impostare i valori finanziari nei report e negli elenchi in modo che vengano visualizzati in una valuta diversa da quella predefinita.
author: Nolan
feature: Reports and Dashboards
exl-id: a0837c70-8330-4c38-98dc-8cf2e7e2e4bd
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# Creazione di report di dati finanziari con tassi di cambio univoci

Se in Adobe Workfront sono stati configurati più tassi di cambio, è possibile impostare i valori finanziari nei report e negli elenchi in modo che vengano visualizzati in una valuta diversa da quella predefinita.

>[!IMPORTANT]
>
>Se selezioni una valuta diversa da quella predefinita in una visualizzazione, non vedrai più i collegamenti **Aggiungi altre attività** e **Aggiungi altri problemi** in fondo all&#39;elenco dei progetti.

Per informazioni su come modificare la valuta predefinita per un determinato progetto, vedere [Modificare la valuta del progetto](../../../manage-work/projects/project-finances/change-project-currency.md).

Se nel rapporto sono presenti progetti con una valuta unica, anche le somme in raggruppamenti vengono visualizzate nella valuta predefinita del sistema.

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
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Prerequisiti

Prima di poter visualizzare le valute alternative come descritto in questa sezione, l’amministratore di Workfront deve innanzitutto abilitare e configurare più valute nell’area Configurazione di Workfront. Per informazioni, vedere [Impostare i tassi di cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Applicare valori finanziari a un rapporto {#apply-financial-values-to-a-report}

Per convertire i valori finanziari tra valute quando si utilizzano i rapporti:

1. Passare al report in cui si desidera convertire i valori finanziari in una valuta diversa.
1. Fai clic sull&#39;elenco a discesa **Visualizza**, fai clic su **Cambia valuta**, quindi seleziona una delle seguenti valute in cui desideri visualizzare i valori finanziari:

   * Valuta originale del progetto
   * Qualsiasi altra valuta

     >[!TIP]
     >
     >È possibile scegliere solo le valute precedentemente selezionate in Configurazione.

   Questa opzione consente di convertire rapidamente i valori finanziari di un rapporto tra i valori dei tassi.

   ![Cambia valuta](assets/qs-change-currency-2022-350x257.png)

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: drafted this tip because I think this is confusing; this is in the step above.)</p>
   -->

   <!--
   <note type="tip">
   You can also select the Change Currency option to convert financial values in other lists.
   <br>
   <img src="assets/nwe-change-currency-new-lists-350x219.png" style="width: 350;height: 219;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   <br>
   <br>
   </note>
   -->

## Visualizzare la valuta predefinita in più progetti con valute diverse

Quando si personalizza la valuta a livello di progetto e si desidera visualizzare le informazioni di tutti i progetti nello stesso rapporto, si verificano i seguenti scenari:

* Se si crea un report che fornisce informazioni finanziarie da due o più progetti a cui sono state applicate valute diverse, per impostazione predefinita il riepilogo del raggruppamento riflette la valuta predefinita del sistema selezionata dall&#39;amministratore Workfront.
* Se si crea un report per due o più progetti che hanno la stessa valuta, ma differiscono da quella predefinita del sistema, le somme nei raggruppamenti vengono visualizzate utilizzando la valuta predefinita del sistema.
* Se si crea un report per due o più progetti con assegnazioni di mansioni associate a una sostituzione della valuta, Workfront converte le informazioni finanziarie dai tassi di valuta sostituiti della mansione nella valuta del progetto (quando si seleziona la valuta originale del progetto nella visualizzazione) o in una valuta diversa selezionata durante la visualizzazione del report. Per informazioni sull&#39;override della valuta di una mansione, vedere [Creare e gestire le mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Per visualizzare in un rapporto due progetti con valute personalizzate:

1. Crea due progetti con valute diverse applicate.

   ![](assets/qs-currency-350x217.png)

1. Registra le ore su entrambi i progetti.

   Per ulteriori informazioni sull&#39;ora di registrazione, vedere [Ora di registrazione](../../../timesheets/create-and-manage-timesheets/log-time.md).

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **Main Menu**, quindi fai clic su **Reporting**.
1. Fai clic su **Nuovo rapporto**, quindi su **Rapporto progetto**.
1. Nella scheda **Colonne (visualizzazione)**, aggiungi una colonna **Costo effettivo** e riepilogala per **Somma**.

   Per informazioni su come creare una colonna, vedere [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Nella scheda **Raggruppamenti**, applica un raggruppamento di **Data di completamento pianificata**.

   Per informazioni su come creare un raggruppamento, consulta [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Nella scheda **Filtri**, aggiungi un filtro per **Nome progetto** e seleziona i due progetti con valute diverse.

   Per informazioni su come creare un filtro, vedere [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Fai clic su **Salva e Chiudi**.

   Il totale del **Costo effettivo** viene visualizzato nel Raggruppamento utilizzando la valuta predefinita del sistema, indipendentemente dalla valuta dei progetti nel report.

   ![Valuta visualizzata nel raggruppamento](assets/qs-currency-displayed-in-groupings-2022-350x292.png)

   Se i due progetti hanno valute diverse tra loro, nel Raggruppamento del rapporto viene visualizzata anche la valuta predefinita del sistema.

## Visualizzare la valuta del progetto in un rapporto a livello di progetto

Se viene applicato un raggruppamento a un’attività o a un elenco di ore all’interno di un progetto, le somme del raggruppamento vengono visualizzate nella valuta del progetto.

1. Crea un progetto con una valuta personalizzata, diversa da quella predefinita dal sistema.
1. Vai al progetto e assicurati che includa le ore registrate per le attività.

   Per ulteriori informazioni sull&#39;ora di registrazione, vedere [Ora di registrazione](../../../timesheets/create-and-manage-timesheets/log-time.md).

   >[!NOTE]
   >
   >Le attività devono essere assegnate a utenti o mansioni con tariffe orarie.

1. Fai clic su **Attività**.
1. Espandi il menu a discesa **Visualizza** e seleziona **Nuova visualizzazione**.
1. Aggiungi **Costo effettivo** nella nuova visualizzazione come nuova colonna e riepilogalo per **Somma**.
1. Fai clic su **Fine**, quindi fai clic su **Salva visualizzazione**.
1. Espandi il menu a discesa **Raggruppamento** e seleziona **Nuovo raggruppamento**.
1. Aggiungi **Data di completamento effettiva** nel nuovo raggruppamento come nuovo campo, quindi fai clic su **Salva raggruppamento**.

   La colonna **Costo effettivo** contiene un riepilogo nel nuovo raggruppamento e visualizza il totale nella valuta del progetto.

## Modificare i rapporti con valute univoche

I campi finanziari di un rapporto non possono essere modificati finché non si modifica l&#39;impostazione del rapporto in modo da visualizzare la valuta originale per i progetti.

Per modificare in linea un campo finanziario in un report:

1. Passare a un report.

   >[!NOTE]
   >
   >Se la valuta predefinita non viene visualizzata per un elenco in qualsiasi altra area, è possibile modificare la visualizzazione in modo da visualizzare la valuta predefinita.\
   >Per informazioni su come modificare la valuta in una visualizzazione, vedere la sezione in questo articolo [Applicare valori finanziari a un report](#apply-financial-values-to-a-report).

1. Fai clic su **Azioni report**, quindi seleziona **Modifica**.
1. Fare clic su **Impostazioni report**.
1. Fai clic sull&#39;elenco a discesa **Valuta predefinita**, quindi seleziona **Valuta originale del progetto**.

   ![](assets/qs-report-settings-default-currency-350x370.png)

1. Fai clic su **Fine**.
