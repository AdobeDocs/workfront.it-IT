---
title: Domande frequenti sulle API SOAP
description: Domande frequenti sulle API SOAP
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# Domande frequenti sulle API SOAP

## Come si crea la prima bozza di file?

Prende 3 semplici passaggi:

**Passaggio 1**: carica il file in Workfront Proof inviandolo tramite una richiesta Post a  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). Ti restituiremo l’hash del file - questo è molto importante! Tieni presente che a questo punto non vedrai nulla nel tuo account, tutto quello che hai fatto finora è inviarci il file ma non ci hai detto cosa farci.

**Passaggio 2**: se non disponi ancora dell’ID sessione, ottenerlo utilizzando i metodi doLogin() o getSessionID(). Utilizza la prima per effettuare l’accesso con l’indirizzo e-mail e la password di un utente oppure, se disponi del token di autenticazione e dell’indirizzo e-mail dell’utente, con il secondo metodo.

**Passaggio 3:** Ora è il momento di creare la tua bozza. Utilizza il metodo createProof() e inviaci almeno i campi obbligatori (al momento ce ne sono solo 5). Assicurati di impostare il parametro Hash sull’hash del file restituito durante il &quot;Passaggio 1&quot;, in quanto questo consente di determinare quale file utilizzare per creare la bozza.

Se accedi al tuo account, verrà visualizzata la bozza.

## Come si crea la prima bozza di istantanea Web?

Prende 2 semplici passaggi:

**Passaggio 1**: se non disponi ancora di un ID sessione, ottenerlo utilizzando i metodi doLogin() o getSessionID(). Utilizza la prima per effettuare l’accesso con l’indirizzo e-mail e la password di un utente oppure, se disponi del token di autenticazione e dell’indirizzo e-mail dell’utente, con il secondo metodo.

**Passaggio 2:**È ora di creare la bozza. Utilizza il metodo createProof() e inviaci almeno i campi obbligatori (al momento ce ne sono solo 5). Accertati di impostare il parametro Hash su &quot;web&quot; e il parametro SourceName come URL della pagina web che desideri acquisire.

Se accedi al tuo account, verrà visualizzata la bozza.

## Qual è la differenza tra una bozza e una versione?

In Workfront le versioni di Proof vengono visualizzate come una singola bozza. Facendo clic su una versione specifica nell’interfaccia utente Web, vengono visualizzati i relativi dettagli. In realtà, ogni versione è una bozza separata e l’interfaccia web li visualizza insieme.

Dal punto di vista dell’API, ogni versione è una bozza separata e le bozze sono collegate tra loro dai rispettivi ID.

**createProof()** creerà sempre **versione 1** della bozza. Supponiamo per il nostro esempio che l’ID restituito per questa bozza sia &quot;100&quot;.

Quando si utilizza **createProofVersion()** invia sempre l’ID della versione precedente. Se si desidera creare **versione 2** sulla bozza &quot;100&quot;, **passa &quot;100&quot; per ParentFileID** parametro. Questo comunica al sistema che questa bozza deve essere la versione 2 del set. Il metodo restituirà un ID di bozza univoco, ad esempio diciamo che è &quot;101&quot;.

Se si utilizza una terza versione, ovvero **versione 3** è obbligatorio, effettuerai una chiamata **createProofVersion()** ancora e questa volta **passa &quot;101&quot; per ParentFileID** che garantirà la corretta creazione dell’elenco collegato delle versioni.

## Devo ottenere un nuovo ID sessione prima di ogni chiamata?

È importante sottolineare che ogni ID sessione è essenzialmente un utente che esegue le azioni. 

Non è necessario ottenere un nuovo ID sessione prima di ogni chiamata all’API, che resterà valido per 24 ore. La data di scadenza viene ripristinata ogni volta che si effettua una chiamata all&#39;API.

## Che cos’è una bozza/un URL personale?

**Team/Pubblico**: ogni versione della bozza ha un URL del team (pubblico) univoco. Se questa opzione è attivata, la bozza verrà aperta in modalità di sola lettura. Puoi ottenere l’URL del team utilizzando [getProofURL()](http://api.proofhq.com/home/proofs/getproofurl) metodo.

**Personale**: un URL personale è univoco per ogni revisore e versione della bozza. Se un set di bozze contiene 3 versioni e un revisore si trova su tutte le versioni, il revisore avrà 3 URL personali univoci. Un URL personale apre la versione della bozza con il revisore già identificato e deve quindi essere mantenuto sicuro e non condiviso. Gli URL personali possono essere ottenuti chiamando il [getProofReviewers()](http://api.proofhq.com/home/proofs/getproofreviewers) e quindi iterazione su ogni  [SOAPRecepientObject](http://api.proofhq.com/home/objects/soaprecipientobject) e ottenere il parametro &quot;proof_url&quot;.

## >Come includere parametri personalizzati quando si apre la miniproof?

La miniproof consente di incorporare lo strumento di correzione nella pagina. È possibile includere un parametro &quot;referer&quot; come parte della miniproof per fornire un URL di reindirizzamento quando un utente fa clic sul pulsante Chiudi nella miniproof. È possibile includere un numero qualsiasi di parametri personalizzati come parte di questo URL di reindirizzamento aggiungendoli utilizzando il carattere &#39;&amp;&#39; di escape, ad esempio %26.

Ad esempio, l’URL miniproof
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` deve essere codificato come 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` affinché i parametri personalizzati possano essere trasmessi.

## Come si crea un client Java Web Service?

[Questo video](http://screencast.com/t/xsSNrqs5b) mostra come creare un client Java Web Service utilizzando Eclipse e la definizione WSDL di Workfront Proof.

