---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli evento
description: In uno scenario  [!DNL Adobe Workfront Fusion] , puoi automatizzare i flussi di lavoro che utilizzano Cvent, nonché collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1059'
ht-degree: 1%

---

# [!DNL Cvent] moduli

In uno scenario [!DNL Adobe Workfront Fusion], è possibile automatizzare i flussi di lavoro che utilizzano [!DNL Cvent] e collegarlo a più applicazioni e servizi di terze parti.

Se hai bisogno di istruzioni per la creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, vedere [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se disponi del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Per utilizzare i moduli [!DNL Cvent], è necessario disporre di un account [!DNL Cvent].

## Informazioni API evento

Il connettore Cvent utilizza quanto segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versione API</td> 
   <td> V200611.ASMX </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tag API</td> 
   <td>v1.7.14</td> 
  </tr>
 </tbody> 
 </table>

## Connetti [!DNL Cvent] a [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>I moduli [!DNL Cvent] funzionano tramite un&#39;API [!UICONTROL SOAP]. Per creare una connessione a [!DNL Cvent], è necessario verificare quanto segue:
>
>* Hai accesso [!UICONTROL SOAP] all&#39;API [!DNL Cvent].
>* Gli indirizzi IP [!DNL Workfront Fusion] sono stati aggiunti al inserisco nell&#39;elenco Consentiti di della tua organizzazione.
>
>  Per un elenco di [!DNL Workfront Fusion] indirizzi IP, vedere [Indirizzi IP per l&#39;accesso [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


Puoi creare una connessione al tuo account [!DNL Cvent] direttamente da un modulo [!DNL Cvent].

1. In qualsiasi modulo [!DNL Cvent], fai clic su **[!UICONTROL Aggiungi]** accanto al campo [!UICONTROL Connessione].
1. Selezionare l&#39;area a cui si desidera connettersi.

   * [!UICONTROL America del Nord]
   * [!UICONTROL Europa]
   * [!UICONTROL Sandbox]

1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

## [!DNL Cvent] moduli e relativi campi

Quando configuri [!DNL Cvent] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati ulteriori campi di [!DNL Cvent], a seconda di fattori quali il livello di accesso nell&#39;app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Azioni](#actions)
* [Ricerche](#searches)

### Azioni

* [[!UICONTROL Chiamata API personalizzata]](#create-meeting-request)
* [[!UICONTROL Leggi un record]](#read-a-record)
* [[!UICONTROL Registra invito]](#register-invitee)
* [[!UICONTROL Aggiungi invito]](#add-invitee)
* [[!UICONTROL Elimina contatto]](#delete-contact)
* [[!UICONTROL Aggiorna contatto]](#update-contact)
* [[!UICONTROL Crea convocazione di riunione]](#create-meeting-request)

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione consente di effettuare una chiamata autenticata personalizzata all&#39;API [!DNL Cvent]. In questo modo è possibile creare un&#39;automazione del flusso di dati che non può essere eseguita dagli altri moduli [!DNL Cvent].

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

Il modulo restituisce il codice di stato a, insieme alle intestazioni e al corpo della chiamata API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Cvent] a [!DNL Workfront Fusion], vedere <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connessione di [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operazione</td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, vedere <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Corpo (XML)</td> 
   <td> <p>Inserisci o mappa il corpo della chiamata API. Deve includere solo il codice XML. Il modulo includerà automaticamente le intestazioni di autenticazione. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggi un record]

Questo modulo di azione legge le informazioni su un record specifico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Cvent] a [!DNL Workfront Fusion], vedere <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connessione di [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo di record]</p> </td> 
   <td>Selezionare il tipo di elemento del record che si desidera leggere.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact] / [!UICONTROL Event] / [!UICONTROL Invitee ID]</td> 
   <td> <p>Immetti o mappa l’ID dell’elemento da leggere.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>Selezionare i campi da includere nell'output del modulo. I campi sono disponibili in base al tipo di elemento selezionato.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Registra invito]

Questo modulo di azione registra un invitato per un evento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Cvent] a [!DNL Workfront Fusion], vedere <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connessione di [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID invito</p> </td> 
   <td> <p>Immettere o mappare l'ID dell'invitato che si desidera registrare per un evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID evento</td> 
   <td> <p>Immettere o mappare l'ID dell'evento per il quale si desidera registrare l'invitato.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungi invito]

Questo modulo di azione invita un contatto a un evento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Cvent] a [!DNL Workfront Fusion], vedere <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connessione di [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID contatto]</p> </td> 
   <td> <p>Inserisci o mappa l’ID del contatto da aggiungere a un evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID evento]</td> 
   <td> <p>Inserisci o mappa l’ID dell’evento a cui desideri aggiungere il contatto.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elimina contatto]

Questo modulo di azione elimina un singolo contatto in Cvent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Cvent] a [!DNL Workfront Fusion], vedere <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connessione di [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID contatto]</td> 
   <td> <p>Immetti o mappa l’ID del contatto da eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiorna contatto]

Questo modulo di azione aggiorna un contatto esistente utilizzando il suo ID.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Cvent] a [!DNL Workfront Fusion], vedere <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connessione di [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID contatto]</p> </td> 
   <td> <p>Immetti o mappa l’ID del contatto da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>Selezionare i campi per i quali si desidera inserire le informazioni, quindi immettere i valori desiderati per tali campi.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi personalizzati]</td> 
   <td> <p>Selezionare i campi per i quali si desidera inserire le informazioni, quindi immettere i valori desiderati per tali campi.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea convocazione di riunione]

Questo modulo di azione aggiunge una convocazione di riunione al tuo account.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Cvent] a [!DNL Workfront Fusion], vedere <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connessione di [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID modulo]</p> </td> 
   <td> <p>Immettere o mappare l'ID del modulo che si desidera utilizzare per creare la nuova convocazione di riunione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi di convocazione riunione]</td> 
   <td> <p>Selezionare i campi della convocazione di riunione per i quali si desidera inserire le informazioni, quindi immettere i valori desiderati per tali campi.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi Richiesta Evento]</td> 
   <td> <p>Seleziona i campi della richiesta di evento per i quali vuoi inserire le informazioni, quindi inserisci i valori desiderati per tali campi.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL RFP Request Fields]</td> 
   <td> <p>Selezionare i campi della richiesta di proposta per i quali si desidera inserire le informazioni, quindi immettere i valori desiderati per tali campi.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

#### [!UICONTROL Elenca record]

Questo modulo di ricerca recupera informazioni su tutti i record di un tipo specifico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Cvent] a [!DNL Workfront Fusion], vedere <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connessione di [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo di record]</p> </td> 
   <td> <p>Selezionare il tipo di record da elencare.</p> 
    <ul> 
     <li> <p>Tutti gli eventi dal tuo account [!DNL Cvent]</p> </li> 
     <li> <p>Tutte le sessioni di un evento</p> </li> 
     <li> <p>Tutti gli invitati a un evento</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID evento]</td> 
   <td> <p>Se vengono elencati gli invitati o le sessioni, immettere o mappare l'ID dell'evento a cui sono associati tali invitati o sessioni.</p> </td> 
  </tr> 
 </tbody> 
</table>
