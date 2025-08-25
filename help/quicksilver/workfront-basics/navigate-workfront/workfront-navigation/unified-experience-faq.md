---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Domande frequenti sull’esperienza unificata in Adobe
description: Alcune funzionalità sono diverse tra  [!DNL Workfront]  e Adobe Experience Cloud e potresti avere alcune domande durante la migrazione dell'istanza  [!DNL Workfront]  all'esperienza unificata.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: f381b37e6d4537e6f83e55ed4a2f4ff7f868dd54
workflow-type: tm+mt
source-wordcount: '1419'
ht-degree: 0%

---

# Domande frequenti su [!DNL Adobe Unified Experience]

>[!IMPORTANT]
>
>Poiché tutte le organizzazioni Workfront sono state migrate a Adobe Admin Console, questo articolo verrà rimosso nel prossimo futuro.

<!--DELETE ME MARCH 2026-->

[!DNL Adobe Unified Experience] per [!DNL Workfront] consente di gestire tutte le applicazioni di [!DNL Adobe] in un&#39;unica posizione con un unico accesso. L&#39;area di navigazione [!DNL Adobe] è integrata direttamente con [!DNL Workfront]. Alcune funzionalità sono diverse e potresti avere alcune domande quando la tua istanza di [!DNL Workfront] verrà migrata all&#39;esperienza unificata.

Per informazioni su come accedere a [!DNL Adobe Unified Experience], vedere [[!DNL Adobe Unified Experience] per [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Confronto tra l&#39;esperienza [!DNL Adobe Unified Experience] e [!DNL Workfront only]

Solo i clienti che utilizzano [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] possono accedere a [!DNL Adobe Unified Experience]. I clienti che non hanno ancora eseguito la migrazione vedranno l&#39;esperienza [!DNL Workfront only], senza la possibilità di passare da un&#39;applicazione all&#39;altra [!DNL Adobe].

Questa tabella descrive alcune funzioni che differiscono tra le due esperienze.

| [!DNL Adobe Unified Experience] | Solo esperienza [!DNL Workfront] |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Menu principale] a sinistra ![Menu principale](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Menu principale] a destra ![Menu principale](assets/main-menu-icon.png) |
| Un singolo URL di accesso è disponibile per tutte le applicazioni [!DNL Adobe Experience Cloud] | Accedi a [!DNL Workfront] con un URL [!DNL Workfront] personalizzato |
| Un &quot;cambio organizzazione&quot; consente di spostarsi tra [!DNL Workfront] organizzazioni e ambienti | Il &quot;selettore organizzazione&quot; non è disponibile |
| La navigazione include un&#39;area di navigazione di primo livello per i prodotti [!DNL Adobe], le notifiche [!DNL Adobe], la guida e il profilo utente, oltre alla barra di navigazione [!DNL Workfront] | La navigazione include solo la barra di navigazione [!DNL Workfront] |
| La Guida è accessibile tramite il [!UICONTROL menu principale] e l&#39;area di navigazione superiore | La Guida è accessibile tramite il [!UICONTROL menu principale] e la barra di navigazione [!DNL Workfront] |
| Il visualizzatore di bozze si apre in una nuova scheda | Il visualizzatore di bozze si apre in Workfront |
| URL utilizzato per accedere a Workfront: `experience.adobe.com` | URL utilizzato per accedere a Workfront: `(CompanyName).my.workfront.com` |
| Il formato della data (ad esempio GG/MM/AAAA) si basa sulle impostazioni della lingua Unified Experience. Se l&#39;utente non ha aggiornato le impostazioni della lingua, verranno utilizzate `en-US` impostazioni. | Il formato della data (ad esempio GG/MM/AAAA) si basa sulle preferenze del browser |

{style="table-layout:auto"}

## Domande frequenti

### Come posso determinare se utilizzo Adobe Unified Experience o Adobe Workfront?

Per determinare se la tua organizzazione utilizza l’esperienza unificata di Adobe, esamina l’URL utilizzato per accedere a Workfront.

| URL | Esperienza Adobe |
|------------|------------|
| (NomeSocietà).my.workfront.com | Esperienza Workfront |
| experience.adobe.com | Esperienza unificata Adobe |

### Come posso saperne di più su [!DNL Adobe Admin Console]?

Per informazioni su [!DNL Admin Console], esaminare gli articoli seguenti:

* [Prepara per  [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Differenze di amministrazione basate su piattaforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] panoramica](https://helpx.adobe.com/it/enterprise/using/admin-console.html)

### Cosa devo fare in qualità di cliente per facilitare la migrazione?

I clienti esistenti verranno contattati per pianificare le migrazioni. I colleghi del team di supporto per la migrazione assisteranno i clienti durante il processo, forniranno consigli sulla configurazione di [!DNL Admin Console] e forniranno i collegamenti alla documentazione necessaria per rendere la migrazione il più semplice e semplice possibile.

* [[!DNL Adobe Workfront] Panoramica del supporto](https://experienceleague.adobe.com/it/docs/customer-one/using/workfront/overview)
* [[!DNL Workfront Admin Console] informazioni](https://experienceleague.adobe.com/it/docs/customer-one/using/workfront/landing)
* [[!DNL Adobe Business Platform] e [!DNL Admin Console] Domande frequenti](https://experienceleague.adobe.com/it/docs/customer-one/using/workfront/faq)

### In che modo gestisci [!DNL Adobe Admin Console] per le aziende che hanno già abilitato questo per i Federated ID in modo diverso rispetto a [!DNL Workfront] SSO configurato?

[!DNL Adobe Admin Console] può includere [!DNL Workfront], sostituendo SSO con Adobe Identity Management System (IMS). Tutti i provisioning degli utenti si verificano in [!DNL Admin Console] e gli utenti visualizzeranno la schermata di accesso di [!DNL Adobe] per accedere a [!DNL Experience Cloud], dove vedranno [!DNL Workfront] come opzione (se dispongono dell&#39;accesso consentito).

### Che impatto ha questo sui clienti che dispongono già del pannello di amministrazione di AEM per [!DNL Adobe Assets], ma l&#39;SSO è configurato in modo diverso rispetto a [!DNL Workfront?]

Una volta aggiunto [!DNL Workfront] come applicazione [!DNL Admin Console], non è necessario eseguire altre operazioni per [!DNL Workfront] per sfruttare la configurazione SSO esistente per [!DNL Adobe Assets].

### In che modo questo influisce su quelli configurati con SSO?

SSO è configurato in [!DNL Admin Console] ed ereditato dall&#39;applicazione [!DNL Workfront].

### SSO con [!DNL Active Directory] interno sarà ancora un&#39;opzione con Adobe Identity Management System (IMS)?

IMS sostituisce l’SSO e funziona per lo più allo stesso modo. Tutte le autorizzazioni utente sono concesse e predisposte in [!DNL Adobe Admin Console] e l&#39;utente visualizzerà la schermata di accesso [!DNL Adobe] in cui potrà scegliere &quot;[!UICONTROL Account personale]&quot; o &quot;[!UICONTROL Account società]&quot; per effettuare l&#39;accesso (se si dispone di [!DNL Active Directory], la maggior parte effettuerà l&#39;accesso con un account società).

### Per gli utenti che non utilizzano SSO, l&#39;URL di accesso di [!DNL Workfront] cambia?

L’URL di accesso cambierà; tuttavia, il vecchio URL verrà reindirizzato al nuovo URL di accesso, pertanto devi istruire nuovamente gli utenti su dove andare.

### Gli alias configurati funzioneranno ancora o i collegamenti [!DNL Workfront] cambieranno con questa migrazione?

[!DNL Workfront] reindirizzamenti/alias sono disponibili per accedere alla home page.

### Può accadere che i reindirizzamenti siano disabilitati? Oppure sarà sempre possibile digitare in my.company.workfront.com?

Puoi sempre utilizzare qualsiasi URL personalizzato. Dopo aver fatto clic su uno di questi collegamenti, verrà indirizzato a [!DNL Workfront] e verrà visualizzato un URL diverso. Tuttavia, è preferibile [!DNL experience] per accedere a experience.adobe.com e aggiungere ai segnalibri i collegamenti dall&#39;interno di [!DNL Experience Cloud]. Un minor reindirizzamento equivale a un minor ritardo/tempo di caricamento.

### I collegamenti diretti alle code di richieste verranno interrotti?

Tutti i collegamenti diretti devono essere reindirizzati ai nuovi pattern URL. Tuttavia, se hai distribuito i collegamenti alle persone, devi inviare un aggiornamento per sfruttare il collegamento diretto e evitare ritardi nel raggiungere la pagina prevista.

### Effettueremo la migrazione a [!DNL Experience Cloud] a livello globale o possiamo selezionare alcuni utenti (non tutti i nostri utenti utilizzano anche altri prodotti Adobe)?

Verrà eseguita la migrazione dell&#39;intero account del cliente [!DNL Workfront]. Non può essere fatto utente per utente.

### Tutti gli utenti [!DNL Workfront] dovranno accedere tramite [!DNL Experience Cloud]? O solo amministratori?

Sì, tutti gli utenti accederanno tramite [!DNL Experience Cloud]. L’accesso a Adobe Identity Management System (IMS) sostituirà l’SSO. È un’esperienza molto simile, ma con una schermata di accesso diversa.

### Gli utenti dovranno collegare i loro account [!DNL Adobe] ai loro account [!DNL Workfront] se hanno già entrambi?

Sì, esiste una procedura per questo e verranno forniti ulteriori dettagli quando è il momento per la tua organizzazione di passare a IMS.

### Cosa succederà agli utenti [!DNL Workfront] che non hanno un account [!DNL Adobe]?

Gli utenti a cui non è stato concesso l&#39;accesso in [!DNL Adobe Admin Console] per accedere a [!DNL Workfront] devono creare un account &quot;[!UICONTROL personal]&quot; o un account ID [!DNL Adobe] per poter accedere. Questo invia un messaggio e-mail all’amministratore per approvare o rifiutare la richiesta, e consente inoltre all’amministratore di configurare il tipo di accesso di cui dispone l’utente. Al momento dell&#39;accesso, l&#39;utente visiterà il sito experience.adobe.com, immetterà il proprio indirizzo e-mail e sceglierà [!UICONTROL Account personale]. Da lì potranno accedere a [!DNL Workfront].

### Cosa succede se non abbiamo [!DNL Adobe] prodotti diversi da [!DNL Workfront?]

È comunque consigliabile eseguire la migrazione dell&#39;organizzazione a [!DNL Adobe Unified Experience]. Riceverai un ID [!DNL Adobe] insieme ai vantaggi elencati sopra.

### Nella nostra istanza [!DNL Workfront] sono inclusi utenti esterni. Non vogliamo che abbiano accesso ad altri prodotti inclusi in [!DNL Adobe]. In che modo limiteremmo il loro accesso all’interno della console?

[!DNL Admin Console] offre agli amministratori un notevole controllo su ciò a cui gli utenti possono e non possono accedere. Ogni volta che un utente esterno desidera accedere, deve creare un ID [!DNL Adobe], che invia un&#39;e-mail all&#39;amministratore. L’amministratore può quindi accettare o rifiutare l’accesso a un prodotto e definire a cosa può/non può accedere per i prodotti di proprietà di tale organizzazione. L&#39;amministratore di sistema [!DNL Workfront] può quindi accedere all&#39;area [!UICONTROL Utenti] di [!DNL Workfront] per concedere ulteriori autorizzazioni granulari all&#39;utente esterno.

### Gli amministratori di gruppi vengono utilizzati per creare persone in [!DNL Workfront]. Con il passaggio a [!DNL Experience Cloud], gli amministratori di gruppo saranno ancora in grado di creare persone?

Sì, la creazione dell&#39;utente è ancora possibile tramite [!DNL Workfront]. Questi utenti possono essere aggiunti automaticamente a [!DNL Experience Cloud]. Puoi anche impostare gli amministratori di gruppo come proprietari del prodotto in [!DNL Admin Console] per consentire loro di assegnare [!DNL Workfront] agli utenti.

### Qual è la scadenza per passare a [!DNL Experience Cloud]?

Nessuna scadenza per lo spostamento a [!DNL Adobe Experience Cloud]. Stiamo lavorando con i clienti per consentire loro di scegliere quando sono pronti per la migrazione.

### Il nostro team di supporto dovrà fare qualcosa per questo cambiamento?

Se il team di supporto è responsabile della creazione di nuovi utenti, dovrà familiarizzare con le interfacce [!DNL Admin Console] utilizzate per la creazione degli utenti e assegnare un diritto a Workfront. In caso contrario, è probabile che non vi siano modifiche significative per il team di supporto interno.

### In che modo questo influisce sulle integrazioni disponibili tramite la funzione API?

Il percorso URL esistente continuerà a essere disponibile per il traffico API. Non dovrebbe essere necessario eseguire alcuna operazione per aggiornare gli endpoint nelle integrazioni. Tuttavia, l&#39;accesso diretto tramite nome utente e password non sarà supportato. È necessario utilizzare una chiave API, ad eccezione dei connettori [!DNL Workfront Fusion].

### E gli utenti [!DNL Creative Cloud]? Quali sono gli effetti della migrazione su di loro? Ci sono dei vantaggi per loro?

Nessun impatto per [!DNL Creative Cloud] utenti con la migrazione a [!DNL Adobe Unified Experience].

### Gli accessi cambieranno per [!DNL Workfront] utenti di dispositivi mobili?

[!DNL Workfront] utenti di dispositivi mobili non dovrebbero essere interessati dalla migrazione a [!DNL Adobe Unified Experience].

### JumpSeat non funziona con [!DNL Adobe Unified Experience]. Come posso risolvere il problema?

JumpSeat funziona con [!DNL Adobe Unified Experience], ma richiede un aggiornamento della configurazione. Utilizzando il pannello di amministrazione JumpSeat, modifica l&#39;URL dell&#39;applicazione da `workfront.com` in modo che termini con `.workfront.adobe.com`
