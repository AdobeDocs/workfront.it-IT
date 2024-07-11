---
title: Moduli CRM HubSpot
description: Il [!DNL Adobe Workfront Fusion] I moduli di gestione delle relazioni con i clienti HubSpot consentono di monitorare eventi, record, contatti, accordi, invii di file e moduli o di creare, recuperare, aggiornare ed eliminare record, contatti, accordi, eventi o file nel [!DNL HubSpot CRM] account.
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 1c56cf8aa9da7ec2644955d5533c71f60160d580
workflow-type: tm+mt
source-wordcount: '2615'
ht-degree: 0%

---

# [!DNL HubSpot CRM] moduli

Il [!DNL Adobe Workfront Fusion] [!DNL HubSpot CRM] I moduli consentono di monitorare eventi, record, contatti, impegni, invii di file e moduli o di creare, recuperare, aggiornare ed eliminare record, contatti, impegni, eventi o file nel [!DNL HubSpot CRM] account.

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

Da utilizzare [!DNL HubSpot CRM] moduli, è necessario disporre di un [!DNL HubSpot CRM] account.

## Connetti [!DNL Adobe Workfront Fusion] a [!DNL HubSpot CRM]

Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi [Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Durante la configurazione di una connessione, selezionare **CRM HubSpot** tipo di connessione. Il tipo di CRM HubSpot (obsoleto) supporta le connessioni esistenti, ma si sconsiglia di utilizzarlo per creare nuove connessioni.

## [!DNL HubSpot CRM] moduli e relativi campi

Quando si configura [!DNL Hubspot CRM] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Hubspot CRM] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Oggetti CRM](#crm-objects)
* [Record (offerte, contatti e società)](#records-deals-contacts-and-companies)
* [Conttati](#contacts)
* [Offerte](#deals)
* [Aziende](#companies)
* [File](#files)
* [Biglietti](#tickets)
* [Effettuare una chiamata API](#make-an-api-call)

### Oggetti CRM

#### [!UICONTROL Cerca oggetti CRM]

Questo modulo di ricerca cerca oggetti CRM per proprietà personalizzate o per query. Per cercare prodotti o elementi riga, utilizza una connessione speciale con un ambito personalizzato richiesto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di elementi restituiti dal modulo in un ciclo di esecuzione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type da cercare]</td> 
   <td>Selezionare il tipo di oggetto CRM Hubspot che si desidera cercare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Proprietà output]</td> 
   <td>Selezionare le proprietà che si desidera visualizzare nell'output del modulo. I campi disponibili dipendono dall’oggetto selezionato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtra per] </td> 
   <td> <p>Seleziona la modalità di filtro della ricerca</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>Immettere o mappare la query</p> </li> 
     <li> <p><strong>Proprietà [!UICONTROL]</strong> </p> <p>Immetti i gruppi o i filtri per la ricerca.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina per]</td> 
   <td> <p>Fai clic su per ordinare i risultati. Se si sceglie di ordinare i risultati, vengono visualizzati i campi riportati di seguito. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome proprietà]</strong> </p> <p>Selezionare la proprietà in base alla quale si desidera ordinare i risultati</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>Scegliere se si desidera ordinare i risultati in senso crescente o decrescente.</p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Start Offset</td> 
    <td>Enter or map the ID of the first item you want to retrieve details for. This module only returns up to 5000 results at a time. Setting a start offset allows you to retrieve items other than the first 5000. If the start offset is 5000, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

### Record (offerte, contatti e società)

* [[!UICONTROL Crea un record (legacy)]](#create-a-record-legacy)
* [[!UICONTROL Ottieni un record]](#get-a-record)
* [[!UICONTROL Aggiornare un record]](#update-a-record)
* [[!UICONTROL Eliminare un record]](#delete-a-record)
* [[!UICONTROL Ottieni una proprietà record]](#get-a-record-property)
* [[!UICONTROL Osserva i record]](#watch-records)

#### [!UICONTROL Crea un record (legacy)]

Questo modulo di azione crea un contatto, un’azienda o un’offerta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record da creare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proprietà [!UICONTROL]</td> 
   <td>Immettere le proprietà che si desidera impostare per il record. I campi disponibili dipendono dal tipo di record che si desidera creare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un record]

Questo modulo di azione ottiene i dettagli di un contatto, un’azienda o un’offerta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
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
   <td role="rowheader">Tipo di ricerca [!UICONTROL]</td> 
   <td>Se stai ricevendo un contatto, seleziona se desideri identificarlo per ID o per indirizzo e-mail.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immettere l'ID del contatto, della società o dell'operazione che si desidera recuperare. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL E-Mail]</td> 
   <td>Immetti l’indirizzo e-mail del contatto di cui desideri recuperare i dettagli. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un record]

Questo modulo di azione aggiorna un contatto, un’azienda o un’offerta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record da aggiornare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo di ricerca [!UICONTROL]</td> 
   <td> <p>Se si sta ottenendo un contatto, selezionare la modalità di identificazione del record:</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> </li> 
     <li> <p>[!UICONTROL E-Mail]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immettere l'ID del contatto, della società o dell'offerta che si desidera aggiornare. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL E-Mail]</td> 
   <td>Immettere l'indirizzo di posta elettronica del contatto di cui si desidera aggiornare i dettagli. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proprietà [!UICONTROL]</td> 
   <td>Immettere le proprietà che si desidera impostare per il record. I campi disponibili dipendono dal tipo di record che si desidera creare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un contatto, un’azienda o un’offerta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record che si desidera eliminare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immettere l'ID del contatto, della società o dell'offerta che si desidera eliminare. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni una proprietà record]

Questo modulo di azione ottiene i metadati per una proprietà record specifica in base al nome (interno).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record con la proprietà per cui si desidera recuperare i metadati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome proprietà [!UICONTROL]</td> 
   <td>Seleziona la proprietà per la quale desideri recuperare i metadati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID opzione]</td> 
   <td> <p> Alcune proprietà dispongono di un set di opzioni disponibili che un utente può selezionare come valore della proprietà. Immetti l’ID dell’opzione che rappresenta il valore della proprietà da recuperare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Osserva i record]

Questo modulo di attivazione avvia uno scenario in cui un contatto, una società o un&#39;offerta è stata modificata o creata negli ultimi 30 giorni. L&#39;output è limitato a 10.000 record.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record con la proprietà che si desidera controllare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL - Ricerca]</td> 
   <td>Specificare se si desidera controllare i record modificati di recente o creati di recente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proprietà output di [!UICONTROL]</td> 
   <td>Selezionare le proprietà da includere nell'output del modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Conttati

* [[!UICONTROL Crea/aggiorna un contatto (legacy)]](#createupdate-a-contact-legacy)
* [[!UICONTROL Crea/aggiorna un gruppo di contatti]](#createupdate-a-group-of-contacts)
* [[!UICONTROL Aggiungere contatti a un elenco]](#add-contacts-to-a-list)
* [[!UICONTROL Rimuovere un contatto da un elenco]](#remove-a-contact-from-a-list)
* [[!UICONTROL Unisci contatti]](#merge-contacts)
* [[!UICONTROL Cerca contatti]](#search-for-contacts)
* [[!UICONTROL Elenca contatti]](#list-contacts)
* [[!UICONTROL Elencare contatti di una società]](#list-contacts-of-a-company)

#### [!UICONTROL Crea/aggiorna un contatto (legacy)]

Crea un contatto se non esiste già in un portale, oppure lo aggiorna con i valori delle proprietà più recenti se esiste già in un portale.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proprietà [!UICONTROL]</td> 
   <td>Specificare le proprietà che si desidera impostare o aggiornare per il contatto. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea/aggiorna un gruppo di contatti]

Crea un gruppo di contatti o li aggiorna se esistono già. Le prestazioni sono migliori quando la dimensione del batch è limitata a un massimo di 100 contatti. Le modifiche apportate tramite questo endpoint vengono elaborate in modo asincrono, pertanto l&#39;applicazione delle modifiche ai record dei contatti potrebbe richiedere alcuni minuti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Batch di contatti da creare/aggiornare] </td> 
   <td> <p>Aggiungi il batch di contatti.</p> <p>Clic <strong>[!UICONTROL Add item]</strong> per aggiungere un nuovo contatto. Nella finestra visualizzata, inserire o mappare le seguenti informazioni:</p> 
    <ul> 
     <li> <p><strong>Tipo di ricerca [!UICONTROL]</strong> </p> <p>Selezionare la modalità di identificazione del contatto:</p> 
      <ul> 
       <li> <p>[!UICONTROL ID]</p> <p>Immettere l'ID del contatto che si desidera creare o aggiornare. </p> </li> 
       <li> <p>[!UICONTROL E-Mail]</p> <p>Immetti l’indirizzo e-mail del contatto da creare o aggiornare. </p> </li> 
      </ul> </li> 
     <li> <p><strong>Proprietà [!UICONTROL]</strong> </p> <p>Specificare le proprietà che si desidera impostare o aggiornare per il contatto.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungere contatti a un elenco]

Questo modulo aggiunge a un elenco contatti i record contatto già creati nel sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID elenco] </td> 
   <td>Selezionare l'ID dell'elenco a cui si desidera aggiungere il contatto. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IDs/E-mail] </td> 
   <td> <p>Selezionare la modalità di identificazione dei contatti che si desidera aggiungere all'elenco:</p> 
    <ul> 
     <li> <p>[!UICONTROL IDs]</p> <p>Aggiungere gli ID dei contatti che si desidera aggiungere all'elenco.</p> </li> 
     <li> <p>[!UICONTROL E-Mail]</p> <p>Aggiungere gli indirizzi di posta elettronica dei contatti che si desidera aggiungere all'elenco.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rimuovere un contatto da un elenco]

Rimuove un contatto da un elenco contatti.

>[!NOTE]
>
>Non è possibile rimuovere manualmente i contatti da un elenco dinamico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID elenco] </td> 
   <td>Selezionare l'ID dell'elenco da cui si desidera rimuovere il contatto. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID contatto] </td> 
   <td>Immettere l'ID del contatto da rimuovere dall'elenco. </td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 1] </td> 
   <td>Immettere l'ID di uno dei contatti da unire. </td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td>Immettere la query di ricerca.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Immetti o mappa il numero massimo di contatti [!DNL Workfront Fusion] deve essere restituito durante un ciclo di esecuzione dello scenario. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenca contatti]

Restituisce tutti i contatti creati nel portale. L&#39;output è limitato a 5000 contatti. Per elencare i contatti precedenti o successivi, è possibile utilizzare [!UICONTROL avanzato] per impostare l&#39;offset dell&#39;elenco.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Numero massimo di contatti [!DNL Workfront Fusion] deve essere restituito durante un ciclo di esecuzione dello scenario. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Proprietà output]</td> 
   <td>Selezionare le proprietà che si desidera visualizzare nell'output del modulo. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Elencare contatti di una società]

Recupera un elenco di contatti della società. L&#39;output è limitato a 5000 contatti. Per elencare i contatti precedenti o successivi, è possibile utilizzare [!UICONTROL avanzato] per impostare l&#39;offset dell&#39;elenco.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immettere l'ID della società di cui si desidera elencare i contatti. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Numero massimo di contatti [!DNL Workfront Fusion] deve essere restituito durante un ciclo di esecuzione dello scenario. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Osservare i contatti aggiunti a un elenco]

Questo modulo di attivazione avvia uno scenario quando un nuovo contatto viene aggiunto a un elenco. È disponibile solo per gli utenti con un account Marketing a pagamento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID elenco]</td> 
   <td>Immettere o mappare l'ID dell'elenco contenente i contatti che si desidera controllare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proprietà output di [!UICONTROL]</td> 
   <td>Selezionare le proprietà da includere nell'output del modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Offerte

* [[!UICONTROL Elenca pipeline di offerte/biglietti]](#list-dealticket-pipelines)
* [[!UICONTROL Ottieni una pipeline CRM per un’offerta]](#get-a-deals-crm-pipeline)

#### [!UICONTROL Elenca pipeline di offerte/biglietti]

Restituisce tutte le pipeline di offerte e biglietti per un determinato portale.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo di oggetto [!UICONTROL] </td> 
   <td>Seleziona se desideri elencare offerte o biglietti.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni una pipeline CRM per un’offerta]

Restituisce una pipeline di offerta specifica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID pipeline di [!UICONTROL] </td> 
   <td>Immetti o mappa l’ID della pipeline per la quale desideri recuperare i dettagli. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID fase] </td> 
   <td>Immetti o mappa l’ID della fase per cui desideri recuperare i dettagli. </td> 
  </tr> 
 </tbody> 
</table>

### Aziende

#### [!UICONTROL Ricerca di società per dominio]

Recupera un elenco di aziende in base a una corrispondenza esatta con la proprietà del dominio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Domain] </td> 
   <td>Immetti il dominio delle aziende da cercare, ad esempio <code>[!DNL hubspot].com</code>. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Numero massimo di società [!DNL Workfront Fusion] deve essere restituito durante un ciclo di esecuzione dello scenario. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Proprietà output]</td> 
   <td>Selezionare le proprietà che si desidera visualizzare nell'output del modulo. </td> 
  </tr> 
 </tbody> 
</table>

### File

* [[!UICONTROL Creare una cartella]](#create-a-folder)
* [[!UICONTROL Eliminare una cartella]](#delete-a-folder)
* [[!UICONTROL Spostare un file]](#move-a-file)

#### [!UICONTROL Creare una cartella]

Questo modulo crea una cartella.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome cartella] </td> 
   <td>Immettere o mappare un nome per la nuova cartella.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID cartella padre] </td> 
   <td>Seleziona l’ID della cartella principale per la cartella che stai creando. </td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immetti l’ID della cartella da eliminare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Spostare un file]

Sposta un file in un&#39;altra cartella.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID file] </td> 
   <td>Immetti o mappa l’ID del file da spostare. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID cartella] </td> 
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

Elimina un ticket esistente in base al suo ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immetti l’ID del ticket da eliminare. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Effettuare una chiamata API]

Consente di eseguire una chiamata API personalizzata.

>[!NOTE]
>
>I seguenti endpoint sono stati dichiarati obsoleti nell’API HubSpot il 31 agosto 2023 e non possono più essere utilizzati nei moduli Fusion.
>
>* Elencare eventi di contenuto
>* Elencare eventi social
>* Elencare eventi attività calendario
>* Elenca tutti gli eventi calendario
>* Crea attività calendario
>* Ottieni attività calendario per ID
>* Aggiorna attività calendario
>* Eliminare un’attività calendario

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL HubSpot CRM] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Immetti un percorso relativo a https://api.hubapi.com/. Ad esempio, /contacts/v1/LISTS/all/contacts/all</p> <p>Per l’elenco degli endpoint disponibili, consulta <a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot] Documentazione API</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Selezionare il metodo HTTP che si desidera utilizzare:</p> <p>[!UICONTROL GET]</p> <p>per recuperare informazioni per una voce.</p> <p>[!UICONTROL POST]</p> <p>per creare una nuova voce.</p> <p>[!UICONTROL PUT]</p> <p>per aggiornare o sostituire una voce esistente.</p> <p>[!UICONTROL PATCH]</p> <p>per aggiornare una voce parziale.</p> <p>[!UICONTROL DELETE]</p> <p>per eliminare una voce.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p> Inserisci le intestazioni di richiesta desiderate. Non è necessario aggiungere intestazioni di autorizzazione; l’abbiamo già fatto per te.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query]</td> 
   <td> <p> Immettere la stringa di query richiesta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.Quando utilizzi istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
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
>Le corrispondenze della ricerca si trovano nell’Output del modulo in [!UICONTROL Bundle] > [!UICONTROL Corpo] > [!UICONTROL contatti].
>
>Nel nostro esempio, sono stati restituiti 3 contatti:
>
>![](assets/hubspot-api-output.png)

## Crea una nuova applicazione

1. Accedi al tuo [!DNL HubSpot] account sviluppatore.
1. Seleziona la **[!UICONTROL Creare un’app]** opzione.
1. Inserisci il nome dell’app e [!UICONTROL Salva] la finestra di dialogo.
1. Seleziona gli ambiti necessari per il webhook.

   Ad esempio, aggiungi gli ambiti dei contatti per attivare il modulo quando viene creato o eliminato un nuovo contatto.

   Il [!UICONTROL ambito contatti] è tutto ciò di cui hai bisogno per ricevere contatti, offerte e webhook di eventi aziendali.

   >[!IMPORTANT]
   >
   >Non compilare il campo [!UICONTROL URL di reindirizzamento] campo.
