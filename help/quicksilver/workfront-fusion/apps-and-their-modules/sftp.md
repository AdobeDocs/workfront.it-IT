---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli SFTP
description: Il [!DNL Adobe Workfront Fusion SFTP] I moduli consentono di monitorare le modifiche apportate ai file in una cartella o sottocartella selezionata, caricare nuovi file nella cartella desiderata, modificare o eliminare i file esistenti già presenti in una cartella o modificare le autorizzazioni per i file.
author: Becky
feature: Workfront Fusion
exl-id: aacc61f8-ffc3-48db-9f54-188685c52067
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1931'
ht-degree: 0%

---

# Moduli SFTP

Il [!DNL Adobe Workfront Fusion] SFI moduli TP consentono di monitorare le modifiche apportate ai file in una cartella o sottocartella selezionata, caricare nuovi file nella cartella desiderata, modificare o eliminare i file esistenti già presenti in una cartella o modificare le autorizzazioni per i file.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o versione successiva</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Per utilizzare SFTP con [!DNL Workfront Fusion], è necessario disporre di un account SFTP (ad esempio [!DNL GoDaddy] web hosting).

## Connetti SFTP a [!DNL Workfront Fusion] {#connect-sftp-to-workfront-fusion}

Per collegare il tuo account SFTP a [!DNL Workfront Fusion] devi immettere l’host di destinazione e le credenziali SFTP (nome utente e password o nome utente e chiave) per il [!UICONTROL Creare una connessione] .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome connessione]</td> 
   <td> <p> Immetti il nome della connessione SFTP.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
   <td> <p>Immetti il nome host del server SFTP che desideri connettere.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Porta [!UICONTROL] </td> 
   <td> <p>Immetti la porta del server SFTP. Ad esempio, 22.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo di autenticazione]</p> </td> 
   <td> <p>Seleziona il metodo di autorizzazione da utilizzare per la connessione al server SFTP.</p> 
    <ul> 
     <li><strong>[!UICONTROL Nome utente e password]</strong>: immetti le credenziali.</li> 
     <li> <p><strong>[!UICONTROL Nome utente e chiave]</strong>: immetti il nome utente e la chiave privata/certificato</p> <p>Carica la chiave privata per utilizzare l’autorizzazione lato client oppure carica il certificato (file P12 o PFX) se desideri utilizzare TLS con il certificato autofirmato. Se utilizzi l’autorizzazione del certificato lato client, puoi immettere qui il certificato CA.</p> <p>[!DNL Workfront Fusion] non conserva né archivia i dati (file, password) forniti in questo documento. File e password vengono utilizzati solo per estrarre una chiave privata o un certificato.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Dopo aver inserito le informazioni di connessione, fai clic su **[!UICONTROL Continua]** per stabilire una connessione.

## [!UICONTROL SFTP] moduli e relativi campi

Quando si configura [!UICONTROL SFTP] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!UICONTROL SFTP] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

#### [!UICONTROL Controllare i file in una cartella]

Restituisce i file con i dettagli quando un file viene creato o modificato in una cartella specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni sulla connessione dell’account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Immetti o mappa la cartella da controllare. Puoi specificare un percorso assoluto, ad esempio <code>/home/user/</code>. Oppure puoi specificare un percorso relativo che punti a una cartella specifica dell’utente connesso, ad esempio <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>Dimensioni buffer [B]</td> 
   <td> <p> Immettere la dimensione del buffer in byte. Il valore definisce la dimensione dei blocchi trasferiti dal server. Alcuni server possono causare problemi o file danneggiati quando il valore è troppo alto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di file restituiti]</td> 
   <td> <p> Imposta il numero massimo di file che [!DNL Workfront Fusion] funzionerà con durante un ciclo</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Osservare le sottocartelle in una cartella]

Restituisce le cartelle con i dettagli quando una cartella viene creata o modificata in una cartella specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell’account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Immetti o mappa la cartella da controllare. Puoi specificare un percorso assoluto, ad esempio <code>/home/user/</code>. Oppure puoi specificare un percorso relativo che punti a una cartella specifica dell’utente connesso, ad esempio <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di file restituiti]</td> 
   <td> <p> Imposta il numero massimo di cartelle [!DNL Workfront Fusion] ritornerà durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

#### [!UICONTROL Elencare il contenuto di una cartella]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni sulla connessione dell’account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show] </td> 
   <td> <p>Seleziona se desideri recuperare file, cartelle o entrambi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Immettere o mappare la cartella contenente i file o le cartelle da elencare. Puoi specificare un percorso assoluto, ad esempio <code>/home/user/</code>. Oppure puoi specificare un percorso relativo che punti a una cartella specifica dell’utente connesso, ad esempio <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL - Ricerca] </td> 
   <td> <p>Inserisci o mappa il termine di ricerca. Ad esempio, se si desidera cercare i file con estensione .txt, immettere: <code>.txt</code>È inoltre possibile immettere o mappare il nome del file che si desidera cercare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordina per]</td> 
   <td> <p> Specificare se si desidera ordinare i risultati in base al nome file, alla dimensione, alla data dell'ultimo accesso o alla data dell'ultima modifica.</p> </td> 
  </tr> 
  <tr> 
   <td>Ordinamento [!UICONTROL] </td> 
   <td> <p>Seleziona se restituire il risultato in ordine crescente o decrescente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Continua l'esecuzione della route anche se il modulo non restituisce alcun risultato]</p> </td> 
   <td>Abilita questa opzione per garantire che questo modulo non interrompa lo scenario se non restituisce alcun risultato.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di risultati restituiti]</td> 
   <td> <p> Imposta il numero massimo di risultati che [!DNL Workfront Fusion] ritornerà durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni file]

Questo modulo elenca i file di una cartella specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni sulla connessione dell’account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dimensione Buffer [B]]</td> 
   <td> <p> Immettere la dimensione del buffer in byte. Il valore definisce la dimensione dei blocchi trasferiti dal server. Alcuni server possono causare problemi o file danneggiati quando il valore è troppo alto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Immettere o mappare la cartella contenente i file o le cartelle da elencare. Puoi specificare un percorso assoluto, ad esempio <code>/home/user/</code>. Oppure puoi specificare un percorso relativo che punti a una cartella specifica dell’utente connesso, ad esempio <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL - Ricerca] </td> 
   <td> <p>Inserisci o mappa il termine di ricerca. Ad esempio, se si desidera cercare i file con estensione .txt, immettere: <code>.txt</code>È inoltre possibile immettere o mappare il nome del file che si desidera cercare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordina per]</td> 
   <td> <p> Specificare se si desidera ordinare i risultati in base al nome del file, alla dimensione, alla data dell'ultimo accesso o alla data dell'ultima modifica.</p> </td> 
  </tr> 
  <tr> 
   <td>Ordinamento [!UICONTROL]</td> 
   <td> <p> Seleziona se restituire il risultato in ordine crescente o decrescente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Continua l'esecuzione della route anche se il modulo non restituisce alcun risultato]</p> </td> 
   <td>Abilita questa opzione per garantire che questo modulo non interrompa lo scenario se non restituisce alcun risultato.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di risultati restituiti]</td> 
   <td> <p> Imposta il numero massimo di file che [!DNL Workfront Fusion] ritornerà durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un file]

Questo modulo recupera i dettagli del file, inclusi i dati di un file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni sulla connessione dell’account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dimensione Buffer [B]]</td> 
   <td> <p> Immettere la dimensione del buffer in byte. Il valore definisce la dimensione dei blocchi trasferiti dal server. Alcuni server possono causare problemi o file danneggiati quando il valore è troppo alto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percorso File] </td> 
   <td> <p>Immettere il percorso del file. Puoi specificare un percorso assoluto, ad esempio <code>/home/user/file.txt</code>. Oppure puoi specificare un percorso relativo che punti a una cartella specifica dell’utente connesso, ad esempio <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carica un file]

Questo modulo ti consente di caricare un file sul server SFTP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni sulla connessione dell’account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Specificare una cartella esistente come percorso di archiviazione del file. Puoi specificare un percorso assoluto, ad esempio <code>/home/user/</code>. Oppure puoi specificare un percorso relativo che punti a una cartella specifica dell’utente connesso, ad esempio <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File di origine]</td> 
   <td> <p> Mappa il file di origine da un modulo precedente, ad esempio [!UICONTROL Dropbox] &gt; [!UICONTROL Get File]. È inoltre possibile immettere o mappare il nome e i dati del file.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permissions]</p> </td> 
   <td> <p>Impostare le autorizzazioni desiderate per il file o la cartella. Utilizzare i parametri chmod. Ad esempio: <code>777 </code>o <code>-rwxrwxrwx</code>.</p> <p>Per ulteriori dettagli su chmod, fare riferimento al <a href="https://ss64.com/bash/chmod.html">documentazione chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rinominare un file]

Rinomina un file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni sulla connessione dell’account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percorso File]</td> 
   <td> <p> Immettere il percorso del file da rinominare. Puoi specificare un percorso assoluto, ad esempio <code>/home/user/file.txt</code>. Oppure puoi specificare un percorso relativo che punti a una cartella specifica dell’utente connesso, ad esempio <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome nuovo file]</td> 
   <td> <p> Immettere il nuovo nome del file, inclusa l'estensione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Spostare un file]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni sulla connessione dell’account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percorso File]</td> 
   <td> <p> Immettere il percorso del file che si desidera spostare. Puoi specificare un percorso assoluto, ad esempio <code>/home/user/file.txt</code>. Oppure puoi specificare un percorso relativo che punti a una cartella specifica dell’utente connesso, ad esempio <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nuova Cartella]</td> 
   <td> <p> Immettere il percorso della nuova posizione del file. Puoi specificare un percorso assoluto, ad esempio <code>/home/user/</code>. Oppure puoi specificare un percorso relativo che punti a una cartella specifica dell’utente connesso, ad esempio <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un file]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni sulla connessione dell’account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percorso File]</td> 
   <td> <p> Immettere il percorso del file che si desidera eliminare. Puoi specificare un percorso assoluto, ad esempio <code>/home/user/file.txt</code>. Oppure puoi specificare un percorso relativo che punti a una cartella specifica dell’utente connesso, ad esempio <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Autorizzazioni di aggiornamento file]

Consente di modificare le autorizzazioni del file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni sulla connessione dell’account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percorso File]</td> 
   <td> <p> Immettere il percorso del file che si desidera spostare. Puoi specificare un percorso assoluto, ad esempio <code>/home/user/file.txt</code>. Oppure puoi specificare un percorso relativo che punti a una cartella specifica dell’utente connesso, ad esempio <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permissions]</p> </td> 
   <td> <p>Imposta le autorizzazioni file desiderate. Utilizzare i parametri chmod. Ad esempio: <code>777 </code>o <code>-rwxrwxrwx</code>.</p> <p>Deve corrispondere al pattern <code> /(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Per ulteriori dettagli su chmod, fare riferimento al <a href="https://ss64.com/bash/chmod.html">documentazione chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea cartella]

Crea una nuova cartella nel percorso specificato.

>[!NOTE]
>
>Se la cartella esiste già, il modulo genera un errore. Per continuare il flusso senza interruzioni, allega al modulo una route di gestore degli errori per rilevare l’errore e utilizzare [!UICONTROL Riprendi] per continuare il flusso. Per informazioni su come allegare una route di gestore errori, vedere [Gestione degli errori in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md). Per informazioni sulla route del gestore degli errori, vedere [Direttive per la gestione degli errori in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni sulla connessione dell’account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Specificare una cartella esistente come percorso di archiviazione per la nuova cartella. Puoi specificare un percorso assoluto, ad esempio <code>/home/user/file.txt</code>. Oppure puoi specificare un percorso relativo che punti a una cartella specifica dell’utente connesso, ad esempio <code>./</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome cartella]</td> 
   <td> <p> Immetti il nome della cartella.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permissions]</p> </td> 
   <td> <p>Imposta le autorizzazioni della cartella desiderate. Utilizzare i parametri chmod. Ad esempio: <code>777 </code>o <code>-rwxrwxrwx</code>.</p> <p>Deve corrispondere al pattern <code>/(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Per ulteriori dettagli su chmod, fare riferimento al <a href="https://ss64.com/bash/chmod.html">Pagina man chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare una cartella]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni sulla connessione dell’account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Folder Path]</td> 
   <td> <p> Specificare il percorso della cartella da eliminare. Puoi specificare un percorso assoluto, ad esempio <code>/home/user/</code>. Oppure puoi specificare un percorso relativo che punti a una cartella specifica dell’utente connesso, ad esempio <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
