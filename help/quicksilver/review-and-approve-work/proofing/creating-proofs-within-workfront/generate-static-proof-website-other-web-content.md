---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Creare una bozza statica per un sito web o altro contenuto web
description: Puoi generare una nuova bozza statica o una nuova versione di una bozza statica esistente per il contenuto web. Il contenuto web può includere annunci con video in streaming, animazioni HTML o banner interattivi, ma verrà tagliato in più schermate per consentire una verifica statica.
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 1%

---

# Creare una bozza statica per un sito web o altro contenuto web

Puoi generare una nuova bozza statica o una nuova versione di una bozza statica esistente per il contenuto web. Il contenuto web può includere annunci con video in streaming, animazioni HTML o banner interattivi, ma verrà tagliato in più schermate per consentire una verifica statica.

Quando crei bozze statiche per un sito web o per altri contenuti web, considera quanto segue:

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
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> 
   <p>Standard</p>
   <p>Lavoro o piano</p> </td> 
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

## Creare una bozza statica per un sito web o altro contenuto web

Per creare una bozza statica, il sito web deve essere accessibile al pubblico (non dietro un firewall), oppure il inserisco nell&#39;elenco Consentiti di gestione dell’organizzazione deve includere il dominio Workfront. Workfront non può acquisire un sito web protetto da password come bozza statica.

>[!TIP]
>
>È consigliabile utilizzare la verifica interattiva anziché la verifica statica per le pagine interne che richiedono autorizzazioni e le pagine protette da password. Per ulteriori informazioni, vedere [Panoramica delle bozze dei contenuti interattivi](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Vai al progetto, all’attività o al problema in cui desideri creare una nuova bozza del sito web o una nuova versione di una bozza esistente.
1. Fai clic su **Documenti** nel pannello a sinistra.
1. (Condizionale) Se stai creando una nuova bozza, fai clic su **Aggiungi nuova**, quindi fai clic su **Bozza** nel menu visualizzato.
1. (Condizionale) Se stai creando una nuova versione di una bozza esistente:

   1. Passa il puntatore del mouse sulla bozza URL per la quale desideri creare una nuova versione, quindi selezionala facendo clic sullo sfondo blu chiaro che la circonda.

      ![Seleziona_bozza_selezionando_sfondo_azzurro_chiaro.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. Fai clic su **Aggiungi nuovo** > **Versione** > **Bozza**.

1. Digitare l&#39;URL del sito Web da verificare nell&#39;area **Aggiungi file**, quindi premere **Invio**.

   >[!NOTE]
   >
   > L&#39;URL deve contenere meno di 2.000 caratteri.

1. Fai clic sull’URL aggiunto.

   Vengono visualizzate le opzioni per la configurazione della bozza del sito Web.

   ![Bozza interattiva](assets/interactive-proof-radio-btn-area-350x199.png)

1. (Facoltativo) Se desideri modificare il nome della bozza dall&#39;URL del sito Web in un altro nome, digita **Nome bozza.**
1. Assicurati che **Acquisisci schermata** sia selezionato e utilizza una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Risoluzione schermata</strong> </td> 
      <td> <p>Regola la risoluzione del contenuto quando i revisori visualizzano la bozza, consentendo loro di vedere come appare su dispositivi di dimensioni diverse, come telefoni, tablet e monitor.</p> <p>Se selezioni più risoluzioni, viene creata una bozza separata per ogni risoluzione selezionata.</p> <p>Nota: quando un revisore aggiunge un commento alla bozza, il commento include la risoluzione che indica quando il commento è stato creato, in modo che gli altri revisori sappiano quale risoluzione è associata al commento. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Cerca pagine secondarie</strong> </td> 
      <td> <p>Acquisisci le pagine secondarie del sito web e le relative pagine principali. Puoi fare clic su Seleziona tutto per includere tutte le pagine, oppure puoi fare clic solo su determinate pagine che desideri includere. I pulsanti più e meno consentono di espandere e chiudere le aree delle pagine secondarie del sito Web.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Non è possibile modificare l’impostazione Acquisisci schermata per nessuna versione successiva della bozza creata.

1. Fai clic su **Fine**.

   Se hai selezionato più risoluzioni di screenshot al passaggio 8, l’elenco include una serie di screenshot per ogni risoluzione. Puoi generare queste schermate come bozze separate o combinarle in un’unica bozza (vedi  in .). È consigliabile combinarle, soprattutto se si sta creando una bozza statica del sito Web.

   >[!NOTE]
   >
   >Se stai aggiungendo una nuova versione a una bozza URL esistente, tutte le opzioni configurate sulla bozza originale o sulla versione precedente vengono mantenute in questa versione.

1. Fai clic su **Crea bozza** per creare una bozza semplice senza processo di revisione.\
   oppure\
   Continua con la configurazione di una bozza avanzata:

   * [Creare una bozza avanzata con un flusso di lavoro di base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Creare una bozza avanzata con un flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
