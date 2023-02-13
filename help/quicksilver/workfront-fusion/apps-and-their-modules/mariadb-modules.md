---
title: Moduli MariaDB
description: In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL MariaDB], nonché collegarlo a più applicazioni e servizi di terze parti.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# [!DNL MariaDB] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL MariaDB], nonché collegarlo a più applicazioni e servizi di terze parti.

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

Per utilizzare [!DNL MariaDB] moduli, è necessario disporre di un [!DNL MariaDB] conto.

## Connetti [!DNL MariaDB] a [!DNL Workfront Fusion]

Puoi creare una connessione al tuo [!DNL MariaDB] account direttamente dall&#39;interno di un [!DNL MariaDB] modulo .

1. In qualsiasi [!DNL MariaDB] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo .
1. Configura i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome connessione]</p> </td> 
      <td> <p>Immettere un nome per la nuova connessione.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Host]</td> 
      <td> <p>Immettere l'indirizzo IP o il nome host dell'istanza di database. Questo host deve essere accessibile dall'esterno della rete.</p> <p>Esempio: <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Port]</td> 
      <td>La porta predefinita è 3306. Se utilizzi una porta non standard, imposta questo numero sulla porta. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Database Name]</td> 
      <td>Immettere il nome del database con cui si desidera interagire.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Username]</td> 
      <td>Immetti il nome utente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Password]</td> 
      <td>Immetti la tua password.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo .

## [!DNL MariaDB] Moduli e relativi campi

Quando si configura [!DNL MariaDB] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL MariaDB] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Eseguire una query (avanzata)

Questo modulo di azione recupera le informazioni dal database in base a una query fornita.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL MariaDB] account a [!DNL Workfront Fusion], vedi <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Connetti [!DNL MariaDB] a [!DNL Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query [!UICONTROL]</td> 
   <td> <p>Immettere la query SQL che si desidera utilizzare nel modulo per recuperare i dati.</p> <p>Importante: Le variabili utilizzate nella query non vengono igienizzate. Assicurati di pulire correttamente le variabili per evitare l'iniezione di SQL.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Selezionare le righe da una tabella (avanzata)]

Questo modulo legge record dal database.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL MariaDB] account a [!DNL Workfront Fusion], vedi <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Connetti [!DNL MariaDB] a [!DNL Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabella]</td> 
   <td> <p>Selezionare la tabella contenente i record che si desidera leggere.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Impostare il filtro in base al quale si desidera selezionare le righe</p> 
    <ul> 
     <li> <p>Selezionare il campo per il quale si desidera eseguire la ricerca</p> </li> 
     <li> <p>Seleziona l’operatore da utilizzare per la ricerca</p> </li> 
     <li> <p>Immetti o mappa il valore da cercare.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort] </td> 
   <td> <p>Per ogni livello per il quale si desidera ordinare i risultati, fare clic su <strong>[!UICONTROL Aggiungi elemento]</strong>, quindi seleziona il campo in base al quale vuoi ordinare i risultati e se desideri ordinare in ordine crescente o decrescente</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>
