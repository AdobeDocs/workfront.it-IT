---
filename: migrate-resource-scheduling-to-workload-balancer
product-area: resource-management
navigation-topic: resource-management-overview
title: Migrare da Resource Scheduling a [!UICONTROL Bilanciamento del carico di lavoro]
description: Vogliamo che tu possa sperimentare il minor numero possibile di interruzioni del lavoro, aiutandoti a progettare un piano di migrazione. I passaggi seguenti ti aiuteranno a formare il tuo team e a determinare il momento migliore per passare al servizio di bilanciamento del carico di lavoro.
author: Alina
exl-id: 4bc08d5f-99c7-40e2-85d6-1de0b585aef8
source-git-commit: d2a8380e3383b97b8245bd2b6d3cb9ff75306e4f
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 0%

---

# Migrazione dalla risorsa [!UICONTROL Pianificazione] al [!UICONTROL Bilanciamento del carico di lavoro]

<span class="preview">Le informazioni evidenziate in questa pagina fanno riferimento a funzionalità non ancora disponibili al pubblico. È disponibile solo nell’ambiente Anteprima.</span>

<!-- drafted for res scheduling deprecation blurb for PREVIEW release - Oct 2022 - CHANGE THIS BLURB TO SOMETHING ELSE AT PRODUCTION:-->

>[!CAUTION]
>  
>  
> <span class="preview">Le aree di programmazione sono state rimosse dall’ambiente di anteprima e verranno rimosse dall’ambiente di produzione in **Gennaio 2023**. </span>\
> <span class="preview"> A partire da gennaio 2023, è necessario pianificare le risorse in Workbench carico di lavoro. </span>
>  
><span class="preview"> Per informazioni sulla pianificazione delle risorse tramite il servizio di bilanciamento del carico di lavoro, consulta la sezione . [Il servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/workload-balancer.md).</span>

Le informazioni contenute in questo articolo si applicano solo se hai gestito la pianificazione delle risorse nella risorsa [!UICONTROL Pianificazione] aree di Adobe Workfront. Workfront ha avviato la rimozione di [!UICONTROL Pianificazione] strumenti nel novembre 2020 e li ha sostituiti con [!UICONTROL Bilanciamento del carico di lavoro].

Per informazioni sul piano di elementi obsoleti per [!UICONTROL Pianificazione delle risorse] gli strumenti e la timeline per la loro sostituzione con [!UICONTROL Bilanciamento del carico di lavoro], vedi [Strumenti di pianificazione delle risorse obsoleti in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

Vogliamo che tu possa sperimentare il minor numero possibile di interruzioni del lavoro, aiutandoti a progettare un piano di migrazione. I passaggi seguenti ti aiuteranno a formare il tuo team e a determinare il momento migliore per passare al [!UICONTROL Bilanciamento del carico di lavoro].

## Individuare gli strumenti di programmazione delle risorse

Tu e i tuoi team potreste usare parte della risorsa [!UICONTROL Pianificazione] strumenti nelle seguenti aree di Workfront:

* La [!UICONTROL Pianificazione] nella sezione [!UICONTROL Risorsa] area
* La [!UICONTROL Pianificazione] sezione di un progetto
* La [!UICONTROL Pianificazione] sezione di un team

Con questa opzione obsoleta, la funzione [!UICONTROL Bilanciamento del carico di lavoro] sostituisce tutte le  [!UICONTROL Pianificazione delle risorse] in tutte le aree elencate sopra.

## Passaggio 1: Formazione dei team

Segui il corso [Programma di gestione delle risorse per la nuova esperienza Adobe Workfront](https://one.workfront.com/s/resource-management-program-nwe) (75 minuti) su Workfront One.

In caso di difficoltà nell&#39;accesso o nell&#39;accesso al corso, contatta l&#39;Assistenza clienti. Per informazioni, consulta [Contatta l’Assistenza clienti](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## Passaggio 2: Determinare il momento migliore per eseguire la migrazione {#step-2-determine-the-best-time-to-migrate}

Segui i passaggi riportati di seguito per determinare quando è il momento migliore per eseguire la migrazione:

1. Determinare le funzionalità nella risorsa [!UICONTROL Pianificazione] gli strumenti più utilizzati dal tuo team e assicurati che tali funzioni siano disponibili nella [!UICONTROL Bilanciamento del carico di lavoro]. Per informazioni sulle funzionalità attualmente disponibili nella [!UICONTROL Bilanciamento del carico di lavoro], consulta la sezione &quot;Disponibilità delle funzioni&quot; nell’articolo [Strumenti di pianificazione delle risorse obsoleti in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

   >[!IMPORTANT]
   >
   >Quasi tutte le funzionalità degli strumenti di pianificazione ora sono nel load Balancer del carico di lavoro.

1. Determinare se il team gestisce le allocazioni degli utenti nelle assegnazioni. Regolare o modificare le allocazioni degli utenti significa modificare le ore pianificate al giorno per ogni utente per tutta la durata di un elemento di lavoro.

   Le allocazioni modificate negli strumenti di programmazione non vengono trasferite al servizio di bilanciamento del carico di lavoro. Per impostazione predefinita, il sistema distribuisce in modo uniforme il totale delle ore pianificate di un elemento di lavoro per l&#39;intera durata dell&#39;elemento.

   È necessario gestire manualmente le allocazioni nel servizio di bilanciamento del carico di lavoro per garantire che le allocazioni corrispondano a quelle disponibili negli strumenti di programmazione. Per informazioni, consulta [Gestire le allocazioni di utenti nel load balancer](../workload-balancer/manage-user-allocations-workload-balancer.md).

1. Eventuali filtri salvati nell’area Pianificazione non verranno trasferiti automaticamente al servizio di bilanciamento del carico di lavoro. Crea i filtri eventualmente necessari nel servizio di bilanciamento del carico di lavoro. Per informazioni sulla creazione di filtri nel servizio di bilanciamento del carico di lavoro, consulta [Filtrare le informazioni nel servizio di bilanciamento del carico di lavoro](../workload-balancer/filter-information-workload-balancer.md).

<!--
1. Using the information gathered from Steps 1 and Step 2, decide which version of Step 3 you should continue with based on the needs of your organization.
-->

## Passaggio 3: Esegui migrazione a [!UICONTROL Bilanciamento del carico di lavoro]{#step-3-migrate-to-the-workload-balancer}

Abbiamo identificato le seguenti versioni per questo passaggio, a seconda dei risultati del passaggio 2:

* [Passaggio 3 bis: Tu o i tuoi team utilizzi il [!UICONTROL Pianificazione] strumenti, ma non modificare l’allocazione utente](#step-3a-you-or-your-teams-use-the-scheudling-tools-but-do-not-modify-user-allocation)
* [Passaggio 3b: Tu o i tuoi team gestisci le allocazioni degli utenti nel [!UICONTROL Pianificazione] strumenti](#step-3b-you-or-your-teams-manage-user-allocations-in-the-scheduling-tools)

### Passaggio 3 bis: Tu o i tuoi team utilizzi il [!UICONTROL Pianificazione] strumenti, ma non modificare l’allocazione utente

Se l&#39;utente o i team non modificano le allocazioni di ore giornaliere nelle assegnazioni di lavoro, è possibile passare le risorse di pianificazione a [!UICONTROL Bilanciamento del carico di lavoro].

![](assets/nwe-workload-balancer-global-350x125.png)

Effettua le seguenti operazioni:

* Scegli una data di transizione.

   >[!TIP]
   >
   >Dai al tuo team un po&#39; di tempo per completare il corso di formazione sull&#39;utilizzo del servizio di bilanciamento del carico di lavoro prima della data di transizione. Per informazioni sulla formazione, consulta la sezione . [Migrazione da Resource Scheduling al load Balancer](#migrate-from-resource-uicontrol-scheduling-to-the-uicontrol-workload-balancer) in questo articolo.

* Segui queste linee guida per assistere i tuoi team:

   * Incoraggiare i team a visitare il [Panoramica [!UICONTROL Bilanciamento del carico di lavoro]](../../resource-mgmt/workload-balancer/overview-workload-balancer.md) e tutte le pagine collegate da lì per approfondire la [!UICONTROL Bilanciamento del carico di lavoro] funziona.
   * Organizza riunioni frequenti in cui i tuoi team possono rispondere a domande la settimana prima della transizione, effettuare il passaggio e quindi tenere un&#39;altra riunione FAQ per rispondere a domande di follow-up.
   * Invia feedback a Workfront utilizzando il pulsante Feedback nella barra degli strumenti superiore. I nostri sviluppatori di prodotti sono sempre interessati a sentire i tuoi casi d&#39;uso per come possiamo fare [!UICONTROL Bilanciamento del carico di lavoro] fornisci più valore.

### Passaggio 3b: Tu o i tuoi team gestisci le allocazioni degli utenti nel [!UICONTROL Pianificazione] strumenti

Se il flusso di lavoro corrisponde a questo scenario, dovresti essere più strategico nel piano di transizione. Le allocazioni giornaliere visualizzate nel [!UICONTROL Pianificazione] gli strumenti sono memorizzati in un database diverso dalle allocazioni giornaliere visualizzate in [!UICONTROL Bilanciamento del carico di lavoro]. Ciò significa che gli adeguamenti delle allocazioni giornaliere eseguite nella risorsa [!UICONTROL Pianificazione] gli strumenti non vengono trasferiti alle allocazioni giornaliere nel [!UICONTROL Bilanciamento del carico di lavoro].

>[!CAUTION]
>
>Hai tempo **Gennaio 2023** per garantire che l&#39;allocazione degli utenti dalle aree di programmazione corrisponda a quella nel load balancer nell&#39;ambiente di produzione. In quel momento, rimuoviamo gli strumenti di programmazione dall’ambiente di produzione. È necessario regolare manualmente le allocazioni nel servizio di bilanciamento del carico di lavoro in modo che corrispondano a quelle negli strumenti di programmazione. <span class="preview">Gli strumenti di pianificazione sono già stati rimossi dall’ambiente Anteprima.</span>


Quando effettui la transizione al [!UICONTROL Bilanciamento del carico di lavoro] quando utilizzi questo [!UICONTROL Pianificazione] funzionalità:

* Bloccare la gestione delle assegnazioni nel [!UICONTROL Pianificazione] come avviene per i responsabili delle risorse. Per eseguire questa operazione:

   * Scopri la durata media delle attività nei progetti correnti e tenerne conto quando si determina per quanto tempo è necessario limitare la gestione delle allocazioni utente.

      >[!TIP]
      >
      >È necessario esaminare solo i progetti correnti o di pianificazione, ovvero quelli per i quali i team eseguono attivamente le assegnazioni e gestiscono le allocazioni giornaliere.

   * Creare un report attività e aggiungere il campo Durata attività nella visualizzazione e raggrupparlo in base al nome del progetto. Riepiloga la colonna Durata nella visualizzazione in base alla media, quindi salva il rapporto.

      Per informazioni sulla creazione di un rapporto, vedi [Creare un rapporto personalizzato](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) .

   * Analizzare il report attività. Ad esempio, se la durata media dell’attività è di 3 giorni, è consigliabile effettuare una transizione di una settimana. Chiedi al team di interrompere la gestione delle allocazioni degli utenti per una settimana. La settimana successiva, passa il team a [!UICONTROL Bilanciamento del carico di lavoro] e inizia a gestire le allocazioni degli utenti la settimana successiva.
   >[!NOTE]
   >
   >Questo suggerimento potrebbe non funzionare se la durata media dell&#39;attività è superiore al tempo rimanente fino alla rimozione degli strumenti di programmazione.


   ![](assets/timeline-stop-using-resource-scheduler-callouts-350x178.png)

   >[!TIP]
   >
   >È possibile continuare a eseguire attività ed eseguire assegnazioni durante il periodo di transizione. Le assegnazioni effettuate si rifletteranno sia nello strumento di pianificazione delle risorse che in [!UICONTROL Bilanciamento del carico di lavoro].

* Se sei un’organizzazione più grande con team che gestiscono risorse per centinaia di progetti, puoi prendere in considerazione la transizione dalla [!UICONTROL Pianificazione] gli strumenti [!UICONTROL Bilanciamento del carico di lavoro] un portafoglio alla volta. Considera un rollout graduale creando filtri personalizzati nel [!UICONTROL Bilanciamento del carico di lavoro] per esaminare un portfolio specifico alla volta.

* Consenti ai responsabili risorse di eseguire il team up: dispongono di una persona che rivede le assegnazioni effettuate nel  [!UICONTROL Pianificazione delle risorse] gli strumenti e una volta apportati gli opportuni adeguamenti [!UICONTROL Bilanciamento del carico di lavoro]. Una volta che quel team di due strumenti si concilia con entrambi, fai in modo che i loro flussi di lavoro vengano spostati verso [!UICONTROL Bilanciamento del carico di lavoro].

## Necessità di ulteriore assistenza

Se hai bisogno di ulteriori informazioni con questa migrazione, contatta il supporto personalizzato. Per informazioni su come contattare il supporto, consulta [Contatta l’Assistenza clienti](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
