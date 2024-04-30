---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Adobe di esperienza unificata per le domande frequenti
description: Alcune funzioni sono diverse tra [!DNL Workfront] e Adobe Experience Cloud, e potresti avere alcune domande come [!DNL Workfront] l’istanza viene migrata all’esperienza unificata.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '1289'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] Domande frequenti

Il [!DNL Adobe Unified Experience] per [!DNL Workfront] consente di gestire tutte le [!DNL Adobe] applicazioni in un&#39;unica posizione con un unico login. Il [!DNL Adobe] l’area di navigazione è integrata perfettamente con [!DNL Workfront]. Alcune funzioni sono diverse e potresti avere alcune domande come [!DNL Workfront] l’istanza viene migrata all’esperienza unificata.

Per informazioni su come accedere a [!DNL Adobe Unified Experience], vedi [[!DNL Adobe Unified Experience] per [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Confronto tra [!DNL Adobe Unified Experience] e [!DNL Workfront only] esperienza

Solo i clienti che utilizzano [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] può accedere a [!DNL Adobe Unified Experience]. I clienti che non hanno ancora eseguito la migrazione visualizzeranno [!DNL Workfront only] senza la possibilità di passare da un [!DNL Adobe] applicazioni.

Questa tabella descrive alcune funzioni che differiscono tra le due esperienze.

| [!DNL Adobe Unified Experience] | [!DNL Workfront] solo esperienza |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Menu principale] è a sinistra ![Menu principale](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Menu principale] è a destra ![Menu principale](assets/main-menu-icon.png) |
| Un singolo URL di accesso è disponibile per tutti [!DNL Adobe Experience Cloud] applicazioni | Accedi a [!DNL Workfront] con un personalizzato [!DNL Workfront] URL |
| Un &quot;selettore organizzazione&quot; consente di spostarsi tra [!DNL Workfront] organizzazioni e ambienti | Il &quot;selettore organizzazione&quot; non è disponibile |
| La navigazione include un’area di navigazione di primo livello per [!DNL Adobe] prodotti, [!DNL Adobe] notifiche, guida e profilo utente, oltre a [!DNL Workfront] barra di navigazione | La navigazione include [!DNL Workfront] solo barra di navigazione |
| L’Aiuto è accessibile tramite [!UICONTROL Menu principale] e area di navigazione superiore | L’Aiuto è accessibile tramite [!UICONTROL Menu principale] e [!DNL Workfront] barra di navigazione |

{style="table-layout:auto"}

## Domande frequenti

### Come posso determinare se utilizzo Adobe Unified Experience o Adobe Workfront?

Per determinare se l’organizzazione si trova nell’esperienza unificata di Adobe, esamina l’URL utilizzato per accedere a Workfront.

| URL | Esperienza Adobe |
|------------|------------|
| (NomeSocietà).my.workfront.com | Esperienza Workfront |
| experience.adobe.com | Adobe di esperienza unificata |

### Come posso saperne di più sul [!DNL Adobe Admin Console]?

Per informazioni su [!DNL Admin Console], leggi questi articoli:

* [Prepararsi per il [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Differenze di amministrazione basate sulla piattaforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] panoramica](https://helpx.adobe.com/it/enterprise/using/admin-console.html)

### Cosa devo fare in qualità di cliente per facilitare la migrazione?

I clienti esistenti verranno contattati per pianificare le migrazioni. I colleghi del supporto del team di migrazione guideranno i clienti attraverso il processo e forniranno consigli su [!DNL Admin Console] e fornire i collegamenti alla documentazione necessaria per rendere la migrazione il più semplice e semplice possibile.

* [[!DNL Adobe Workfront] Panoramica del supporto](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] informazioni](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] e [!DNL Admin Console] Domande frequenti](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

### Come gestisci [!DNL Adobe Admin Console] per le aziende che hanno già abilitato questo per i Federated ID in modo diverso da [!DNL Workfront] SSO configurato?

[!DNL Adobe Admin Console] ha l’opzione di includere [!DNL Workfront], sostituzione di SSO con IMS. Tutto il provisioning degli utenti avviene in [!DNL Admin Console], e gli utenti visualizzeranno [!DNL Adobe] schermata di accesso per accedere a [!DNL Experience Cloud] dove vedranno [!DNL Workfront] come opzione (se è loro consentito l’accesso).

### In che modo questo influisce sui clienti che dispongono già del pannello di amministrazione dell’AEM per [!DNL Adobe Assets] - ma l&#39;SSO è configurato in modo diverso rispetto a [!DNL Workfront?]

Una volta [!DNL Workfront] viene aggiunto come [!DNL Admin Console] non è necessario eseguire altre operazioni per [!DNL Workfront] per sfruttare la configurazione SSO esistente disponibile per [!DNL Adobe Assets].

### In che modo questo influisce su quelli configurati con SSO?

SSO è configurato in [!DNL Admin Console] ed ereditato da [!DNL Workfront] applicazione.

### È SSO con il nostro interno [!DNL Active Directory] Sarà ancora disponibile un’opzione con IMS?

IMS sostituisce l’SSO e funziona per lo più allo stesso modo. Tutte le autorizzazioni utente vengono concesse e fornite in [!DNL Adobe Admin Console]e l&#39;utente visualizzerà il [!DNL Adobe] schermata di accesso in cui è possibile scegliere &quot;[!UICONTROL Account personale]&quot; o &quot;[!UICONTROL Account società]&quot; per accedere (se si dispone di [!DNL Active Directory], la maggior parte effettuerà l&#39;accesso con un account aziendale).

### Per coloro che non utilizzano SSO, il [!DNL Workfront] cambiare l&#39;URL di accesso?

L’URL di accesso cambierà; tuttavia, il vecchio URL verrà reindirizzato al nuovo URL di accesso, pertanto devi istruire nuovamente gli utenti su dove andare.

### Gli alias impostati funzioneranno ancora o sono [!DNL Workfront] collegamenti che cambiano con questa migrazione?

[!DNL Workfront] Sono disponibili reindirizzamenti/alias per accedere alla home page.

### Può accadere che i reindirizzamenti siano disabilitati? Oppure sarà sempre possibile digitare in my.company.workfront.com?

Puoi sempre utilizzare qualsiasi URL personalizzato. Dopo aver fatto clic su uno di questi collegamenti, ti indirizzerà a [!DNL Workfront] e mostrare un URL diverso. Tuttavia, è un [!DNL experience] per accedere a experience.adobe.com e aggiungere i segnalibri ai collegamenti da [!DNL Experience Cloud]. Un minor reindirizzamento equivale a un minor ritardo/tempo di caricamento.

### I collegamenti diretti alle code di richieste verranno interrotti?

Tutti i collegamenti diretti devono essere reindirizzati ai nuovi pattern URL. Tuttavia, se hai distribuito i collegamenti alle persone, devi inviare un aggiornamento per sfruttare il collegamento diretto e evitare ritardi nel raggiungere la pagina prevista.

### Migreremo a [!DNL Experience Cloud] a livello globale o possiamo scegliere per determinati utenti (non tutti i nostri utenti utilizzano anche altri prodotti di Adobe)?

L&#39;intero [!DNL Workfront] verrà effettuata la migrazione dell’account del cliente. Non può essere fatto utente per utente.

### Verrà [!DNL Workfront] Gli utenti devono effettuare l&#39;accesso tramite [!DNL Experience Cloud]? O solo amministratori?

Sì, tutti gli utenti accederanno tramite [!DNL Experience Cloud]. L’accesso IMS sostituirà l’SSO. È un’esperienza molto simile, ma con una schermata di accesso diversa.

### Gli utenti dovranno collegare i propri [!DNL Adobe] account per i [!DNL Workfront] se hanno già entrambi i conti?

Sì, esiste una procedura per questo e verranno forniti ulteriori dettagli quando è il momento per la tua organizzazione di passare a IMS.

### Cosa succede al [!DNL Workfront] utenti che non dispongono di un [!DNL Adobe] account?

Utenti a cui non è stato concesso l’accesso in [!DNL Adobe Admin Console] per accedere a [!DNL Workfront] deve creare un &quot;[!UICONTROL account personale]&quot; o un [!DNL Adobe] Account ID per accedere. Questo invia un messaggio e-mail all’amministratore per approvare o rifiutare la richiesta, e consente inoltre all’amministratore di configurare il tipo di accesso di cui dispone l’utente. Una volta effettuato l&#39;accesso, il visitatore si recherà all&#39;indirizzo experience.adobe.com, immetterà il proprio indirizzo e-mail e sceglierà [!UICONTROL Account personale]. Da lì, potranno accedere [!DNL Workfront].

### E se non ne avessimo [!DNL Adobe] prodotti diversi da [!DNL Workfront?]

È comunque consigliabile che la tua organizzazione esegua la migrazione a [!DNL Adobe Unified Experience]. Riceverai un [!DNL Adobe] ID insieme ai vantaggi elencati sopra.

### Gli utenti esterni sono inclusi nel [!DNL Workfront] dell&#39;istanza. Non vogliamo che abbiano accesso ad altri prodotti inclusi in [!DNL Adobe]. In che modo limiteremmo il loro accesso all’interno della console?

[!DNL Admin Console] offre agli amministratori un ampio controllo su ciò a cui gli utenti possono e non possono accedere. Ogni volta che un utente esterno desidera accedere, deve creare un [!DNL Adobe] ID, che invia un messaggio e-mail all’amministratore. L’amministratore può quindi accettare o rifiutare l’accesso a un prodotto e definire a cosa può/non può accedere per i prodotti di proprietà di tale organizzazione. Quindi, il [!DNL Workfront] L&#39;amministratore di sistema può accedere al [!UICONTROL Utenti] area di [!DNL Workfront] per rendere più granulari i permessi per l&#39;utente esterno.

### Gli amministratori di gruppi vengono utilizzati per creare persone in [!DNL Workfront]. Con il passaggio a [!DNL Experience Cloud], gli amministratori di gruppo saranno ancora in grado di creare persone?

Sì, la creazione di utenti è ancora possibile tramite [!DNL Workfront]. Questi utenti possono essere aggiunti a [!DNL Experience Cloud] automaticamente. Puoi anche impostare gli amministratori di gruppo come proprietari del prodotto nel [!DNL Admin Console] per consentire loro di assegnare [!DNL Workfront] agli utenti.

### Scadenza del passaggio a [!DNL Experience Cloud]?

Al momento non è presente alcuna scadenza in cui spostarsi [!DNL Adobe Experience Cloud]. Stiamo lavorando con i clienti per consentire loro di scegliere quando sono pronti per la migrazione.

### Il nostro team di supporto dovrà fare qualcosa per questo cambiamento?

Se il team di supporto è responsabile della creazione di nuovi utenti, dovrà acquisire familiarità con [!DNL Admin Console] interfacce utilizzate per creare utenti e assegnare un diritto a Workfront. In caso contrario, è probabile che non vi siano modifiche significative per il team di supporto interno.

### In che modo questo influisce sulle integrazioni disponibili tramite la funzione API?

Il percorso URL esistente continuerà a essere disponibile per il traffico API. Non dovrebbe essere necessario eseguire alcuna operazione per aggiornare gli endpoint nelle integrazioni. Tuttavia, l’accesso diretto tramite nome utente e password non sarà supportato: devi utilizzare una chiave API, ad eccezione di [!DNL Workfront Fusion] connettori.

### E per quanto riguarda [!DNL Creative Cloud] utenti? Quali sono gli effetti della migrazione su di loro? Ci sono dei vantaggi per loro?

Nessun impatto su [!DNL Creative Cloud] utenti con la migrazione a [!DNL Adobe Unified Experience].

### Gli accessi cambieranno per [!DNL Workfront] utenti di dispositivi mobili?

[!DNL Workfront] gli utenti di dispositivi mobili non devono essere interessati dalla migrazione a [!DNL Adobe Unified Experience].
