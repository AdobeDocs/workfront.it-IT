---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Domande frequenti su Adobe Workfront Fusion
description: Questo articolo tratta le domande comuni relative a [!DNL Adobe Workfront Fusion], incluse informazioni sugli oggetti comunemente utilizzati nei flussi di lavoro di Fusion
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: f2d67401782abc7e7714d9e14c495a4a6ba2fcc7
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 0%

---

# Domande frequenti su Adobe Workfront Fusion

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
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

## Che cos&#39;è uno scenario?

### Risposta

Uno scenario definisce una sequenza di passaggi da eseguire da [!DNL Adobe Workfront Fusion]. Per ogni scenario, specificare l&#39;origine dati, la modalità di elaborazione dei dati, i dati da utilizzare e gli elementi da ignorare. [!DNL Workfront Fusion] consente di creare scenari il più complessi possibile, anche quelli più sofisticati.

Per ulteriori informazioni, consulta [Creare uno scenario di integrazione pratica in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## È possibile utilizzare più moduli in uno scenario? O solo un trigger e un&#39;azione?

### Risposta

Puoi utilizzare tutti i moduli che desideri in uno scenario. È possibile creare percorsi indipendenti e specificare quali dati devono passare attraverso di essi. Puoi anche utilizzare i risultati restituiti dalle singole azioni e quindi trasmetterli all’azione successiva.

## Can [!DNL Workfront Fusion] utilizzare i file?

### Risposta

Sì. Utilizzo di [!DNL Workfront Fusion], i file possono essere ricevuti, salvati, trasformati, convertiti, crittografati e così via. Inoltre, [!DNL Workfront Fusion] offre un&#39;ampia gamma di funzioni integrate progettate per consentire agli utenti di lavorare in modo efficace e creativo con i dati contenuti nei file.

Per ulteriori informazioni, consulta [Informazioni sulla mappatura dei file in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## Cosa succede se lascio [!DNL Workfront Fusion] elaborare un messaggio e-mail contenente più allegati?

### Risposta

Se si utilizza [!UICONTROL E-mail] modulo [!UICONTROL Recupera allegati], ogni allegato viene inviato singolarmente tramite gli altri moduli dello scenario. Moduli simili sono disponibili anche in altre app che ricevono più file contemporaneamente.

Per ulteriori informazioni, consulta [[!UICONTROL E-mail] moduli](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Alcuni trigger consentono l’esecuzione immediata degli scenari. Cosa significa &quot;istantaneamente&quot;?

### Risposta

Gli scenari comuni vengono eseguiti a intervalli in base alla pianificazione specificata, ad esempio ogni ora, ogni 5 minuti, una volta al mese e così via. Esistono trigger speciali, denominati trigger istantanei (webhook), che possono avviare lo scenario immediatamente dopo aver ricevuto i dati da un determinato servizio. I trigger istantanei possono essere estremamente utili. È consigliabile utilizzarli quando possibile. Contribuiscono a ridurre il numero di operazioni. I dati ricevuti vengono elaborati immediatamente senza attendere la successiva esecuzione pianificata. Ad esempio, il [!DNL Google Sheets] modulo [!UICONTROL Osserva modifiche] avvia uno scenario immediatamente dopo l&#39;aggiornamento di una cella.

## Cosa sono gli aggregatori?

### Risposta

Un [!UICONTROL Aggregatore] unisce i dati in una singola raccolta. Un esempio è dato dai file compressi in un archivio zip e inviati come allegato e-mail.

Per ulteriori informazioni, consulta [[!UICONTROL Aggregatore] modulo in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Che cos&#39;è un&#39;operazione?

### Risposta

Per operazione si intende qualsiasi operazione eseguita da un modulo. Un&#39;operazione si verifica, ad esempio, ogni volta che viene eseguito un trigger e ogni volta che un&#39;azione esegue un&#39;attività.

## Che cos’è il trasferimento di dati?

### Risposta

Il trasferimento di dati si riferisce alla quantità di dati trasferiti attraverso lo scenario. Ad esempio, supponiamo che tu abbia uno scenario in cui recuperi un&#39;immagine di 100 KB da FTP, ne riduca le dimensioni a 50 KB e salvi entrambe le immagini in [!DNL Dropbox]. La quantità di dati utilizzata in questo scenario è di 250 KB.

## Che cos&#39;è una connessione?

### Risposta

Una connessione è il collegamento tra [!DNL Workfront Fusion] e il servizio di terze parti che desideri utilizzare. La connessione può essere creata facilmente durante la modifica di uno scenario. Per aggiungere una connessione, fare clic su **[!UICONTROL Aggiungi]** nell&#39;impostazione del modulo e seguire le istruzioni dettagliate.

Per ulteriori informazioni, consulta [Informazioni sulla connessione [!DNL Adobe Workfront Fusion] a un’app o a un servizio](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
