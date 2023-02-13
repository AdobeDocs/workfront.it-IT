---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Domande frequenti su Adobe Workfront Fusion
description: Questo articolo tratta le domande comuni relative a [!DNL Adobe Workfront Fusion], comprese informazioni sugli oggetti comunemente utilizzati nei flussi di lavoro Fusion
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: aa58a64ea6b09192f93fa89a42a4bf6731052d10
workflow-type: tm+mt
source-wordcount: '620'
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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Cos&#39;è uno scenario?

### Risposta

Uno scenario definisce una sequenza di passaggi da eseguire [!DNL Adobe Workfront Fusion]. Per ogni scenario, è necessario specificare l’origine dati, il modo in cui i dati devono essere elaborati, i dati da utilizzare e gli elementi da ignorare. [!DNL Workfront Fusion] consente di creare scenari complessi per quanto necessario; anche gli scenari più sofisticati sono possibili.

Per ulteriori informazioni, consulta [Creare uno scenario di integrazione pratica in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## Posso utilizzare più moduli in uno scenario? O solo un attivatore e un&#39;azione?

### Risposta

In uno scenario è possibile utilizzare tutti i moduli desiderati. È possibile creare percorsi indipendenti e specificare quali dati devono scorrere attraverso di essi. Puoi inoltre utilizzare i risultati restituiti da singole azioni e quindi passarli all’azione successiva.

## Can [!DNL Workfront Fusion] lavorare con i file?

### Risposta

Sì. Utilizzo [!DNL Workfront Fusion], i file possono essere ricevuti, salvati, trasformati, convertiti, crittografati e così via. Inoltre, [!DNL Workfront Fusion] offre un&#39;ampia gamma di funzioni integrate progettate per consentire agli utenti di lavorare in modo efficace e creativo con i dati contenuti nei file.

Per ulteriori informazioni, consulta [Informazioni sulla mappatura dei file in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## Cosa succede se lascio [!DNL Workfront Fusion] elaborare un messaggio e-mail contenente più allegati?

### Risposta

Se utilizzi [!UICONTROL E-mail] modulo [!UICONTROL Recupera allegati], ogni allegato viene inviato singolarmente attraverso il resto dei moduli nello scenario. Moduli simili sono disponibili anche in altre app che ricevono più file contemporaneamente.

Per ulteriori informazioni, consulta [[!UICONTROL E-mail] moduli](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Alcuni trigger consentono l&#39;esecuzione immediata degli scenari. Cosa significa &quot;istantaneamente&quot;?

### Risposta

Gli scenari comuni vengono eseguiti a intervalli in base alla pianificazione specificata (ad esempio, ogni ora, ogni 5 minuti, una volta al mese e simili). Ci sono trigger speciali, chiamati trigger istantanei (webhook), che possono avviare il tuo scenario immediatamente dopo che ricevono i dati da un dato servizio. Gli attivatori istantanei possono essere estremamente utili. Si consiglia di utilizzarli quando possibile. Contribuiscono a ridurre il numero di operazioni. I dati ricevuti vengono elaborati immediatamente senza attendere la successiva esecuzione pianificata. Ad esempio, il [!DNL Google Sheets] modulo [!UICONTROL Modifiche di controllo] avvia uno scenario subito dopo l&#39;aggiornamento di una cella.

## Cosa sono gli aggregatori?

### Risposta

Un [!UICONTROL Aggregatore] unisce i dati in un’unica raccolta. Un esempio è rappresentato dai file compressi in un archivio zip e inviati come allegato e-mail.

Per ulteriori informazioni, consulta [[!UICONTROL Aggregatore] modulo in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Cos&#39;è un&#39;operazione?

### Risposta

Un&#39;operazione è un&#39;attività eseguita da un modulo. Ad esempio, si verifica un&#39;operazione ogni volta che viene eseguito un trigger e ogni volta che un&#39;azione esegue un&#39;attività.

## Che cos’è il trasferimento di dati?

### Risposta

Il trasferimento di dati si riferisce alla quantità di dati trasferiti nel tuo scenario. Ad esempio, supponiamo di avere uno scenario che recupera un&#39;immagine da 100 KB da FTP e ne riduce le dimensioni a 50 KB e salva entrambe le immagini in [!DNL Dropbox]. La quantità di dati utilizzata in questo scenario è di 150 KB.

## Che cos&#39;è una connessione?

### Risposta

Una connessione è il collegamento tra [!DNL Workfront Fusion] account e il servizio di terze parti che desideri utilizzare. La connessione può essere facilmente creata quando si modifica uno scenario. Per aggiungere una connessione, fai clic sul pulsante **[!UICONTROL Aggiungi]** nell’impostazione del modulo e segui le istruzioni dettagliate.

Per ulteriori informazioni, consulta [Informazioni sulla connessione [!DNL Adobe Workfront Fusion] a un&#39;app o a un servizio](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
