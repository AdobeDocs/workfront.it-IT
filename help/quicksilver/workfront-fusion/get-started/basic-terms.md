---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Termini di base in Adobe Workfront Fusion
description: Adobe Workfront Fusion richiede una licenza Adobe Workfront Fusion oltre a una licenza Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: 2169dc2e-2135-47e0-a615-3de12cd120a9
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 0%

---

# Termini di base in [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] richiede un [!DNL Adobe Workfront Fusion] oltre a una licenza [!UICONTROL Adobe Workfront] licenza.


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Azione</p> </td> 
   <td>Un modulo che consente di leggere o scrivere bundle da o in un'app o servizio selezionati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Aggregatore [!UICONTROL]</p> </td> 
   <td> <p>Tipo di modulo che unisce più bundle (più array di dati) in un unico bundle. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/aggregator-module.md" class="MCXref xref">Modulo Aggregator in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Chiave API</td> 
   <td>Codice univoco che identifica l'utente, lo sviluppatore o il programma che sta chiamando l'API di un software, utilizzato per l'autenticazione. Da [!DNL Adobe Workfront Fusion] I moduli funzionano tramite la connessione delle API, a volte sono necessarie le chiavi API. Le chiavi API sono distribuite dall’app che le richiede. Ad esempio, se hai bisogno di una chiave API per [!DNL ActiveCampaign], lo richiederebbe tramite il tuo [!DNL ActiveCampaign] conto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">App o servizio</td> 
   <td> <p>Un'applicazione software, più comunemente.</p> <p>Un’app può anche essere una funzione speciale che manipola i dati, ad esempio un iteratore o un aggregatore. </p> <p>Un servizio è un’origine di bundle che possono includere un’API web, una pagina web, diversi tipi di server (FTP, SMTP, IMAP) e così via. </p> <p> <img src="assets/apps-350x420.jpg" style="width: 350;height: 420;"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connettore app</td> 
   <td>Un'app che si connette a un altro sistema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Bundle</p> </td> 
   <td> <p>Un bundle è un'unità di base restituita o ricevuta dai moduli. Un bundle è costituito da elementi.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Quando si aggiunge un'app o un servizio a uno scenario, molto probabilmente sarà necessario prima creare una connessione tra [!DNL Workfront Fusion] e l'app o il servizio per recuperare o inviare i dati selezionati. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref">Informazioni sulla connessione [!DNL Adobe Workfront Fusion] a un'app o a un servizio</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ciclo</p> </td> 
   <td> <p>Un ciclo si riferisce a due fasi dell'esecuzione dello scenario: funzionamento e commit. Lo scenario può essere costituito da uno o più cicli. Per informazioni più dettagliate, consulta <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Archiviazione dati</p> </td> 
   <td> <p>Strumento che memorizza i dati da scenari o consente di trasferire i dati tra scenari singoli o esecuzioni di scenari. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/data-stores.md" class="MCXref xref">Archivio dati in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Trasferimento dati</p> </td> 
   <td> <p>La quantità di dati trasferiti nel tuo scenario. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Dettagli dello scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Filtro</p> </td> 
   <td> <p>Funzionalità aggiuntive che possono essere applicate tra due moduli. Un filtro consente quindi di lavorare solo con bundle che soddisfano determinati criteri. Puoi applicare diversi filtri. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Aggiungere un filtro a uno scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID</p> </td> 
   <td> <p>Nome utilizzato per identificare in modo univoco un bundle. Un ID viene solitamente utilizzato per differenziare un bundle che deve essere aggiornato o eliminato da un determinato servizio.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Voci</p> </td> 
   <td> <p>Parte di un bundle. I bundle possono essere costituiti da più elementi. Esistono diversi tipi di elementi: testo, numero, booleano (sì/no), data, ora, buffer (dati binari), raccolte, menu di selezione, array e convalida.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Iterator]</p> </td> 
   <td> <p>Tipo di modulo che consente di prendere un unico bundle di dati (un array di dati) e dividerlo in bundle separati. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">Modulo iteratore in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Modulo</p> </td> 
   <td> <p>Un singolo passaggio all'interno di uno scenario che esegue una funzione, ad esempio la creazione di un record, all'interno dell'app o del servizio associato.</p> <p>Ogni app o servizio dispone di vari moduli che definiscono il modo in cui risponde a una richiesta.</p> <p>Esistono 4 tipi di moduli: azioni, trigger, iteratori e aggregatori.</p> <p> <img src="assets/module.jpg"> </p> <p>Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Tipi di moduli</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Operazione</p> </td> 
   <td> <p>Attività eseguita da un modulo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Chiavi pubbliche/private</td> 
   <td>Le chiavi pubbliche e private vengono utilizzate per crittografare e decrittografare i dati. La chiave pubblica può essere distribuita e chiunque disponga della chiave pubblica può crittografare i dati, ma solo la chiave privata può decifrarli. Allo stesso modo, un utente con una chiave privata può crittografare i dati che qualsiasi utente con la chiave pubblica può decrittografare. La crittografia a chiave privata assicura che i dati provengano dal proprietario della chiave privata e funge da convalida dell’origine dei dati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Router [!UICONTROL]</p> </td> 
   <td>Consente di duplicare i dati o di aggiungere nuovi percorsi a uno scenario, in modo da riindirizzare i dati e gestire separatamente diversi gruppi di dati. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/router-module.md" class="MCXref xref">Modulo [!UICONTROL Router] in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Scenario</p> </td> 
   <td> <p>Serie di passaggi automatizzati creati dall'utente, ciascuno rappresentato ed eseguito da un modulo. Lo scopo di uno scenario è quello di spostare e manipolare i dati.</p> <p> <img src="assets/scenario-350x178.jpg" style="width: 350;height: 178;"> </p> <p> Per ulteriori informazioni, consulta <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Transazioni</p> </td> 
   <td> <p>[!DNL Workfront Fusion] utilizza l’elaborazione transazionale per acquisire il ciclo di vita dello scenario. Una transazione consiste in diverse fasi durante le quali i dati vengono trasformati da uno stato coerente a un altro stato coerente. Ci sono 4 fasi: inizializzazione, funzionamento (lettura o scrittura), commit/rollback e finalizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Trigger</p> </td> 
   <td> <p>Un modulo che consente di recuperare i bundle aggiunti o aggiornati dall’ultima esecuzione di uno scenario. I trigger sono di due tipi: sondaggi e istantanei (webhooks). Per ulteriori informazioni, consulta <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Trigger istantanei (webhook) in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Webhook</p> </td> 
   <td> <p>Uno speciale tipo di trigger che ti consente di eseguire uno scenario immediatamente dopo che è disponibile un nuovo bundle. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Trigger istantanei (webhook) in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
