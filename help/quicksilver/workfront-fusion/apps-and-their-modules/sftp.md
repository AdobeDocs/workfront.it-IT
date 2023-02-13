---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli SFTP
description: La [!DNL Adobe Workfront Fusion SFTP] I moduli consentono di monitorare le modifiche apportate ai file in una cartella o sottocartella selezionata, caricare nuovi file nella cartella desiderata, modificare o eliminare i file esistenti già presenti in una cartella o modificare le autorizzazioni dei file.
author: Becky
feature: Workfront Fusion
exl-id: aacc61f8-ffc3-48db-9f54-188685c52067
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '1883'
ht-degree: 0%

---

# Moduli SFTP

La [!DNL Adobe Workfront Fusion] SFI moduli TP consentono di monitorare le modifiche dei file in una cartella o sottocartella selezionata, caricare nuovi file nella cartella desiderata, modificare o eliminare i file esistenti già presenti in una cartella o modificare le autorizzazioni dei file.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o superiore</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Per utilizzare SFTP con [!DNL Workfront Fusion], è necessario disporre di un account SFTP (ad esempio [!DNL GoDaddy] web hosting).

## Connetti SFTP a [!DNL Workfront Fusion] {#connect-sftp-to-workfront-fusion}

Per collegare il tuo account SFTP a [!DNL Workfront Fusion] devi immettere l’host di destinazione e le credenziali SFTP (nome utente e password o nome utente e chiave) nel modulo [!UICONTROL Creare una connessione] finestra di dialogo.

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
   <td> <p>Immetti il nome host del server SFTP da connettere.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Port] </td> 
   <td> <p>Immetti la porta del server SFTP. Ad esempio, 22.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Auth type]</p> </td> 
   <td> <p>Seleziona il metodo di autorizzazione da utilizzare per la connessione al server SFTP.</p> 
    <ul> 
     <li><strong>[!UICONTROL Nome utente e password]</strong>: Immetti le tue credenziali.</li> 
     <li> <p><strong>[!UICONTROL Nome utente e chiave]</strong>: Immetti il nome utente e la chiave privata/certificato</p> <p>Carica la chiave privata per utilizzare l’autorizzazione lato client o carica il certificato (file P12 o PFX) se desideri utilizzare TLS utilizzando il certificato autofirmato. Se utilizzi l’autorizzazione del certificato lato client, puoi immettere il certificato CA qui.</p> <p>[!DNL Workfront Fusion] non conserva né archivia i dati (file, password) forniti qui. I file e le password vengono utilizzati solo per estrarre una chiave/certificato privata.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Dopo aver inserito le informazioni sulla connessione, fai clic su **[!UICONTROL Continua]** stabilire una connessione.

## [!UICONTROL SFTP] moduli e relativi campi

Quando si configura [!UICONTROL SFTP] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!UICONTROL SFTP] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

#### [!UICONTROL Visualizzare i file in una cartella]

Restituisce file con dettagli quando un file viene creato o modificato in una cartella specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni su come collegare il tuo account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Immetti o mappa la cartella da guardare. È possibile specificare un percorso assoluto, ad esempio <code>/home/user/</code>. Oppure puoi specificare un percorso relativo che punta a una cartella specifica dell’utente connesso, ad esempio <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>Dimensione buffer [B]</td> 
   <td> <p> Immettere la dimensione del buffer in byte. Il valore definisce le dimensioni dei blocchi trasferiti dal server. Alcuni server possono causare problemi o file danneggiati quando il valore è troppo alto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di file restituiti]</td> 
   <td> <p> Imposta il numero massimo di file che [!DNL Workfront Fusion] funziona con durante un ciclo</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Visualizzare le sottocartelle in una cartella]

Restituisce cartelle con dettagli quando una cartella viene creata o modificata in una cartella specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Immetti o mappa la cartella da guardare. È possibile specificare un percorso assoluto, ad esempio <code>/home/user/</code>. Oppure puoi specificare un percorso relativo che punta a una cartella specifica dell’utente connesso, ad esempio <code>./.</code></p> </td> 
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
   <td> <p>Per istruzioni su come collegare il tuo account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show] </td> 
   <td> <p>Selezionare se si desidera recuperare file, cartelle o entrambi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Immettere o mappare la cartella contenente i file o le cartelle da elencare. È possibile specificare un percorso assoluto, ad esempio <code>/home/user/</code>. Oppure puoi specificare un percorso relativo che punta a una cartella specifica dell’utente connesso, ad esempio <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Immetti o mappa il termine di ricerca. Ad esempio, se desideri cercare i file con estensione .txt, immetti <code>.txt</code>.È inoltre possibile immettere o mappare il nome del file che si desidera cercare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordina per]</td> 
   <td> <p> Selezionare se si desidera ordinare i risultati per nome file, dimensione, data dell'ultimo accesso o data dell'ultima modifica.</p> </td> 
  </tr> 
  <tr> 
   <td>Ordinamento [!UICONTROL] </td> 
   <td> <p>Seleziona se il risultato deve essere restituito in ordine crescente o decrescente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Continua l’esecuzione del percorso anche se il modulo non restituisce risultati]</p> </td> 
   <td>Abilita questa opzione per garantire che questo modulo non interrompa lo scenario se non restituisce risultati.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di risultati restituiti]</td> 
   <td> <p> Imposta il numero massimo di risultati che [!DNL Workfront Fusion] ritornerà durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni file]

Questo modulo elenca i file provenienti da una cartella specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni su come collegare il tuo account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dimensione buffer [B]]</td> 
   <td> <p> Immettere la dimensione del buffer in byte. Il valore definisce le dimensioni dei blocchi trasferiti dal server. Alcuni server possono causare problemi o file danneggiati quando il valore è troppo alto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Immettere o mappare la cartella contenente i file o le cartelle da elencare. È possibile specificare un percorso assoluto, ad esempio <code>/home/user/</code>. Oppure puoi specificare un percorso relativo che punta a una cartella specifica dell’utente connesso, ad esempio <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Immetti o mappa il termine di ricerca. Ad esempio, se desideri cercare i file con estensione .txt, immetti <code>.txt</code>.È inoltre possibile immettere o mappare il nome del file che si desidera cercare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordina per]</td> 
   <td> <p> Seleziona se ordinare i risultati in base al nome del file, alla dimensione, alla data dell’ultimo accesso o all’ultima data di modifica.</p> </td> 
  </tr> 
  <tr> 
   <td>Ordinamento [!UICONTROL]</td> 
   <td> <p> Seleziona se il risultato deve essere restituito in ordine crescente o decrescente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Continua l’esecuzione del percorso anche se il modulo non restituisce risultati]</p> </td> 
   <td>Abilita questa opzione per garantire che questo modulo non interrompa lo scenario se non restituisce risultati.</td> 
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
   <td> <p>Per istruzioni su come collegare il tuo account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dimensione buffer [B]]</td> 
   <td> <p> Immettere la dimensione del buffer in byte. Il valore definisce le dimensioni dei blocchi trasferiti dal server. Alcuni server possono causare problemi o file danneggiati quando il valore è troppo alto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path] </td> 
   <td> <p>Immettere il percorso del file. È possibile specificare un percorso assoluto, ad esempio <code>/home/user/file.txt</code>. Oppure puoi specificare un percorso relativo che punta a una cartella specifica dell’utente connesso, ad esempio <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Caricare un file]

Questo modulo ti consente di caricare un file sul server SFTP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni su come collegare il tuo account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Specificare una cartella esistente come posizione di archiviazione per il file. È possibile specificare un percorso assoluto, ad esempio <code>/home/user/</code>. Oppure puoi specificare un percorso relativo che punta a una cartella specifica dell’utente connesso, ad esempio <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File di origine]</td> 
   <td> <p> Mappa il file di origine da un modulo precedente, ad esempio [!UICONTROL Dropbox] &gt; [!UICONTROL Get File]. È inoltre possibile immettere o mappare il nome del file e i dati del file.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorizzazioni [!UICONTROL]</p> </td> 
   <td> <p>Imposta le autorizzazioni desiderate per il file o la cartella. Utilizza i parametri chmod. Ad esempio: <code>777 </code>o <code>-rwxrwxrwx</code>.</p> <p>Per ulteriori dettagli sul chmod, consulta la <a href="https://ss64.com/bash/chmod.html">documentazione di chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rinomina un file]

Rinomina un file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni su come collegare il tuo account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path]</td> 
   <td> <p> Immettere il percorso del file che si desidera rinominare. È possibile specificare un percorso assoluto, ad esempio <code>/home/user/file.txt</code>. Oppure puoi specificare un percorso relativo che punta a una cartella specifica dell’utente connesso, ad esempio <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nuovo nome file]</td> 
   <td> <p> Immetti il nuovo nome per il file, inclusa l’estensione del file.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sposta un file]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni su come collegare il tuo account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path]</td> 
   <td> <p> Immettere il percorso del file che si desidera spostare. È possibile specificare un percorso assoluto, ad esempio <code>/home/user/file.txt</code>. Oppure puoi specificare un percorso relativo che punta a una cartella specifica dell’utente connesso, ad esempio <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nuova Cartella]</td> 
   <td> <p> Immettere il percorso della nuova posizione del file. È possibile specificare un percorso assoluto, ad esempio <code>/home/user/</code>. Oppure puoi specificare un percorso relativo che punta a una cartella specifica dell’utente connesso, ad esempio <code>./.</code></p> </td> 
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
   <td> <p>Per istruzioni su come collegare il tuo account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path]</td> 
   <td> <p> Immettere il percorso del file da eliminare. È possibile specificare un percorso assoluto, ad esempio <code>/home/user/file.txt</code>. Oppure puoi specificare un percorso relativo che punta a una cartella specifica dell’utente connesso, ad esempio <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare le autorizzazioni del file]

Consente di modificare le autorizzazioni del file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni su come collegare il tuo account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path]</td> 
   <td> <p> Immettere il percorso del file che si desidera spostare. È possibile specificare un percorso assoluto, ad esempio <code>/home/user/file.txt</code>. Oppure puoi specificare un percorso relativo che punta a una cartella specifica dell’utente connesso, ad esempio <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorizzazioni [!UICONTROL]</p> </td> 
   <td> <p>Imposta le autorizzazioni desiderate per i file. Utilizza i parametri chmod. Ad esempio: <code>777 </code>o <code>-rwxrwxrwx</code>.</p> <p>Deve corrispondere a un pattern <code> /(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Per ulteriori dettagli sul chmod, consulta la <a href="https://ss64.com/bash/chmod.html">documentazione di chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea cartella]

Crea una nuova cartella nel percorso specificato.

>[!NOTE]
>
>Se la cartella esiste già, il modulo genera un errore. Per continuare il flusso ininterrotto, allega al modulo un percorso del gestore errori per rilevare l&#39;errore e utilizzare il [!UICONTROL Riprendi] direttiva per continuare il flusso. Per informazioni sull&#39;associazione di un percorso del gestore di errori, vedi [Gestione degli errori in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md). Per informazioni sulla route del gestore degli errori, vedi [Direttive sulla gestione degli errori [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni su come collegare il tuo account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Specificare una cartella esistente come percorso di archiviazione per la nuova cartella. È possibile specificare un percorso assoluto, ad esempio <code>/home/user/file.txt</code>. Oppure puoi specificare un percorso relativo che punta a una cartella specifica dell’utente connesso, ad esempio <code>./</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome cartella]</td> 
   <td> <p> Immettere il nome della cartella.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorizzazioni [!UICONTROL]</p> </td> 
   <td> <p>Imposta le autorizzazioni di cartella desiderate. Utilizza i parametri chmod. Ad esempio: <code>777 </code>o <code>-rwxrwxrwx</code>.</p> <p>Deve corrispondere a un pattern <code>/(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Per ulteriori dettagli sul chmod, consulta la <a href="https://ss64.com/bash/chmod.html">pagina man chmod</a>.</p> </td> 
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
   <td> <p>Per istruzioni su come collegare il tuo account SFTP a [!DNL Workfront Fusion], vedi <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Folder Path]</td> 
   <td> <p> Specifica il percorso della cartella da eliminare. È possibile specificare un percorso assoluto, ad esempio <code>/home/user/</code>. Oppure puoi specificare un percorso relativo che punta a una cartella specifica dell’utente connesso, ad esempio <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
