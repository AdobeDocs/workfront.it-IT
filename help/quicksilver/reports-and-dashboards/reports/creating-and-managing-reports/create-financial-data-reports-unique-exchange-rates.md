---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Creare rapporti di dati finanziari con tassi di cambio univoci
description: Se sono stati configurati più tassi di cambio in Adobe Workfront, è possibile impostare i valori finanziari nei rapporti e negli elenchi in modo che vengano visualizzati in una valuta diversa da quella predefinita.
author: Nolan
feature: Reports and Dashboards
exl-id: a0837c70-8330-4c38-98dc-8cf2e7e2e4bd
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1028'
ht-degree: 0%

---

# Creare rapporti di dati finanziari con tassi di cambio univoci

Se sono stati configurati più tassi di cambio in Adobe Workfront, è possibile impostare i valori finanziari nei rapporti e negli elenchi in modo che vengano visualizzati in una valuta diversa da quella predefinita.

>[!IMPORTANT]
>
>Se in una visualizzazione si seleziona una valuta diversa da quella predefinita, i collegamenti non vengono più visualizzati **Aggiungi altre attività** e **Aggiungi altri problemi** in fondo a un elenco di progetti.

Per informazioni su come modificare la valuta predefinita per un determinato progetto, consulta [Modificare la valuta del progetto](../../../manage-work/projects/project-finances/change-project-currency.md).

Se nel rapporto sono presenti progetti con una moneta unica, anche le somme in raggruppamenti vengono visualizzate nella valuta predefinita del sistema.

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
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di visualizzare le valute alternative come descritto in questa sezione, l&#39;amministratore di Workfront deve prima abilitare e configurare più valute nell&#39;area Configurazione di Workfront. Per informazioni, consulta [Imposta i tassi di cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Applicazione di valori finanziari a un report {#apply-financial-values-to-a-report}

Per convertire i valori finanziari tra le valute quando si utilizzano i rapporti:

1. Passare al report in cui si desidera convertire i valori finanziari in una valuta diversa.
1. Fai clic sul pulsante **Visualizza** elenco a discesa, fai clic su **Cambia valuta**, quindi selezionare una delle seguenti valute in cui si desidera visualizzare i valori finanziari:

   * Valuta originale del progetto
   * Tutte le altre valute

      >[!TIP]
      >
      >È possibile scegliere solo le valute precedentemente selezionate in Configurazione.
   L&#39;utilizzo di questa opzione consente di convertire rapidamente i valori finanziari in un rapporto tra valori di tasso.

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

## Visualizza la valuta predefinita in più progetti con valute diverse

Quando si personalizza la valuta a livello di progetto e si desidera visualizzare le informazioni di tutti i progetti nello stesso rapporto, esistono i seguenti scenari:

* Se si crea un report contenente informazioni finanziarie provenienti da due o più progetti a cui sono applicate valute diverse, per impostazione predefinita il riepilogo dei raggruppamenti riflette la valuta predefinita del sistema selezionata dall&#39;amministratore Workfront.
* Se si crea un rapporto per due o più progetti che hanno la stessa valuta ma che differiscono da quella predefinita del sistema, le somme dei raggruppamenti vengono visualizzate utilizzando la valuta predefinita del sistema.
* Se si crea un rapporto per due o più progetti che presentano assegnazioni di ruoli di lavoro associate a una sostituzione di valuta, Workfront converte le informazioni finanziarie dai tassi di cambio di sostituzione del ruolo di lavoro nella divisa del progetto (quando si seleziona Divisa originale del progetto nella visualizzazione) o in una valuta diversa selezionata al momento della visualizzazione del rapporto. Per informazioni sulla sostituzione della valuta di un ruolo di lavoro, vedere [Creare e gestire ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Per visualizzare due progetti con valute personalizzate in un rapporto:

1. Crea due progetti con diverse valute applicate.

   ![](assets/qs-currency-350x217.png)

1. Accedi alle ore su entrambi i progetti.

   Per ulteriori informazioni sul tempo di registrazione, vedi [Tempo di log](../../../timesheets/create-and-manage-timesheets/log-time.md).

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png), quindi fai clic su **Reporting**.
1. Fai clic su **Nuovo rapporto**, quindi **Rapporto sul progetto**.
1. In **Colonne (visualizzazione)** aggiungi una scheda **Costo effettivo** e riepilogalo per **Somma**.

   Per informazioni su come creare una colonna, consulta [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. In **Raggruppamenti** , applica un **Data completamento pianificata** raggruppamento.

   Per informazioni su come creare un raggruppamento, consulta [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. In **Filtri** aggiungi un filtro per **Nome progetto** e selezionare i due progetti con le diverse valute.

   Per informazioni su come creare un filtro, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Fai clic su **Salva e chiudi**.

   Il totale del **Costo effettivo** viene visualizzato nel gruppo utilizzando la valuta predefinita del sistema, indipendentemente dalla valuta dei progetti nel rapporto.

   ![Divisa visualizzata nel raggruppamento](assets/qs-currency-displayed-in-groupings-2022-350x292.png)

   Se i due progetti hanno valute diverse l&#39;uno dall&#39;altro, la valuta predefinita del sistema viene visualizzata anche nel Raggruppamento del rapporto.

## Visualizza la divisa del progetto in un rapporto a livello di progetto

Se un raggruppamento viene applicato a un&#39;attività o a un elenco di ore all&#39;interno di un progetto, le somme nel raggruppamento vengono visualizzate nella valuta del progetto.

1. Crea un progetto con una valuta personalizzata diversa dalla valuta predefinita del sistema.
1. Vai al progetto e assicurati che includa le ore registrate per le attività.

   Per ulteriori informazioni sul tempo di registrazione, vedi [Tempo di log](../../../timesheets/create-and-manage-timesheets/log-time.md).

   >[!NOTE]
   >
   >Le attività devono essere assegnate a utenti o ruoli di lavoro con tariffe di costo per ora.

1. Fai clic su **Attività**.
1. Espandi la **Visualizza** menu a discesa e seleziona **Nuova vista**.
1. Aggiungi **Costo effettivo** nella nuova colonna Visualizza come nuova e riepilogala per **Somma**.
1. Fai clic su **Fine**, quindi fai clic su **Salva visualizzazione**.
1. Espandi la **Raggruppamento** menu a discesa e seleziona **Nuovo raggruppamento**.
1. Aggiungi **Data completamento effettivo** nel nuovo raggruppamento come nuovo campo, fai clic su **Salva raggruppamento**.

   La **Costo effettivo** La colonna riepiloga nel nuovo raggruppamento e visualizza il totale nella valuta del progetto.

## Modificare rapporti con valute univoche

I campi finanziari di un rapporto non possono essere modificati finché non si modifica l&#39;impostazione del rapporto per visualizzare la valuta originale dei progetti.

Per modificare in linea un campo finanziario in un rapporto:

1. Passa a un rapporto.

   >[!NOTE]
   >
   >Se la valuta predefinita non viene visualizzata per un elenco in un&#39;altra area, è possibile modificare la visualizzazione per visualizzare la valuta predefinita.\
   >Per informazioni su come modificare la valuta in una visualizzazione, consulta la sezione in questo articolo [Applicazione di valori finanziari a un report](#apply-financial-values-to-a-report).

1. Fai clic su **Azioni dei rapporti**, quindi seleziona **Modifica**.
1. Fai clic su **Impostazioni dei rapporti**.
1. Fai clic sul pulsante **Valuta predefinita** a discesa, quindi seleziona **Valuta originale del progetto**.

   ![](assets/qs-report-settings-default-currency-350x370.png)

1. Fai clic su **Fine**.
