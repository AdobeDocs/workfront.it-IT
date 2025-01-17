---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Domande frequenti su Adobe Workfront Fusion
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 1%

---

# Domande frequenti su Adobe Workfront Fusion

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Domande frequenti sulla pianificazione dello scenario](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/plan-a-scenario/faq.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

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
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Che cos&#39;è uno scenario?

### Risposta

Uno scenario definisce una sequenza di passaggi che devono essere eseguiti da [!DNL Adobe Workfront Fusion]. Per ogni scenario, specificare l&#39;origine dati, la modalità di elaborazione dei dati, i dati da utilizzare e gli elementi da ignorare. [!DNL Workfront Fusion] consente di creare scenari complessi in base alle esigenze; anche gli scenari più sofisticati sono possibili.

Per ulteriori informazioni, vedere [Creare uno scenario di integrazione dell&#39;esercitazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## È possibile utilizzare più moduli in uno scenario? O solo un trigger e un&#39;azione?

### Risposta

Puoi utilizzare tutti i moduli che desideri in uno scenario. È possibile creare percorsi indipendenti e specificare quali dati devono passare attraverso di essi. Puoi anche utilizzare i risultati restituiti dalle singole azioni e quindi trasmetterli all’azione successiva.

## [!DNL Workfront Fusion] può lavorare con i file?

### Risposta

Sì. Utilizzando [!DNL Workfront Fusion] è possibile ricevere, salvare, trasformare, convertire, crittografare e così via i file. Inoltre, [!DNL Workfront Fusion] offre un&#39;ampia gamma di funzionalità incorporate progettate per consentire agli utenti di lavorare in modo efficace e creativo con i dati contenuti nei file.

Per ulteriori informazioni, vedere [Informazioni sui file di mapping in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## Cosa succede se consento a [!DNL Workfront Fusion] di elaborare un&#39;e-mail contenente più di un allegato?

### Risposta

Se utilizzi il modulo [!UICONTROL E-mail] [!UICONTROL Recupera allegati], ogni allegato viene inviato singolarmente tramite gli altri moduli dello scenario. Moduli simili sono disponibili anche in altre app che ricevono più file contemporaneamente.

Per ulteriori informazioni, vedere [[!UICONTROL E-mail] moduli](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Alcuni trigger consentono l’esecuzione immediata degli scenari. Cosa significa &quot;istantaneamente&quot;?

### Risposta

Gli scenari comuni vengono eseguiti a intervalli in base alla pianificazione specificata, ad esempio ogni ora, ogni 5 minuti, una volta al mese e così via. Esistono trigger speciali, denominati trigger istantanei (webhook), che possono avviare lo scenario immediatamente dopo aver ricevuto i dati da un determinato servizio. I trigger istantanei possono essere estremamente utili. È consigliabile utilizzarli quando possibile. Contribuiscono a ridurre il numero di operazioni. I dati ricevuti vengono elaborati immediatamente senza attendere la successiva esecuzione pianificata. Ad esempio, il modulo [!DNL Google Sheets] [!UICONTROL Osserva modifiche] avvia uno scenario immediatamente dopo l&#39;aggiornamento di una cella.

## Cosa sono gli aggregatori?

### Risposta

Un [!UICONTROL Aggregator] unisce i dati in un&#39;unica raccolta. Un esempio è dato dai file compressi in un archivio zip e inviati come allegato e-mail.

Per ulteriori informazioni, vedere il modulo [[!UICONTROL Aggregator] in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Che cos&#39;è un&#39;operazione?

### Risposta

Per operazione si intende qualsiasi operazione eseguita da un modulo. Un&#39;operazione si verifica, ad esempio, ogni volta che viene eseguito un trigger e ogni volta che un&#39;azione esegue un&#39;attività.

## Che cos’è il trasferimento di dati?

### Risposta

Il trasferimento di dati si riferisce alla quantità di dati trasferiti attraverso lo scenario. Si supponga, ad esempio, di disporre di uno scenario che recupera un&#39;immagine da 100 KB da FTP, ne riduce le dimensioni a 50 KB e salva entrambe le immagini in [!DNL Dropbox]. La quantità di dati utilizzata in questo scenario è di 250 KB.

## Che cos&#39;è una connessione?

### Risposta

Una connessione è il collegamento tra l&#39;account [!DNL Workfront Fusion] e il servizio di terze parti che si desidera utilizzare. La connessione può essere creata facilmente durante la modifica di uno scenario. Per aggiungere una connessione, fare clic sul pulsante **[!UICONTROL Aggiungi]** nell&#39;impostazione del modulo e seguire le istruzioni dettagliate.

Per ulteriori informazioni, vedere [Panoramica delle connessioni](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
