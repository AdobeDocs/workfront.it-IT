---
title: Panoramica sulla versione del quarto trimestre 2025
description: Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del quarto trimestre 2025. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 298473d4-7d7d-4401-80bf-899a01f570a6
source-git-commit: eafc56adab1fad3bbc1a4f3dc8f61e599ab21f57
workflow-type: tm+mt
source-wordcount: '1190'
ht-degree: 2%

---

# Panoramica sulla versione del quarto trimestre 2025

Questa pagina fornisce informazioni sulle funzionalità incluse nel rilascio del quarto trimestre 2025 pianificato per ottobre 2025.

I miglioramenti in questa pagina sono disponibili nell’ambiente di anteprima. Questa pagina verrà aggiornata con ulteriori miglioramenti man mano che il rilascio del quarto trimestre 2025 si avvicina al rilascio pianificato in produzione.


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>Salvo diversa indicazione, i rilasci mensili e trimestrali dovrebbero essere disponibili il giovedì della seconda settimana completa del mese.
>
>| Versione mensile | Versione trimestrale |
>|----|----|
>| <ul><li>25.8 (agosto 2025)</li><li>25.9 (settembre 2025)</li><li>25.10 (ottobre 2025)</li></ul> | <ul><li>25.10 (ottobre 2025)</li></ul> |
>
>Tieni presente che per la versione finale di ogni trimestre (le 25.10 di questo trimestre), gli utenti che rientrano nella pianificazione del rilascio rapido riceveranno la versione con un giorno di anticipo.
>
>Per ulteriori informazioni sul processo di rilascio rapido, vedere [Attivare o disattivare il processo di rilascio rapido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Miglioramenti di Adobe Workfront

* [Miglioramenti per gli amministratori](#administrator-enhancements)
* [Miglioramenti di documenti e bozze](#document-and-proofing-enhancements)
<!--* [Home enhancements](#home-enhancements)
* [Requests enhancements](#requests-enhancements)-->
* [Miglioramenti alla gestione delle risorse](#resource-management-enhancements)
* [Altri miglioramenti](#other-enhancements)

### Miglioramenti per gli amministratori

<table style="table-layout:auto">
  <tbody>
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


### Miglioramenti di documenti e bozze

<table style="table-layout:auto">
  <tbody>
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

<!--### Home enhancements

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-home.md" class="MCXref xref" xrefformat="{para}">Updates to the My Requests widget in Home</a><p></p>
            <p>To create a more seamless experience between Workfront and Workfront Planning, we've redesigned the My Requests widget in Home. The new widget features the following changes:
            <ul>
                <li>Improved layout and organization of request information</li>
                <li>Enhanced filtering and sorting options</li>
                <li>Integration with Workfront Planning for better visibility into resource allocation</li>
            </ul>
            </p>
        </td>
        <td>July 31, 2025</td>
        <td>August 14, 2025</td>
        <td>October 16, 2025</td>
    </tr>     
  </tbody>
</table> 

### Requests enhancements

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-requests.md" class="MCXref xref" xrefformat="{para}">Updates to Requesting experience</a><p></p>
            <p>To create a better user experience when making requests in Workfront and Workfront Planning, we've updated the requesting experience. Now you can:
            <ul>
                <li>View Workfront and Workfront Planning requests in a single list.</li>
                <li>Filter submitted requests based on criteria you specify.</li>
                <li>Search for and select Workfront request queues and Workfront Planning forms in a consolidated experience.</li>
                <li>Hide and reorder columns in the submitted requests list.</li>
            </ul>
            </p>
        </td>
        <td>July 31, 2025</td>
        <td>August 14, 2025</td>
        <td>October 16, 2025</td>
    </tr>     
  </tbody>
</table> -->

### Miglioramenti alla gestione delle risorse

<table style="table-layout:auto">
  <tbody>
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

### Altri miglioramenti

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Funzionalità</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Date di rilascio</span>
                        </p>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti look-and-feel durante il periodo di rilascio della versione del quarto trimestre 2025</a></p>
                        <p>Aggiornamenti minori al look and feel di varie aree dell’applicazione Adobe Workfront vengono effettuati entro l’arco temporale del rilascio del quarto trimestre 2025. </p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: nell’arco temporale di rilascio del quarto trimestre 2025<br /></p>
                            </li>
                            <li>
                                <p>Versione di produzione: almeno 2 settimane dopo il rilascio in anteprima (se non diversamente specificato)</p>
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

## Modernizzazione dell&#39;interfaccia

Stiamo aggiornando l’interfaccia in Adobe Workfront per migliorare l’esperienza utente e per coerenza con altre applicazioni Adobe. Queste modifiche vengono rilasciate al di fuori della pianificazione standard. Per un elenco di queste modifiche, vedere [Modernizzazione interfaccia](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

## Note sulla versione per altre aree

### Miglioramenti apportati a Workfront Fusion

Le nuove funzioni di Workfront Fusion sono disponibili in produzione a una cadenza al di fuori della pianificazione di rilascio standard. Per ulteriori informazioni sulle funzionalità più recenti, vedere [Attività di Adobe Workfront Fusion release](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Miglioramenti di Workfront Planning

Le nuove funzioni di Workfront Planning sono disponibili in Produzione. Per ulteriori informazioni sulle funzioni più recenti, consulta [Attività sulla versione del quarto trimestre 2025 per Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q4.md).

A questo punto della versione non sono presenti aggiornamenti per i seguenti elementi:

* Pianificazione scenario
* Bozza
* Obiettivi

## Aggiornamenti del visualizzatore per la verifica del desktop

### Versione 2.1.52

**Versione di produzione per tutti i clienti: 31 luglio 2025**

Il Visualizzatore bozze per desktop è stato aggiornato alla versione 2.1.52, che risolve alcuni bug.

L’aggiornamento del 2.1.51 includeva aggiornamenti interni degli strumenti e non influiva sulle funzionalità dell’utente finale.

Questo aggiornamento è sia per Mac che per Windows.

## Notifiche

### Nuova versione di Workfront per Microsoft Teams

Poiché [Microsoft passa al client Nuovi team](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability), il client Team classici non sarà più disponibile dopo il 1° luglio 2025. Per continuare a utilizzare Microsoft Teams e le app integrate come Workfront, i clienti devono effettuare la transizione al client Nuovi team prima di tale data.

L’integrazione aggiornata di Workfront è ora disponibile e completamente compatibile con l’esperienza Nuovi team. Nella maggior parte dei casi, Workfront viene visualizzato automaticamente dopo la transizione degli utenti. In caso contrario, l’integrazione può essere installata manualmente dall’App Store di Microsoft Teams. Per installare o verificare l&#39;integrazione di Workfront nel client New Teams, vedere [Installa [!DNL Adobe Workfront] per Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

### Workfront per Microsoft Outlook

Microsoft [È in corso la disabilitazione del supporto per i token online di Exchange legacy](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), attualmente utilizzati dal componente aggiuntivo di Workfront Outlook per l&#39;autenticazione. Questa modifica di Microsoft ha già iniziato a interessare i clienti e continuerà a essere implementata in più fasi fino a ottobre 2025.

* **Dopo la completa disattivazione di questi token da parte di Microsoft, l&#39;integrazione di Workfront per Microsoft Outlook non funzionerà più.**

Come parte di questa modifica, Microsoft ha deciso di cambiare il modo in cui i token vengono riabilitati. Dopo il **30 giugno 2025**, gli amministratori non saranno più in grado di riabilitare i token personalmente. Solo il supporto Microsoft può concedere eccezioni. **Il 1° ottobre 2025, i token legacy verranno disattivati per tutti i tenant. Le eccezioni non verranno concesse.**

### Altre transizioni all&#39;integrazione di Workfront

Per offrire integrazioni più stabili e scalabili, stiamo passando a un approccio di integrazione moderno e flessibile che utilizza l’automazione e l’integrazione di Workfront (Fusion). Nell&#39;ambito di questo processo di transizione, le seguenti integrazioni non saranno disponibili dopo il **28 febbraio 2026**:

* Workfront per G Suite
* Workfront per Jira
* Workfront per Salesforce.

È consigliabile utilizzare l&#39;automazione e l&#39;integrazione di Workfront per le esigenze di integrazione dell&#39;organizzazione con Google Workspace.
Per una panoramica dell&#39;automazione e dell&#39;integrazione di Workfront, vedere [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).

### API versione 20

Workfront API versione 20 è stato rilasciato il 4 maggio 2025. Per API versione 20, abbiamo modificato alcune risorse ed endpoint. Alcune delle modifiche supportano nuove funzionalità, mentre altre semplificano l’utilizzo delle informazioni disponibili tramite l’API.

Per informazioni sulle novità e sugli aggiornamenti, vedere [Novità della versione API 20](/help/quicksilver/wf-api/api/new-api-version-19.md).

Per informazioni sulle versioni API, vedere [Controllo delle versioni e pianificazione del supporto API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Aggiornamenti di manutenzione per Workfront

Per informazioni sugli aggiornamenti di manutenzione effettuati durante la versione del primo trimestre 2025, vedi [Aggiornamenti di manutenzione di Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=it).

### Aggiornamenti dei corsi di formazione

Scopri gli ultimi aggiornamenti apportati a programmi di apprendimento, percorsi di apprendimento, video e guide per ogni versione di Adobe Workfront. Per ulteriori informazioni, vedere la sezione &quot;Novità&quot; della [pagina delle esercitazioni di Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=it).
