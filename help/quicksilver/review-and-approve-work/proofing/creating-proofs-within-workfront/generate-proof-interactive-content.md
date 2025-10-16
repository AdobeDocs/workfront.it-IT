---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Creare una bozza per il contenuto interattivo in un file ZIP
description: Puoi generare una bozza per il contenuto interattivo non-sito web memorizzato in un file ZIP. Esempi di questo tipo di contenuti web includono annunci con streaming video o audio, animazioni HTML, banner interattivi.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# Creare una bozza per il contenuto interattivo in un file ZIP

Puoi generare una bozza per il contenuto interattivo non-sito web memorizzato in un file ZIP. Esempi di questo tipo di contenuti web includono annunci con streaming video o audio, animazioni HTML, banner interattivi.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Standard</p>
   <p>Lavoro o piano</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai documenti</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una bozza per il contenuto interattivo in un file ZIP

Dopo aver aggiunto il contenuto interattivo in un file ZIP a una bozza, Adobe Workfront crea una bozza dei documenti compressi. A seconda delle dimensioni del file, il tempo di caricamento può variare. La creazione di file di grandi dimensioni richiede più tempo. Puoi spostarti dalla pagina e Workfront continua a creare il file. La dimensione massima per il caricamento dei file è di 4 GB. 

1. Prepara il contenuto creando un file ZIP in bundle.

   Il file ZIP deve soddisfare i seguenti requisiti:

   * Tutte le risorse, come CSS, JavaScript, video, suoni e immagini devono essere incluse nel file del bundle.
   * Assicurarsi che il file principale (ad esempio index.html, index.htm) si trovi nella cartella principale e che sia l&#39;unico file html/.htm memorizzato.

     Se il file principale non viene inserito nella cartella principale, Workfront cerca la cartella per trovare il file principale.

   * La dimensione massima del bundle è di 500 MB.
   * Nel caso di file ZIP creati in iOS, lo strumento identifica automaticamente la cartella corretta in cui viene inserito il contenuto.

1. Vai al progetto, all’attività o al problema in cui desideri caricare il file ZIP.
1. Fai clic su **Documenti** nel pannello a sinistra.
1. Fai clic su **Aggiungi nuovo**, quindi fai clic su **Bozza** nel menu visualizzato.
1. Nella sezione **Aggiungi file**, trascina o sfoglia il file ZIP necessario.
1. Fai clic su **Crea bozza** per creare una bozza semplice senza processo di revisione.\
   oppure\
   Continua con la configurazione di una bozza avanzata:

   * [Creare una bozza avanzata con un flusso di lavoro di base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Creare una bozza avanzata con un flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
