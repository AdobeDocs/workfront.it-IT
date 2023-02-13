---
title: Moduli CRM HubSpot
description: La [!DNL Adobe Workfront Fusion] I moduli di gestione delle relazioni con i clienti di HubSpot consentono di monitorare gli eventi, i record, i contatti, i contatti, i coinvolgimenti, i file e gli invii, oppure di creare, recuperare, aggiornare ed eliminare record, contatti, coinvolgimenti, eventi o file nel tuo [!DNL HubSpot CRM] conto.
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2485'
ht-degree: 0%

---

# [!DNL HubSpot CRM] moduli

La [!DNL Adobe Workfront Fusion] [!DNL HubSpot CRM] I moduli consentono di monitorare eventi, record, contatti, impegni, file e moduli inviati oppure di creare, recuperare, aggiornare ed eliminare record, contatti, impegni, eventi o file nel [!DNL HubSpot CRM] conto.

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

Per utilizzare [!DNL HubSpot CRM] moduli, è necessario disporre di un [!DNL HubSpot CRM] conto.

## Connetti [!DNL Adobe Workfront Fusion] a [!DNL HubSpot CRM]

Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi [Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL HubSpot CRM] moduli e relativi campi

Quando si configura [!DNL Hubspot CRM] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Hubspot CRM] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Oggetti CRM](#crm-objects)
* [Record (Offerte, Contatti e Aziende)](#records-deals-contacts-and-companies)
* [Conttati](#contacts)
* [Offerte](#deals)
* [Aziende](#companies)
* [File](#files)
* [Biglietti](#tickets)
* [Effettuare una chiamata API](#make-an-api-call)

### Oggetti CRM

#### [!UICONTROL Cerca oggetti CRM]

Questo modulo di ricerca cerca gli oggetti CRM per proprietà personalizzate o per query. Per cercare prodotti o elementi di riga, utilizza una connessione speciale con un ambito personalizzato richiesto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di elementi che il modulo restituirà in un ciclo di esecuzione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di oggetto da cercare]</td> 
   <td>Selezionare il tipo di oggetto CRM di hub che si desidera cercare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Proprietà di output]</td> 
   <td>Selezionare le proprietà che si desidera visualizzare nell'output del modulo. I campi disponibili dipendono dall’oggetto selezionato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtra per] </td> 
   <td> <p>Selezionare la modalità di filtro della ricerca</p> 
    <ul> 
     <li> <p><strong>Query [!UICONTROL]</strong> </p> <p>Immettere o mappare la query</p> </li> 
     <li> <p><strong>[!UICONTROL Properties]</strong> </p> <p>Inserisci i gruppi o i filtri per la ricerca.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina per]</td> 
   <td> <p>Fai clic su se desideri ordinare i risultati. Se si sceglie di ordinare i risultati, vengono visualizzati i campi seguenti. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome proprietà]</strong> </p> <p>Selezionare la proprietà in base alla quale si desidera ordinare i risultati</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>Scegli se ordinare i risultati in una direzione ascendente o decrescente.</p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Start Offset</td> 
    <td>Enter or map the ID of the first item you want to retrieve details for. This module only returns up to 5000 results at a time. Setting a start offset allows you to retrieve items other than the first 5000. If the start offset is 5000, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

### Record (Offerte, Contatti e Aziende)

* [[!UICONTROL Creare un record (legacy)]](#create-a-record-legacy)
* [[!UICONTROL Ottieni un record]](#get-a-record)
* [[!UICONTROL Aggiornare un record]](#update-a-record)
* [[!UICONTROL Eliminare un record]](#delete-a-record)
* [[!UICONTROL Ottieni una proprietà record]](#get-a-record-property)
* [[!UICONTROL Registra record]](#watch-records)

#### [!UICONTROL Creare un record (legacy)]

Questo modulo di azione crea un contatto, un&#39;azienda o un&#39;offerta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record da creare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>Compila le proprietà che desideri impostare per il record. I campi disponibili dipendono dal tipo di record che si desidera creare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un record]

Questo modulo di azione ottiene i dettagli di un contatto, di un&#39;azienda o di un&#39;offerta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record.</p> 
    <ul> 
     <li>[!UICONTROL Contatto]</li> 
     <li>[!UICONTROL Company] </li> 
     <li>[!UICONTROL Deal]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search Type]</td> 
   <td>Se ricevi un contatto, seleziona se desideri identificarlo per ID o per indirizzo e-mail.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immetti l'ID del contatto, della società o dell'offerta che desideri recuperare. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">E-MAIL [!UICONTROL]</td> 
   <td>Immettere l'indirizzo e-mail del contatto di cui si desidera recuperare i dati. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un record]

Questo modulo di azione aggiorna un contatto, un&#39;azienda o un&#39;offerta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record da aggiornare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search Type]</td> 
   <td> <p>Se ricevi un contatto, seleziona come desideri identificare il record:</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> </li> 
     <li> <p>E-MAIL [!UICONTROL]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immetti l'ID del contatto, della società o dell'offerta che desideri aggiornare. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">E-MAIL [!UICONTROL]</td> 
   <td>Immettere l'indirizzo e-mail del contatto di cui si desidera aggiornare i dettagli. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>Compila le proprietà che desideri impostare per il record. I campi disponibili dipendono dal tipo di record che si desidera creare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un contatto, un&#39;azienda o un&#39;offerta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record da eliminare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immetti l’ID del contatto, della società o dell’offerta da eliminare. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni una proprietà record]

Questo modulo di azione ottiene i metadati per una specifica proprietà record dal nome (interno) corrispondente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record per il quale si desidera recuperare i metadati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome proprietà]</td> 
   <td>Seleziona la proprietà per la quale desideri recuperare i metadati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID opzione [!UICONTROL]</td> 
   <td> <p> Alcune proprietà dispongono di un set di opzioni disponibili che un utente può selezionare come valore della proprietà. Immetti l’ID dell’opzione che rappresenta il valore della proprietà che desideri recuperare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Registra record]

Questo modulo trigger avvia uno scenario in cui un contatto, un&#39;azienda o un&#39;offerta è stata modificata o creata negli ultimi 30 giorni. La produzione è limitata a 10.000 record.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record con la proprietà che si desidera controllare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Seleziona se visualizzare i record modificati di recente o creati di recente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Seleziona le proprietà da includere nell'output del modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Conttati

* [[!UICONTROL Creare/aggiornare un contatto (legacy)]](#createupdate-a-contact-legacy)
* [[!UICONTROL Creare/aggiornare un gruppo di contatti]](#createupdate-a-group-of-contacts)
* [[!UICONTROL Aggiungi contatti a un elenco]](#add-contacts-to-a-list)
* [[!UICONTROL Rimuovere un contatto da un elenco]](#remove-a-contact-from-a-list)
* [[!UICONTROL Unisci contatti]](#merge-contacts)
* [[!UICONTROL Cerca contatti]](#search-for-contacts)
* [[!UICONTROL Elenco contatti]](#list-contacts)
* [[!UICONTROL Elenco contatti di una società]](#list-contacts-of-a-company)

#### [!UICONTROL Creare/aggiornare un contatto (legacy)]

Crea un contatto se non esiste già in un portale o lo aggiorna con i valori delle proprietà più recenti se esiste in un portale.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>Compila le proprietà che desideri impostare o aggiornare per il contatto. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare/aggiornare un gruppo di contatti]

Crea un gruppo di contatti o li aggiorna se esistono già. Le prestazioni sono ottimali quando la dimensione del batch è limitata a 100 contatti o meno. Le modifiche apportate tramite questo endpoint vengono elaborate in modo asincrono, pertanto potrebbero essere necessari diversi minuti perché le modifiche vengano applicate ai record di contatto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Batch di contatti da creare/aggiornare] </td> 
   <td> <p>Aggiungi il batch di contatti.</p> <p>Fai clic su <strong>[!UICONTROL Aggiungi elemento]</strong> per aggiungere un nuovo contatto. Nella finestra visualizzata, immetti o mappa le seguenti informazioni:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Search Type]</strong> </p> <p>Selezionare la modalità di identificazione del contatto:</p> 
      <ul> 
       <li> <p>[!UICONTROL ID]</p> <p>Immettere l'ID del contatto che si desidera creare o aggiornare. </p> </li> 
       <li> <p>E-MAIL [!UICONTROL]</p> <p>Immettere l'indirizzo e-mail del contatto che si desidera creare o aggiornare. </p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Properties]</strong> </p> <p>Compila le proprietà che desideri impostare o aggiornare per il contatto.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungi contatti a un elenco]

Questo modulo aggiunge i record di contatto già creati nel sistema a un elenco di contatti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID] </td> 
   <td>Selezionare l'ID dell'elenco a cui si desidera aggiungere il contatto. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID/E-mail di [!UICONTROL] </td> 
   <td> <p>Selezionare la modalità di identificazione dei contatti che si desidera aggiungere all'elenco:</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> <p>Aggiungi gli ID dei contatti da aggiungere all'elenco.</p> </li> 
     <li> <p>E-mail [!UICONTROL]</p> <p>Aggiungi gli indirizzi e-mail dei contatti che desideri aggiungere all’elenco.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rimuovere un contatto da un elenco]

Rimuove un contatto da un elenco di contatti.

>[!NOTE]
>
>Non è possibile rimuovere manualmente i contatti da un elenco dinamico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID] </td> 
   <td>Selezionare l'ID dell'elenco da cui si desidera rimuovere il contatto. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact ID] </td> 
   <td>Immettere l'ID del contatto che si desidera rimuovere dall'elenco. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Unisci contatti]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 1] </td> 
   <td>Immettere l'ID di uno dei contatti che si desidera unire. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 2] </td> 
   <td>Immettere l'ID dell'altro contatto che si desidera unire.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cerca contatti]

Recupera un elenco di contatti utilizzando la query di ricerca.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query [!UICONTROL]</td> 
   <td>Inserisci la query di ricerca.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Immettere o mappare il numero massimo di contatti [!DNL Workfront Fusion] dovrebbe essere restituito durante un ciclo di esecuzione di uno scenario. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenco contatti]

Restituisce tutti i contatti creati nel portale. L&#39;output è limitato a 5000 contatti. Per elencare i contatti precedenti o successivi, puoi utilizzare la [!UICONTROL avanzato] per eseguire l&#39;offset dell&#39;elenco.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Numero massimo di contatti [!DNL Workfront Fusion] dovrebbe essere restituito durante un ciclo di esecuzione di uno scenario. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Proprietà di output]</td> 
   <td>Selezionare le proprietà che si desidera visualizzare nell'output del modulo. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Elenco contatti di una società]

Recupera un elenco di contatti nella società. L&#39;output è limitato a 5000 contatti. Per elencare i contatti precedenti o successivi, puoi utilizzare la [!UICONTROL avanzato] per eseguire l&#39;offset dell&#39;elenco.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immettere l'ID della società di cui si desidera elencare i contatti. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Numero massimo di contatti [!DNL Workfront Fusion] dovrebbe essere restituito durante un ciclo di esecuzione di uno scenario. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Controlla i contatti aggiunti a un elenco]

Questo modulo di attivazione avvia uno scenario in cui viene aggiunto un nuovo contatto a un elenco. Questa opzione è disponibile solo per gli utenti con un account marketing a pagamento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Immettere o mappare l'ID dell'elenco contenente i contatti che si desidera visualizzare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Seleziona le proprietà da includere nell'output del modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Offerte

* [[!UICONTROL Elenco transazioni/biglietti]](#list-dealticket-pipelines)
* [[!UICONTROL Ottieni una pipeline CRM di un accordo]](#get-a-deals-crm-pipeline)

#### [!UICONTROL Elenco transazioni/biglietti]

Restituisce tutte le pipeline delle offerte e dei ticket per un portale specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di oggetto] </td> 
   <td>Seleziona se desideri elencare offerte o biglietti.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni una pipeline CRM di un accordo]

Restituisce una pipeline di offerta specifica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID pipeline [!UICONTROL] </td> 
   <td>Immetti o mappa l’ID della pipeline per la quale desideri recuperare i dettagli. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stage ID] </td> 
   <td>Immetti o mappa l’ID della fase per la quale desideri recuperare i dettagli. </td> 
  </tr> 
 </tbody> 
</table>

### Aziende

#### [!UICONTROL Cerca società per dominio]

Recupera un elenco di aziende in base a una corrispondenza esatta alla proprietà del dominio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Domain] </td> 
   <td>Immetti il dominio delle società che desideri cercare, ad esempio <code>[!DNL hubspot].com</code>. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Il numero massimo di società [!DNL Workfront Fusion] dovrebbe essere restituito durante un ciclo di esecuzione di uno scenario. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Proprietà di output]</td> 
   <td>Selezionare le proprietà che si desidera visualizzare nell'output del modulo. </td> 
  </tr> 
 </tbody> 
</table>

### File

* [[!UICONTROL Creare una cartella]](#create-a-folder)
* [[!UICONTROL Eliminare una cartella]](#delete-a-folder)
* [[!UICONTROL Sposta un file]](#move-a-file)

#### [!UICONTROL Creare una cartella]

Questo modulo crea una cartella.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome cartella] </td> 
   <td>Immettere o mappare un nome per la nuova cartella.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID cartella padre] </td> 
   <td>Selezionare l'ID della cartella principale per la cartella che si sta creando. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare una cartella]

Contrassegna una cartella come eliminata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immetti l’ID della cartella da eliminare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sposta un file]

Sposta un file in una cartella diversa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID] </td> 
   <td>Immetti o mappa l’ID del file da spostare. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID cartella [!UICONTROL] </td> 
   <td>Selezionare l'ID della cartella in cui si desidera spostare il file. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Immettere un nome per il file spostato.</td> 
  </tr> 
 </tbody> 
</table>

### Biglietti

#### [!UICONTROL Eliminare un ticket]

Elimina un ticket esistente in base al relativo ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immetti l’ID del ticket da eliminare. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Effettuare una chiamata API]

Ti consente di eseguire una chiamata API personalizzata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Immetti un percorso relativo a https://api.hubapi.com/. Ad esempio, /contatti/v1/lists/all/contact/all</p> <p>Per l’elenco degli endpoint disponibili, consulta <a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot] Documentazione API</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL, Metodo]</p> </td> 
   <td> <p>Seleziona il metodo HTTP da utilizzare:</p> <p>[!UICONTROL GET]</p> <p>per recuperare le informazioni relative a una voce.</p> <p>[!UICONTROL POST]</p> <p>per creare una nuova voce.</p> <p>[!UICONTROL PUT]</p> <p>per aggiornare/sostituire una voce esistente.</p> <p>[!UICONTROL PATCH]</p> <p>per eseguire un aggiornamento parziale della voce.</p> <p>[!UICONTROL DELETE]</p> <p>per eliminare una voce.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p> Immetti le intestazioni di richiesta desiderate. Non è necessario aggiungere intestazioni di autorizzazione; l'abbiamo già fatto per te.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Immetti la stringa di query della richiesta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto del corpo della chiamata API sotto forma di un oggetto JSON standard. Quando utilizzi istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Esempio:** La seguente chiamata API restituisce tutti i contatti nel tuo [!DNL HubSpot] account:
>
>**URL**: `/contacts/v1/lists/all/contacts/all`
>
>**Metodo**: `GET`
>
>![](assets/hubspot-api-config.png)
>
>Le corrispondenze della ricerca si trovano nell&#39;Output del modulo in [!UICONTROL Bundle] > [!UICONTROL Corpo] > [!UICONTROL contatti].
>
>Nel nostro esempio sono stati restituiti 3 contatti:
>
>![](assets/hubspot-api-output.png)

## Creare una nuova applicazione

1. Accedi al tuo [!DNL HubSpot] account sviluppatore.
1. Seleziona la **[!UICONTROL Creare un’app]** opzione .
1. Immetti il Nome app e [!UICONTROL Salva] la finestra di dialogo.
1. Selezionare gli ambiti necessari per il tuo webhook.

   Ad esempio, aggiungi gli ambiti dei contatti per attivare il modulo quando viene creato o eliminato un nuovo contatto.

   La [!UICONTROL ambito contatti] è tutto ciò che devi ricevere contatti, offerte e webhook di eventi aziendali.

   >[!IMPORTANT]
   >
   >Non compilare il [!UICONTROL URL di reindirizzamento] campo .
