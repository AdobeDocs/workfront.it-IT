---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli di cvent
description: In un [!DNL Adobe Workfront Fusion] In questo caso, puoi automatizzare i flussi di lavoro che utilizzano Cvent e collegarli a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 1%

---

# [!DNL Cvent] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Cvent], nonché collegarlo a più applicazioni e servizi di terze parti.

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Per utilizzare [!DNL Cvent] moduli, è necessario disporre di un [!DNL Cvent] conto.

## Connetti [!DNL Cvent] a [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>La [!DNL Cvent] i moduli funzionano tramite [!UICONTROL SOAP] API. Per creare una connessione a [!DNL Cvent], assicurati quanto segue:
>
>* Hai [!UICONTROL SOAP] accesso al [!DNL Cvent] API.
>* La [!DNL Workfront Fusion] Gli indirizzi IP sono stati aggiunti all’inserire nell&#39;elenco Consentiti della tua organizzazione.
>
>  Per un elenco di [!DNL Workfront Fusion] Indirizzi IP, vedi [Indirizzi IP per l&#39;accesso [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


Puoi creare una connessione al tuo [!DNL Cvent] account direttamente dall&#39;interno di un [!DNL Cvent] modulo .

1. In qualsiasi [!DNL Cvent] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo .
1. Selezionare l&#39;area a cui si desidera connettersi.

   * [!UICONTROL America del Nord]
   * [!UICONTROL Europa]
   * [!UICONTROL Sandbox]

1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo .

## [!DNL Cvent] moduli e relativi campi

Quando si configura [!DNL Cvent] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Cvent] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Azioni](#actions)
* [Ricerche](#searches)

### Azioni

* [[!UICONTROL Chiamata API personalizzata]](#create-meeting-request)
* [[!UICONTROL Leggi un record]](#read-a-record)
* [[!UICONTROL Registrare l&#39;invitato]](#register-invitee)
* [[!UICONTROL Aggiungi invitato]](#add-invitee)
* [[!UICONTROL Cancella Contatto]](#delete-contact)
* [[!UICONTROL Aggiorna contatto]](#update-contact)
* [[!UICONTROL Crea richiesta di riunione]](#create-meeting-request)

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata al [!DNL Cvent] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Cvent] moduli.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

Il modulo restituisce il codice di stato a, insieme alle intestazioni e al corpo della chiamata API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Cvent] account a [!DNL Workfront Fusion], vedi <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operazione</td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Corpo (XML)</td> 
   <td> <p>Immetti o mappa il corpo della chiamata API. Deve includere solo il codice XML. Il modulo includerà automaticamente le intestazioni di autenticazione. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggi un record]

Questo modulo di azione legge informazioni su un record specifico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Cvent] account a [!DNL Workfront Fusion], vedi <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo di record]</p> </td> 
   <td>Selezionare il tipo di elemento del record che si desidera leggere.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact] / [!UICONTROL Event] / [!UICONTROL Invitee ID]</td> 
   <td> <p>Immettere o mappare l'ID dell'elemento che si desidera leggere.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td> <p>Seleziona i campi da includere nell’output del modulo. I campi sono disponibili in base al tipo di elemento selezionato.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Registrare l&#39;invitato]

Questo modulo di azione registra un invitato per un evento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Cvent] account a [!DNL Workfront Fusion], vedi <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID invito</p> </td> 
   <td> <p>Immetti o mappa l’ID dell’invitato a cui desideri registrarti per un evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID evento</td> 
   <td> <p>Immetti o mappa l’ID dell’evento per il quale desideri registrare l’invitato.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungi invitato]

Questo modulo di azione invita un contatto a un evento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Cvent] account a [!DNL Workfront Fusion], vedi <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contact ID]</p> </td> 
   <td> <p>Immetti o mappa l'ID del contatto che desideri aggiungere a un evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID evento]</td> 
   <td> <p>Immetti o mappa l'ID dell'evento a cui desideri aggiungere il contatto.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cancella Contatto]

Questo modulo di azione elimina un singolo contatto in Cvent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Cvent] account a [!DNL Workfront Fusion], vedi <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact ID]</td> 
   <td> <p>Immettere o mappare l'ID del contatto che si desidera eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiorna contatto]

Questo modulo di azione aggiorna un contatto esistente utilizzando il relativo ID.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Cvent] account a [!DNL Workfront Fusion], vedi <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contact ID]</p> </td> 
   <td> <p>Immetti o mappa l'ID del contatto che desideri aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>Seleziona i campi per i quali desideri inserire le informazioni, quindi compila i valori desiderati per tali campi.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi personalizzati]</td> 
   <td> <p>Seleziona i campi per i quali desideri inserire le informazioni, quindi compila i valori desiderati per tali campi.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea richiesta di riunione]

Questo modulo di azione aggiunge una convocazione di riunione al tuo account.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Cvent] account a [!DNL Workfront Fusion], vedi <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Form ID]</p> </td> 
   <td> <p>Immettere o mappare l'ID del modulo che si desidera utilizzare per creare la nuova convocazione di riunione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi Richiesta Riunione]</td> 
   <td> <p>Selezionare i campi di richiesta della riunione per i quali si desidera inserire le informazioni, quindi inserire i valori desiderati per tali campi.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event Request Fields]</td> 
   <td> <p>Seleziona i campi di richiesta dell’evento per i quali desideri inserire le informazioni, quindi compila i valori desiderati per tali campi.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL RFP Request Fields]</td> 
   <td> <p>Seleziona i campi di richiesta per i quali desideri inserire le informazioni, quindi compila i valori desiderati per tali campi.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

#### [!UICONTROL Elencare record]

Questo modulo di ricerca recupera informazioni su tutti i record di un tipo specifico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Cvent] account a [!DNL Workfront Fusion], vedi <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo di record]</p> </td> 
   <td> <p>Selezionare il tipo di record da elencare.</p> 
    <ul> 
     <li> <p>Tutti gli eventi dal tuo [!DNL Cvent] account</p> </li> 
     <li> <p>Tutte le sessioni per un evento</p> </li> 
     <li> <p>Tutti gli invitati a un evento</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID evento]</td> 
   <td> <p>Se inserisci degli invitati o delle sessioni, immetti o mappa l’ID dell’evento a cui sono associati gli invitati o le sessioni.</p> </td> 
  </tr> 
 </tbody> 
</table>
