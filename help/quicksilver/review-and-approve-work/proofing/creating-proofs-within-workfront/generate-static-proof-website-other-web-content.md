---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Creare una bozza statica per un sito web o altro contenuto web
description: Puoi generare una nuova bozza statica o una nuova versione di una bozza statica esistente per il contenuto web. I contenuti web possono includere annunci con video in streaming, animazioni HTML o banner interattivi, ma saranno tagliati in più schermate per consentire la correzione statica.
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

# Creare una bozza statica per un sito web o altro contenuto web

Puoi generare una nuova bozza statica o una nuova versione di una bozza statica esistente per il contenuto web. I contenuti web possono includere annunci con video in streaming, animazioni HTML o banner interattivi, ma saranno tagliati in più schermate per consentire la correzione statica.

Quando crei bozze statiche per un sito web o altro contenuto web, considera quanto segue:

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Piano attuale: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Seleziona o Premium</p> <p>Per ulteriori informazioni sulla verifica dell’accesso con i diversi piani, consulta <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alle funzionalità di correzione in Workfront</a>.</p> </td> 
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

## Creare una bozza statica per un sito web o altro contenuto web

Per creare una bozza statica, il sito web deve essere accessibile al pubblico (non dietro un firewall) oppure il inserire nell&#39;elenco Consentiti dell’organizzazione deve includere il dominio Workfront . Workfront non è in grado di acquisire un sito web protetto da password come bozza statica.

>[!TIP]
>
>Per le pagine interne che richiedono autorizzazioni e pagine protette da password, è consigliabile eseguire prove interattive anziché eseguire prove statiche. Per ulteriori informazioni, consulta [Panoramica delle bozze dei contenuti interattivi](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Passa al progetto, all’attività o al problema in cui desideri creare una nuova bozza del sito web o una nuova versione di una versione esistente.
1. Fai clic su **Documenti** nel pannello a sinistra .
1. (Condizionale) Se crei una nuova bozza, fai clic su **Aggiungi nuovo**, quindi fai clic su **Prova** nel menu visualizzato.
1. (Condizionale) Se crei una nuova versione di una bozza esistente:

   1. Passa il puntatore del mouse sulla bozza dell’URL per la quale desideri creare una nuova versione, quindi selezionala facendo clic su in blu chiaro sullo sfondo che lo circonda.

      ![Select_proof_by_select_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. Fai clic su **Aggiungi nuovo** > **Versione** > **Prova**.

1. Digita l’URL del sito web da verificare nel **Aggiungi file** area, quindi premere **Invio**.

   L’URL viene visualizzato sotto la casella in cui è stato digitato.

   ![](assets/url-name-appears-below-350x142.png)

1. Fai clic sull’URL aggiunto.

   Vengono visualizzate le opzioni per la configurazione della bozza del sito web.

   ![](assets/interactive-proof-radio-btn-area-350x199.png)

1. (Facoltativo) Per modificare il nome della bozza dall’URL del sito Web a qualcos’altro, digita un **Nome della bozza.**
1. Assicurati **Schermata di acquisizione** è selezionato e utilizza una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Risoluzione dello schermo</strong> </td> 
      <td> <p>Regola la risoluzione dei contenuti quando i revisori visualizzano la bozza, consentendo loro di vedere come appare su dispositivi di dimensioni diverse, come telefoni, tablet e monitor.</p> <p>Se selezioni più risoluzioni, viene creata una bozza separata per ogni risoluzione selezionata.</p> <p>Nota: Quando un revisore commenta la bozza, il commento include la risoluzione che mostra quando è stato fatto il commento, in modo che altri revisori sappiano quale risoluzione è associata al commento. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Cercare pagine secondarie</strong> </td> 
      <td> <p>Acquisire le pagine secondarie del sito web e le relative pagine principali. È possibile fare clic su Seleziona tutto per includere tutte le pagine oppure fare clic solo su alcune pagine da includere. I pulsanti più e meno consentono di espandere e chiudere le aree della pagina secondaria del sito web.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Non è possibile modificare l&#39;impostazione Capture screenshot per le versioni successive della bozza creata.

1. Fai clic su **Fine**.

   Se hai selezionato più risoluzioni dello screenshot nel passaggio 8, l&#39;elenco include un set di schermate per ogni risoluzione. Puoi generare queste schermate come bozze separate o combinarle in un’unica bozza (vedi in .). È consigliabile combinarle, soprattutto se si sta creando una bozza statica del sito web.

   >[!NOTE]
   >
   >Se aggiungi una nuova versione a una bozza URL esistente, tutte le opzioni configurate sulla bozza originale o sulla versione precedente vengono mantenute in questa versione.

1. Fai clic su **Crea bozza** per creare una bozza semplice senza processo di revisione.\
   oppure\
   Continua configurando una bozza avanzata:

   * [Creare una bozza avanzata con un flusso di lavoro di base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Creare una bozza avanzata con un flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
