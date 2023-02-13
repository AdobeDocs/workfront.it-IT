---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Gestire le chiavi API
description: Per ridurre al minimo le vulnerabilità relative alla sicurezza API, gli amministratori di Adobe Workfront possono gestire le chiavi API utilizzate per consentire alle applicazioni di accedere a Workfront per conto di un utente.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1374'
ht-degree: 2%

---

# Gestire le chiavi API

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

Per ridurre al minimo le vulnerabilità relative alla sicurezza API, gli amministratori di Adobe Workfront possono gestire le chiavi API utilizzate per consentire alle applicazioni di accedere a Workfront per conto di un utente.

Puoi ripristinare o rimuovere la chiave API amministratore corrente, configurare le chiavi API in modo che scadano e rimuovere le chiavi API per tutti gli utenti.

Esempi di applicazioni che sfruttano l’API Workfront sono:

* Integrazioni di documenti come Dropbox, Google Drive e Workfront DAM
* Applicazioni mobili Workfront

>[!IMPORTANT]
>
>Quando si reimposta o si rimuove una chiave API, tutte le applicazioni che sfruttano l’API Workfront e si autenticano in Workfront tramite questa chiave API devono essere riconfigurate per poter recuperare l’accesso a Workfront.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Chiavi API Workfront

Ogni utente in Workfront ha una chiave API univoca. Questa chiave viene generata in base all’utente nel momento in cui l’utente accede a un’integrazione che sfrutta l’API Workfront (ad esempio l’app mobile Workfront o un’integrazione di documenti).

>[!NOTE]
>
> Le chiavi API generate nell&#39;ambiente di produzione vengono copiate nell&#39;ambiente di anteprima durante l&#39;aggiornamento settimanale. Eventuali chiavi API generate nell’ambiente di anteprima verranno sovrascritte con le chiavi API di produzione durante l’aggiornamento settimanale.

Gli amministratori di Workfront hanno anche una chiave API univoca. Quando un&#39;applicazione utilizza una chiave API amministratore per accedere a Workfront, l&#39;applicazione dispone dell&#39;accesso amministratore a Workfront.

## Gestire una chiave API amministratore

Puoi generare, reimpostare o rimuovere la chiave API dell’account utente amministratore.

>[!NOTE]
>
>Puoi anche generare una chiave API tramite l’API. Per ulteriori informazioni, consulta la sezione [API iscrizione agli eventi](../../../wf-api/general/event-subs-api.md) sezione [API iscrizione agli eventi](../../../wf-api/general/event-subs-api.md).

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Sistema >** **Informazioni sul cliente.**
1. (Condizionale) Esegui una delle seguenti operazioni:

   Per generare una chiave API: In **Impostazioni chiave API** sezione, fai clic su **Genera chiave API**.

   Oppure\
   Per reimpostare una chiave API: In **Impostazioni chiave API** sezione, fai clic su **Reimposta**, quindi **Reimposta.**

   Oppure

   Per rimuovere la chiave API: In **Impostazioni chiave API** sezione, fai clic su **Rimuovi**, quindi **Rimuovi**.

## Generare una chiave API per utenti non amministratori

Puoi generare e gestire le chiavi API per gli utenti con ruoli diversi dall’amministratore Workfront.

>[!NOTE]
>
>Questa opzione non è disponibile se l’istanza Workfront della tua organizzazione è abilitata con Adobe IMS. Per ulteriori informazioni, rivolgiti al tuo amministratore di rete o IT.

1. (Condizionale) Se l&#39;organizzazione utilizza la gestione degli accessi Single Sign-On (SSO), disattiva temporaneamente l&#39;opzione che richiede l&#39;autenticazione SSO.

   1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

   1. Espandi **Sistema**, quindi fai clic su **Single Sign-On (SSO)**.\
      ![](assets/sysadmin-security-sso-disable-31620-350x320.png)

   1. Disattiva la casella di controllo che richiede l&#39;autenticazione SSO.

      Ad esempio, se la tua organizzazione utilizza SAML 2.0, disattiva **Consenti solo autenticazione SAML 2.0**.

1. Nella barra degli indirizzi di un browser, immetti la seguente chiamata API:

   `<domain>`**.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**username**&amp;password=**password**&amp;method=PUT

   Sostituisci `<domain>` con il nome di dominio di Workfront, il nome utente e la password con le credenziali Workfront dell&#39;utente.

1. (Condizionale) Abilita l&#39;opzione che richiede l&#39;autenticazione SSO se l&#39;hai disabilitata nel passaggio 1.

   1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

   1. Espandi **Sistema**, quindi fai clic su **Single Sign-On (SSO)**.

   1. Seleziona il tuo metodo SSO nel **Tipo** menu a discesa.
   1. Seleziona la casella di controllo che richiede l’autenticazione SSO.

## Configura quando scadono le chiavi API

Puoi configurare le chiavi API in modo che scadano per tutti gli utenti del tuo sistema. Quando la chiave API di un utente scade, l’utente deve effettuare nuovamente l’autenticazione in tutte le applicazioni che utilizzano l’API Workfront per accedere a Workfront. Puoi modificare la frequenza con cui scadono le chiavi API. Puoi anche configurare se le chiavi API scadono alla scadenza della password di un utente.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Sistema** > **Informazioni cliente**.
1. In **Impostazioni chiave API** nella zona **Dopo la creazione**, **Le chiavi API scadono in** dall’elenco a discesa, seleziona l’intervallo di tempo in cui vuoi che le chiavi API scadano.

   Quando modifichi questa opzione, il nuovo arco temporale inizia dal momento in cui hai apportato la modifica. Ad esempio, se modifichi questa opzione da *1 mese* a *6 mesi*, le chiavi API scadono 6 mesi dal momento in cui apporti la modifica.

   Per impostazione predefinita, le chiavi API scadono ogni mese.

1. Per configurare le chiavi API in modo che scadano alla scadenza delle password degli utenti, seleziona **Rimuovi chiave API quando scade la password di un utente**.

   Per impostazione predefinita, questa opzione non è selezionata.

   Per informazioni su come configurare le password utente affinché scadano, vedi [Configurare le preferenze di sicurezza del sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Fai clic su **Salva**.

## Rimuovi le chiavi API per tutti gli utenti

Se sei preoccupato di una particolare violazione della sicurezza relativa al tuo sistema Workfront, puoi rimuovere contemporaneamente le chiavi API per tutti gli utenti.

>[!IMPORTANT]
>
>La rimozione delle chiavi API per tutti gli utenti invalida TUTTE le chiavi API per tutti gli utenti del sistema. Questa azione causerà un errore in tutte le integrazioni in Workfront finché non genererai una nuova chiave API in Workfront e non aggiornerai tutte le integrazioni.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Espandi **Sistema**, quindi fai clic su **Informazioni sul cliente.**

1. In **Impostazioni chiave API** area, fai clic su **Rimuovi tutte le chiavi API**, quindi fai clic su **Rimuovi** **Tutto**.

## Limitazione degli accessi API con un certificato X.509

>[!IMPORTANT]
>
>La procedura descritta in questa sezione si applica solo alle organizzazioni che non sono ancora state integrate nell’Adobe Business Platform. L’accesso a Workfront tramite l’API Workfront non è disponibile se l’organizzazione è stata caricata su Adobe Business Platform.
>
>Per un elenco delle procedure che differiscono a seconda che l’organizzazione sia stata imbarcata in Adobe Business Platform, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Le applicazioni di terze parti possono comunicare con Workfront tramite API. Per aumentare la sicurezza del sito Workfront, puoi configurare Workfront per limitare le richieste di accesso API caricando un certificato X.509 su Workfront. Una volta abilitate, tutte le richieste di accesso tramite l’API devono includere un certificato client oltre a nome utente e password.

>[!NOTE]
>
>Questa opzione non è disponibile se l’istanza Workfront della tua organizzazione è abilitata con Adobe IMS. Per ulteriori informazioni, rivolgiti al tuo amministratore di rete o IT.

* [Ottieni il certificato X.509](#obtain-the-x-509-certificate)
* [Caricare il certificato in Workfront](#upload-the-certificate-to-workfront)
* [Verifica che le chiamate di accesso API siano limitate](#verify-api-login-calls-are-restricted)

### Ottieni il certificato X.509 {#obtain-the-x-509-certificate}

Ottieni un certificato X.509 valido da un’autorità di certificazione attendibile (ad esempio Verifica) e inseriscilo in una posizione temporanea sulla tua workstation.

### Caricare il certificato in Workfront {#upload-the-certificate-to-workfront}

Dopo aver ottenuto il certificato X.509 dall’autorità di certificazione, è necessario caricarlo in Workfront.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Espandi **Sistema**, quindi fai clic su **Informazioni cliente**.

1. In **Impostazioni chiave API** area, selezionare **Abilita certificato X.509**.
1. Nella workstation, individua e seleziona il certificato X.509 scaricato in precedenza.
1. (Facoltativo) Fai clic su **Visualizza dettagli** accanto al nome del certificato per visualizzare i seguenti dettagli sul certificato:

   * Nome comune soggetto
   * Organizzazione soggetto
   * Unità organizzazione soggetto
   * Nome comune emittente
   * Organizzazione emittente
   * Unità organizzazione emittente
   * Numero di serie
   * Data di emissione
   * Data di Scadenza

1. Fai clic su **Salva**.

### Verifica che le chiamate di accesso API siano limitate {#verify-api-login-calls-are-restricted}

Prima di configurare l’istanza di Workfront per richiedere un certificato X.509, esegui una richiesta API al `/login` endpoint utilizzando parametri di nome utente e password validi. Riceverai una risposta di 200 che contiene un sessionID.

Dopo aver reso il certificato X.509 un requisito tramite la pagina di informazioni sul cliente nella tua istanza di Workfront, effettua un altro tentativo di accesso. Questa volta riceverai una risposta di errore 500 con il seguente messaggio: &quot;Richiesta non attendibile. Contattare l&#39;amministratore di sistema e allegare il certificato.&quot;

Dopo aver confermato che il certificato X.509 è obbligatorio, esegui la stessa richiesta di accesso con un parametro aggiuntivo per apiCertificate impostato sul valore del certificato. Se questa operazione è stata eseguita correttamente, riceverai una risposta di 200 che contiene un sessionID valido.
