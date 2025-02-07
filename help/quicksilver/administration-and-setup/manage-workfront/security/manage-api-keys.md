---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Gestire le chiavi API
description: Per ridurre al minimo le vulnerabilità di sicurezza API, gli amministratori di Adobe Workfront possono gestire le chiavi API utilizzate per consentire alle applicazioni di accedere a Workfront per conto di un utente.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '1330'
ht-degree: 2%

---

# Gestire le chiavi API

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

Per ridurre al minimo le vulnerabilità di sicurezza API, gli amministratori di Adobe Workfront possono gestire le chiavi API utilizzate per consentire alle applicazioni di accedere a Workfront per conto di un utente.

Puoi reimpostare o rimuovere la chiave API dell’amministratore corrente, configurare le chiavi API in scadenza e rimuovere le chiavi API per tutti gli utenti.

Esempi di applicazioni che sfruttano l’API di Workfront sono:

* Integrazioni di documenti come Dropbox, Google Drive e Workfront DAM
* Applicazioni mobili Workfront

>[!IMPORTANT]
>
>Quando si ripristina o si rimuove una chiave API, qualsiasi applicazione che sfrutta l’API Workfront e si autentica in Workfront tramite questa chiave API deve essere riconfigurata per poter riottenere l’accesso a Workfront.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Chiavi API Workfront

Ogni utente in Workfront ha una chiave API univoca. Questa chiave viene generata per singolo utente nel momento in cui l’utente accede a un’integrazione che sfrutta l’API di Workfront (ad esempio l’app mobile Workfront o un’integrazione con un documento).

>[!NOTE]
>
> Le chiavi API generate nell&#39;ambiente di produzione vengono copiate nell&#39;ambiente di anteprima durante l&#39;aggiornamento settimanale. Tutte le chiavi API generate nell’ambiente di anteprima verranno sovrascritte con le chiavi API di produzione durante l’aggiornamento settimanale.

Gli amministratori di Workfront dispongono inoltre di una chiave API univoca. Quando un’applicazione utilizza una chiave API amministratore per accedere a Workfront, ha accesso amministratore a Workfront.

## Gestire una chiave API di amministratore

Puoi generare, reimpostare o rimuovere la chiave API per l’account utente amministratore.

>[!NOTE]
>
>Puoi anche generare una chiave API tramite l’API. Per ulteriori informazioni, vedere la sezione [API sottoscrizione eventi](../../../wf-api/general/event-subs-api.md) in [API sottoscrizione eventi](../../../wf-api/general/event-subs-api.md).

{{step-1-to-setup}}

1. Fai clic su **Sistema >** **Informazioni cliente.**
1. (Condizionale) Esegui una delle azioni seguenti:

   Per generare una chiave API: nella sezione **Impostazioni chiave API**, fai clic su **Genera chiave API**.

   Oppure\
   Per reimpostare una chiave API: nella sezione **Impostazioni chiave API**, fare clic su **Reimposta**, quindi su **Reimposta.**

   Oppure

   Per rimuovere la chiave API: nella sezione **Impostazioni chiave API**, fare clic su **Rimuovi**, quindi su **Rimuovi**.

## Generare una chiave API per gli utenti non amministratori

Puoi generare e gestire le chiavi API per gli utenti con ruoli diversi da Amministratore Workfront.

>[!NOTE]
>
>Questa opzione non è disponibile se l’istanza Workfront della tua organizzazione è abilitata con Adobe IMS. Per ulteriori informazioni, rivolgersi all&#39;amministratore di rete o IT.

1. (Condizionale) Se l’organizzazione utilizza la gestione degli accessi Single Sign-On (SSO), disabilita temporaneamente l’opzione che richiede l’autenticazione SSO.

   {{step-1-to-setup}}

   1. Espandere **Sistema**, quindi fare clic su **Single Sign-on (SSO)**.
   1. Nel campo **Tipo**, seleziona il tipo di SSO utilizzato dalla tua organizzazione.
   1. Con il tipo selezionato, scorri verso il basso e deseleziona la casella di controllo **Abilita**.
      ![Abilita SSO](assets/sysadmin-security-sso-disable-31620-350x320.png)
   1. Fai clic su **Salva**.


1. Nella barra degli indirizzi di un browser, immetti la seguente chiamata API:

   `<domain>`**.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**nomeutente**&amp;password=**password**&amp;method=PUT

   Sostituisci `<domain>` con il tuo nome di dominio Workfront e nome utente e password con le credenziali Workfront dell&#39;utente.

1. (Condizionale) Abilita l&#39;opzione che richiede l&#39;autenticazione SSO se l&#39;hai disabilitata nel passaggio 1.

   {{step-1-to-setup}}

   1. Espandere **Sistema**, quindi fare clic su **Single Sign-on (SSO)**.

   1. Selezionare il metodo SSO nel menu a discesa **Tipo**.
   1. Selezionare la casella di controllo che richiede l&#39;autenticazione SSO.

## Configurare quando scadono le chiavi API

Puoi configurare le chiavi API in modo che scadano per tutti gli utenti nel sistema. Quando la chiave API di un utente scade, l’utente deve autenticare nuovamente tutte le applicazioni che utilizzano l’API Workfront per accedere a Workfront. Puoi modificare la frequenza di scadenza delle chiavi API. Puoi anche configurare la scadenza delle chiavi API quando scade la password di un utente.

{{step-1-to-setup}}

1. Fai clic su **Sistema** > **Informazioni cliente**.
1. Nell&#39;area **Impostazioni chiave API**, nell&#39;elenco a discesa **Dopo la creazione**, **Le chiavi API scadono**, selezionare l&#39;intervallo di tempo in cui si desidera che scadano le chiavi API.

   Quando si modifica questa opzione, il nuovo intervallo temporale inizia dal momento in cui è stata apportata la modifica. Ad esempio, se modifichi questa opzione da *1 mese* a *6 mesi*, le chiavi API scadono dopo 6 mesi dal momento in cui effettui la modifica.

   Per impostazione predefinita, le chiavi API scadono ogni mese.

1. Per configurare le chiavi API in modo che scadano alla scadenza delle password degli utenti, selezionare **Rimuovi chiave API alla scadenza della password di un utente**.

   Per impostazione predefinita, questa opzione non è selezionata.

   Per informazioni su come configurare le password utente in modo che scadano, vedere [Configurare le preferenze di sicurezza del sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Fai clic su **Salva**.

## Rimuovi le chiavi API per tutti gli utenti

Se sei preoccupato di una particolare violazione di sicurezza relativa al tuo sistema Workfront, puoi rimuovere le chiavi API simultaneamente per tutti gli utenti.

>[!IMPORTANT]
>
>La rimozione delle chiavi API per tutti gli utenti invalida TUTTE le chiavi API per tutti gli utenti del sistema. Questa azione causerà un errore in tutte le integrazioni in Workfront fino a quando non genererai una nuova chiave API in Workfront e non aggiornerai tutte le integrazioni.

{{step-1-to-setup}}

1. Espandi **Sistema**, quindi fai clic su **Informazioni cliente**.

1. Nell&#39;area **Impostazioni chiave API**, fare clic su **Rimuovi tutte le chiavi API**, quindi su **Rimuovi** **Tutte**.

## Limitazione degli accessi API con un certificato X.509

>[!IMPORTANT]
>
>La procedura descritta in questa sezione si applica solo alle organizzazioni che non hanno ancora effettuato l’onboarding in Adobe Business Platform. L’accesso a Workfront tramite l’API Workfront non è disponibile se l’organizzazione è stata integrata in Adobe Business Platform.
>
>Per un elenco delle procedure che differiscono a seconda che l&#39;organizzazione sia stata integrata o meno in Adobe Business Platform, consulta [Differenze di amministrazione basate su Platform (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Le applicazioni di terze parti possono comunicare con Workfront tramite l’API. Per aumentare la sicurezza del sito Workfront, puoi configurare Workfront in modo da limitare le richieste di accesso API caricando un certificato X.509 in Workfront. Una volta abilitate, tutte le richieste di accesso tramite l’API devono includere un certificato client oltre a nome utente e password.

>[!NOTE]
>
>Questa opzione non è disponibile se l’istanza Workfront della tua organizzazione è abilitata con Adobe IMS. Per ulteriori informazioni, rivolgersi all&#39;amministratore di rete o IT.

* [Ottieni il certificato X.509](#obtain-the-x-509-certificate)
* [Carica il certificato in Workfront](#upload-the-certificate-to-workfront)
* [Verificare che le chiamate di accesso API siano limitate](#verify-api-login-calls-are-restricted)

### Ottenere il certificato X.509 {#obtain-the-x-509-certificate}

Ottenere un certificato X.509 valido da un&#39;autorità di certificazione attendibile (ad esempio Verisign) e collocarlo in una posizione temporanea sulla workstation.

### Carica il certificato in Workfront {#upload-the-certificate-to-workfront}

Dopo aver ottenuto il certificato X.509 dall’autorità di certificazione, devi caricarlo in Workfront.

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic sull&#39;icona **Setup** ![Gear settings](assets/gear-icon-settings.png).

1. Espandi **Sistema**, quindi fai clic su **Informazioni cliente**.

1. Nell&#39;area **Impostazioni chiave API**, selezionare **Abilita certificato X.509**.
1. Sulla workstation, individua e seleziona il certificato X.509 scaricato in precedenza.
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

### Verificare che le chiamate di accesso API siano limitate {#verify-api-login-calls-are-restricted}

Prima di configurare l&#39;istanza di Workfront per richiedere un certificato X.509, eseguire una richiesta API all&#39;endpoint `/login` utilizzando parametri validi per nome utente e password. Riceverai una risposta 200 contenente un sessionID.

Dopo aver impostato il certificato X.509 come obbligatorio tramite la pagina di informazioni sul cliente nell’istanza di Workfront, effettua un altro tentativo di accesso. Questa volta riceverai una risposta di errore 500 con il seguente messaggio: &quot;Richiesta non attendibile. Contatta l’amministratore di sistema e allega il certificato.&quot;

Dopo aver confermato che il certificato X.509 è obbligatorio, esegui la stessa richiesta di accesso con un parametro aggiuntivo per apiCertificate impostato sul valore del certificato. Se questa operazione è stata eseguita correttamente, riceverai una risposta 200 contenente un sessionID valido.
