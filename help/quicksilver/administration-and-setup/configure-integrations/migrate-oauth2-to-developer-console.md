---
title: Migrazione da Workfront OAuth2 a Adobe Developer Console
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: È in corso il ritiro del servizio applicativo legacy personalizzato OAuth2 di Workfront. Scopri cosa cambia, chi è interessato e come migrare le integrazioni personalizzate in Adobe Developer Console.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
source-git-commit: db7e6a6fa0c5fc5332213c388d9b4db3a5c59f53
workflow-type: tm+mt
source-wordcount: '1474'
ht-degree: 1%

---

# Migrazione da Workfront OAuth2 a Adobe Developer Console

Il servizio applicativo OAuth2 personalizzato legacy di Workfront (le integrazioni configurate in **Configurazione** > **Sistema** > **OAuth2**) verrà ritirato. In futuro, tutte le integrazioni personalizzate che eseguono l’autenticazione in Workfront dovranno utilizzare il flusso di autenticazione di Adobe Developer Console (developer.adobe.com).

Questa modifica influisce su qualsiasi integrazione personalizzata, script o strumento di terze parti che al momento si autentica utilizzando un ID client OAuth2 e un segreto rilasciati da Workfront. Questo non influisce sul modo in cui si accede a Workfront, né sulle integrazioni standard gestite da Adobe, come le integrazioni Microsoft Teams o Slack, di cui Adobe esegue separatamente la migrazione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Configurazioni dei livelli di accesso di Adobe Workfront</td> 
   <td><p>Amministratore di sistema</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Diritti Adobe Developer Console</td> 
   <td><p>Per accedere a Adobe Developer Console for Workfront sono necessari i diritti di amministratore dell’organizzazione IMS. Questo ruolo è più ampio di quello di amministratore di prodotto Workfront, in quanto gestisce l’intera organizzazione Adobe e tutti i prodotti che la compongono.</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## Date chiave

| Data | Milestone | Che cosa significa per te |
|---|---|---|
| 1 novembre 2026 | Creazione di una nuova app disabilitata | Non è più possibile creare nuove applicazioni OAuth2 personalizzate in Workfront. Le applicazioni esistenti continuano a funzionare. |
| 1 febbraio 2027 | Servizio legacy ritirato | Le applicazioni OAuth2 personalizzate esistenti cessano completamente di funzionare. A questo punto, qualsiasi integrazione che non sia stata migrata a Adobe Developer Console non potrà più accedere all’API di Workfront. |

>[!IMPORTANT]
>
>Consigliamo vivamente di pianificare e completare la migrazione prima del 1° novembre 2026, in modo che le integrazioni continuino a essere eseguite senza interruzioni, evitando di eseguire la migrazione rispetto alla scadenza fissa del 1° febbraio 2027.

## Organizzazioni interessate

Questa modifica interessa la tua organizzazione se dispone di integrazioni, script o strumenti che si connettono a Workfront utilizzando un ID client OAuth2 personalizzato e un segreto rilasciato tramite la schermata di configurazione legacy di Workfront OAuth2. Esempi comuni includono:

* Integrazioni personalizzate gestite dal team tecnico rispetto all’API di Workfront.
* Connettori di terze parti o creati da partner configurati con un ID client rilasciato da Workfront. Consigliamo di contattare il fornitore se non sei sicuro di come si autentica la loro integrazione.
* Script di automazione interna, reporting o sincronizzazione dati che chiamano direttamente l’API Workfront.

Se non sai se la tua organizzazione dispone di uno di questi elementi, l&#39;amministratore di Workfront può controllare l&#39;elenco delle applicazioni OAuth2 in **Configurazione** > **Sistema** > **OAuth2** per visualizzare ciò che è attualmente registrato. Per informazioni, consulta [Visualizzare e gestire applicazioni OAuth2 personalizzate](/help/quicksilver/administration-and-setup/configure-integrations/manage-custom-oauth2-apps.md).

## Comprendere i tipi di autenticazione di Adobe Developer Console

Adobe Developer Console supporta più metodi di autenticazione. Puoi selezionare il tipo che corrisponde al funzionamento dell’integrazione:

* **Autenticazione server-to-server**: per un&#39;applicazione in esecuzione nel backend che chiama le API Adobe per conto della tua organizzazione, senza coinvolgere alcun utente finale. Questa è la corrispondenza più simile al pattern Workfront OAuth2 legacy utilizzato con ID client e segreti ed è il tipo che la maggior parte delle integrazioni Workfront personalizzate, degli script e delle automazioni deve utilizzare.
* **Autenticazione utente**: per i casi in cui un utente di Adobe deve accedere e concedere il consenso prima che l&#39;applicazione possa visualizzare o modificare i propri dati. Se l’integrazione deve agire per conto di un utente Workfront specifico connesso anziché per l’intera organizzazione, utilizza invece questo tipo.

  Se scegli Autenticazione utente, sono disponibili tre ulteriori opzioni a seconda dell’architettura dell’applicazione:

  * **App Web OAuth**: per applicazioni con interfaccia utente front-end e server back-end. Il server memorizza in modo sicuro il segreto client e recupera i token.
  * **App a pagina singola OAuth**: per applicazioni Web solo browser senza server back-end. L’app web recupera i token.
  * **App nativa OAuth**: per applicazioni mobili o desktop eseguite in modo nativo su un dispositivo e prive di server back-end. L’app nativa recupera i token.

La maggior parte delle organizzazioni che eseguono la migrazione di un’integrazione back-end, di uno script o di un’automazione del servizio OAuth2 legacy richiede l’autenticazione server-to-server.

## Confronto delle funzioni: versioni precedenti di OAuth2 e Adobe Developer Console

Il servizio legacy Workfront OAuth2 (disponibile in **Configurazione** > **Sistema** > **Applicazioni OAuth2**) offre tre tipi di applicazioni, con un limite di 10 applicazioni OAuth2 per istanza di Workfront. Ecco come si confrontano questi aspetti con Adobe Developer Console:

| Tipo Workfront legacy | Metodo di flusso/autenticazione | Equivalente Developer Console | Adatta |
|---|---|---|---|
| Applicazione machine-to-machine (CLI, daemon, script back-end) | JWT con coppia di chiavi pubblica/privata | Autenticazione server-to-server | Lo stesso scopo di non coinvolgere l’utente finale, ma il meccanismo cambia. Il flusso legacy utilizza una coppia di chiavi pubblica/privata e JWT, mentre Server-to-Server utilizza un ID client e un segreto client con una concessione di credenziali client OAuth. Non si tratta di uno scambio di credenziali per l&#39;eliminazione. È necessario modificare il codice di autenticazione dell’integrazione, non solo i valori delle credenziali. Per informazioni, consulta [Utilizzo del flusso JWT per le applicazioni OAuth 2 personalizzate](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md). |
| Applicazione Web (applicazioni lato server: Go, Java, .NET, Node, PHP) | Flusso codice di autorizzazione OAuth 2.0 | OAuth Web App (in Autenticazione utente) | La più vicina corrispondenza 1:1. Questo ha lo stesso flusso e la stessa forma di base in cui un server backend memorizza il segreto client. Per informazioni, consulta [Flusso del codice di autorizzazione per le applicazioni OAuth 2 personalizzate](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md). |
| Applicazione Web a pagina singola (JS, Angular, React, Vue) | Flusso del codice di autorizzazione con PKCE, nessun segreto client | App a pagina singola OAuth (in Autenticazione utente) | Corrispondenza 1:1 più vicinaQuesto ha lo stesso flusso senza segreto basato su PKCE. Per informazioni, vedere [Utilizzo del flusso PKCE per le applicazioni OAuth 2](/help/quicksilver/wf-api/api/oauth-app-pkce-flow.md). |
| (nessun equivalente legacy) | — | App nativa OAuth (in Autenticazione utente) | Questa è una nuova funzionalità. La versione precedente di Workfront OAuth2 non dispone di un tipo dedicato per applicazioni native per dispositivi mobili o desktop. |

<!--

>[!NOTE]
>
>A few legacy capabilities don't have a confirmed equivalent yet in Adobe Developer Console, and are being validated with the Developer Console team:
>
>* Per-app controls the legacy UI offers: refresh token rotation toggle, absolute vs. inactivity refresh token expiration, custom logo, privacy policy URL, and developer contact fields.
>* Whether Developer Console enforces a cap on credentials or projects similar to the legacy 10-app-per-instance limit.
>* Whether a JWT/key pair-based option remains available anywhere in Developer Console for Machine to Machine customers, or whether all such integrations must move to the client-secret-based Server-to-Server grant.

-->

## Procedura di migrazione

### Se si è un amministratore di sistema di Workfront

>[!NOTE]
>
>Se sei un amministratore di prodotto Workfront ma non un amministratore organizzazione, devi collaborare con l’amministratore organizzazione per completare questa migrazione o richiedere di crearne una.

1. Accedi a [developer.adobe.com](https://developer.adobe.com) e crea un nuovo progetto. I progetti sono il modo in cui la console organizza diverse integrazioni o app client.
1. Aggiungi un&#39;API dal progetto e seleziona **Adobe Workfront**. Questa API si trova nella categoria Experience Cloud. Tutte le API di Workfront, incluse Planning, Workflow e Revisione e Approvazioni, condividono questa singola API.
1. Seleziona l&#39;opzione di autenticazione **Server-to-Server**, quindi scegli l&#39;istanza corretta se l&#39;organizzazione IMS dispone di più istanze di Workfront.

   Per informazioni sulla scelta di un tipo di autenticazione, vedere [Comprendere i tipi di autenticazione di Adobe Developer Console](#understand-adobe-developer-console-authentication-types) in questo articolo.
1. Nella pagina Progetto, apri i dettagli della nuova credenziale server-to-server OAuth per trovare l’ID client, il segreto client e le informazioni necessarie per generare i token di accesso.
1. Aggiorna l’integrazione, lo script o lo strumento per eseguire l’autenticazione con queste nuove credenziali al posto del vecchio ID client Workfront OAuth2 e del segreto.
1. Conferma l’accesso in Workfront. Il client API viene aggiunto automaticamente come utente Workfront &quot;`techacct`&quot;. Per impostazione predefinita, viene aggiunto come Collaboratore con accesso limitato, ma è possibile regolarne il livello di accesso come si farebbe per qualsiasi altro utente.
1. (Facoltativo) Per concedere i diritti di amministratore dell&#39;utente `techacct`, aggiungi l&#39;e-mail dell&#39;account tecnico come amministratore del profilo di prodotto pertinente in Admin Console.
1. Testare l’integrazione end-to-end.
1. Dopo aver confermato il funzionamento della nuova connessione, ritira la vecchia voce dell’applicazione OAuth2 in Workfront.

Per informazioni dettagliate e schermate dettagliate, consulta [Ottenere l&#39;accesso](https://developer.adobe.com/workfront-apis/guides/gaining_access/) nella documentazione di Adobe Developer Console.

### Se non si è un amministratore di sistema

Per completare la migrazione, è necessario effettuare un ciclo nell’amministratore dell’organizzazione IMS della tua organizzazione, in quanto la configurazione delle nuove credenziali in Adobe Developer Console richiede tale livello di accesso. Se gestisci o gestisci un’integrazione ma sai chi è l’amministratore dell’organizzazione IMS della tua organizzazione, contatta una delle seguenti persone:

* Il team del tuo account Workfront
* Il tuo team IT interno
* Contatto tecnico

## Se non esegui la migrazione

Le integrazioni che utilizzano ancora il pattern legacy OAuth2 ID client/secret dopo il 1° febbraio 2027 cessano di essere in grado di eseguire l’autenticazione in base all’API Workfront e qualsiasi flusso di lavoro, sincronizzazione o automazione dipendente non riesce. Non è pianificata alcuna estensione oltre questa data, quindi esegui la migrazione delle integrazioni con largo anticipo.

## Domande frequenti

**Questo problema influisce sulle integrazioni fornite da Adobe, ad esempio Slack o Microsoft Teams?**

No. Le applicazioni globali gestite da Adobe vengono migrate direttamente da Adobe e non richiedono alcun intervento da parte tua.

**L&#39;integrazione esistente smetterà di funzionare prima del 1° febbraio 2027?**

No. Le applicazioni OAuth2 personalizzate esistenti continuano a funzionare normalmente fino al 1° febbraio 2027. È interessata solo la possibilità di creare nuove applicazioni OAuth2 personalizzate, a partire dal 1° novembre 2026.

**La migrazione ha un costo?**

No, non ci sono costi aggiuntivi associati all’autenticazione tramite Adobe Developer Console.

**Dove posso trovare assistenza?**

Rivolgiti al team del tuo account Workfront o apri un caso di supporto in caso di domande sull’integrazione o sulla tempistica specifiche. Per la procedura dettagliata di configurazione ufficiale e aggiornata con le schermate, consulta [Ottenere l&#39;accesso](https://developer.adobe.com/workfront-apis/guides/gaining_access/) nella documentazione di Adobe Developer Console.
