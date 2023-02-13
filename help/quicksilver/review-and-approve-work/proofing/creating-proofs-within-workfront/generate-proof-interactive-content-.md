---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Creare una bozza per il contenuto interattivo in un file ZIP
description: Puoi generare una bozza per il contenuto interattivo non del sito web memorizzato in un file ZIP. Esempi di questo tipo di contenuto web includono annunci con streaming video o audio, animazioni HTML, banner interattivi.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# Creare una bozza per il contenuto interattivo in un file ZIP

Puoi generare una bozza per il contenuto interattivo non del sito web memorizzato in un file ZIP. Esempi di questo tipo di contenuto web includono annunci con streaming video o audio, animazioni HTML, banner interattivi.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Piano attuale: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Premium</p> <p>Per ulteriori informazioni sulla verifica dell’accesso con i diversi piani, consulta <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alle funzionalità di correzione in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano attuale: Lavoro o piano</p> <p>Piano legacy: Qualsiasi (è necessario che la correzione sia attivata per l’utente)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il ruolo o il profilo delle autorizzazioni di prova, contattare l&#39;amministratore Workfront o Workfront Proof.

## Creare una bozza per il contenuto interattivo in un file ZIP

Una volta aggiunto il contenuto interattivo in un file ZIP a una bozza, Adobe Workfront crea una bozza dei documenti compressi. A seconda delle dimensioni del file, il tempo di caricamento può variare. La creazione di file più grandi richiede più tempo. Puoi allontanarti dalla pagina e Workfront continua a creare il file. La dimensione massima di caricamento dei file è 4 GB. 

1. Prepara il contenuto creando un file ZIP in bundle.

   Il file ZIP deve soddisfare i seguenti requisiti:

   * Tutte le risorse, come CSS, JavaScript, video, suoni e immagini, devono essere incluse nel file del bundle.
   * Assicurati che il file principale (ad esempio index.html, index.htm) si trovi nella cartella principale e che sia l&#39;unico file .html/.htm memorizzato in tale cartella.

      Se il file principale non si trova nella cartella principale, Workfront cerca nella cartella il file principale.

   * La dimensione massima del bundle è 500 MB.
   * Nel caso di file ZIP creati in iOS, lo strumento identifica automaticamente la cartella corretta in cui viene posizionato il contenuto.

1. Vai al progetto, all&#39;attività o al problema in cui desideri caricare il file ZIP.
1. Fai clic su **Documenti** nel pannello a sinistra .
1. Fai clic su **Aggiungi nuovo**, quindi fai clic su **Prova** nel menu visualizzato.
1. In **Aggiungi file** , trascina e rilascia o sfoglia il file ZIP necessario.
1. Fai clic su **Crea bozza** per creare una bozza semplice senza processo di revisione.\
   oppure\
   Continua configurando una bozza avanzata:

   * [Creare una bozza avanzata con un flusso di lavoro di base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Creare una bozza avanzata con un flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
