---
title: Domande frequenti sulle API SOAP
description: Domande frequenti sulle API SOAP
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# Domande frequenti sulle API SOAP

## Come si crea la prima bozza di file?

Sono necessari 3 semplici passaggi:

**Passaggio 1**: Carica il file in Workfront Proof inviandolo tramite una richiesta Post a  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). Ti restituiremo l&#39;hash del file - questo è molto importante! Nota che a questo punto non vedrai nulla nel tuo account, tutto quello che hai fatto finora è inviarci il file ma non ci ha detto cosa fare con esso.

**Passaggio 2**: Se non disponi ancora dell&#39;ID sessione, ottenerlo utilizzando i metodi doLogin() o getSessionID() . Usa il primo per &quot;accedere&quot; utilizzando l&#39;indirizzo e-mail e la password di un utente o il secondo metodo se disponi dell&#39;indirizzo e-mail e del token di autenticazione dell&#39;utente.

**Passaggio 3:** Ora è il momento di creare le prove. Utilizza il metodo createProof() e inviaci almeno i campi richiesti (attualmente ce ne sono solo 5). Assicurati di impostare il parametro Hash sull&#39;hash del file restituito durante il &quot;Passaggio 1&quot;, in quanto questo ci consente di determinare quale file utilizzare durante la creazione della bozza.

Se ora accedi al tuo account, visualizzerai la bozza.

## Come posso creare la mia prima bozza web snapshot?

Sono necessari 2 semplici passaggi:

**Passaggio 1**: Se non disponi ancora di un ID sessione, ottenerlo utilizzando i metodi doLogin() o getSessionID() . Usa il primo per &quot;accedere&quot; utilizzando l&#39;indirizzo e-mail e la password di un utente o il secondo metodo se disponi dell&#39;indirizzo e-mail e del token di autenticazione dell&#39;utente.

**Passaggio 2:**Ora è il momento di creare la bozza. Utilizza il metodo createProof() e inviaci almeno i campi richiesti (attualmente ce ne sono solo 5). Assicurati di impostare il parametro Hash su &quot;web&quot; e il parametro SourceName come URL della pagina web che desideri acquisire.

Se ora accedi al tuo account, visualizzerai la bozza.

## Qual è la differenza tra una bozza e una versione?

Nelle versioni di Workfront Proof vengono visualizzate come una singola bozza. Facendo clic su una versione specifica nell’interfaccia utente Web verranno visualizzati i dettagli di tale versione. In realtà, ogni versione è una bozza separata e l’interfaccia utente web le visualizza insieme.

Dal punto di vista dell’API, ogni versione è una bozza separata e le bozze sono collegate tra loro dai rispettivi ID.

**createProof()** creerà sempre **versione 1** della prova. Supponiamo per il nostro esempio che l’ID restituito per questa prova &quot;100&quot;.

Quando utilizzi **createProofVersion()** invia sempre l’ID della versione precedente. Se vogliamo creare **versione 2** sulla prova &quot;100&quot;, noi **passa &quot;100&quot; per il ParentFileID** parametro . Questo indica al sistema che questa prova deve essere la versione 2 del set. Il metodo restituirà un ID di prova univoco, per il nostro esempio supponiamo che sia &quot;101&quot;.

Se una terza versione è **versione 3** è obbligatorio, chiamerai **createProofVersion()** ancora e questa volta **passa &quot;101&quot; per il ParentFileID** che garantirà la corretta creazione dell’elenco collegato delle versioni.

## È necessario ottenere un nuovo ID sessione prima di ogni chiamata?

È importante sottolineare che ogni ID sessione è essenzialmente un utente che esegue le azioni. 

Non devi ottenere un nuovo ID sessione prima di ogni chiamata all’API e rimarrà valido per 24 ore. Il tempo di scadenza viene reimpostato ogni volta che effettui una chiamata all’API.

## Che cos’è una bozza / URL personale?

**Team/Pubblico**: Ogni versione della bozza dispone di un URL univoco per Team (Public). Se abilitata, la bozza viene aperta in modalità di sola lettura. Puoi ottenere l’URL del team utilizzando la [getProofURL()](http://api.proofhq.com/home/proofs/getproofurl) metodo .

**Personale**: Un URL personale è univoco per ogni revisore e versione della bozza. Se un set di prove contiene 3 versioni e un revisore è su tutte le versioni, il revisore avrà 3 URL personali univoci. Un URL personale apre la versione della bozza con il revisore già identificato e deve pertanto essere mantenuto sicuro e non condiviso. Gli URL personali possono essere ottenuti chiamando il [getProofReviewers()](http://api.proofhq.com/home/proofs/getproofreviewers) e quindi iterazione su ogni  [SOAPRecepientObject](http://api.proofhq.com/home/objects/soaprecipientobject) e ottenere il parametro &quot;proof_url&quot;.

## >Come includere parametri personalizzati all’apertura della miniproof?

La miniproof consente di incorporare lo strumento di correzione nella pagina. Un parametro &quot;referer&quot; può essere incluso come parte della miniproof per fornire un URL di reindirizzamento quando un utente fa clic sul pulsante Chiudi nel miniproof. Puoi includere qualsiasi numero di parametri personalizzati come parte di questo URL di reindirizzamento aggiungendoli utilizzando il carattere di escape &#39;&amp;&#39;, ad esempio %26.

Ad esempio, l’URL a prova di miniatura
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` deve essere codificato come 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` per trasmettere i parametri personalizzati.

## Come si crea un client Java Web Service?

[Questo video](http://screencast.com/t/xsSNrqs5b) mostra come creare un client Java Web Service utilizzando Eclipse e la definizione WSDL di prova di Workfront.
