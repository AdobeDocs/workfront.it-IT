---
title: Panoramica sullo stato del progetto
content-type: reference
description: La funzione Integrità del progetto utilizza la potenza di AI Assistant per fornire immediatamente una valutazione delle prestazioni dei progetti.
author: Jenny
feature: Get Started with Workfront
exl-id: e4d200c6-7f35-4919-96d3-2880a655ed62
hide: true
hidefromtoc: true
source-git-commit: 97b2118b1897f75dea0e45758e3d7f7c3409b234
workflow-type: tm+mt
source-wordcount: '1862'
ht-degree: 0%

---

# Panoramica sullo stato del progetto

>[!IMPORTANT]
>
>La funzione Integrità del progetto è attualmente disponibile solo per gli utenti che partecipano alla fase beta.

La funzione Integrità dei progetti di Adobe Workfront utilizza la potenza di AI Assistant per fornire immediatamente una valutazione delle prestazioni dei progetti, delle aree che richiedono la tua attenzione e di come evitare problemi che possono costarti tempo e denaro.

L&#39;Assistente IA può generare una valutazione dello stato del progetto per i seguenti oggetti:

* Un singolo progetto
* Un singolo programma
* Più progetti

Per ulteriori informazioni sull&#39;Assistente di IA, vedere [Panoramica dell&#39;Assistente di IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

+++ Espandere per visualizzare i requisiti di accesso. 
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>piano Adobe Workfront</p></td> 
   <td> 
<p>Seleziona, Prime o Ultimate </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td> 
<p>Standard</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td> 
   <td><p>Amministratore per gestire le configurazioni di integrità del progetto </p>
   <p>Modifica per applicare le configurazioni di integrità del progetto </p>
     <p>Visualizza per visualizzare le configurazioni di integrità del progetto </p>
  </td> 
  </tr>  
    </tr>  
</tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Iscriviti alla versione beta di Project Health

Per utilizzare Project Health (Integrità del progetto), l’organizzazione deve avere l’Assistente AI abilitato.

Per abilitare l’Assistente AI e l’integrità del progetto per la tua organizzazione, devono essere applicate tutte le seguenti condizioni:

* La tua organizzazione deve aver eseguito la migrazione ad Adobe IMS (Identity Management System).
* La tua organizzazione deve disporre di un piano Select, Prime o Ultimate Workfront
* L’esperienza unificata di Adobe deve essere abilitata.
* Adobe deve disporre di un accordo Adobe Gen AI firmato su file.
* L’amministratore di Workfront deve abilitare l’Assistente IA per gli utenti dell’organizzazione. L’Assistente AI è abilitato tramite i livelli di accesso.
* Entrambe le opzioni Abilita AI e Integrità progetto devono essere selezionate nella sezione Preferenze AI in Configurazione > Preferenze.

  ![Sezione Preferenze AI](assets/ai-preferences.png)

Per ulteriori informazioni, vedere [Panoramica dell&#39;Assistente AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md) e [Configurare le preferenze di sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Elenco dei prompt dell&#39;Assistente AI

Di seguito è riportato un elenco di prompt che è possibile utilizzare per richiedere una valutazione IA per generare una valutazione dello stato del progetto per un progetto, un programma o tutti i progetti nel proprio account.

<table>
    <tr>
        <td><b>Posizione</b></td>
        <td><b>Prompt</b></td>
    </tr>
    <tr>
        <td>Pagina dei dettagli di un progetto specifico</td>
        <td><em>Qual è lo stato di salute di questo progetto?</em></td>
    </tr>
    <tr>
        <td>Qualsiasi pagina in Workfront </td>
        <td><em>Qual è lo stato del progetto [PROJECT NAME]?</em></td>
    </tr>
    <tr>
        <td>Qualsiasi pagina in Workfront </td>
        <td><em>Qual è lo stato dei miei progetti?</em></td>
    </tr>
       <tr>
        <td>Pagina dei dettagli di un programma specifico</td>
        <td><em>Qual è lo stato di salute di questo programma?</em></td>
    </tr>
       <tr>
        <td>Qualsiasi pagina in Workfront </td>
        <td><em>Qual è lo stato del programma [NOME PROGRAMMA]?</em></td>
    </tr>
   </table>


## Elenco condizioni progetto e programma

Di seguito sono riportate le condizioni disponibili che l&#39;Assistente IA assegnerà al progetto o al programma durante la generazione di una valutazione dello stato del progetto.

<table>
    <tr>
        <td><b>Condizione progetto</b></td>
        <td><b>Stato avanzamento progetto</b></td>
    </tr>
    <tr>
        <td>Puntuale</td>
        <td>Quando lo stato di avanzamento del progetto è Puntuale, la condizione del progetto è Puntuale.</td>
    </tr>
    <tr>
        <td>A Rischio</td>
        <td>Quando lo stato di avanzamento del progetto è In ritardo o A rischio, la condizione del progetto è A rischio.</td>
    </tr>
    <tr>
        <td>In difficoltà</td>
        <td>Quando lo stato di avanzamento del progetto è In ritardo, la condizione del progetto è A rischio.</td>
    </tr>
    </tr>
   </table>

## Gestisci configurazioni integrità progetto

Una configurazione dell&#39;integrità di un progetto contiene criteri specifici che determinano la modalità di calcolo dell&#39;integrità del progetto. Dopo aver creato una configurazione, puoi applicarla a un progetto.

>[!NOTE]
>
>Per gestire le configurazioni dell&#39;integrità del progetto è necessario essere amministratore di sistema.

{{step-1-to-setup}}

1. Fai clic su **Preferenze progetto** nel pannello a sinistra, quindi seleziona **Integrità progetto** nel menu a discesa visualizzato.

1. Nell&#39;angolo superiore destro della pagina, seleziona **Nuova configurazione**.

1. (Facoltativo) Nella pagina dei dettagli delle configurazioni, sostituisci *Configurazione senza titolo* con una nuova configurazione **Nome**.

1. Nella sezione **Quali fattori si desidera includere nell&#39;integrità del progetto** deselezionare i fattori che non si desidera includere nella determinazione dei criteri di integrità del progetto:
   * **Scorrimento ambito**: quanto è stato espanso l&#39;ambito del progetto dall&#39;avvio.

   * **Campi obbligatori**: se mancano campi obbligatori (ad esempio, la descrizione del progetto). Questi campi obbligatori determinano la completezza del progetto e sono specificati in **Quali campi si desidera verificare?** sezione di configurazione di seguito.


   * **Modifiche alla pianificazione**: quante modifiche alla pianificazione si sono verificate dall&#39;avvio del progetto.

   * **Stima attività**: la precisione con cui è stato stimato il lavoro dell&#39;attività (ad esempio, nessuna attività scaduta attualmente nel progetto).

   * **Burndown attività**: avanzamento del progetto rispetto alla sequenza temporale.

   * **Attività scadute**: quante attività sono attualmente scadute.

   * **Costo**: se il progetto ha superato il preventivo.

1. In **Quando inizia ufficialmente il progetto?**, seleziona dall&#39;elenco a discesa l&#39;evento che segnala l&#39;inizio del progetto.

1. In **Come si stima l&#39;ambito del lavoro su un progetto?** sezione, selezionare il fattore di progetto che aumenterà con l&#39;aumento dell&#39;ambito del progetto.

1. In **Quali campi si desidera verificare la completezza?** sezione, selezionare uno o più campi che verranno controllati per determinare la completezza del progetto.

   ![Campi di completezza progetto](assets/project-completeness-fields.png)


1. Fai clic su **Salva** nell&#39;angolo superiore destro.

## Applica configurazioni integrità progetto

Dopo che un amministratore ha creato una configurazione di Integrità progetto, gli utenti con accesso in modifica possono applicarla a un progetto.


{{step1-to-projects}}

1. Nella pagina **Progetti**, seleziona un progetto.

1. Fai clic sull&#39;icona **Altro** ![Icona Altro](assets/more-icon.png) a destra del nome del progetto, quindi seleziona **Modifica**. Viene aperto il pannello laterale **Modifica progetto**.

1. Nel pannello a sinistra, seleziona **Impostazioni progetto**.

1. Nel campo **Configurazione integrità progetto**, selezionare la configurazione da applicare al progetto.

   ![Campo configurazione integrità progetto](assets/project-health-configurations.png)

1. Fai clic su **Salva** nell&#39;angolo inferiore sinistro del pannello.

## Generare una valutazione dello stato del progetto per un progetto o un programma

Se si dispone dell&#39;accesso di visualizzazione per un progetto o un programma, è possibile generare la relativa valutazione dello stato del progetto utilizzando l&#39;assistente di IA.

Se stai generando una valutazione per un progetto, ciò può essere fatto dalla pagina del progetto o facendo riferimento al nome del progetto quando chiedi all&#39;assistente come sta andando il progetto.

Per generare una valutazione per un programma, è possibile utilizzare la pagina dei dettagli del programma.

>[!NOTE]
>
>Per un progetto non è possibile generare una valutazione di integrità finché il progetto non è stato avviato. È possibile configurare l’evento che attiva un progetto a partire dalle impostazioni del progetto.

Per ulteriori informazioni, vedere la sezione seguente in questo articolo: [Gestione configurazioni integrità progetto](#manage-project-health-configurations).

1. Passare al progetto o al programma per il quale si desidera generare una valutazione dello stato del progetto.

1. Nella pagina dei dettagli del progetto/programma, fai clic sull&#39;icona **Assistente AI** ![Assistente AI](assets/ai-assistant-icon.png) nell&#39;angolo superiore destro della schermata. Viene aperto l’Assistente AI.

1. Digitare quanto segue nel campo **Chiedi informazioni su Workfront**: *Informazioni sullo stato del progetto*

   Oppure

   Digitare quanto segue nel campo **Chiedi informazioni su Workfront**: *Qual è lo stato del programma?*

   >[!NOTE]
   >
   >Se si accede all&#39;Assistente IA da una pagina diversa di Workfront, è possibile digitare *Informazioni sullo stato del progetto [NOME PROGETTO]?* o *Qual è l&#39;integrità del programma [NOME PROGRAMMA]?* <br>
   >Per un elenco completo dei prompt correnti che è possibile immettere, vedere la sezione seguente in questo articolo: [Elenco dei prompt dell&#39;Assistente AI](#ai-assistant-prompts-list).

1. Premi l&#39;icona **Invia** ![Invia icona](assets/send-icon.png). La valutazione dello stato del progetto viene generata e visualizzata nel pannello. Nella parte superiore di ogni valutazione dello stato del progetto viene visualizzato un badge che riflette le condizioni correnti del progetto.

   ![Valutazione dell&#39;integrità del progetto](assets/health-assessment.png)

   Se stai generando una valutazione per un portfolio, verranno elencati più badge che mostrano le condizioni di ciascun progetto nel programma. Per ulteriori informazioni sulle etichette dei badge, vedere la seguente sezione in questo articolo: [Elenco delle condizioni del progetto e del programma](#project-and-program-conditions-list).

1. (Facoltativo) Fare clic su uno dei punti di valutazione per espandere i relativi dettagli.

1. (Facoltativo) Nella modalità dettagli espansi, fai clic sul collegamento dell’attività per aprire i dettagli dell’attività.

   ![Dettagli estesi](assets/expanded-details.png)

1. Dopo aver esaminato i dettagli di integrità del progetto, fai clic sull&#39;icona **Chiudi** ![Chiudi](assets/close-icon.png) nell&#39;angolo superiore destro dell&#39;Assistente IA.

## Generare una valutazione dello stato del progetto per più progetti

È possibile generare una valutazione combinata dello stato del progetto per tutti i progetti per i quali si dispone attualmente dell&#39;accesso di visualizzazione (o di livello superiore).

Un progetto verrà incluso nella valutazione combinata dello stato del progetto solo se il progetto è stato avviato. È possibile configurare l’evento che attiva un progetto a partire dalle impostazioni del progetto. Per ulteriori informazioni, vedere la sezione seguente in questo articolo: [Gestione configurazioni integrità progetto](#manage-project-health-configurations).

1. Fai clic sull&#39;icona **Assistente AI** ![Icona Assistente AI](assets/ai-assistant-icon.png) nell&#39;angolo superiore destro della schermata. Viene aperto l’Assistente AI.

1. Digita quanto segue nel campo **Chiedi informazioni su Workfront**: *Qual è lo stato dei miei progetti?*

   Per un elenco completo dei prompt correnti che è possibile immettere, vedere la sezione seguente in questo articolo: [Elenco dei prompt dell&#39;Assistente AI](#ai-assistant-prompts-list).

1. Premi l&#39;icona **Invia** ![Invia icona](assets/send-icon.png). La valutazione dello stato del progetto viene generata e visualizzata nel pannello.

   ![Valutazione di più progetti](assets/multiple-projects-assessment.png)

   Durante la generazione di una valutazione per più progetti, l’Assistente IA raggruppa i risultati in base alle prestazioni correnti dei progetti.

1. (Facoltativo) Fai clic su uno dei badge di condizione di integrità del progetto per espandere l’elenco dei progetti, quindi seleziona un collegamento per un progetto specifico per passare alla pagina dei dettagli del progetto.

1. Dopo aver esaminato i dettagli di integrità dei progetti, fai clic sull&#39;icona **Chiudi** ![Chiudi](assets/close-icon.png) nell&#39;angolo superiore destro dell&#39;Assistente IA per chiuderlo.


## Creare un report di tabella di stato del progetto in un dashboard Area di lavoro

>[!IMPORTANT]
>
>La funzione Dashboard di Canvas è attualmente disponibile solo per gli utenti che partecipano alla fase beta. Per ulteriori informazioni, vedere [Informazioni sulla versione beta delle dashboard di Canvas](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

Puoi aggiungere un rapporto di tabella a un dashboard di Canvas per visualizzare facilmente i dati di Project Health in formato tabella.

### Prerequisiti

È necessario creare un dashboard prima di creare un rapporto di tabella.

Per ulteriori informazioni, vedere [Creare un dashboard Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

### Creare un report di tabella di stato del progetto

Sono disponibili molte opzioni di configurazione per la creazione di un report della tabella Integrità progetto. In questa sezione ti guideremo nel processo di creazione di un sito che visualizzi le seguenti colonne:

* **Nome**: contiene il nome del progetto.
* **Analisi integrità progetto**: contiene un riepilogo della valutazione dell&#39;integrità del progetto.
* **Integrità del progetto creata alle**: contiene la data/ora dell&#39;ultima generazione della valutazione dell&#39;integrità del progetto.
* **Etichetta integrità progetto**: contiene l&#39;etichetta del progetto (ad esempio Su Target, A Rischio, O In Difficoltà).

{{step1-to-dashboards}}

1. Nel pannello a sinistra, fai clic su **Dashboard Canvas**.
1. Nell&#39;angolo superiore destro fare clic su **Nuovo dashboard**.
1. Nella casella **Crea dashboard** immettere il **Nome** e la **Descrizione** del dashboard.
1. Fai clic su **Crea**.
1. Nella casella **Aggiungi report** selezionare **Crea report**.
1. Sul lato sinistro, selezionare **Tabella**.
1. Nell&#39;angolo superiore destro fare clic su **Crea report**.
1. (Facoltativo) Segui i passaggi seguenti per configurare la sezione **Dettagli** ![Icona Dettagli](assets/details-icon.png):
   1. Immetti un rapporto **Nome**.
   1. Immetti un rapporto **Descrizione**.
1. Segui i passaggi seguenti per configurare la sezione **Tabella di compilazione** ![Icona tabella di compilazione](assets/drilldown-column.png):
   1. Nel pannello a sinistra, fai clic sull&#39;icona **Colonne tabella**.
   1. Fai clic su **Aggiungi colonna**, quindi seleziona **Progetto** > **Nome**.
   1. Fai clic su **Aggiungi colonna**, quindi seleziona **Progetto** > **Integrità progetto** > **Analisi integrità**.
   1. Fai clic su **Aggiungi colonna**, quindi seleziona **Progetto** > **Integrità progetto** > **Creato alle**.
   1. Fai clic su **Aggiungi colonna**, quindi seleziona **Progetto** > **Integrità progetto** > **Etichetta integrità**.

1. Segui i passaggi seguenti per configurare la sezione **Filtro** ![Icona filtro](assets/filter-icon.png):
   1. Nel pannello a sinistra, fai clic sull&#39;icona **Filtro**.
   1. Selezionare **Modifica filtro**.
   1. Fare clic su **Aggiungi condizione** e quindi specificare il campo in base al quale si desidera filtrare e il modificatore che definisce il tipo di condizione che il campo deve soddisfare. La colonna viene visualizzata nella sezione di anteprima a destra.
   1. (Facoltativo) Fai clic su **Aggiungi gruppo di filtri** per aggiungere un altro set di criteri di filtro. L&#39;operatore di default tra i set è AND. Fai clic sull’operatore per modificarlo in O.

1. Segui i passaggi seguenti per configurare la sezione **Impostazioni gruppo di espansione** ![Impostazioni gruppo](assets/drilldown-group-icon.png):
   1. Nel pannello a sinistra, fai clic sull&#39;icona **Impostazioni gruppo**.
   1. Fare clic sul pulsante **Aggiungi raggruppamento** e quindi selezionare il campo da creare come raggruppamento. La colonna di raggruppamento viene visualizzata nella sezione di anteprima a destra.

1. Fai clic su **Salva** per creare il report.
