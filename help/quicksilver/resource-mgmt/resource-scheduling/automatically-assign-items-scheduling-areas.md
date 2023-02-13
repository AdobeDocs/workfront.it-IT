---
product-area: resource-management
navigation-topic: resource-scheduling
title: Assegnazione automatica di attività e problemi non assegnati nelle aree di programmazione
description: Quando si utilizzano gli strumenti di programmazione, è possibile consentire ad Adobe Workfront di analizzare le assegnazioni di lavoro correnti tra gli utenti disponibili e proporre assegnazioni logiche intelligenti per tutte le attività o i problemi non ancora assegnati. È possibile modificare tutte le assegnazioni proposte prima di finalizzarle.
author: Alina
feature: Resource Management
exl-id: 087fe3ef-9b85-491b-9fdc-436a01822ede
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1579'
ht-degree: 0%

---

# Assegnazione automatica di attività e problemi non assegnati nelle aree di programmazione

>[!IMPORTANT]
>  
><span class="preview">La funzionalità di pianificazione descritta in questo articolo è stata rimossa e rimossa da Adobe Workfront a partire dalla versione 23.1 di gennaio 2023.   </span>
>  
> <span class="preview"> Questo articolo verrà rimosso anche poco dopo la versione 23.1, all’inizio del 2023. Al momento, è consigliabile aggiornare di conseguenza tutti i segnalibri. </span>
> 
><span class="preview"> Ora puoi utilizzare il servizio di bilanciamento del carico di lavoro per pianificare il lavoro per le risorse. </span>
>  
> <span class="preview">Per informazioni sulla pianificazione delle risorse tramite il servizio di bilanciamento del carico di lavoro, consulta la sezione . [Il servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

Quando si utilizzano gli strumenti di programmazione, è possibile consentire ad Adobe Workfront di analizzare le assegnazioni di lavoro correnti tra gli utenti disponibili e proporre assegnazioni logiche intelligenti per tutte le attività o i problemi non ancora assegnati. È possibile modificare tutte le assegnazioni proposte prima di finalizzarle.

Workfront esamina le attività e i problemi disponibili nell’area Non assegnato all’interno dell’intervallo di date attualmente selezionato e propone le assegnazioni per ogni elemento contemporaneamente. È possibile creare un filtro per limitare il numero di elementi disponibili nell’area Non assegnata.

L’amministratore di sistema determina il modo in cui Workfront calcola la disponibilità delle risorse a livello di sistema (considerando le ore e la disponibilità di FTE). A seconda di questa impostazione a livello di sistema, la disponibilità delle risorse viene calcolata utilizzando la pianificazione predefinita o la pianificazione dell’utente. Per ulteriori informazioni, consulta [Configurare il modo in cui Workfront calcola la disponibilità di ore risorsa e FTE per l’area di pianificazione](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).

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
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Accesso a progetti, attività e problemi</p> <p><strong>NOTA</strong>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute o superiori ai progetti, alle attività e ai problemi per i quali vengono aggiornate le assegnazioni</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti {#prerequisites}

Workfront utilizza un algoritmo proprietario per determinare le proposte di assegnazione. Per facilitare i risultati migliori, assicurati che le seguenti informazioni siano accurate in Workfront:

* Informazioni sulle attività e sui problemi, tra cui:

   * Assegnazioni ruoli\
      Non viene presentata alcuna proposta per i compiti e le questioni che non sono assegnati a un ruolo.
   * Lavoro Necessario\
      Se un&#39;attività o un problema al momento non dispone di ore pianificate, Workfront prevede 4 ore pianificate per giorno lavorativo quando si assegna automaticamente il lavoro. Tali ore non vengono assegnate automaticamente all&#39;elemento di lavoro; sono utilizzati solo per garantire distribuzioni di assegnazione più realistiche.
   * Date di inizio pianificate e date di completamento pianificate

* Informazioni utente, tra cui:

   * Assegnazioni di ruoli principali e secondari nel profilo utente
   * Informazioni sul team di progetto

## Configurare i limiti dei ruoli

I limiti del ruolo controllano il numero di utenti, con un ruolo specifico, a cui è possibile assegnare il lavoro automaticamente. I limiti di ruolo funzionano a livello di singolo progetto per garantire che le attività basate sul ruolo non vengano distribuite tra un gran numero di utenti.

I seguenti scenari descrivono come si applicano i limiti di ruolo ai progetti:

* **Scenario 1**: Se al team di progetto non sono assegnati utenti, il sistema utilizza il limite di ruolo per assegnare le attività.\
   Ad esempio, disponi di un progetto senza utenti assegnati al team del progetto. Questo progetto dispone di 10 attività di gestione del progetto da assegnare ed è stato impostato un limite di ruolo pari a 1 per il ruolo di Project Manager. Il sistema assegna tutte e 10 le attività a 1 project manager perché il limite di ruolo è impostato su 1.

* **Scenario 2**: Se il limite di ruolo è maggiore del numero di utenti assegnati al team di progetto, ad altri utenti vengono assegnate attività.\
   Ad esempio, hai un progetto con un autore assegnato al team del progetto. Questo progetto ha 12 attività di scrittura da assegnare e si dispone di un limite di ruolo di 2 impostato per il ruolo Scrittore. Il sistema assegna tutte e 12 le attività tra il project team writer e un altro writer perché il limite di ruolo è impostato su 2.

* **Scenario 3**: Se il limite di ruolo è inferiore al numero di utenti assegnati al team di progetto, il limite di ruolo viene ignorato.\
   Ad esempio, hai un progetto con 4 designer assegnati al team del progetto. È necessario assegnare a questo progetto 8 attività di progettazione ed è stato impostato un limite di ruolo di 2 per il ruolo di Designer. Il sistema assegna tutte e 8 le attività tra i 4 progettisti del team di progetto, anche se il limite di ruolo è impostato su 2.

Per impostare i limiti per le assegnazioni di ruoli di lavoro:

1. Passa alla tempistica di programmazione per più progetti o per un singolo progetto:

   * **Per progetti multipli**:  Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, fai clic su **Origine > Bilanciamento carico di lavoro**, quindi seleziona **Pianificazione** nel menu a discesa in alto a sinistra.
   * **Per un singolo progetto**: Passa a un progetto e fai clic sul pulsante **Bilanciamento del carico di lavoro** nel pannello a sinistra, quindi seleziona **Pianificazione** dal menu a discesa in alto a sinistra.

1. Fai clic sul pulsante **Impostazioni** icona.\
   ![Automode_settings.png](assets/automode-settings.png)

1. Nella sezione Programmazione automatica delle risorse , fai clic su nella **Limite** in linea con l&#39;elemento nel **Ruolo** e immettere un numero positivo.\
   Workfront salva automaticamente le modifiche.

   >[!NOTE]
   >
   >Tutti i membri del team di progetto correnti sono automaticamente idonei per tutti i lavori consigliati, indipendentemente dal limite di ruolo impostato.

   ![Set_Role_Limits.png](assets/set-role-limits-350x341.png)

1. (Facoltativo) Fai clic sul pulsante **Visualizzazione** nella parte superiore della colonna Limite e selezionare le opzioni di visualizzazione desiderate.
1. Per tornare all’area di pianificazione delle risorse, fai clic su **Torna alla pianificazione**.

## Assegnazione automatica di attività e problemi

È possibile assegnare attività e problemi agli utenti nella timeline della pianificazione, sia che si sia nella scheda Pianificazione (quando si pianifica risorse per più progetti) o nella scheda Staffing (quando si pianifica risorse per un singolo progetto).

Per consentire a Workfront di proporre automaticamente assegnazioni per attività e problemi nell&#39;area Non assegnata:

1. Passa alla tempistica di programmazione per più progetti o per un singolo progetto:

   * **Per progetti multipli**:  Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, fai clic su **Origine > Bilanciamento carico di lavoro**, quindi seleziona **Pianificazione** nel menu a discesa in alto a sinistra.
   * **Per un singolo progetto**: Passa a un progetto e fai clic sul pulsante **Bilanciamento del carico di lavoro** nel pannello a sinistra, quindi seleziona **Pianificazione** dal menu a discesa in alto a sinistra.

1. (Facoltativo) Crea un filtro per personalizzare il contenuto visualizzato nell’area Non assegnata nella timeline della pianificazione.\
   Per ulteriori informazioni sulla creazione di un filtro, consulta [Filtrare le informazioni nell&#39;area Pianificazione](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md#creating-and-modifying-filters-on-the-scheduling-tab-for-projects) in [Filtrare le informazioni nell&#39;area Pianificazione](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md) [Filtrare le informazioni nell&#39;area Pianificazione](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md)

   >[!TIP]
   >
   >Per garantire che Workfront assegni il lavoro agli utenti più idonei:
   >
   >* Filtrare solo le informazioni che influiscono sulle attività visualizzate nell&#39;area Non assegnata (ad esempio Portfoli, programmi e progetti).
   >* È consigliabile non filtrare le informazioni che influiscono sugli utenti disponibili da assegnare sulla timeline della pianificazione. In questo modo Workfront non può visualizzare tutti i potenziali assegnatari, il che può comportare assegnazioni meno soddisfacenti.


1. (Facoltativo) Modifica l’intervallo di date visualizzato nella timeline della pianificazione, come descritto in [Regola l&#39;intervallo di date delle aree di programmazione](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) in [Guida introduttiva alla pianificazione delle risorse](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md). Workfront esegue le assegnazioni solo per le attività e i problemi all&#39;interno dell&#39;intervallo di date visibile nella sequenza temporale di pianificazione.

1. Fai clic sul pulsante **Automatico** nell&#39;angolo in alto a destra della timeline della pianificazione.\
   ![programmazione_auto.png](assets/scheduling-auto-350x221.png)\
   Workfront propone assegnazioni per ogni attività o problema nel **Non assegnato** area.

   >[!TIP]
   >
   >I compiti e i problemi devono già essere assegnati a un ruolo per poter proporre un&#39;assegnazione. Per garantire i migliori risultati, le attività e i problemi devono contenere le informazioni descritte in [Prerequisiti](#prerequisites).

   Le assegnazioni proposte sono differenziate con una struttura tratteggiata intorno a ciascuna attività o problema, come segue:\
   **Assegnazione task proposta:**

   **Assegnazione attività esistente:**

1. (Facoltativo) È possibile modificare le assegnazioni proposte o esistenti prima di finalizzare le assegnazioni:

   >[!NOTE]
   >
   >Se si modifica un&#39;assegnazione esistente, viene modificato in uno stato proposto.

   * Per assegnare un elemento a un utente diverso:

      * Trascinare l&#39;attività o il problema dall&#39;utente proposto alla riga di un altro utente che si desidera assegnare.

         <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE: lists in this article need to be reformatted and maybe split - too many levels in)      
        </MadCap:conditionalText>      
        -->

         Per un determinato utente vengono visualizzate al massimo 10 attività al giorno. È possibile espandere l’elenco per visualizzare tutte le attività attualmente assegnate a tale utente. (Dopo aver effettuato le assegnazioni nella tempistica di programmazione, potrebbero essere visualizzate temporaneamente più di 10 attività.)\
         Quando si trascina un elemento, vengono visualizzate le seguenti informazioni prima di rilasciare l&#39;attività o il problema e di completare l&#39;assegnazione:

         * Un indicatore di rilascio viene visualizzato nella riga dell’utente. Questo consente di vedere dove viene assegnato un elemento prima di eseguire l&#39;assegnazione.
         * Se le allocazioni degli utenti sono abilitate nella timeline di pianificazione, vengono visualizzati gli indicatori di sovrallocazione rossi se il completamento dell&#39;assegnazione determina una sovrallocazione dell&#39;utente.\
            Per ulteriori informazioni sugli indicatori di sovrallocazione, vedi [Indicatori di allocazione](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md#understanding-allocation-indicators).

         * Gli utenti che non possono ricevere l&#39;assegnazione sono disattivati.
      * Espandi l’attività o il problema che desideri assegnare, fai clic sulla freccia a discesa nel **Assegnazioni** inizia a digitare il nome dell&#39;utente che desideri assegnare, quindi fai clic sul nome dell&#39;utente nell&#39;elenco a discesa.\
         ![schedario_task_espanso.png](assets/schedule-task-expanded-350x170.png)
   * Per posticipare la creazione di un&#39;assegnazione, trascina un&#39;attività o un problema che non sei ancora pronto per assegnare nuovamente a **Non assegnato** area.



1. Fai clic sul pulsante **Assegna assegnazioni** pulsante nella parte superiore della sequenza temporale di programmazione per finalizzare le assegnazioni proposte.\
   Oppure\
   Fai clic su **Annulla** restituire tutte le assegnazioni proposte alle posizioni precedenti.
