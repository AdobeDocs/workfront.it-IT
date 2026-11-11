---
title: Utilizzare la promozione dell'ambiente per Adobe Workfront Planning
description: È possibile copiare aree di lavoro, tipi di record, campi e viste di Workfront Planning da un ambiente Workfront a un altro utilizzando le funzionalità di promozione dell'ambiente. Invece di ricostruire tutto manualmente, assembli la configurazione in un pacchetto nell’ambiente sorgente e installala nell’ambiente di destinazione.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 82ebe4df89bd9db39629b36c31c0ae2a4e133838
workflow-type: tm+mt
source-wordcount: '1377'
ht-degree: 2%
---

# Utilizzare la promozione dell&#39;ambiente per Adobe Workfront Planning

<!--add to TOC-->
<!--add to miniTOC-->

<!--
Not sure if this bit will ever be needed because this only exists when both Preview and Prod have the features in parity. Features released here always come to both environments at the same time: 

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono ad Adobe Workfront Planning. Per accedere a Workfront Planning, la società deve acquistare un pacchetto Planning aggiuntivo.
>
>La funzionalità qui descritta non è disponibile se l&#39;organizzazione ha acquistato Workfront Planning come prodotto standalone.
>
>Per informazioni generali su Workfront Planning, vedere [Introduzione ad Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
> 
>

<!--
Future - when they make it available in Planning: replace the above with this OR ... insert the snippet:

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning which your organization can purchase either as an Adobe Workfront package or a standalone product. 
>
>Not all capabilities included in the Planning package are available to Workfront Planning when it is purchased as a standalone product. 
>
>For general information about Workfront Planning, see [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
> 
>For information about Workfront Planning as a standalone product, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md). 
>
-->

È possibile copiare le aree di lavoro di Workfront Planning e i relativi oggetti aggiuntivi da un ambiente Workfront a un altro utilizzando le funzionalità di promozione dell&#39;ambiente di Adobe Workfront.

Invece di ricostruire tutto manualmente, assembli la configurazione in un pacchetto nell’ambiente sorgente e installala nell’ambiente di destinazione.

L&#39;utilizzo della promozione dell&#39;ambiente con Planning è simile all&#39;utilizzo con Workfront. Per ulteriori informazioni, vedere la sezione &quot;Promozione dell&#39;ambiente&quot; nell&#39;articolo [Ambienti di test Adobe Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-testing-environments.md).

## Considerazioni sull&#39;utilizzo della promozione dell&#39;ambiente con Planning

* Per utilizzare la promozione dell’ambiente è necessario essere amministratore di Workfront.
* Quando copiate un workspace in un altro ambiente, vengono importati anche i seguenti oggetti associati a tale workspace mediante la promozione dell&#39;ambiente:

  * Aree di lavoro
  * Sezioni Workspace
  * Tipi di record
  * Campi
  * Viste
  * Gerarchie
  * Impostazioni di condivisione per tutti gli oggetti
  * Moduli di richiesta
  * Regole di business
  * Oggetti connessi
  * Oggetti da cui dipende il workspace o con cui sono condivisi altri oggetti, ad esempio gruppi, team, mansioni, aziende e utenti.

    Esistono i seguenti scenari:

    * Se nell&#39;ambiente di destinazione esiste già un oggetto con lo stesso nome, Workfront contrassegna un conflitto e decidi come gestirlo.
    * Se nell&#39;ambiente di destinazione non esiste un team o un gruppo con cui è condiviso un oggetto, la promozione lo crea.
  <!--* Automations -- this is not promoted, for now, per Lilit -->
* Per ogni oggetto, potete effettuare le seguenti operazioni:

  * Crea come nuovo oggetto
  * Usa l&#39;oggetto esistente ma crealo con un nuovo nome
  * Sovrascrivi un oggetto esistente. La sovrascrittura sostituisce la configurazione nella destinazione.
* Non è possibile esportare i seguenti oggetti:

  * Automazioni che appartengono all&#39;area di lavoro da copiare
  * Record
  * Campi che non appartengono alle aree di lavoro esportate

* I tipi di record connessi tra aree di lavoro diverse non possono essere promossi, a meno che non esistano già nell’ambiente di destinazione.

  È consigliabile innanzi tutto promuovere le aree di lavoro che contengono i tipi di record collegabili tra più aree di lavoro e solo successivamente promuovere le aree di lavoro che fanno riferimento a tali tipi di record.

* L&#39;installazione può richiedere alcuni minuti. Se necessario, è possibile eseguire il rollback di un&#39;installazione dalla pagina dei risultati.
* Se possibile, si consiglia di verificare il processo prima di procedere. Puoi installarlo in un ambiente sandbox o di anteprima prima di promuoverlo in produzione.


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacchetti Adobe Workfront</p></td> 
   <td> 
<p>Pacchetto di flussi di lavoro Prime o Ultimate con un pacchetto Prime o Ultimate Planning</p>
<!--This might come later: <p>Prime or Ultimate Planning package when purchased as a standalone product</p>-->
   </td> 
   </tr>
  <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Standard flusso di lavoro</p>    
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Planning</p></td> 
   <td><p>Standard di pianificazione</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Devi essere un Amministratore di sistema</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>   <p>Gestire le autorizzazioni per le aree di lavoro</p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  
   </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Importa configurazione di Planning tramite Promozione ambiente

Di seguito sono riportati i passaggi principali per promuovere la configurazione di Planning in un altro ambiente:

* [Crea un pacchetto nell&#39;ambiente di origine](#create-a-package-in-the-source-environment)
* [Prepara il pacchetto all’installazione](#make-the-package-ready-to-install)
* [Installare il pacchetto nell’ambiente di destinazione](#install-the-package-in-the-target-environment)
* [Verifica i risultati](#verify-the-results)

Seguire le istruzioni riportate nelle sezioni seguenti per copiare una configurazione Planning tra due ambienti Workfront.

### Creare un pacchetto nell’ambiente di origine

1. Vai a un ambiente sorgente in cui è presente la configurazione desiderata.
1. Nell&#39;ambiente di origine, fare clic sul **menu principale** ![menu principale](assets/main-menu-shell.png), quindi passare a **Configurazione** > **Sistema** > **Promozione ambiente**.
Nell&#39;elenco **Pacchetti di configurazione** sono visualizzati i pacchetti esistenti con il relativo stato, l&#39;ambiente di origine e la posizione in cui sono stati distribuiti.
1. Fare clic su **Crea pacchetto**.

   >[!TIP]
   >
   >Un pacchetto richiede almeno un oggetto prima di poter essere assemblato e installato.
1. Nella scheda **Dettagli pacchetto** immettere un **Nome** e una **Descrizione** per il pacchetto. L’ambiente di origine è già compilato con l’ambiente corrente (di origine).
1. Nell&#39;elenco dei tipi di oggetto a sinistra, selezionare **Area di lavoro di Planning**.
1. Cercare l&#39;area di lavoro che si desidera promuovere, selezionare la relativa casella di controllo e fare clic su **Aggiungi area di lavoro di Planning**. L&#39;area di lavoro viene visualizzata in **Contenuto pacchetto**.

   ![Workspace selezionato per la promozione ambiente](assets/workspace-selected-for-environment-promotion.png)
1. Fare clic su **Salva e assembla**.

   Workfront assembla il pacchetto e aggiunge una voce nella scheda **Aggiornamenti** del pacchetto. È possibile esaminare gli elementi inclusi nel pacchetto nella scheda Contenuto.
1. (Condizionale e facoltativo) Fare clic su **Salva e chiudi** se si desidera terminare in un secondo momento.
1. (Facoltativo) Fai clic su **Sommario** per esaminare il contenuto del pacchetto oppure fai clic su **Distribuzioni** per verificare se il pacchetto è stato distribuito più volte.

   Continua a preparare il pacchetto per l’installazione.

### Prepara il pacchetto all’installazione

Prima di installare il pacchetto nell’ambiente di destinazione, si consiglia di testarlo in un ambiente di test.

1. Dopo aver completato la compilazione del pacchetto come descritto nella sezione precedente, fare clic su **Dettagli pacchetto**, quindi su **Modifica**, impostare **Stato** su **Test**, quindi fare clic su **Salva e chiudi**.

   >[!TIP]
   >
   >Dopo aver generato il pacchetto, il relativo stato è impostato su **Bozza**. Lo stato **Attivo** non è disponibile finché non hai testato prima il pacchetto.
1. (Consigliato) Fai clic su **Installa** e scegli uno degli ambienti di test disponibili per distribuirlo e testare la configurazione.

   >[!TIP]
   >
   >L&#39;ambiente di produzione non è disponibile come una delle opzioni se lo stato è impostato su **Test**.

1. Dopo averlo installato in un ambiente di test, fare di nuovo clic su **Modifica** e impostare **Stato** su **Attivo**, quindi fare clic su **Salva e chiudi**.

   >[!TIP]
   >
   >L’installazione del pacchetto in un ambiente di test è simile all’installazione in produzione, come descritto nella sezione seguente.

   Continua con la sezione seguente per installare il pacchetto nell’ambiente di destinazione.


### Installare il pacchetto nell’ambiente di destinazione

1. Nella pagina del pacchetto, dopo averlo verificato, fai clic su **Installa**.
1. Nell&#39;elenco **Ambiente di destinazione** selezionare l&#39;ambiente in cui eseguire la distribuzione (ad esempio, l&#39;ambiente di produzione) e fare clic su **Continua**. La destinazione predefinita è l&#39;ambiente corrente.
1. Nella pagina **Informazioni sul pacchetto**, confermare l&#39;ambiente di origine e l&#39;ambiente in cui si sta distribuendo.
1. Nella sezione **Mappatura oggetto**, espandere ogni raggruppamento di oggetti, ad esempio un **area di lavoro di Planning**, per esaminare gli oggetti.

   >[!TIP]
   >
   >Qui possono essere visualizzati gruppi, team, ruoli, aziende e utenti, se uno qualsiasi degli oggetti del workspace è condiviso con loro.

1. Per ogni oggetto, controlla le colonne **Collisione** e **Stato**, quindi scegli un&#39;azione **Distribuzione** dall&#39;elenco. Scegli una tra le opzioni seguenti:


   * **Crea nuovo**: aggiunge l&#39;oggetto alla destinazione. Utilizzalo quando non viene rilevata alcuna collisione.
   * **Usa esistente**: esegue il mapping dell&#39;oggetto a un oggetto già esistente nella destinazione, ad esempio un&#39;area di lavoro con lo stesso nome.
   * **Crea con nuovo nome**: aggiunge l&#39;oggetto con un nome specificato.
   * **Sovrascrivi**: sostituisce l&#39;oggetto esistente nella destinazione con quello del pacchetto.

   >[!TIP]
   >
   >Se il sistema non trova un workspace con lo stesso ID, tenta di trovare una corrispondenza in base al nome del workspace.

1. (Facoltativo) Per modificare più oggetti contemporaneamente, selezionare le relative caselle di controllo, scegliere un&#39;azione nell&#39;elenco Azione di distribuzione nella parte superiore del gruppo e fare clic su Applica a selezionati. Utilizza i filtri sopra l’elenco, ad esempio Mostra solo errori, per evidenziare oggetti specifici.
1. Risolvi eventuali indicatori di errore. Se si seleziona **Usa esistente** per un oggetto, è necessario selezionare anche l&#39;oggetto a cui è associato.  In caso contrario, lo stato mostra un errore e **Distribuzione** rimane non disponibile.
1. Fai clic su **Distribuisci**, quindi su **Distribuisci** per confermare.


   Workfront mostra una pagina di installazione con il messaggio **Installazione del pacchetto in corso**. L&#39;operazione potrebbe richiedere alcuni minuti.

   Al termine dell&#39;installazione, nella pagina viene visualizzato un messaggio di operazione riuscita, l&#39;ambiente in cui è stato installato il pacchetto e un elenco degli oggetti installati, con uno stato per ciascuno, ad esempio **Usato esistente** o **Installato (Crea nuovo)**.
1. (Facoltativo) Se necessario, fare clic su **Ripristina l&#39;installazione** per ripristinare l&#39;installazione e rimuovere la configurazione dall&#39;ambiente di destinazione.

   Continuare a verificare i risultati dell&#39;installazione.

### Verifica i risultati

1. Vai all&#39;ambiente di destinazione > **Main Menu** > **Planning** e trova l&#39;area di lavoro importata.
1. Aprire i tipi di record e le visualizzazioni per verificare che i campi e il layout corrispondano all&#39;origine. I record non sono inclusi, pertanto le tabelle sono vuote.


