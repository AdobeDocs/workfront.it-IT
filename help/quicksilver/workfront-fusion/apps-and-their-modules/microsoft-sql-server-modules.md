---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Microsoft SQL Server
description: È possibile utilizzare [!DNL Adobe Workfront Fusion] per connettersi a Microsoft SQL Server.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# [!DNL Microsoft SQL Server] moduli

È possibile utilizzare [!DNL Adobe Workfront Fusion] per connettersi a [!UICONTROL Microsoft SQL Server].

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

## Utilizzo [!DNL Microsoft SQL Server] moduli

È possibile eseguire la logica personalizzata direttamente sul server di database tramite le stored procedure. [!DNL Adobe Workfront Fusion] carica dinamicamente l&#39;interfaccia dei parametri di input/output e del set di record in modo che ogni parametro o valore possa essere mappato singolarmente. Prima di iniziare a configurare lo scenario, assicurati che l&#39;account utilizzato per la connessione al database abbia accesso in lettura a `INFORMATION_SCHEMA.ROUTINES` e `INFORMATION_SCHEMA.PARAMETERS` visualizzazioni.

Quando [!DNL Fusion] stabilisce il collegamento [!DNL SQL server] la destinazione, [!DNL Fusion] l’utente identifica l’host (il nome di dominio o l’indirizzo IP in cui è ospitato il server) e la porta. [!DNL Fusion] può connettersi a qualsiasi host e porta disponibili.

Per informazioni su indirizzi IP specifici utilizzati da [!DNL Workfront Fusion], vedi [Indirizzi IP per l&#39;accesso [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

Per ulteriori informazioni sulla creazione di una stored procedure, consulta [!DNL Microsoft SQL Server] documentazione.

>[!NOTE]
>
>[!DNL Workfront Fusion] non supporta più set di record. Viene elaborata solo la prima.

## Errore di risoluzione dei problemi [!UICONTROL ER_LOCK_WAIT_TIMEOUT: Timeout di attesa blocco superato; prova a riavviare la transazione]

Questo errore si verifica quando si modificano gli stessi dati utilizzando più moduli. È causato dalle transazioni SQL.

Quando viene eseguito un modulo SQL, viene avviata una transazione. La transazione è terminata dopo che lo scenario è stato eseguito completamente.

Se un altro modulo tenta di accedere agli stessi dati, deve attendere il completamento della transazione precedente. Dal momento che la prima transazione verrà completata al termine dello scenario, la seconda transazione non potrà mai iniziare.

### Soluzione:

Attiva il commit automatico. Il commit automatico termina (impegna) ogni transazione immediatamente dopo l&#39;esecuzione del modulo.

1. Fai clic sul pulsante [!UICONTROL Impostazioni dello scenario] icona ![](assets/scenario-settings-icon.png)nella parte inferiore dello schermo.
1. Fai clic sul pulsante **[!UICONTROL commit automatico]** casella di controllo.
1. Fai clic su **[!UICONTROL OK]** per salvare le impostazioni dello scenario.
