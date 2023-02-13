---
product-area: resource-management
navigation-topic: resource-scheduling
title: Filtrare le informazioni nell'area Pianificazione
description: L'utilizzo di un filtro nell'area Programmazione risorse consente di determinare quali elementi di lavoro vengono visualizzati nella sequenza temporale di programmazione. Ciò include quali attività e problemi vengono visualizzati nell'area Non assegnata e quali utenti vengono visualizzati.
author: Alina
feature: Resource Management
exl-id: 974b2515-ed10-459d-a317-36e62c52afc7
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '2452'
ht-degree: 0%

---

# Filtrare le informazioni nell&#39;area Pianificazione

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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

<!--
<p>(SEVERAL SECTIONS BELOW LINKED TO THE PRODUCT. SEE NOTES</p>
-->

L&#39;utilizzo di un filtro nell&#39;area Programmazione risorse consente di determinare quali elementi di lavoro vengono visualizzati nella sequenza temporale di programmazione. Ciò include quali attività e problemi vengono visualizzati nell&#39;area Non assegnata e quali utenti vengono visualizzati.

Prima di iniziare a filtrare il contenuto come descritto in questa sezione, acquisisci familiarità con il funzionamento della pianificazione delle risorse in Adobe Workfront.\
Per informazioni sulla pianificazione delle risorse in Workfront, consulta l’articolo [Guida introduttiva alla pianificazione delle risorse](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).\
Per ulteriori informazioni sulla timeline della programmazione, consulta l’articolo [Guida introduttiva alla pianificazione delle risorse](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

È possibile pianificare le risorse o un singolo team di cui si è membri o per qualsiasi progetto per il quale si è il Gestione risorse.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

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
   <td> <p>Visualizza l'accesso o superiore a Progetti, Attività e Problemi</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza autorizzazioni o versioni successive a progetti, attività e problemi</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

<!--
<p>(NOTE: sections below - LINKED TO THE ui. DO NOT RENAME/ DELETE)</p>
-->

## Crea un filtro nella sezione Pianificazione (per Team)

Le attività e i problemi relativi ai progetti, agli utenti e ai ruoli definiti nel filtro vengono visualizzati nella timeline della pianificazione nella scheda Attivato. Utilizza le opzioni nel filtro per determinare quali progetti, utenti e ruoli sono rappresentati nella timeline della pianificazione.

>[!NOTE]
>
>Non è possibile salvare un filtro nella scheda Lavorazione (per un team). Quando aggiorni la pagina o ti allontani da essa, il filtro ripristina le impostazioni predefinite.

Per creare un filtro per la timeline della pianificazione nella scheda Attivato per i team:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **Team**, seleziona un team e fai clic su **Bilanciamento del carico di lavoro** nel pannello a sinistra, seleziona **Pianificazione** dal menu a discesa in alto a sinistra.
1. Fai clic su **Filtro**.
1. Determinare quali progetti sono rappresentati nell&#39;area Non assegnato specificando le seguenti informazioni:

   <!--
   <p>(NOTE: Alina: there was a note that [This step is linked to from the context-sensitive help] but I could not find from where in the UI it is linked.)&nbsp;</p>
   -->

   * **Priorità del progetto:** Seleziona la priorità dei progetti da rappresentare nella timeline della pianificazione. Le attività e i problemi dei progetti con le priorità selezionate vengono visualizzati nella timeline della pianificazione.\
      Solo le priorità dei progetti che includono attività o problemi assegnati al team sono disponibili per scegliere da questo menu.
   * **Stati del progetto:** Seleziona lo stato dei progetti da rappresentare nella timeline della pianificazione. Le attività e i problemi dei progetti con gli stati selezionati vengono visualizzati nella timeline della pianificazione.\
      È possibile scegliere da questo menu solo gli stati dei progetti che includono attività o problemi assegnati al team.
   * **Progetti:** Seleziona i progetti da rappresentare nella timeline della pianificazione. Le attività e i problemi dei progetti selezionati vengono visualizzati nella timeline della pianificazione.\
      Le selezioni effettuate nei campi precedenti determinano i progetti disponibili per la selezione.\
      È possibile scegliere da questo menu solo i progetti che includono attività o problemi assegnati al team.

1. Stabilisci quali utenti vengono visualizzati nella timeline della pianificazione specificando le seguenti informazioni. Per impostazione predefinita, vengono visualizzati tutti i membri del team.

   <!--
   <p>(NOTE: this step is linked in the UI.)</p>
   -->

   * **Ruoli:** Seleziona i ruoli da rappresentare nella timeline della pianificazione.\
      Nell&#39;area Non assegnata vengono visualizzate solo le attività assegnate a tale ruolo. Vengono visualizzati solo gli utenti con i ruoli selezionati che possono essere assegnati a tali attività.\
      Gli utenti vengono visualizzati sulla timeline della pianificazione, organizzati in base al ruolo del lavoro.
   * **Utenti:** Seleziona i singoli utenti che desideri rappresentare nella timeline della pianificazione.\
      Vengono visualizzati solo gli utenti selezionati, indipendentemente dal fatto che abbiano un&#39;assegnazione di ruolo corrispondente all&#39;assegnazione di ruolo delle attività nell&#39;area Non assegnata.\
      Questa opzione non influisce sulle attività e sui problemi visualizzati nell&#39;area Non assegnata.

      <!--   
     <p>(NOTE: Alina: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])</p>   
     -->

1. (Facoltativo) Per apportare ulteriori modifiche alla tempistica di pianificazione (ad esempio per modificare l’intervallo di date) e per apportare modifiche alle assegnazioni degli utenti, consulta l’articolo [Assegnazione manuale di attività e problemi non assegnati nelle aree di programmazione](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

<!--
<p>(NOTE: below - LINKED TO THE UI, DO NOT RENAME/ DELETE/ CHANGE)</p>
-->

## Creare e modificare filtri nella sezione Pianificazione (per più progetti)

Puoi creare un nuovo filtro, applicare un filtro creato in precedenza, modificare un filtro creato in precedenza o eliminare un filtro. Non puoi condividere i filtri creati con altri utenti.

* [Crea un filtro nella sezione Pianificazione (per i progetti)](#create-a-filter-in-the-scheduling-section-for-projects)
* [Applicazione di un filtro salvato](#apply-a-saved-filter)
* [Modificare un filtro salvato](#modify-a-saved-filter)
* [Eliminare un filtro salvato](#delete-a-saved-filter)

### Crea un filtro nella sezione Pianificazione (per i progetti) {#create-a-filter-in-the-scheduling-section-for-projects}

<!--
<p>(NOTE: *****LINKED TO THE PRODUCT FROM THE GLOBAL SCHEDULER >> BOTH THE FIRST AND THE SECOND AREAS) </p>
-->

Nella timeline della pianificazione della scheda Pianificazione vengono visualizzate le attività e i problemi relativi a progetti, utenti e ruoli definiti nel filtro. Utilizza le opzioni nel filtro per determinare quali progetti, utenti e ruoli sono rappresentati nella timeline della pianificazione.

Per creare un filtro per la timeline della pianificazione nella scheda Pianificazione per più progetti:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, fai clic su **Origine > Bilanciamento carico di lavoro**, quindi seleziona **Pianificazione** nel menu a discesa in alto a sinistra.
1. Fai clic su **Filtro**.\
   ![](assets/scheduling-filter-350x351.png)

1. Lascia la **Filtri salvati** campo vuoto.
1. Determinare quali progetti sono rappresentati nell&#39;area Non assegnato specificando le seguenti informazioni:

   <!--
   <p>(NOTE: Alina: this step is linked in the UI.) </p>
   -->

   * **Portfoli:** Seleziona tutti i portfolio che includono programmi e progetti da rappresentare nella timeline della pianificazione.

      Solo i programmi all’interno dei portfolio selezionati sono disponibili per la selezione nella **Programma** campo .

   * **Programmi:** Seleziona i programmi che includono i progetti da rappresentare nella timeline della pianificazione.\
      Le selezioni nella **Portfolio** determina i programmi disponibili per la selezione.\
      Solo i progetti all’interno dei programmi selezionati sono disponibili per la selezione nella **Progetti** campo .

   * **Priorità del progetto:** Seleziona la priorità dei progetti da rappresentare nella timeline della pianificazione.\
      Sono rappresentati solo i progetti con le priorità selezionate.

   * **Stati del progetto:** Seleziona lo stato dei progetti da rappresentare nella timeline della pianificazione.\
      Sono rappresentati solo i progetti con gli stati selezionati.

   * **Società di progetto:** Le attività e i problemi vengono visualizzati nella timeline della pianificazione solo quando appartengono a un progetto che corrisponde a una società selezionata.

   * **Gruppi di progetto:** Le attività e i problemi vengono visualizzati nella timeline della pianificazione solo quando appartengono a un progetto che corrisponde a un gruppo selezionato.

   * **Progetti:** Seleziona i progetti da rappresentare nella timeline della pianificazione. Le attività e i problemi dei progetti selezionati vengono visualizzati nella timeline della pianificazione.\
      Le selezioni effettuate nei campi precedenti determinano i progetti disponibili per la selezione.\
      Le attività e i problemi dei progetti selezionati vengono visualizzati nella timeline della pianificazione. È possibile scegliere da questo menu solo i progetti che includono attività o problemi assegnati al team.

1. Stabilisci quali utenti vengono visualizzati nella timeline della pianificazione specificando le seguenti informazioni: Per impostazione predefinita, vengono visualizzati solo gli utenti idonei per l’assegnazione di un’attività o un problema dall’area Non assegnata. Quando selezioni singoli utenti, gli utenti vengono visualizzati sulla timeline della pianificazione indipendentemente dal fatto che siano idonei a ricevere un’attività o un problema dall’area Non assegnata.) 

   <!--
   <p>(NOTE: Alina: this step had a note that it is linked in the UI but I could not find from where.) </p>
   -->

   * **Società utente:** Questo campo ti consente di impedire la visualizzazione degli utenti di altre aziende sulla timeline della pianificazione.\
      Lascia vuoto questo campo se desideri aggiungere gli utenti di qualsiasi società. Se specifichi società singole, solo gli utenti di tali società possono essere aggiunti alla cronologia di programmazione. La specificazione di una società non aggiunge automaticamente gli utenti di tale società alla tempistica di pianificazione. Utilizza invece i campi seguenti per aggiungere utenti specifici.\
      Questa opzione non influisce sulle attività e sui problemi visualizzati nell&#39;area Non assegnata.****

   * **Gruppi di utenti:** Tutti gli utenti di qualsiasi gruppo di utenti specificato vengono visualizzati nella timeline della pianificazione.

   * **Team:** Tutti gli utenti di un qualsiasi team specificato vengono visualizzati nella timeline della pianificazione.\
      Questa opzione non influisce sulle attività e sui problemi visualizzati nell&#39;area Non assegnata.

   * **Ruoli:** Seleziona i ruoli da rappresentare nella timeline della pianificazione.\
      Nell&#39;area Non assegnata vengono visualizzate solo le attività assegnate a tale ruolo. Vengono visualizzati solo gli utenti con i ruoli selezionati che possono essere assegnati a tali attività.\
      Gli utenti vengono visualizzati sulla timeline della pianificazione, organizzati in base al ruolo del lavoro.

   * **Utenti:** Seleziona i singoli utenti che desideri rappresentare nella timeline della pianificazione.\
      Vengono visualizzati solo gli utenti selezionati, indipendentemente dal fatto che abbiano un&#39;assegnazione di ruolo corrispondente all&#39;assegnazione di ruolo delle attività nell&#39;area Non assegnata.\
      Questa opzione non influisce sulle attività e sui problemi visualizzati nell&#39;area Non assegnata.
   <!--
   <p>NOTE: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])<br></p>
   -->

1. Fai clic su **Salva nuovo filtro**.\
   I dati vengono visualizzati sulla timeline della pianificazione.

1. (Facoltativo) Per apportare ulteriori modifiche alla tempistica di pianificazione (ad esempio per modificare l’intervallo di date) e per apportare modifiche alle assegnazioni degli utenti, consulta l’articolo [Assegnazione manuale di attività e problemi non assegnati nelle aree di programmazione](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Applicazione di un filtro salvato {#apply-a-saved-filter}

>[!NOTE]
>
>Questa opzione si applica solo quando si pianificano risorse per più progetti (dalla scheda Pianificazione); non è possibile applicare un filtro salvato durante la pianificazione delle risorse per un team (dalla scheda Lavoro in corso) o durante la pianificazione delle risorse per un singolo progetto (dalla scheda Gestione risorse).

Puoi applicare un filtro creato in precedenza.

Per applicare un filtro salvato per più progetti:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, fai clic su **Origine > Bilanciamento carico di lavoro**, quindi seleziona **Pianificazione** nel menu a discesa in alto a sinistra.
1. Fai clic su **Filtro**.
1. In **Filtri salvati** selezionare il filtro da applicare.\
   I dati vengono visualizzati sulla timeline della pianificazione.

1. (Facoltativo) Per apportare ulteriori modifiche alla tempistica di pianificazione (ad esempio per modificare l’intervallo di date) e per apportare modifiche alle assegnazioni degli utenti, consulta l’articolo [Assegnazione manuale di attività e problemi non assegnati nelle aree di programmazione](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Modificare un filtro salvato {#modify-a-saved-filter}

>[!NOTE]
>
>Questa opzione si applica solo quando si pianificano risorse per più progetti (dalla scheda Pianificazione); non è possibile modificare un filtro salvato durante la pianificazione delle risorse per un team (dalla scheda Lavoro in corso) o durante la pianificazione delle risorse per un singolo progetto (dalla scheda Gestione risorse).

Puoi modificare un filtro creato in precedenza.

Per modificare un filtro salvato per più progetti:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, fai clic su **Origine > Bilanciamento carico di lavoro**, quindi seleziona **Pianificazione** nel menu a discesa in alto a sinistra.
1. Fai clic su **Filtro**.
1. In **Filtri salvati** selezionare il filtro da modificare dall&#39;elenco a discesa.
1. Specifica i dati da visualizzare nella timeline della pianificazione.
1. Fai clic su **Salva**.\
   I dati vengono visualizzati sulla timeline della pianificazione.

1. (Facoltativo) Per apportare ulteriori modifiche alla tempistica di pianificazione (ad esempio per modificare l’intervallo di date) e per apportare modifiche alle assegnazioni degli utenti, consulta l’articolo [Assegnazione manuale di attività e problemi non assegnati nelle aree di programmazione](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Eliminare un filtro salvato {#delete-a-saved-filter}

>[!NOTE]
Questa opzione si applica solo quando si pianificano risorse per più progetti (dalla scheda Pianificazione); non è possibile eliminare un filtro salvato durante la pianificazione delle risorse per un team (dalla scheda Lavoro in corso) o durante la pianificazione delle risorse per un singolo progetto (dalla scheda Gestione risorse).

È possibile eliminare un filtro creato in precedenza.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, fai clic su **Origine > Bilanciamento carico di lavoro**, quindi seleziona **Pianificazione** nel menu a discesa in alto a sinistra.
1. Fai clic su **Filtro**.
1. In **Filtri salvati** nell’elenco a discesa, fai clic su (x) accanto al filtro da eliminare. 

## Creare e modificare filtri nella sezione Pianificazione (per un singolo progetto)

<!--
<p>(NOTE: **** LINKED FROM THE PRODUCT FROM THE PROJECT> STAFFING> SCHEDULING AREA) </p>
-->

Le attività e i problemi relativi a utenti, team e ruoli definiti nel filtro vengono visualizzati nella timeline della pianificazione nella scheda Staffing . Utilizza le opzioni nel filtro per determinare quali utenti, team e ruoli sono rappresentati nella timeline della pianificazione.

>[!NOTE]
Non è possibile salvare un filtro nella scheda Staffing (per un singolo progetto). Quando aggiorni la pagina o ti allontani da essa, il filtro ripristina le impostazioni predefinite.

Per creare un filtro per la timeline della pianificazione nella scheda Staffing (Staffing) per un singolo progetto:

1. Passa a un progetto e fai clic sul pulsante **Bilanciamento del carico di lavoro** nel pannello a sinistra, quindi seleziona **Pianificazione** dal menu a discesa in alto a sinistra.
1. Stabilisci quali utenti vengono visualizzati nella timeline della pianificazione specificando le seguenti informazioni: Per impostazione predefinita, vengono visualizzati solo gli utenti idonei per l’assegnazione di un’attività o un problema dall’area Non assegnata. Quando selezioni singoli utenti, gli utenti vengono visualizzati sulla timeline della pianificazione indipendentemente dal fatto che siano idonei a ricevere un’attività o un problema dall’area Non assegnata.) 

   <!--
   <p><span>(NOTE: Alina: [This step is linked to from the context-sensitive help]) </span> </p>
   -->

   * **Società utente:** Questo campo ti consente di impedire la visualizzazione degli utenti di altre aziende sulla timeline della pianificazione.\
      Lascia vuoto questo campo se desideri aggiungere gli utenti di qualsiasi società. Se specifichi società singole, solo gli utenti di tali società possono essere aggiunti alla cronologia di programmazione. La specificazione di una società non aggiunge automaticamente gli utenti di tale società alla tempistica di pianificazione. Utilizza invece i campi seguenti per aggiungere utenti specifici.\
      Questa opzione non influisce sulle attività e sui problemi visualizzati nell&#39;area Non assegnata.

   * **Gruppi di utenti:** Tutti gli utenti di qualsiasi gruppo di utenti specificato vengono visualizzati nella timeline della pianificazione.

   * **Team:** Tutti gli utenti di un qualsiasi team specificato vengono visualizzati nella timeline della pianificazione.\
      Questa opzione non influisce sulle attività e sui problemi visualizzati nell&#39;area Non assegnata.

   * **Ruoli:** Seleziona i ruoli da rappresentare nella timeline della pianificazione.\
      Nell&#39;area Non assegnata vengono visualizzate solo le attività assegnate a tale ruolo. Vengono visualizzati solo gli utenti con i ruoli selezionati che possono essere assegnati a tali attività.\
      Gli utenti vengono visualizzati sulla timeline della pianificazione, organizzati in base al ruolo del lavoro.

   * **Utenti:** Seleziona i singoli utenti che desideri rappresentare nella timeline della pianificazione.\
      Vengono visualizzati solo gli utenti selezionati, indipendentemente dal fatto che abbiano un&#39;assegnazione di ruolo corrispondente all&#39;assegnazione di ruolo delle attività nell&#39;area Non assegnata.\
      Questa opzione non influisce sulle attività e sui problemi visualizzati nell&#39;area Non assegnata.
   <!--
   <p>(NOTE: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])<br></p>
   -->
