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
source-git-commit: 30e9b175e29acaed638f005eb6a701777f65e0bc
workflow-type: tm+mt
source-wordcount: '2352'
ht-degree: 0%

---

# [!DNL Power BI] Moduli

[!DNL Power BI] è un’applicazione che ti consente di visualizzare e presentare i dati alle tue parti interessate. Può prendere dati da diverse fonti.

>[!NOTE]
>
>[!DNL Workfront Fusion] non è un&#39;origine dati. Quando [!DNL Workfront Fusion] può creare e utilizzare origini dati, non memorizza i dati.


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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

&#42;&#42;Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!DNL Power BI] moduli e relativi campi

Quando si configura [!DNL Power BI], [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati campi aggiuntivi, a seconda di fattori come il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all&#39;altro in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Dashboard

#### [!UICONTROL Dashboard a elenco]

Questo modulo di ricerca recupera un elenco di dashboard.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>
        <p>Seleziona o mappa l’ID del gruppo proprietario delle dashboard da elencare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Elenca riquadri del dashboard]

Questo modulo di ricerca recupera un elenco di riquadri del dashboard.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Immettere un ID dashboard]</td>
    <td>
      <p>Selezionare o mappare l’opzione per scegliere il dashboard di cui si desidera elencare i riquadri.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Dashboard ID]</td>
    <td>
      <p>Immetti o mappa l’ID del dashboard contenente i riquadri che desideri elencare.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Group ID]  </td>
    <td>Seleziona o mappa l’ID del gruppo proprietario delle dashboard contenenti i riquadri che desideri elencare.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Limit]  </td>
    <td>
      <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Ottenere un dashboard]

Questo modulo di azione recupera i metadati di un dashboard specificato.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Immettere un ID dashboard]</td>
      <td>
        <p>Seleziona o mappa l’opzione per scegliere il dashboard per il quale desideri recuperare i metadati.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard ID]</td>
      <td>
        <p>Immetti o mappa l’ID del dashboard per il quale desideri recuperare i metadati.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleziona o mappa l’ID del gruppo a cui appartengono le dashboard per le quali desideri recuperare i metadati.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ottenere un riquadro del dashboard]

Questo modulo di azione recupera i metadati di un riquadro del dashboard specificato.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Immettere un ID dashboard]</td>
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
      <td>Immettere o mappare l'ID del [!DNL Power BI] riquadro per cui desideri recuperare i dettagli.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleziona o mappa l’ID del gruppo a cui appartiene il riquadro che desideri recuperare.</td>
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
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Immetti o mappa un nome per il dashboard.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleziona o mappa l’ID del gruppo proprietario del nuovo dashboard.</td>
    </tr>
  </tbody>
</table>

### Report

#### [!UICONTROL Report elenco]

Questo modulo di ricerca recupera un elenco di rapporti.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>
        <p>Seleziona o mappa l’ID del gruppo a cui appartengono i rapporti che desideri elencare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ottieni un rapporto]

Questo modulo di azione recupera i metadati di un report specificato.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Immettere un ID rapporto]</td>
      <td>
        <p>Seleziona o mappa l’opzione per scegliere il rapporto per il quale desideri recuperare i metadati.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">ID rapporto</td>
      <td>
        <p>Immetti o mappa l’ID del rapporto per il quale desideri recuperare i metadati.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
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
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Immettere un ID rapporto]</td>
      <td>
        <p>Seleziona o mappa l’opzione per scegliere il rapporto da copiare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">ID rapporto</td>
      <td>
        <p>Immettere o mappare l'ID del rapporto che si desidera copiare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleziona o mappa l’ID del gruppo a cui appartiene il rapporto che desideri copiare.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nuovo Nome Report Copiato]</td>
      <td>Immettere o mappare un nome per il nuovo rapporto.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminare un rapporto]

Questo modulo di azione elimina un report.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Immettere un ID rapporto]</td>
      <td>
        <p>Seleziona o mappa l’opzione per scegliere il rapporto da eliminare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">ID rapporto</td>
      <td>
        <p>Immettere o mappare l'ID del rapporto che si desidera eliminare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleziona o mappa l’ID del gruppo a cui appartiene il rapporto da eliminare.</td>
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
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleziona o mappa l’ID del gruppo a cui appartiene il rapporto per il quale desideri recuperare i metadati.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>
        <p>Immettere o mappare il numero massimo di record che si desidera che il modulo [action] venga utilizzato durante ogni ciclo di esecuzione di uno scenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ottieni un set di dati]

Questo modulo di azione recupera i metadati di un set di dati specificato.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Immettere un ID rapporto]</td>
      <td>
        <p>Seleziona o mappa l’opzione per scegliere il rapporto per il quale desideri recuperare i metadati.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">ID rapporto</td>
      <td>
        <p>Immetti o mappa l’ID del set di dati per il quale desideri recuperare i metadati.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleziona o mappa l’ID del gruppo proprietario del set di dati per il quale desideri recuperare i metadati.</td>
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
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Immetti o mappa un nome per il set di dati.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleziona o mappa l’ID del gruppo proprietario del nuovo set di dati.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Modalità predefinita]</td>
      <td>
        <p>Seleziona o mappa la modalità predefinita per il set di dati:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL As Azure]</b>: Un set di dati con una connessione in tempo reale a [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[!UICONTROL As on Prem]</b>: Un set di dati con una connessione in tempo reale a [!DNL On-premise Analysis] Servizio</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>: Un set di dati che consente l’accesso programmatico per l’invio di dati in [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>: Un set di dati che supporta lo streaming dei dati e consente l’accesso programmatico per l’invio di dati in [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>: Un set di dati che supporta lo streaming di dati</p>
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
            <p>[!UICONTROL FIFO DI BASE]</p>
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
      <td role="rowheader">[!UICONTROL Columns]</td>
      <td>
        <p>Aggiungi le colonne:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Inserisci (mappa) un nome di colonna.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Data Type]</b>
            </p>
            <p>Seleziona o mappa il tipo di dati:</p>
            <ul>
              <li>
                <p>[!UICONTROL String]</p>
              </li>
              <li>
                <p>[!UICONTROL Integer]</p>
              </li>
              <li>
                <p>[!UICONTROL Boolean]</p>
              </li>
              <li>
                <p>[!UICONTROL Data e ora]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>[!UICONTROL Formato String]</b>
            </p>
            <p>Immettere (mappare) la stringa di formato.</p>
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
      <td>Aggiungi la misura per le tabelle.</td>
    </tr>
  </tbody>
</table>

##### Campi origini dati

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Database]  </td>
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
      <td role="rowheader">[!UICONTROL Data Source ID]</td>
      <td>
        <p>  Immetti o mappa l’ID dell’origine dati.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo di origine dati]  </td>
      <td>
        <p>Seleziona o mappa il tipo di origine dati. Esempio: SQL.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gateway ID]  </td>
      <td>Immettere o mappare l'ID del gateway che si desidera utilizzare.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Aggiungere o eliminare righe in una tabella di set di dati]

Questo modulo di azione aggiunge o elimina le righe di una tabella di set di dati push specificata.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserisci una tabella]</td>
      <td>Seleziona o mappa l’opzione per selezionare il set di dati contenente la tabella da regolare.</td>
    </tr>
    <tr>
      <td role="rowheader">ID set di dati [!UICONTROL]</td>
      <td>Immetti o mappa l’ID del set di dati contenente le righe che desideri aggiungere o eliminare.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Table Name]  </td>
      <td>
        <p>Immettere o mappare il nome della tabella contenente le righe che si desidera aggiungere o eliminare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Immetti o mappa l’ID del gruppo proprietario del set di dati.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Seleziona l’azione]</td>
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
            <p>Immettere o mappare il nome della chiave.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Tipo di campo]</b>
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
            <p>[!UICONTROL Value]</p>
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
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Immettere un set di dati]</td>
      <td>Seleziona o mappa l’opzione per selezionare il set di dati da aggiornare.</td>
    </tr>
    <tr>
      <td role="rowheader">ID set di dati [!UICONTROL]</td>
      <td>Immetti o mappa l’ID del set di dati da aggiornare.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Table Name]  </td>
      <td>
        <p>Immettere o mappare il nome della tabella contenente le righe che si desidera aggiungere o eliminare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Immetti o mappa l’ID del gruppo proprietario del set di dati.</td>
    </tr>
    <tr>
      <td role="rowheader">Opzione di notifica [!UICONTROL]  </td>
      <td>
        <p>Seleziona o mappa l’opzione per la notifica:</p>
        <ul>
          <li>
            <p>[!UICONTROL Posta al completamento]</p>
          </li>
          <li>
            <p>[!UICONTROL Mail in caso di errore]</p>
          </li>
          <li>
            <p>[!UICONTROL Nessuna Notifica]</p>
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
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Immettere un ID rapporto]</td>
      <td>
        <p>Seleziona o mappa l’opzione per scegliere il set di dati da eliminare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">ID rapporto</td>
      <td>
        <p>Immetti o mappa l’ID del set di dati da eliminare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleziona o mappa l’ID del gruppo proprietario del set di dati da eliminare.</td>
    </tr>
  </tbody>
</table>

### App

#### [!UICONTROL App di controllo]

Questo modulo di attivazione avvia uno scenario quando un’app viene aggiornata.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Elencare app]

Questo modulo di ricerca recupera un elenco di tutte le app installate.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Elencare i report dell&#39;app]

Questo modulo di ricerca recupera un elenco di tutti i rapporti dall’app specificata.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>Seleziona o mappa l’ID dell’app da cui vuoi elencare i rapporti.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Elencare dashboard dell&#39;app]

Questo modulo di ricerca recupera un elenco di dashboard da una specifica app.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>Seleziona o mappa l’ID dell’app da cui vuoi elencare le dashboard.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ottenere un’app]

Questo modulo di azione recupera i metadati di una specifica app.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Seleziona o mappa l’ID dell’app da recuperare.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ottieni un rapporto dell’app]

Questo modulo di azione recupera i metadati del rapporto di una specifica app.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Seleziona o mappa l'ID dell'app che contiene il rapporto che desideri recuperare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">ID rapporto</td>
      <td>
        <p>  Seleziona o mappa l’ID del rapporto che desideri recuperare.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ottieni dashboard di un&#39;app]

Questo modulo di azione recupera i metadati del dashboard di una specifica app.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Seleziona o mappa l’ID dell’app che contiene il dashboard da recuperare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">ID rapporto</td>
      <td>
        <p>  Seleziona o mappa l’ID del dashboard da rivivere.</p>
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
   <td> <p>Per istruzioni su come collegare le [!DNL Power BI] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Immettere un percorso relativo a <code>https://api.powerbi.com</code>. Esempio: <code>/v1.0/myorg/datasets</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL, Metodo]</p>
      </td>
      <td>
        <p>Seleziona il metodo di richiesta [!UICONTROL HTTP] necessario per configurare la chiamata API. Per ulteriori informazioni, consulta Metodi di richiesta [!UICONTROL HTTP].</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p>
        <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] aggiunge automaticamente intestazioni di autorizzazione e intestazioni x-api-key.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Immetti la stringa di query della richiesta.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
