---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli di Microsoft SQL Server
description: È possibile utilizzare [!DNL Adobe Workfront Fusion] per connettersi a Microsoft SQL Server.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '502'
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



## Collegamento di [!DNL Microsoft SQL Server] servizio a [!DNL Workfront Fusion]

Per istruzioni sulla connessione [!DNL Microsoft SQL Server] account a [!UICONTROL Workfront Fusion], vedi [Creare una connessione a [!UICONTROL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Alcune app Microsoft utilizzano la stessa connessione, che è associata alle autorizzazioni dei singoli utenti. Pertanto, durante la creazione di una connessione, nella schermata di consenso delle autorizzazioni vengono visualizzate tutte le autorizzazioni concesse in precedenza alla connessione dell’utente, oltre alle nuove autorizzazioni necessarie per l’applicazione corrente.
>
>Ad esempio, se un utente dispone delle autorizzazioni &quot;Leggi tabella&quot; concesse tramite il connettore Excel e quindi crea una connessione nel connettore Outlook per leggere le e-mail, nella schermata di consenso delle autorizzazioni verranno visualizzate sia l’autorizzazione &quot;Leggi tabella&quot; già concessa che l’autorizzazione &quot;Scrivi e-mail&quot; appena richiesta.

## Utilizzo di [!DNL Microsoft SQL Server] moduli

È possibile eseguire la logica personalizzata direttamente sul server di database tramite stored procedure. [!DNL Adobe Workfront Fusion] carica dinamicamente l&#39;interfaccia dei parametri di input/output e del recordset in modo che ogni parametro o valore possa essere mappato singolarmente. Prima di iniziare a configurare lo scenario, verificare che l&#39;account utilizzato per la connessione al database disponga dell&#39;accesso in lettura a `INFORMATION_SCHEMA.ROUTINES` e `INFORMATION_SCHEMA.PARAMETERS` visualizzazioni.

Quando [!DNL Fusion] stabilisce la connessione al [!DNL SQL server] destinazione, il [!DNL Fusion] L&#39;utente identifica l&#39;host (il nome di dominio o l&#39;indirizzo IP in cui è ospitato il server) e la porta. [!DNL Fusion] può connettersi a qualsiasi host e porta disponibile.

Per informazioni su indirizzi IP specifici utilizzati da [!DNL Workfront Fusion], vedi [Indirizzi IP per l&#39;accesso [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

Per ulteriori informazioni sulla creazione di una stored procedure, vedere [!DNL Microsoft SQL Server] documentazione.

>[!NOTE]
>
>[!DNL Workfront Fusion] non supporta più recordset. Viene elaborato solo il primo.

## Risoluzione dei problemi di errore [!UICONTROL ER_LOCK_WAIT_TIMEOUT: timeout di attesa blocco superato; provare a riavviare la transazione]

Questo errore si verifica quando si modificano gli stessi dati utilizzando più moduli. È causata da transazioni SQL.

Quando viene eseguito un modulo SQL, viene avviata una transazione. La transazione è terminata dopo che lo scenario è stato completamente eseguito.

Se un altro modulo tenta di accedere agli stessi dati, deve attendere il completamento della transazione precedente. Poiché la prima transazione verrà completata al termine dello scenario, la seconda transazione non potrà mai iniziare.

### Soluzione:

Attiva il commit automatico. Il commit automatico termina (esegue il commit) ogni transazione subito dopo l&#39;esecuzione del modulo.

1. Fai clic su [!UICONTROL Impostazioni scenario] icona ![](assets/scenario-settings-icon.png)nella parte inferiore dello schermo.
1. Fai clic su **[!UICONTROL Commit automatico]** casella di controllo.
1. Clic **[!UICONTROL OK]** per salvare le impostazioni dello scenario.
