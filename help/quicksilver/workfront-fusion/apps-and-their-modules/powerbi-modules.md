---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Power BI
description: Adobe Workfront Fusion richiede una licenza Adobe Workfront Fusion oltre a una licenza Adobe Workfront.
author: Becky
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '2398'
ht-degree: 0%

---

# [!DNL Power BI] Moduli

[!DNL Power BI] è un’applicazione che ti consente di visualizzare e presentare i dati alle parti interessate. Può acquisire dati da diverse fonti.

>[!NOTE]
>
>[!DNL Workfront Fusion] non è un’origine dati. Mentre [!DNL Workfront Fusion] può creare e utilizzare origini dati, non memorizza i dati.


## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!DNL Pro] o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!DNL Plan], [!DNL Work]</p> </td> 
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

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

&#42;&#42;Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!DNL Power BI] moduli e relativi campi

Quando si configura [!DNL Power BI], [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati campi aggiuntivi, a seconda di fattori come il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Dashboard

#### [!UICONTROL Elenca dashboard]

Questo modulo di ricerca recupera un elenco di dashboard.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID gruppo]  </td>
      <td>
        <p>Seleziona o mappa l’ID del gruppo a cui appartengono le dashboard che desideri elencare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Elencare riquadri del dashboard]

Questo modulo di ricerca recupera un elenco di riquadri del dashboard.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Inserisci un ID dashboard]</td>
    <td>
      <p>Seleziona o mappa l’opzione per scegliere il dashboard di cui desideri elencare le tessere.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Dashboard ID]</td>
    <td>
      <p>Inserisci o mappa l’ID del dashboard contenente le tessere che desideri elencare.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ID gruppo]  </td>
    <td>Seleziona o mappa l’ID del Gruppo a cui appartengono le dashboard contenenti le tessere che desideri elencare.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Limit]  </td>
    <td>
      <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Ottieni un dashboard]

Questo modulo di azione recupera i metadati di un dashboard specificato.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserisci un ID dashboard]</td>
      <td>
        <p>Seleziona o mappa l’opzione per scegliere il dashboard per il quale desideri recuperare i metadati.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard ID]</td>
      <td>
        <p>Inserisci o mappa l’ID del dashboard per cui desideri recuperare i metadati.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID gruppo]  </td>
      <td>Seleziona o mappa l’ID del gruppo a cui appartengono le dashboard per le quali desideri recuperare i metadati.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ottieni sezione dashboard]

Questo modulo di azione recupera i metadati di una sezione del dashboard specificata.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserisci un ID dashboard]</td>
      <td>
        <p>Seleziona o mappa l’opzione per scegliere i dettagli del dashboard da recuperare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard ID]</td>
      <td>
        <p>Immetti o mappa l’ID del dashboard per il quale desideri recuperare i dettagli.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tile ID]</td>
      <td>Inserisci o mappa l’ID del [!DNL Power BI] riquadro per cui desideri recuperare i dettagli.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID gruppo]  </td>
      <td>Seleziona o mappa l’ID del gruppo a cui appartiene la sezione da recuperare.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Creare un dashboard]

Questo modulo di azione crea un nuovo dashboard.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Immettete o mappate un nome per il dashboard.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID gruppo]  </td>
      <td>Seleziona o mappa l’ID del gruppo proprietario del nuovo dashboard.</td>
    </tr>
  </tbody>
</table>

### Report

#### [!UICONTROL Elencare rapporti]

Questo modulo di ricerca recupera un elenco di rapporti.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID gruppo]  </td>
      <td>
        <p>Seleziona o mappa l’ID del gruppo a cui appartengono i rapporti che desideri elencare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ottieni un rapporto]

Questo modulo di azione recupera i metadati di un rapporto specificato.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserisci un ID report]</td>
      <td>
        <p>Seleziona o mappa l’opzione per scegliere il rapporto per il quale desideri recuperare i metadati.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID report]</td>
      <td>
        <p>Inserisci o mappa l’ID del rapporto per il quale desideri recuperare i metadati.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID gruppo]  </td>
      <td>Seleziona o mappa l’ID del gruppo a cui appartiene il rapporto per il quale desideri recuperare i metadati.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Copiare un rapporto]

Questo modulo di azione copia un rapporto esistente.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserisci un ID report]</td>
      <td>
        <p>Seleziona o mappa l’opzione per scegliere il rapporto da copiare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID report]</td>
      <td>
        <p>Inserisci o mappa l’ID del rapporto da copiare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID gruppo]  </td>
      <td>Seleziona o mappa l’ID del gruppo a cui appartiene il rapporto da copiare.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nome nuovo report copiato]</td>
      <td>Immettere o mappare un nome per il nuovo rapporto.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminare un rapporto]

Questo modulo di azione elimina un rapporto.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserisci un ID report]</td>
      <td>
        <p>Seleziona o mappa l’opzione per scegliere il rapporto da eliminare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID report]</td>
      <td>
        <p>Inserisci o mappa l’ID del rapporto da eliminare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID gruppo]  </td>
      <td>Seleziona o mappa l’ID del gruppo proprietario del rapporto che desideri eliminare.</td>
    </tr>
  </tbody>
</table>

### Set di dati

#### [!UICONTROL Elencare set di dati]

Questo modulo di ricerca recupera un elenco di set di dati.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID gruppo]  </td>
      <td>Seleziona o mappa l’ID del gruppo a cui appartiene il rapporto per il quale desideri recuperare i metadati.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>
        <p>Immettere o mappare il numero massimo di record che si desidera vengano inseriti nel modulo in [action] durante ogni ciclo di esecuzione dello scenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ottenere un set di dati]

Questo modulo di azione recupera i metadati di un set di dati specificato.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserisci un ID report]</td>
      <td>
        <p>Seleziona o mappa l’opzione per scegliere il rapporto per il quale desideri recuperare i metadati.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID report]</td>
      <td>
        <p>Inserisci o mappa l’ID del set di dati per il quale desideri recuperare i metadati.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID gruppo]  </td>
      <td>Seleziona o mappa l’ID del gruppo a cui appartiene il set di dati per il quale desideri recuperare i metadati.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Creare un set di dati]

Questo modulo di azione crea un nuovo set di dati.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Inserisci o mappa un nome per il set di dati.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID gruppo]  </td>
      <td>Seleziona o mappa l’ID del gruppo proprietario del nuovo set di dati.</td>
    </tr>
    <tr>
      <td role="rowheader">Modalità predefinita [!UICONTROL]</td>
      <td>
        <p>Seleziona o mappa la modalità predefinita per il set di dati:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Come Azure]</b>: set di dati con una connessione live a [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[!UICONTROL come in Prem]</b>: set di dati con una connessione live a [!DNL On-premise Analysis] Servizio</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>: set di dati che consente l’accesso programmatico per la trasmissione di dati in [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>: set di dati che supporta lo streaming di dati e consente l’accesso programmatico per la trasmissione di dati in [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>: set di dati che supporta lo streaming di dati</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tabelle]</td>
      <td>Aggiungi tabelle al set di dati. Per i campi, consulta <a href="#Table" class="MCXref_0">Campi tabella</a></td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Data sources]</td>
      <td>Aggiungi le origini dati. Per i campi, consulta <a href="#Data" class="MCXref_0">Campi origini dati</a>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Default Retention Policy]  </td>
      <td>
        <p>Seleziona o mappa il criterio intenzionale per il set di dati:</p>
        <ul>
          <li>
            <p>[!UICONTROL Nessuno]</p>
          </li>
          <li>
            <p>[!UICONTROL FIFO di base]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Campi tabella

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>
        <p>  Immettere o mappare un nome per la tabella.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Colonne]</td>
      <td>
        <p>Aggiungi le colonne:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Immetti (mappare) un nome di colonna.</p>
          </li>
          <li>
            <p><b>Tipo di dati [!UICONTROL]</b>
            </p>
            <p>Selezionare o mappare il tipo di dati:</p>
            <ul>
              <li>
                <p>[!UICONTROL Stringa]</p>
              </li>
              <li>
                <p>[!UICONTROL Integer]</p>
              </li>
              <li>
                <p>[!UICONTROL Boolean]</p>
              </li>
              <li>
                <p>[!UICONTROL Date Time]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>[!UICONTROL Format String]</b>
            </p>
            <p>Immetti (mappa) la stringa di formato.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rows]</td>
      <td>Immetti o mappa i dettagli della riga.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Misure]</td>
      <td>Aggiungere la misura per le tabelle.</td>
    </tr>
  </tbody>
</table>

##### Campi origini dati

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Database [!UICONTROL]  </td>
      <td>
        <p>Immettere o mappare il database che si desidera utilizzare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Server]  </td>
      <td>
        <p>Immettere o mappare il nome del server che si desidera utilizzare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]  </td>
      <td>
        <p>Inserisci o mappa l’URL da utilizzare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID origine dati]</td>
      <td>
        <p>  Immetti o mappa l’ID dell’origine dati.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Tipo di origine dati [!UICONTROL]  </td>
      <td>
        <p>Selezionare o mappare il tipo di origine dati. Esempio: SQL.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID gateway]  </td>
      <td>Immettere o mappare l'ID del gateway che si desidera utilizzare.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Aggiungere o eliminare righe in una tabella di set di dati]

Questo modulo di azione aggiunge o elimina righe di una tabella di set di dati push specificata.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Immettere una tabella]</td>
      <td>Seleziona o mappa l’opzione per selezionare il set di dati contenente la tabella da regolare.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID set di dati]</td>
      <td>Inserisci o mappa l’ID del set di dati contenente le righe da aggiungere o eliminare.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nome Tabella]  </td>
      <td>
        <p>Immettere o mappare il nome della tabella contenente le righe che si desidera aggiungere o eliminare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID gruppo]  </td>
      <td>Inserisci o mappa l’ID del gruppo proprietario del set di dati.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Seleziona azione]</td>
      <td>
        <p>Seleziona o mappa l’azione da eseguire.</p>
        <ul>
          <li>
            <p>[!UICONTROL Aggiungi righe]</p>
          </li>
          <li>
            <p>[!UICONTROL Elimina tutte le righe]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rows]</td>
      <td>
        <p>Aggiungi i campi riga.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Key]</b>
            </p>
            <p>Immetti o mappa il nome della chiave.</p>
          </li>
          <li>
            <p><b>Tipo di campo [!UICONTROL]</b>
            </p>
            <p>Seleziona o mappa il tipo di campo:</p>
            <ul>
              <li>
                <p>Booleano</p>
              </li>
              <li>
                <p>Data</p>
              </li>
              <li>
                <p>Testo</p>
              </li>
              <li>
                <p>Numero</p>
              </li>
            </ul>
          </li>
          <li>
            <p>Valore [!UICONTROL]</p>
            <p>Immetti o mappa il valore chiave.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Aggiornare un set di dati]

Questo modulo di azione aggiorna un set di dati specificato.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Immettere un set di dati]</td>
      <td>Seleziona o mappa l’opzione per selezionare il set di dati da aggiornare.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID set di dati]</td>
      <td>Immetti o mappa l’ID del set di dati da aggiornare.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nome Tabella]  </td>
      <td>
        <p>Immettere o mappare il nome della tabella contenente le righe che si desidera aggiungere o eliminare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID gruppo]  </td>
      <td>Inserisci o mappa l’ID del gruppo proprietario del set di dati.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Opzione Notify]  </td>
      <td>
        <p>Seleziona o mappa l’opzione per la notifica:</p>
        <ul>
          <li>
            <p>[!UICONTROL Mail al completamento]</p>
          </li>
          <li>
            <p>[!UICONTROL Mail on Failure]</p>
          </li>
          <li>
            <p>[!UICONTROL Nessuna notifica]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminare un set di dati]

Questo modulo di azione elimina un set di dati.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserisci un ID report]</td>
      <td>
        <p>Seleziona o mappa l’opzione per scegliere il set di dati da eliminare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID report]</td>
      <td>
        <p>Inserisci o mappa l’ID del set di dati da eliminare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID gruppo]  </td>
      <td>Seleziona o mappa l’ID del gruppo proprietario del set di dati da eliminare.</td>
    </tr>
  </tbody>
</table>

### App

#### [!UICONTROL Guarda le app]

Questo modulo di attivazione avvia uno scenario quando un’app viene aggiornata.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Elenca app]

Questo modulo di ricerca recupera un elenco di tutte le app installate.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Elencare i rapporti dell’app]

Questo modulo di ricerca recupera un elenco di tutti i rapporti dall’app specificata.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID app]</td>
      <td>Seleziona o mappa l’ID dell’app da cui desideri elencare i rapporti.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Elencare dashboard dell’app]

Questo modulo di ricerca recupera un elenco di dashboard da un’app specificata.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID app]</td>
      <td>Seleziona o mappa l’ID dell’app da cui desideri elencare le dashboard.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ottieni un’app]

Questo modulo di azione recupera i metadati di un’app specificata.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID app]  </td>
      <td>
        <p>Seleziona o mappa l’ID dell’app da recuperare.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ottenere un rapporto dell’app]

Questo modulo di azione recupera i metadati del rapporto di un’app specificata.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID app]  </td>
      <td>
        <p>Seleziona o mappa l’ID dell’app che contiene il rapporto da recuperare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID report]</td>
      <td>
        <p>  Seleziona o mappa l’ID del rapporto che desideri recuperare.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ottieni dashboard di un’app]

Questo modulo di azione recupera i metadati del dashboard di un’app specificata.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID app]  </td>
      <td>
        <p>Seleziona o mappa l’ID dell’app che contiene il dashboard da recuperare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID report]</td>
      <td>
        <p>  Seleziona o mappa l’ID del dashboard che desideri recuperare.</p>
      </td>
    </tr>
  </tbody>
</table>

### Altro

#### [!UICONTROL Effettuare una chiamata API]

Questo modulo di azione esegue una chiamata API al [!DNL Power BI] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Inserisci un percorso relativo a <code>https://api.powerbi.com</code>. Esempio: <code>/v1.0/myorg/datasets</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
      <td>
        <p>Seleziona il metodo di richiesta [!UICONTROL HTTP] necessario per configurare la chiamata API. Per ulteriori informazioni, vedere Metodi di richiesta [!UICONTROL HTTP].</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p>
        <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione e le intestazioni x-api-key.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stringa Di Query]  </td>
      <td>
        <p>Immettere la stringa di query richiesta.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali quali <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
