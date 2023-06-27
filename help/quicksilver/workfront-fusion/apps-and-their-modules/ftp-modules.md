---
filename: ftp-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli FTP
description: I moduli FTP consentono di monitorare le modifiche apportate ai file in una cartella selezionata, caricare nuovi file nella cartella desiderata e modificare o eliminare i file esistenti già presenti in una cartella.
author: Becky
exl-id: 360825a4-4580-4039-894e-583e82132ed6
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1343'
ht-degree: 0%

---

# Moduli FTP

I moduli FTP consentono di monitorare le modifiche apportate ai file in una cartella selezionata, caricare nuovi file nella cartella desiderata e modificare o eliminare i file esistenti già presenti in una cartella.

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

Per utilizzare [App Fusion] con [!DNL Workfront Fusion], è necessario disporre di un account FTP.

## Creare una connessione in un modulo FTP {#create-a-connection}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Nome connessione]</td> 
   <td> <p> Immetti il nome della connessione FTP.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Host] </td> 
   <td> <p>Immetti il nome host del server FTP. E.g. <code>myftp123.server.com</code></p> </td> 
  </tr> 
  <tr> 
   <td>Porta [!UICONTROL] </td> 
   <td> <p>Immettere il numero di porta del server FTP. E.g. <code>21</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome utente] </td> 
   <td> <p>Immetti il nome utente dell'account FTP.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Password] </td> 
   <td> <p>Immettere la password dell'account FTP.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilizzare una connessione protetta (TLS)</p> </td> 
   <td> <p>Selezionare se si desidera utilizzare una connessione protetta.</p> <p style="font-weight: bold;">[!UICONTROL No]</p> <p>Connessione non protetta.</p> <p style="font-weight: bold;">[!UICONTROL Crittografia esplicita o Crittografia implicita]</p> <p>La connessione è protetta tramite SSL.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Rifiuta certificati non autorizzati]</p> </td> 
   <td> <p>Abilita questa opzione per verificare il certificato del server FTP. Se la verifica non riesce, la connessione non viene creata. Per superare la verifica, il certificato deve soddisfare uno dei seguenti criteri:</p> 
    <ul> 
     <li>essere firmato da una radice <a href="https://en.wikipedia.org/wiki/Certificate_authority">Autorità di certificazione</a></li> 
     <li>essere firmata da un’autorità di certificazione intermedia (cfr. <a href="https://knowledge.digicert.com/solution/SO16297.html">Funzionamento delle catene di certificati</a> per ulteriori spiegazioni). In questo caso, tutti i certificati intermedi devono essere installati sul server FTP.</li> 
     <li>essere un certificato autofirmato fornito nel campo [!UICONTROL Self-signed certificate] (vedi di seguito)</li> </ul>

Se questa opzione è disabilitata, il certificato del server FTP non viene verificato. Consigliamo vivamente di non disabilitare l’opzione in quanto rende la connessione insicura e comporta un grave rischio per la sicurezza.</td>
</tr> 
  <tr> 
   <td> <p>[!UICONTROL Self-signed certificate]</p> </td> 
   <td> <p>Fai clic su <b>[!UICONTROL Extract]</b> per aprire la finestra di dialogo di caricamento.</p> <p>Carica il certificato per utilizzare TLS con il certificato autofirmato. [!DNL Workfront Fusion] non conserva né archivia i dati forniti, ad esempio file e password. File e password vengono utilizzati solo per estrarre il certificato.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Moduli FTP e relativi campi

* [Triggers](#triggers)
* [Azioni](#actions)

### Triggers

#### [!UICONTROL Guarda i file]

[!UICONTROL Guarda i file] è l&#39;unico modulo di attivazione per l&#39;FTP. Controlla il contenuto del file della cartella selezionata. Il trigger viene eseguito quando un nuovo file viene inserito nella cartella specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come stabilire una connessione all'account FTP, vedi <a href="#create-a-connection" class="MCXref xref">[!UICONTROL Crea una connessione] in un modulo FTP</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Folder]</p> </td> 
   <td> <p>Seleziona la cartella da controllare.</p> <p><b>Nota:</b> È consentita una sola cartella per scenario. Le sottocartelle vengono ignorate.</p> <p><b>Suggerimento</b> Per tenere traccia di più cartelle, crea uno scenario indipendente per ciascuna di esse.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di file restituiti] </td> 
   <td> <p>Imposta il numero massimo di risultati che [!DNL Workfront Fusion] funzionerà con durante un ciclo. Se il valore è impostato su un valore troppo alto, la connessione potrebbe essere interrotta sul lato del servizio di terze parti specificato (timeout). [!DNL Workfront Fusion] non ha alcuna influenza su questo. È consigliabile impostare un valore più basso e definire un valore più alto per il numero massimo di cicli oppure eseguire lo scenario più frequentemente.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Modificare le autorizzazioni]](#change-permissions)
* [[!UICONTROL Creare una cartella]](#create-a-folder)
* [[!UICONTROL Eliminare un file]](#delete-a-file)
* [[!UICONTROL Eliminare una cartella]](#delete-a-folder)
* [[!UICONTROL Ottieni un file]](#get-a-file)
* [[!UICONTROL Elenco dei file in una cartella]](#list-of-files-in-a-folder)
* [[!UICONTROL Spostare un file o una cartella]](#move-a-file-or-folder)
* [[!UICONTROL Carica] un file](#upload-a-file)

#### [!UICONTROL Modificare le autorizzazioni]

Questo modulo di azione modifica le impostazioni delle autorizzazioni di un file o di una cartella.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Per istruzioni su come stabilire una connessione all'account FTP, vedi <a href="#Create" class="MCXref xref" >[!UICONTROL Crea una connessione] in un modulo FTP</a> in questo articolo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL Modifica le impostazioni delle autorizzazioni di]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">
               <p>Specificare se si desidera modificare le impostazioni di un file o di una cartella.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Percorso file]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Immettere o mappare il percorso del file alla cartella o al file.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Permissions]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
               <p>Imposta le autorizzazioni per il file o la cartella desiderate. Utilizzare i parametri chmod. Ad esempio: <code>777 </code>o <code>-rwxrwxrwx</code>.</p>
               <p>Le autorizzazioni devono corrispondere al pattern <code> /(.?([r-][w-][x-]){3})|[0-7]{3,4}/</code>.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Creare una cartella]

Questo modulo di azione crea una nuova cartella.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Per istruzioni su come stabilire una connessione all'account FTP, vedi <a href="#Create" class="MCXref xref" >[!UICONTROL Crea una connessione] in un modulo FTP</a> in questo articolo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL Percorso cartella]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Immettere o mappare il percorso del file alla nuova cartella.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL Nome nuova cartella]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">
               <p>Immettere o mappare un nome per la nuova cartella.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Eliminare un file]

Elimina un file dalla cartella specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Per istruzioni su come stabilire una connessione all'account FTP, vedi <a href="#Create" class="MCXref xref" >[!UICONTROL Crea una connessione] in un modulo FTP</a> in questo articolo.</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selezionare la cartella FTP da cui si desidera eliminare un file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome file]</td> 
   <td> <p> Immettere il nome del file, inclusa l'estensione. Esempio: <code>[!DNL image].png</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare una cartella]

Questo modulo di azione elimina definitivamente la cartella specificata.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Per istruzioni su come stabilire una connessione all'account FTP, vedi <a href="#Create" class="MCXref xref" >[!UICONTROL Crea una connessione] in un modulo FTP</a> in questo articolo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL Folder]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">
               <p>Selezionare la cartella FTP da cui si desidera eliminare un file.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Ottieni un file]

Recupera un file dal server FTP che può essere ulteriormente elaborato, ad esempio caricato in [!DNL Dropbox].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come stabilire una connessione all'account FTP, vedi <a href="#creating-the-ftp-connection" class="MCXref xref">Creazione della connessione FTP</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percorso file]</td> 
   <td> <p> Immettere il percorso del file che si desidera ottenere.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenco dei file in una cartella]

Recupera le informazioni sul file e/o sulla cartella.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come stabilire una connessione all'account FTP, vedi <a href="#creating-the-ftp-connection" class="MCXref xref">Creazione della connessione FTP</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleziona la cartella FTP in cui desideri eseguire la ricerca.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show] </td> 
   <td> <p>Specificare se si desidera recuperare informazioni su file, cartelle o entrambi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL - Ricerca] </td> 
   <td> <p>Immettere il termine di ricerca. Se non viene immesso alcun termine di ricerca, verranno recuperati tutti i file e le cartelle della cartella specificata.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di file restituiti]</td> 
   <td> <p> Imposta il numero massimo di file recuperati da questo modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Spostare un file o una cartella]

Questo modulo di azione sposta un file o una cartella in una posizione diversa.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Per istruzioni su come stabilire una connessione all'account FTP, vedi <a href="#Create" class="MCXref xref" >[!UICONTROL Crea una connessione] in un modulo FTP</a> in questo articolo.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL Percorso file precedente]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">
               <p>Immettere il percorso da cui si desidera spostare il file. Esempio: <code>/folder1/document.txt</code>.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Percorso nuovo file]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">
               <p>Immettere il percorso in cui spostare il file. Esempio: <code>/folder2/document.txt</code>.</p>
            </td>
         </tr>
   </tbody>
</table>


#### [!UICONTROL Carica un file]

Carica un file sul server FTP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come stabilire una connessione all'account FTP, vedi <a href="#creating-the-ftp-connection" class="MCXref xref">Creazione della connessione FTP</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selezionare la cartella FTP in cui si desidera caricare il file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File di origine] </td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggiungi a un file già esistente]</td> 
   <td> <p>Se questa opzione è abilitata e il file esiste già sul server FTP, il contenuto del file viene aggiunto al file esistente. Se questa opzione non è abilitata, il contenuto del file verrà sovrascritto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Crea cartelle se non esiste] </td> 
   <td> <p>Se questa opzione è abilitata e la cartella immessa nel campo Cartella non esiste sul server FTP, il modulo crea la cartella</p> </td> 
  </tr> 
 </tbody> 
</table>

## Risoluzione dei problemi {#troubleshooting}

Se riscontri problemi con l’app FTP durante la creazione della connessione o durante l’operazione di un modulo, prova a utilizzare uno dei client FTP più diffusi e prova a eseguire la stessa azione (ad esempio, crea una connessione o elenca i file in una cartella). con il client FTP. Se si verificano gli stessi problemi anche con il client FTP, il motivo potrebbe essere una configurazione errata del server FTP.
