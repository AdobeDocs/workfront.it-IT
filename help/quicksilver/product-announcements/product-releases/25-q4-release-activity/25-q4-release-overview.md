---
title: Panoramica sul rilascio del quarto trimestre 2025
description: Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del quarto trimestre 2025. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 298473d4-7d7d-4401-80bf-899a01f570a6
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '2245'
ht-degree: 39%

---

# Panoramica sul rilascio del quarto trimestre 2025

Questa pagina fornisce informazioni sulle funzionalità incluse nel rilascio del quarto trimestre 2025 pianificato per ottobre 2025.

I miglioramenti in questa pagina sono disponibili nell’ambiente di anteprima. Questa pagina verrà aggiornata con ulteriori miglioramenti man mano che il rilascio del quarto trimestre 2025 si avvicina al rilascio pianificato in produzione.


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
>| <ul><li>25.8 (14 agosto 2025)</li><li>25.9 (11 settembre 2025)</li><li>25.10 (16 ottobre 2025)</li></ul> | <ul><li>25.10 (16 ottobre 2025)</li></ul> |
>
>Tieni presente che per il rilascio finale di ogni trimestre (25.10 questo trimestre), gli utenti che seguono la pianificazione del rilascio rapido riceveranno il rilascio con un giorno di anticipo (giovedì 15 ottobre 2025).
>
>Per ulteriori informazioni sul processo di rilascio rapido, consulta [Abilitare o disabilitare il processo di rilascio rapido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Miglioramenti in Adobe Workfront

* [Miglioramenti per gli amministratori](#administrator-enhancements)
* [Miglioramenti alle dashboard](#dashboards)
* [Miglioramenti di documenti e bozze](#document-and-proofing-enhancements)
* [Miglioramenti alla Home](#home-enhancements)
* [Miglioramenti ai progetti](#project-enhancements)
* [Miglioramenti alla gestione delle risorse](#resource-management-enhancements)
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
        <td><strong>Ogni trimestre</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> Conferma durante la rimozione di un modulo personalizzato da un oggetto</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>Per garantire il mantenimento dell’accesso ai dati necessari, è stata aggiunta una finestra di dialogo di conferma durante la rimozione di un modulo personalizzato da un oggetto. Se si rimuove un modulo personalizzato da un oggetto, i dati contenuti in tale modulo vengono rimossi definitivamente dall’oggetto. Ora, la finestra di dialogo ti consente di confermare che comprendi che questi dati verranno rimossi, assicurandoti di non rimuovere i dati necessari. </p>
        </td>
        <td>giovedì 24 settembre 2025</td>
        <td>25 settembre 2025</td>
        <td>25 settembre 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Visualizzazione amministrazione nuove bacheche</a><p></p>
            <p>La Vista di amministrazione delle bacheche contiene un elenco di tutte le bacheche nel tuo account che gli amministratori di sistema possono utilizzare per ottenere un’istantanea rapida dei dettagli complessivi delle bacheche, tra cui quando sono state aggiornate l’ultima volta, quante schede ciascuna e altro ancora.</p>
        </td>
        <td>11 settembre 2025</td>
        <td>giovedì 15 ottobre 2025</td>
        <td>venerdì 16 ottobre 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Abilitare le funzionalità di AI Beta per la tua organizzazione</a><p></p>
            <p>Per semplificarti la visualizzazione e l’influenza delle prossime funzioni di intelligenza artificiale, ti abbiamo reso possibile abilitare i Beta per tali funzioni per la tua organizzazione. Ora puoi scegliere di abilitare una o più delle funzioni di AI Beta attualmente disponibili nelle Preferenze di sistema.</p>
        </td>
        <td>venerdì 28 agosto 2025</td>
        <td>11 settembre 2025</td>
        <td>venerdì 16 ottobre 2025</td>
    </tr>     
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti al profilo utente di Workfront</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>Il profilo utente di Workfront è stato aggiornato a un design moderno, coerente con le altre aree di Workfront. Questi aggiornamenti si applicano sia a un amministratore che modifica un singolo profilo o che modifica in blocco più profili, sia a un utente che modifica il proprio profilo.</p>
            <p>Esistono alcune piccole differenze di funzionalità rispetto al profilo utente corrente, tra cui:</p>
            <ul>
                <li>Alcune caselle di controllo, ad esempio per contrassegnare l'utente come attivo, sono state modificate in interruttori o pulsanti.</li>
                <li>L'opzione "Invia lavoro assegnato a me stesso alla scheda Lavori in corso" in Preferenze è stata rinominata "Imposta automaticamente lo stato dell'attività su In corso quando le attività vengono assegnate autonomamente" per rispecchiare lo scopo.</li>
            </ul>
        </td>
        <td>venerdì 28 agosto 2025</td>
        <td>Rollout graduale a partire dal 25 settembre 2025</td>
        <td>Rollout graduale a partire dal 25 settembre 2025</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Aggiungere più opzioni di valore da un'API esterna a un modulo personalizzato</a><p></p>
            <p>In Progettazione moduli personalizzati è ora disponibile un nuovo tipo di campo, Ricerca esterna a selezione multipla. Quando i dati sono memorizzati su un sistema esterno, questo tipo di campo ti consente di caricare opzioni da un’API esterna e di filtrare in base ad altri valori di campo nel modulo personalizzato. È lo stesso di una ricerca esterna a selezione singola.</p>
            <p>Quando il modulo viene aggiunto a un oggetto, i valori restituiti dall’API vengono visualizzati in un campo a discesa e l’utente può selezionare più valori.</p>
        </td>
        <td>venerdì 31 luglio 2025</td>
        <td>venerdì 14 agosto 2025</td>
        <td>venerdì 16 ottobre 2025</td>
    </tr>     
  </tbody>
</table>

### Miglioramenti alle dashboard

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funzione</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Ogni trimestre</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-dashboards.md" class="MCXref xref" xrefformat="{para}">Nuove dashboard Canvas aperte versione beta</a>
            <p>La nuova funzione delle dashboard di Canvas consente di visualizzare facilmente i dati di Adobe Workfront aggiungendo tipi di rapporto a un’area di lavoro che offre diverse opzioni di layout flessibili, tra cui ridimensionamento, trascinamento e rilascio di e altro ancora.</p>
        </td>
        <td>mercoledì 26 agosto 2025</td>
        <td>mercoledì 26 agosto 2025</td>
        <td>mercoledì 26 agosto 2025</td>
    </tr> 
</table>

### Miglioramenti di documenti e bozze

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funzione</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Ogni trimestre</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-document-and-proof.md" class="MCXref xref" xrefformat="{para}">Rollout Graduale Delle Approvazioni Unificate</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>Stiamo attivando le approvazioni unificate, precedentemente note come nuove approvazioni dei documenti, in un rollout graduale. Questa funzionalità verrà abilitata automaticamente nell’istanza di Workfront nei prossimi sei mesi.</p>
            <p>Le approvazioni unificate sostituiscono le approvazioni di documenti legacy e forniscono la nuova funzionalità. 
</p>
        </td>
        <td>Rollout graduale a partire dal 17 luglio 2025</td>
        <td>Rollout graduale a partire dal 17 luglio 2025</td>
        <td>Rollout graduale a partire dal 17 luglio 2025</td>
    </tr> 
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-document-and-proof.md" class="MCXref xref" xrefformat="{para}">Nuovo revisore di Workfront AI</a><p></p>
            <p>Nota: questa funzione è attualmente in versione beta.</p>
            <p>Il nuovo Workfront AI Reviewer garantisce la conformità del brand dell’immagine rivedendo automaticamente i contenuti in base alle linee guida del brand, a partire dalle linee guida per le immagini. Fornisce un punteggio e un feedback fruibile per semplificare il processo di approvazione. </p>
            <p>Puoi aggiungere il revisore IA ai modelli di approvazione o alle singole richieste di revisione e approvazione, consentendo una produzione di contenuti più rapida e mantenendo al contempo gli standard del marchio.</p>
        </td>
        <td>venerdì 14 agosto 2025</td>
        <td>venerdì 14 agosto 2025</td>
        <td>venerdì 14 agosto 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-document-and-proof.md" class="MCXref xref" xrefformat="{para}">Nuova integrazione di verifica per Adobe Express</a><p></p>
            <p>Siamo entusiasti di annunciare una nuova integrazione tra Adobe Express e Workfront Proof.</p>
            <ul>
            <li>Semplificazione della collaborazione tra team creativi, legali e di conformità per ridurre i tempi di pubblicazione, mantenendo al contempo la supervisione</li>
            <li>Eseguire revisioni approfondite utilizzando le annotazioni di disegno, le annotazioni e i commenti con il visualizzatore di bozze di Workfront</li>
            <li>Conformità agli standard di conformità aziendale con firme elettroniche e registri di audit completi</li>
            <li>Richiedi approvazione per tutti i file remixati da un modello con marchio Express</li>
            <li>Mappare un modello Express a un flusso di lavoro di revisione e approvazione in più fasi utilizzando modelli di bozza avanzati</li>
            </ul>
        </td>
        <td>martedì 28 luglio 2025</td>
        <td>martedì 28 luglio 2025</td>
        <td>martedì 28 luglio 2025</td>
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
        <td><strong>Ogni trimestre</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-home.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti al widget Richieste personali nella Home</a><p></p>
            <p>Per creare un'esperienza più fluida tra Workfront e Workfront Planning, abbiamo riprogettato il widget Richieste personali in Home. Il nuovo widget presenta le seguenti modifiche:
            <ul>
                <li>Miglioramento del layout e dell'organizzazione delle informazioni sulle richieste</li>
                <li>Opzioni di filtro e ordinamento migliorate</li>
                <li>Integrazione con Workfront Planning per una migliore visibilità nell’allocazione delle risorse</li>
            </ul>
            </p>
            <p>Il nuovo widget Richieste personali visualizza solo le richieste create nella nuova esperienza di richiesta.</p>
        </td>
        <td>venerdì 21 agosto 2025</td>
        <td>11 settembre 2025</td>
        <td>venerdì 16 ottobre 2025</td>
    </tr>     
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
        <td><strong>Ogni trimestre</strong></td>
    </tr>
      <!--
      <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}">Create project intake forms in Workfront</a>
            <p>To make it easier to create requested projects without converting from issues, we've created Project intake forms. You can configure these intake forms with specific fields, templates, and custom forms, and set approvers for project creation. Then, when a user uses this form, the project is configured to your specifications and sent for approval.</p>
        </td>
        <td>August 21, 2025</td>
        <td>September 11, 2025</td>
        <td>October 16, 2025</td>
    </tr>
    -->
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}">Nuova versione beta per l'integrità del progetto</a>
            <p>La nuova funzione Project Health utilizza la potenza di AI Assistant per fornire immediatamente una valutazione delle prestazioni dei progetti e delle aree che richiedono la tua attenzione.</p>
            <p>L’Assistente AI può generare una valutazione dello stato del progetto per un progetto, un programma e più progetti.</p>
        </td>
        <td>11 settembre 2025</td>
        <td>11 settembre 2025</td>
        <td>11 settembre 2025</td>
    </tr> 
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}">Nuove espressioni aggiunte ai campi formula in Planning e campi personalizzati calcolati in Workfront</a><p><p>[!BADGE Off schedule]{type=Neutral}</p></p>
            <p>Sono state aggiunte nuove espressioni con il seguente utilizzo ai campi formula in Workfront Planning e ai campi personalizzati calcolati in Workfront:</p>
            <ul>
            <li>REMOVEACCENTS(string): rimuove i segni diacritici da tutti i caratteri accentati nella stringa di input.</li>
            <li>REPLACEPATTERN(string, pattern, replace string): sostituisce le corrispondenze del pattern specificato con la stringa di sostituzione.</li>
            <li>PASCAL(string): converte la stringa di input in PascalCase digitando la prima lettera di ogni parola e rimuovendo tutti gli spazi.</li>
            </ul>
        </td>
        <td>venerdì 7 agosto 2025</td>
        <td>venerdì 7 agosto 2025</td>
        <td>venerdì 7 agosto 2025</td>
    </tr> 
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}">Modo aggiuntivo per accedere alle assegnazioni avanzate dagli elenchi</a><p></p>
            <p>È ora disponibile un pulsante <b>Avanzate</b> per le assegnazioni negli elenchi, che consente di accedere più rapidamente alla pagina Assegnazioni avanzate. L'icona <b>Persone</b> per accedere alle assegnazioni avanzate è disponibile anche nelle assegnazioni negli elenchi.</p>
        </td>
        <td>venerdì 7 agosto 2025</td>
        <td>11 settembre 2025</td>
        <td>venerdì 16 ottobre 2025</td>
    </tr> 
  </tbody>
  </table>

### Miglioramenti alla gestione delle risorse

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funzione</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Ogni trimestre</strong></td>
    </tr>
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-resource-mgmt.md" class="MCXref xref" xrefformat="{para}">Il Bilanciatore dei carichi di lavoro è ora disponibile nel tuo profilo utente</a><p></p>
            <p>Ora tutti gli utenti possono visualizzare i propri dati sulla domanda e sulla capacità nel Bilanciatore dei carichi di lavoro dal proprio profilo, indipendentemente dal loro livello di accesso. Quando accedi al profilo utente di Workfront, nel pannello di navigazione a sinistra viene visualizzato il Bilanciatore dei carichi di lavoro.</p>
            <p>I dati del Bilanciatore dei carichi di lavoro per un utente sono di sola lettura. Non è possibile assegnare lavoro, annullare l'assegnazione del lavoro o adeguare le allocazioni a livello di utente.</p>
        </td>
        <td>venerdì 31 luglio 2025</td>
        <td>venerdì 14 agosto 2025</td>
        <td>venerdì 16 ottobre 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-resource-mgmt.md" class="MCXref xref" xrefformat="{para}">Le assegnazioni dei ruoli vengono visualizzate nel Bilanciatore dei carichi di lavoro </a><p></p>
            <p>I responsabili delle risorse possono ora rivedere le assegnazioni dei ruoli nel Bilanciatore dei carichi di lavoro. Le assegnazioni vengono visualizzate nell’area Lavoro non assegnato, sotto le attività o i problemi a cui sono assegnati i ruoli. Nell'area Lavoro assegnato vengono visualizzati solo gli elementi di lavoro assegnati agli utenti. </p>
            <p>Una nuova impostazione del Bilanciatore dei carichi di lavoro, Mostra assegnazioni di ruolo, determina se visualizzare o meno le assegnazioni di ruolo. L'impostazione è attivata per impostazione predefinita.</p>
        </td>
        <td>venerdì 31 luglio 2025</td>
        <td>venerdì 14 agosto 2025</td>
        <td>venerdì 16 ottobre 2025</td>
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
        <td><strong>Ogni trimestre</strong></td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-requests.md" class="MCXref xref" xrefformat="{para}">Creare e salvare le visualizzazioni nell'area Richieste</a><p></p>
            <p>Per visualizzare più facilmente le informazioni necessarie, è stata aggiunta la possibilità di creare e salvare viste nell’area Richieste. Ora puoi salvare una vista, inclusi i filtri e le configurazioni di colonna, e passare da una vista all’altra. Un amministratore di Workfront può aggiungere la nuova visualizzazione ai modelli di layout.</p>
        </td>
        <td>venerdì 2 ottobre 2025</td>
        <td>giovedì 15 ottobre 2025</td>
        <td>venerdì 16 ottobre 2025</td>
    </tr> 
    <!--
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-requests.md" class="MCXref xref" xrefformat="{para}">New combined Status column in unified Request list</a><p></p>
            <p>To simplify the unified request experience, the Status column now displays both Request Status and Approval Status, whichever applies to a given request.</p>
        </td>
        <td>August 28, 2025</td>
        <td>September 11, 2025</td>
        <td>October 16, 2025</td>
    </tr>
    -->
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-requests.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti all'esperienza richiedente</a><p></p>
            <p>Per migliorare l’esperienza utente nell’esecuzione delle richieste in Workfront e Workfront Planning, è stata aggiornata la sezione delle richieste. Ora è possibile:
            <ul>
                <li>Visualizzare le richieste di Workfront e Workfront Planning in un unico elenco.</li>
                <li>Filtra le richieste inviate in base ai criteri specificati.</li>
                <li>Cerca e seleziona le code di richieste di Workfront e i moduli di Workfront Planning in un’esperienza consolidata.</li>
                <li>Nascondi e riordina le colonne nell’elenco delle richieste inviate.</li>
            </ul>
            </p>
        </td>
        <td>venerdì 21 agosto 2025</td>
        <td>11 settembre 2025</td>
        <td>venerdì 16 ottobre 2025</td>
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
        <td><strong>Ogni trimestre</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-other.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience ora disponibile per altre organizzazioni Workfront</a><p></p>
            <p>Per consentire alle organizzazioni di accedere ai vantaggi di Adobe Unified Experience, la disponibilità è stata estesa per i clienti esistenti di Workfront.</p><p><span style="color: #ff0000;">L'esperienza unificata di Adobe viene resa disponibile in un rollout graduale.</span> </p>
        </td>
        <td><p>11 settembre 2025</p><p>Oppure</p><p>venerdì 11 dicembre 2025</p></td>
        <td><p>venerdì 16 ottobre 2025</p><p>Oppure</p><p>venerdì 15 gennaio 2026</p></td>
        <td><p>venerdì 16 ottobre 2025</p><p>Oppure</p><p>venerdì 15 gennaio 2026</p></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-other.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti agli elenchi avanzati</a><p></p>
            <p>Con il layout avanzato degli elenchi, puoi utilizzare filtri e raggruppamenti per visualizzare i tuoi lavori e mantenerli meglio organizzati. Ora viene visualizzato un indicatore a punti blu sopra un widget per comunicare quando un filtro o un raggruppamento è stato applicato a un elenco nelle seguenti aree:</p>
            <ul>
                <li>Widget Richieste personali</li>
                <li>Priorità</li>
            </ul>
        </td>
        <td>venerdì 28 agosto 2025</td>
        <td>11 settembre 2025</td>
        <td>venerdì 16 ottobre 2025</td>
    </tr>     
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti look-and-feel durante il periodo di rilascio della versione del quarto trimestre 2025</a></p>
                        <p>Aggiornamenti minori al look and feel di varie aree dell’applicazione Adobe Workfront vengono effettuati entro l’arco temporale del rilascio del quarto trimestre 2025. </p>
                    </td>
                    <td><p>Nell’arco temporale di rilascio del quarto trimestre 2025<br /></p>
                    <td colspan="2"><p>Rilascio rapido: almeno 1 settimana dopo il rilascio in anteprima (se non diversamente specificato)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

<!--
### Functionality soon to be removed from Workfront

* 
-->

## Modernizzazione dell’interfaccia

L’interfaccia di Adobe Workfront è in fase di aggiornamento per migliorare l’esperienza utente e per uniformarla alle altre applicazioni Adobe. Queste modifiche vengono rilasciate al di fuori della pianificazione di rilascio standard. Per un elenco di queste modifiche, consulta [Modernizzazione dell’interfaccia](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

## Note sulla versione per altre aree

### Miglioramenti di Workfront Fusion

Le nuove funzioni di Workfront Fusion sono disponibili nell’ambiente di Produzione con una cadenza al di fuori della pianificazione di rilascio standard. Per ulteriori informazioni sulle funzioni più recenti, consulta [Attività di rilascio di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Miglioramenti di Pianificazione di Workfront

Nuove funzioni di Pianificazione di Workfront sono disponibili nell’ambiente di Produzione. Per ulteriori informazioni sulle funzioni più recenti, consulta [Attività sulla versione del quarto trimestre 2025 per Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q4.md).

Al momento, in questa versione non sono presenti aggiornamenti per i seguenti elementi:

* Pianificazione scenari
* Bozza
* Obiettivi

## Aggiornamenti del visualizzatore di bozza desktop

### Versione 2.1.52

**Rilascio in produzione per tutti i clienti: 31 luglio 2025**

Il Visualizzatore di bozza per desktop è stato aggiornato alla versione 2.1.52, che risolve alcuni bug.

L’aggiornamento 2.1.51 ha incluso modifiche interne relative agli strumenti senza interessare le funzionalità dell’utente finale.

Questo aggiornamento è valido sia per Mac che per Windows.

## Annunci

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

### Versione 20 dell’API

La versione 20 dell’API di Workfront è stata rilasciata il lunedì 4 maggio 2025. Nella versione 20 dell’API sono state modificate alcune risorse ed endpoint. Alcune delle modifiche supportano nuove funzionalità, mentre altre semplificano l’utilizzo delle informazioni disponibili tramite l’API.

Per informazioni sulle novità e sugli aggiornamenti, consulta [Novità della versione 20 dell’API](/help/quicksilver/wf-api/api/new-api-version-19.md).

Per informazioni sulle versioni API, consulta [Controllo delle versioni e pianificazione del supporto API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Aggiornamenti di manutenzione per Workfront

Per informazioni sugli aggiornamenti di manutenzione effettuati durante il rilascio del primo trimestre 2025, consulta [Aggiornamenti di manutenzione di Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=it).

### Aggiornamenti della formazione

Esplora gli ultimi aggiornamenti apportati a programmi e percorsi di apprendimento, video e guide per ciascuna versione di Adobe Workfront. Per ulteriori informazioni, consulta la sezione “Novità” della [pagina dei tutorial di Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=it).
