---
title: Panoramica del rilascio del primo trimestre 2026
description: Questa pagina fornisce informazioni sulle funzionalità incluse nel rilascio del primo trimestre 2026. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: ed348f44-eae1-4478-8425-6114f2b310ad
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '2885'
ht-degree: 100%

---

# Panoramica del rilascio del primo trimestre 2026

Questa pagina fornisce informazioni sulle funzionalità incluse nel rilascio del primo trimestre 2026 pianificato per gennaio 2026.

I miglioramenti in questa pagina sono disponibili nell’ambiente di anteprima. Questa pagina verrà aggiornata con ulteriori miglioramenti man mano che il rilascio del primo trimestre 2026 si avvicina al rilascio pianificato in produzione.


<!--
 Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>.
-->

>[!IMPORTANT]
>
>
>Salvo diversa indicazione, i rilasci mensili e trimestrali dovrebbero essere disponibili il giovedì della seconda settimana completa del mese.
>
>| Rilascio mensile | Rilascio trimestrale |
>|----|----|
>| <ul><li>25.11 (13 novembre 2025)</li><li>25.12 (11 dicembre 2025)</li><li>26.1 (14 gennaio 2026)</li></ul> | <ul><li>26.1 (15 gennaio 2026)</li></ul> |
>
>Tieni presente che per il rilascio finale di ogni trimestre (26.1 questo trimestre), gli utenti che seguono la pianificazione del rilascio rapido riceveranno il rilascio con un giorno di anticipo (14 gennaio 2026).
>
>Per ulteriori informazioni sul processo di rilascio rapido, consulta [Abilitare o disabilitare il processo di rilascio rapido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Miglioramenti in Adobe Workfront

* [Miglioramenti per gli amministratori](#administrator-enhancements)
* [Miglioramenti in documenti e approvazioni](#documents-and-approvals-enhancements)
* [Miglioramenti alla Home](#home-enhancements)
* [Miglioramenti dell’integrazione](#integration-enhancements)
* [Miglioramenti ai progetti](#project-enhancements)
* [Miglioramenti al reporting](#reporting-enhancements)
* [Miglioramenti alle richieste](#requests-enhancements)
* [Altri miglioramenti](#other-enhancements)

### Miglioramenti per gli amministratori

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funzione</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Trimestrale</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Gestire le priorità nel modello layout</a>
            <p><span class="preview">Temporaneamente non disponibile nell’ambiente di anteprima</span></p>
            <p>Ora puoi abilitare o disabilitare le Priorità per utenti specifici nel modello layout. Se in precedenza avevi disabilitato le Priorità per la tua organizzazione, con questa modifica tale opzione rimarrà disabilitata nel modello layout.</p>
        </td>
        <td>18 dicembre 2025</td>
        <td>14 gennaio 2025</td>
        <td>15 gennaio 2025</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Verificare la presenza di conflitti tra più moduli per i campi personalizzati calcolati</a>
            <p>Per fornire visibilità su quali oggetti potrebbero essere interessati dalla modifica di un’espressione nei campi personalizzati, è stata aggiunta un’opzione per verificare la presenza di conflitti. Questa finestra di dialogo mostra tutti gli oggetti che potrebbero essere interessati dalla modifica della formula, raggruppati per tipo di oggetto. Puoi passare ai dettagli relativi a ciascun oggetto ed esaminare i campi per decidere se un campo deve essere rimosso da uno dei moduli o se l’espressione deve rimanere invariata.</p>
        </td>
        <td>18 dicembre 2025</td>
        <td>14 gennaio 2025</td>
        <td>15 gennaio 2025</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Data inserimento e ID dell’autore dell’inserimento memorizzati negli oggetti personalizzati</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>La data di inserimento e l’ID dell’autore inserimento sono ora memorizzati nelle sezioni, nei campi e nei moduli personalizzati. Puoi utilizzare queste opzioni dati nei rapporti come filtri, viste o raggruppamenti. Per visualizzarli nell’elenco delle sezioni, dei campi o dei moduli personalizzati in Configurazione, aggiungi Data di inserimento e il nome dell’Autore dell’inserimento come colonne in una vista nuova o esistente.</p>
        </td>
        <td>13 novembre 2025</td>
        <td>13 novembre 2025</td>
        <td>13 novembre 2025</td>
    </tr>  
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti ai nomi dei pulsanti durante la modifica di un modello layout</a>
            <p>Per garantire maggiore coerenza con altre aree di configurazione, come il designer dei moduli personalizzati, i pulsanti visualizzati durante la modifica di un modello layout sono stati modificati in Applica, Salva e chiudi e Annulla. La nuova opzione Applica ti consente di salvare le modifiche apportate al modello layout e continuare a modificarle. In precedenza, le opzioni disponibili erano Salva e Annulla. </p>
        </td>
        <td>30 ottobre 2025</td>
        <td>13 novembre 2025</td>
        <td>15 gennaio 2026</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> Gestione dei campi migliorata con il flag Attivo sui campi personalizzati</a>
            <p>Quando nel sistema è presente un numero elevato di campi personalizzati, la gestione di tali campi nei rapporti e nei moduli personalizzati può risultare complessa. Ora puoi contrassegnare i campi personalizzati come inattivi con il nuovo flag <b>Attivo</b>. Questo flag è disponibile quando utilizzi un campo in un modulo personalizzato o quando aggiungi o modifichi un campo dall’elenco Campi. </p>
        </td>
        <td>30 ottobre 2025</td>
        <td>13 novembre 2025</td>
        <td>15 gennaio 2026</td>
    </tr>   
  </tbody>
</table>

### Miglioramenti in documenti e approvazioni

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funzione</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Trimestrale</strong></td>
        </tr>
       <!--
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Set up brands for the AI reviewer in Workfront<p>[!BADGE Off schedule]{type=Neutral}</p> </a>
            <p>You can now set up brands for the AI reviewer in the Workfront Setup area. This allows you to customize the AI review process based on your organization's branding guidelines.</p>
            <p>The AI reviewer is currently in beta.</p>
        </td>
        <td>January 8, 2026</td>
        <td>January 8, 2026</td>
        <td>January 8, 2026</td>
    </tr>
    -->
    </tr>
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Scegliere un progetto Workfront durante l’invio di una revisione in Adobe Express<p>[!BADGE Off schedule]{type=Neutral}</p> </a>
            <p>Puoi scegliere un progetto Workfront a cui inviare una bozza. In questo modo puoi mantenere tutte le risorse e le bozze correlate organizzate all’interno dello stesso progetto.</p>
        </td>
        <td>15 dicembre 2025</td>
        <td>15 dicembre 2025</td>
        <td>15 dicembre 2025</td>
    </tr> 
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Supporto multi-organizzazione per Adobe Express con la bozza di Workfront<p>[!BADGE Off schedule]{type=Neutral}</p> </a>
            <p>Sta per essere introdotto il supporto multi-organizzazione per Adobe Express con la bozza di Workfront. Questo miglioramento consente ai clienti che operano su più organizzazioni IMS di utilizzare e gestire senza interruzioni i flussi di lavoro di bozza.</p>
        </td>
        <td>13 novembre 2025</td>
        <td>13 novembre 2025</td>
        <td>13 novembre 2025</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Adobe Experience Manager ora disponibile con l’integrazione Frame.io <p>[!BADGE Off schedule]{type=Neutral}</p> </a>
            <p>Ora puoi utilizzare Experience Manager Assets per gestire e archiviare le risorse digitali che hanno completato il ciclo di revisione e approvazione. Questa integrazione consente di sfruttare le funzionalità di Adobe Experience Manager, Frame.io e Workfront per semplificare la gestione dei contenuti e i processi di collaborazione. </p>
        </td>
        <td>30 ottobre 2025</td>
        <td>30 ottobre 2025</td>
        <td>30 ottobre 2025</td>
    </tr>   
  </tbody>
</table>



### Miglioramenti alla Home

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funzione</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Trimestrale</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-home.md" class="MCXref xref" xrefformat="{para}">Aggiornamento al widget Menzioni della Home</a>
            <p>Al widget Menzioni della Home sono stati apportati i seguenti miglioramenti: <ul><li>La stessa esperienza nell’area Aggiornamenti della maggior parte degli oggetti Workfront è ora disponibile anche nel widget Menzioni della Home. </li><li>Il widget Menzioni ora contiene i commenti che l’utente ha inserito o in cui è stato taggato nelle ultime due settimane</li><ul></p>
        </td>
        <td>giovedì 17 dicembre 2025</td>
        <td>14 gennaio 2026</td>
        <td>15 gennaio 2026</td>
    </tr>   
  </tbody>
</table>

### Miglioramenti dell’integrazione

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funzione</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Trimestrale</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">Scegliere un progetto Workfront durante l’invio di una revisione in Creative Cloud Express</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>Puoi scegliere un progetto Workfront a cui inviare una bozza. In questo modo puoi mantenere tutte le risorse e le bozze correlate organizzate all’interno dello stesso progetto. </p>
        </td>
        <td>15 dicembre 2025</td>
        <td>15 dicembre 2025</td>
        <td>15 dicembre 2025</td>
    </tr>   
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">È stato aggiornato il selettore risorse per l’integrazione nativa di Adobe Workfront for Experience Manager Assets </a>
            <p>Il selettore delle risorse è stato aggiornato nell’integrazione Adobe Workfront for Experience Manager Assets. Con questo aggiornamento, ora puoi selezionare ed estrarre le raccolte AEM direttamente in Workfront. </p>
        </td>
        <td>20 novembre 2025</td>
        <td>11 dicembre 2025</td>
        <td>15 gennaio 2026</td>
    </tr>   
    <!--
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">New version of Salesforce integration now available </a>
            <p>To stay up-to-date with recent changes to the Workfront API, we've created a new Salesforce integration. The new integration features the same functionality as the previous version, and was updated to avoid losing functionality deprecated in the API.</p><p>NOTE: The Workfront for Salesforce integration, including the new version, will not be available after **February 28, 2026**. </p>
        </td>
        <td>October 30, 2025</td>
        <td>October 30, 2025</td>
        <td>October 30, 2025</td>
    </tr>
    -->
  </tbody>
</table>

### Miglioramenti ai progetti

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funzione</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Trimestrale</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-projects.md" class="MCXref xref" xrefformat="{para}">Gli utenti Light possono registrare le ore sui progetti</a>
            <p>Gli utenti Light adesso possono registrare le ore direttamente sui progetti. In precedenza, solo gli utenti con licenza Standard potevano registrare le ore sui progetti.</p>
        </td>
        <td>11 dicembre 2025</td>
        <td>15 gennaio 2026</td>
        <td>15 gennaio 2026</td>
    </tr>   
  </tbody>
</table>

### Miglioramenti al reporting

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funzione</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Trimestrale</strong></td>
    </tr>
 <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti della valuta nelle dashboard dell’area di lavoro</a>
            <p>Sono stati apportati i seguenti aggiornamenti ai campi valuta:<ul><li>Quando in Workfront sono definite più valute, ora puoi sceglierne una predefinita per la dashboard durante la creazione. </li><li>Durante la creazione di un rapporto, puoi bloccare un campo valuta. In questo modo la preferenza di valuta a livello di dashboard non influisce sulla visualizzazione di questi valori.</li><li>Quando visualizzi una dashboard, gli utenti possono passare da una valuta definita all’altra in Workfront. Queste modifiche si applicano all’intera dashboard ad eccezione dei campi di valuta bloccati</li></ul></p>
        </td>
        <td>18 dicembre 2025</td>
        <td>14 gennaio 2026</td>
        <td>15 gennaio 2026</td>
    </tr>
 <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}"> Risultati della tabella di ricerca rapida nelle dashboard dell’area di lavoro</a>
            <p>È stata aggiunta una ricerca rapida nella tabella rapporti. Questa ricerca funziona su tutte le pagine, quindi puoi trovare i dati anche se non sono attualmente visibili.</p>
        </td>
        <td>18 dicembre 2025</td>
        <td>14 gennaio 2026</td>
        <td>15 gennaio 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Nuova opzione Mostra totale per i grafici a torta</a>
            <p>È stata introdotta una nuova opzione Mostra totale che converte i grafici a torta in grafici ad anello. Questa funzione consente agli utenti di visualizzare un valore centrale che rappresenta il totale di tutti i segmenti nel grafico.</p>
        </td>
        <td>18 dicembre 2025</td>
        <td>14 gennaio 2026</td>
        <td>15 gennaio 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Nuove opzioni di configurazione per i grafici a torta nelle dashboard dell’area di lavoro</a>
            <p>Sono state introdotte due nuove opzioni di configurazione per i grafici a torta: <ul><li>Nascondi etichette segmento: ora puoi scegliere di nascondere le etichette dei segmenti di un grafico a torta se sono troppo lunghe e influiscono sulla leggibilità del grafico.</li><li>Nascondi e riposiziona legenda grafico: ora puoi scegliere di nascondere la legenda di un grafico a torta. Inoltre puoi impostare la posizione della legenda a destra (impostazione predefinita), a sinistra, in alto o in basso rispetto al grafico. </li></ul></p>
        </td>
        <td>18 dicembre 2025</td>
        <td>14 gennaio 2026</td>
        <td>15 gennaio 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Miglioramenti nel conteggio dei raggruppamenti delle dashboard dell’area di lavoro</a>
            <p>La barra di raggruppamento nelle dashboard dell’area di lavoro è stata aggiornata per mostrare il conteggio dei record della pagina corrente e il conteggio complessivo dei record del raggruppamento su tutte le pagine. </p>
        </td>
        <td>18 dicembre 2025</td>
        <td>14 gennaio 2026</td>
        <td>15 gennaio 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Nuova funzione Linea di riferimento nei rapporti nelle dashboard dell’area di lavoro</a>
            <p>Ora puoi definire una linea di riferimento nei grafici a barre, a colonne e a linee per impostare un target o una soglia nei tuoi rapporti basati su serie. </p>
        </td>
        <td>18 dicembre 2025</td>
        <td>14 gennaio 2026</td>
        <td>15 gennaio 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Personalizzare le etichette degli assi nei rapporti con grafico nelle dashboard dell’area di lavoro</a>
            <p>Ora puoi personalizzare le etichette degli assi nei rapporti con grafico. Questa nuova funzione consente di inserire un’etichetta dell’asse sostitutiva da mostrare al posto dell’oggetto e del percorso di campo predefiniti. Inoltre, puoi scegliere di nascondere completamente le etichette degli assi.</p>
        </td>
        <td>18 dicembre 2025</td>
        <td>14 gennaio 2026</td>
        <td>15 gennaio 2026</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Duplicare un rapporto in una dashboard dell’area di lavoro</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>Ora puoi duplicare un rapporto di KPI, tabella o grafico in una dashboard dell’area di lavoro dopo averlo creato. Una volta duplicato, puoi modificare il rapporto in base alle esigenze prima di salvarlo.</p>
        </td>
        <td>23 ottobre 2025</td>
        <td>23 ottobre 2025</td>
        <td>23 ottobre 2025</td>
    </tr>   
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Rimozione delle opzioni di campo dai filtri dei rapporti</a>
            <p>Sono state rimosse le seguenti opzioni di campo precedentemente disponibili durante l’applicazione di un filtro a un rapporto:
            <ul>
            <li>ID di altri gruppi</li>
            <li>ID di altri ruoli</li>
            <li>ID di altri team</li>
            </ul>
            </p>
        </td>
        <td>6 novembre 2025</td>
        <td>13 novembre 2025</td>
        <td>15 gennaio 2026</td>
    </tr>    
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Nuovi guardrail per migliorare i tempi di caricamento nelle dashboard dell’area di lavoro</a>
            <p>Per evitare ritardi nei tempi di caricamento e migliorare le prestazioni complessive delle dashboard dell’area di lavoro, sono stati applicati dei limiti al numero di componenti che è possibile aggiungere a una dashboard:
            <ul>
            <li>Rapporti per dashboard: limite di 25</li>
            <li>Raggruppamenti su viste tabella: limite di 5</li>
            <li>Distanza dall’oggetto di base del rapporto: limite di 10</li>
            <li>Colonne in una vista a tabella: limite di 25</li>
            <li>Prompt di filtro a livello di dashboard: limite di 10</li>
            </ul></p>
        </td>
       <td>6 novembre 2025</td>
        <td>13 novembre 2025</td>
        <td>15 gennaio 2026</td>
    </tr>   
  </tbody>
</table>

### Miglioramenti alle richieste

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funzione</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Trimestrale</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Sono ora disponibili collegamenti a oggetti creati nell’area Richieste e nel widget Le mie richieste</a>
            <p>Per facilitare l’accesso all’oggetto creato da una richiesta specifica, sono stati introdotti i collegamenti nella colonna Oggetto creato. Ora puoi fare clic sul collegamento in questa colonna per passare direttamente alla pagina dell’oggetto creato.</p>
        </td>
        <td>18 dicembre 2025</td>
        <td>14 gennaio 2026</td>
        <td>15 gennaio 2026</td>
    </tr> 
    <!--
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Create groupings in the Requests list and My Requests widget</a>
            <p>To make it easier for you to find the requests you need, we've added groupings to the Requests list and the My Requests widget. Now, you can group requests by any column on the list. These groupings become part of the view that you are using when you create the grouping.</p>
        </td>
        <td>December 18, 2025</td>
        <td>January 14, 2026</td>
        <td>January 15, 2026</td>
    </tr>
    -->
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Aggiungere campi personalizzati all’elenco Richieste e al widget Le mie richieste</a>
            <p>Per facilitare la visualizzazione delle informazioni necessarie, è stata introdotta la possibilità di aggiungere campi personalizzati come colonne nell’elenco Richieste e il widget Le mie richieste nella Home. Ora puoi aggiungere campi dai moduli personalizzati come colonna; le richieste che contengono informazioni in quel campo visualizzeranno tali informazioni nell’elenco o nel widget.</p><p>Questa funzionalità è disponibile solo nella nuova esperienza Richieste.</p>
        </td>
        <td>18 dicembre 2025</td>
        <td>14 gennaio 2026</td>
        <td>15 gennaio 2026</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Carattere jolly dell’utente corrente ora disponibile nel filtro Richieste</a>
            <p>Per filtrare più facilmente le richieste che ti riguardano, è stato creato un carattere jolly per l’utente corrente. Ora, quando applichi un filtro, puoi selezionare “Me (utente connesso)”. Il filtro verrà quindi applicato all’utente che sta visualizzando l’elenco delle richieste.   </p>
        </td>
        <td>18 dicembre 2025</td>
        <td>14 gennaio 2026</td>
        <td>15 gennaio 2026</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Compilazione moduli basata sull’IA ora disponibile per le richieste</a>
            <p>Per semplificare la creazione delle richieste, è stata creata la compilazione moduli basata sull’IA. Ora puoi incollare un prompt o caricare un documento in un modulo di richiesta: l’IA ne estrarrà le informazioni pertinenti e compilerà il modulo.  </p>
        </td>
        <td>11 dicembre 2025</td>
        <td>11 dicembre 2025</td>
        <td>11 dicembre 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Condividere le viste nell’area Richieste e nel widget Le mie richieste</a>
            <p>Per facilitare e garantire la visualizzazione delle informazioni necessarie, nella nuova esperienza di richiesta è stata introdotta la possibilità di condividere le viste. Ora puoi condividere le viste con altri utenti, team o gruppi. </p>
        </td>
        <td>4 dicembre 2025</td>
        <td>14 gennaio 2026</td>
        <td>15 gennaio 2026</td>
    </tr> 
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Salvare bozze di richieste nella nuova esperienza di richiesta</a>
            <p>Per semplificare la creazione e l’invio delle richieste, nella nuova esperienza è stata introdotta la possibilità di salvare le bozze. Ora, se inizi a compilare una richiesta e la chiudi, questa viene salvata con lo stato Bozza ed è disponibile nel modulo di richiesta utilizzato per creare la bozza. Puoi quindi riaprire, aggiornare e inviare la bozza nel modo che preferisci. </p>
        </td>
        <td>20 novembre 2025</td>
        <td>14 gennaio 2026</td>
        <td>15 gennaio 2026</td>
    </tr>  
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Eliminare le richieste inviate nella nuova esperienza di richiesta</a>
            <p>Per facilitare l’organizzazione delle richieste e mantenerle in ordine, nella nuova esperienza è stata introdotta la possibilità di eliminare le richieste. Ora puoi eliminare le richieste inviate. Gli amministratori di Workfront e della pianificazione dell’area di lavoro di Workspace possono eliminare le richieste.</p>
        </td>
        <td>20 novembre 2025</td>
        <td>14 gennaio 2026</td>
        <td>15 gennaio 2026</td>
    </tr>   
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Creare nuove richieste copiando quelle inviate in precedenza nella nuova esperienza di richiesta</a>
            <p>Per facilitare l’invio delle richieste, nella nuova esperienza è stata introdotta la possibilità di copiare le richieste. Ora puoi copiare una richiesta, modificarne tutti i campi e inviarla come nuova. </p>
        </td>
        <td>20 novembre 2025</td>
        <td>11 dicembre 2025</td>
        <td>15 gennaio 2026</td>
    </tr>    
  </tbody>
</table>

### Altri miglioramenti

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Funzione</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Trimestrale</strong></td>
    </tr>   
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti dell’aspetto durante l’arco temporale di rilascio del primo trimestre 2026</a>
                        <p>Aggiornamenti minori all’aspetto di varie aree dell’applicazione Adobe Workfront vengono effettuati entro l’arco temporale di rilascio del primo trimestre 2026. </p>
                    </td>
                    <td><p>Durante tutto l’arco temporale di rilascio del primo trimestre 2026<br /></p>
                    <td colspan="2"><p>Rilascio rapido: almeno 1 settimana dopo il rilascio in anteprima (se non diversamente specificato)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                 <td>
                <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}"> Limiti di selezione per campi a selezione multipla</a>
              <p>I campi che consentono selezioni multiple, come caselle di controllo e menu a discesa a selezione multipla, ora sono limitati a 5000 selezioni quando l’utente compila il modulo.</p>
             </td>
        <td>30 ottobre 2025</td>
        <td>13 novembre 2025</td>
        <td>15 gennaio 2026</td>
             </tr>   
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience ora disponibile per altre organizzazioni Workfront</a><p></p>
            <p>Per consentire alle organizzazioni di accedere ai vantaggi di Adobe Unified Experience, la disponibilità è stata estesa per i clienti esistenti di Workfront.</p>
        </td>
        <td><p>venerdì 11 dicembre 2025</p></td>
        <td><p>giovedì 11 febbraio 2026</p></td>
        <td><p>giovedì 11 febbraio 2026</p></td>
    <tr>
            </tbody>
        </table>


### Funzionalità che verrà presto rimossa da Workfront

#### Rimozione della valuta di sostituzione per le mansioni con la versione 25.11

Come parte della semplificazione del modello finanziario, il 30 ottobre sarà rimossa la valuta di sostituzione sulle mansioni negli ambienti di Anteprima e in Produzione per tutti i clienti che hanno la versione 25.11. Questa modifica interessa la configurazione di valute e tariffe per le mansioni nell’area Configura.

* I campi **Sovrascrivi valuta** in una mansione non saranno più disponibili.
* Ciascuna mansione disporrà di una singola valuta con il relativo costo e tariffa di fatturazione.
* Tutti le valute di sostituzione esistenti e i relativi valori delle tariffe verranno migrati automaticamente per diventare l’unica valuta e tariffe per quella mansione.

## Modernizzazione dell’interfaccia

L’interfaccia di Adobe Workfront è in fase di aggiornamento per migliorare l’esperienza utente e per uniformarla alle altre applicazioni Adobe. Queste modifiche vengono rilasciate al di fuori della pianificazione di rilascio standard. Per un elenco di queste modifiche, consulta [Modernizzazione dell’interfaccia](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

## Note sulla versione per altre aree

### Miglioramenti di Workfront Fusion

Le nuove funzioni di Workfront Fusion sono disponibili nell’ambiente di Produzione con una cadenza al di fuori della pianificazione di rilascio standard. Per ulteriori informazioni sulle funzioni più recenti, consulta [Attività di rilascio di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Miglioramenti di Pianificazione di Workfront

Nuove funzioni di Pianificazione di Workfront sono disponibili nell’ambiente di Produzione. Per ulteriori informazioni sulle funzioni più recenti, consulta [Attività di rilascio del primo trimestre 2026 per la Pianificazione di Adobe Workfront](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q1.md).

Al momento, in questa versione non sono presenti aggiornamenti per i seguenti elementi:

* Pianificazione scenari
* Bozza
* Obiettivi

## Aggiornamenti del visualizzatore di bozza desktop

### Versione 2.1.54

**Rilascio in produzione per tutti i clienti: 11 dicembre 2025**

Il Visualizzatore di bozza per desktop è stato aggiornato dalla versione 2.1.52 alla 2.1.54 e ha incluso aggiornamenti interni relativi agli strumenti, senza interessare le funzionalità dell’utente finale.

Anche la versione 2.1.53 ha incluso modifiche interne agli strumenti.

Questo aggiornamento è valido sia per Mac che per Windows.

### Versione 2.1.52

**Rilascio in produzione per tutti i clienti: 31 luglio 2025**

Il Visualizzatore di bozza per desktop è stato aggiornato alla versione 2.1.52, che risolve alcuni bug.

L’aggiornamento 2.1.51 ha incluso modifiche interne relative agli strumenti senza interessare le funzionalità dell’utente finale.

Questo aggiornamento è valido sia per Mac che per Windows.

## Annunci

### Versione 21 dell’API

La versione 21 dell’API di Workfront è stata rilasciata il 23 ottobre 2025. Nella versione 21 dell’API sono state modificate alcune risorse ed endpoint. Alcune delle modifiche supportano nuove funzionalità, mentre altre semplificano l’utilizzo delle informazioni disponibili tramite l’API.

>[!IMPORTANT]
>
>Questa modifica alla versione API comporta delle interruzioni e potrebbe interessare le chiamate API esistenti. Ciò è dovuto al fatto che la versione 21 dell’API utilizza la versione 2 delle sottoscrizioni eventi.
>
> Per i campi a selezione multipla, la versione 2 di Sottoscrizioni eventi invia sempre come array. La versione 1 inviava un array solo se venivano selezionati più valori. Se veniva selezionato un solo valore, veniva inviata una stringa.

Per informazioni sulle novità e sugli aggiornamenti, consulta [Novità della versione 21 dell’API](/help/quicksilver/wf-api/api/new-api-version-21.md).

Per informazioni sulle versioni API, consulta [Controllo delle versioni e pianificazione del supporto API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Nuova versione di Workfront per Microsoft Teams

Poiché [Microsoft sta eseguendo la transizione al nuovo client Teams](https://learn.microsoft.com/it-it/microsoftteams/teams-classic-client-end-of-availability), il client Teams classico non sarà più disponibile dopo il 1° luglio 2025. Per continuare a utilizzare Microsoft Teams e le app integrate come Workfront, è necessario effettuare la transizione al nuovo client Teams prima di tale data.

L’integrazione aggiornata di Workfront è ora disponibile e completamente compatibile con la nuova esperienza Teams. Nella maggior parte dei casi, Workfront verrà visualizzato automaticamente dopo la transizione degli utenti. In caso contrario, l’integrazione potrà essere installata manualmente dall’App Store di Microsoft Teams. Per installare o verificare l’integrazione di Workfront nel nuovo client Teams, consulta [Installare  [!DNL Adobe Workfront]  per Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

### Workfront per Microsoft Outlook

[Microsoft sta procedendo alla disabilitazione del supporto per i token legacy di Exchange Online](https://learn.microsoft.com/it-it/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), attualmente utilizzati dal componente aggiuntivo di Workfront per Outlook per l’autenticazione. Questa modifica di Microsoft sta già interessando i clienti a e continuerà ad essere introdotta in più fasi fino a ottobre 2025.

* **Dopo la completa disabilitazione di questi token da parte di Microsoft, l’integrazione di Workfront per Microsoft Outlook non funzionerà più.**

Come parte di questa modifica, Microsoft ha deciso di modificare il modo in cui i token possono essere riabilitati. Dopo il **30 giugno 2025**, gli amministratori non saranno più in grado di riabilitare i token personalmente. Solo il supporto Microsoft potrà concedere eccezioni. **Il 1° ottobre 2025, i token legacy verranno disattivati per tutti i tenant. Non verranno concesse eccezioni.**

### Altre transizioni all’integrazione di Workfront

Per garantire maggiore stabilità e scalabilità alle integrazioni, è stato adottato un approccio moderno e flessibile basato su Workfront Automation and Integration (Fusion). Nell’ambito di questo processo di transizione, le seguenti integrazioni non saranno disponibili dopo il **28 febbraio 2026**:

* Workfront per G Suite
* Workfront per Jira
* Workfront per Salesforce.

Per le esigenze di integrazione dell’organizzazione è consigliabile utilizzare Workfront Automation and Inegration con Google Workspace.
Per una panoramica di Workfront Automation and Integration consulta [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).


### Aggiornamenti di manutenzione di Workfront

Per informazioni sugli aggiornamenti di manutenzione effettuati durante il rilascio del primo trimestre 2025, consulta [Aggiornamenti di manutenzione di Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=it).

### Aggiornamenti della formazione

Esplora gli ultimi aggiornamenti apportati a programmi e percorsi di apprendimento, video e guide per ciascuna versione di Adobe Workfront. Per ulteriori informazioni, consulta la sezione “Novità” della [pagina dei tutorial di Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=it).
