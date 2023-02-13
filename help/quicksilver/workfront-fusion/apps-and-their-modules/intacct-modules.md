---
title: Moduli Intact
description: Moduli Intact
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: fa1aa943-fbda-4eb4-bfa1-ab94a56785a7
source-git-commit: 9a4a847b542783845a3f896ec4e35d5efc7c122b
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---

# Moduli Intact

In un [!DNL Adobe Workfront Fusion] In questo caso, puoi automatizzare i flussi di lavoro che utilizzano Intact, nonché collegarli a più applicazioni e servizi di terze parti.

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

Per utilizzare i moduli Intacct, è necessario disporre di un account Intact.

## Connetti Intact a Workfront Fusion

### Autorizzazione [!DNL Workfront Fusion] per apportare modifiche in Intact

Prima [!DNL Workfront Fusion] può connettersi a [!DNL Intacct], devi autorizzarlo.

Nell’account Intact, accedi alla sezione **[!UICONTROL Azienda]** scheda .

1. Fai clic su **Informazioni aziendali**.
1. Passa a **Sicurezza** scheda .
1. Fai clic su [!UICONTROL Modifica] nell&#39;angolo superiore destro
1. Selezionare Autorizzazioni servizi Web.
1. Fai clic sull’icona più
1. Inserisci AzuquaMPP come sender_id.
1. (Facoltativo) Immettere una descrizione per la connessione

### Imposta una connessione in [!DNL Workfront Fusion] {#set-up-a-connection-in-workfront-fusion}

Puoi creare una connessione al tuo [!DNL Intacct] account direttamente dall&#39;interno di un [!DNL Intacct] modulo .

1. In qualsiasi modulo Intact, fai clic su **[!UICONTROL Aggiungi]** accanto al campo Connessione .
1. Immetti le credenziali Intact

   * ID Azienda
   * ID utente
   * Password

1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo .

## Moduli Intact e relativi campi

Quando si configura [!DNL Intacct] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati campi Intact aggiuntivi, a seconda di fattori come il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Effettuare una chiamata API personalizzata]](#make-a-custom-api-call)
* [[!UICONTROL Cerca record]](#search-records)

### [!UICONTROL Effettuare una chiamata API personalizzata] {#make-a-custom-api-call}

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata al [!DNL Intacct] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Intacct] moduli.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connessione</p> </td> 
   <td> <p>Per istruzioni su come collegare l’account Intact a [!DNL Workfront Fusion] 2.0, vedi <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Impostare una connessione in Workfront Fusion</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Corpo XML</td> 
   <td> <p>Include solo il codice XML all'interno del corpo. La richiesta include automaticamente le intestazioni di autenticazione.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Cerca record]

Questo modulo di ricerca recupera un elenco di record che corrispondono a criteri di ricerca specifici.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connessione</p> </td> 
   <td> <p>Per istruzioni su come collegare l’account Intact a [!DNL Workfront Fusion] 2.0, vedi <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Impostare una connessione in Workfront Fusion</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record da cercare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Criteri di ricerca</p> </td> 
   <td> 
    <ul> 
     <li> <p>Selezionare il campo in base al quale si desidera eseguire la ricerca</p> </li> 
     <li> <p>Selezionare l’operatore da utilizzare per la ricerca</p> </li> 
     <li> <p>Immettere il valore da cercare</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Set di risultati</td> 
   <td>Selezionare se si desidera restituire tutti i record corrispondenti o solo il primo record corrispondente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limite</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ordina per</td> 
   <td>Selezionare il campo in base al quale si desidera ordinare i risultati. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Disposizione</td> 
   <td>Seleziona se desideri ordinare in ordine crescente o decrescente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uscite</td> 
   <td> <p>Selezionare le informazioni che si desidera includere nel pacchetto di output per questo modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sensibilità delle maiuscole</td> 
   <td>Abilita questa opzione per fare in modo che la query faccia distinzione tra maiuscole e minuscole.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query su entità private</td> 
   <td>Abilita questa opzione per consentire al modulo di eseguire ricerche in entità private.</td> 
  </tr> 
 </tbody> 
</table>
