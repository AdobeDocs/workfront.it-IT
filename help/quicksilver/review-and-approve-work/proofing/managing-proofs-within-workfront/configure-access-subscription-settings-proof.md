---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: Configurare le impostazioni di accesso e abbonamento per una bozza
description: Puoi configurare alcune impostazioni di accesso e abbonamento per le singole bozze, ad esempio se richiedere agli utenti di accedere e se consentire agli utenti di abbonarsi alla bozza. È possibile impostare le impostazioni di accesso e abbonamento per una bozza durante la sua creazione oppure impostarle per una bozza già esistente in Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 0%

---

# Configurare le impostazioni di accesso e abbonamento per una bozza

Puoi configurare alcune impostazioni di accesso e abbonamento per le singole bozze, ad esempio se richiedere agli utenti di accedere e se consentire agli utenti di abbonarsi alla bozza. È possibile impostare le impostazioni di accesso e abbonamento per una bozza durante la sua creazione oppure impostarle per una bozza già esistente in Workfront.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Piano corrente: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Premium</p> <p>Per ulteriori informazioni sulla verifica dell'accesso con i diversi piani, vedere <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alla funzionalità di verifica in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano corrente: Lavoro o Piano</p> <p>Piano legacy: qualsiasi (per l’utente deve essere abilitata la verifica)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, la mansione o il profilo di autorizzazione della bozza di cui si dispone, contattare l&#39;amministratore di Workfront o Workfront Proof.

## Configurare le impostazioni di accesso e abbonamento durante la creazione di una bozza

Per impostare le impostazioni di accesso e abbonamento per una bozza durante la sua creazione:

1. Vai al progetto, all&#39;attività o al problema in cui desideri la bozza, quindi fai clic sulla sezione **Documenti**.
1. Fai clic su **Aggiungi nuovo** in alto a destra.
1. Scorri fino alla sezione **Impostazioni bozza** nell&#39;angolo inferiore destro della pagina **Nuova bozza**.

1. Configura le seguenti impostazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Consenti condivisione bozze tramite URL pubblico o codice di incorporamento</strong> </td> 
      <td>Quando questa opzione è selezionata, la bozza può essere condivisa tramite un URL pubblico o un codice di incorporamento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Consenti l'iscrizione alla bozza tramite URL pubblico o codice di incorporamento</strong> </td> 
      <td>Quando questa opzione è selezionata, le persone che non sono state aggiunte esplicitamente alla bozza possono abbonarsi alla bozza. Alla persona che si abbona alla bozza vengono assegnati il ruolo e l’e-mail definiti nelle seguenti impostazioni:
       <ul>
        <li><p><strong>Ruolo del sottoscrittore:</strong> Ruolo di bozza predefinito assegnato a tutti i revisori che sottoscrivono la bozza. </p><p>Importante: se <strong>Consenti condivisione con</strong> è impostato su un valore diverso da <strong>Tutti</strong> nelle impostazioni di Workfront Proof, l'abbonamento funziona solo per gli utenti dell'organizzazione. Per ulteriori informazioni, vedere <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configurare le impostazioni di bozza in Workfront Proof</a>.</p></li>
        <li><strong>Impostazioni degli avvisi e-mail per i sottoscrittori:</strong> L'avviso e-mail predefinito assegnato a tutti i revisori che si abbonano alla bozza.</li>
       </ul><p>
        <ul>
         <li><strong>Accesso alla bozza tramite collegamento e-mail richiesto per:</strong> Configurare se il sottoscrittore riceve un'e-mail con un collegamento alla bozza. È possibile selezionare <strong>Nessuna e-mail</strong> (il collegamento e-mail non è necessario per accedere alla bozza), <strong>Solo e-mail di notifica bozza</strong> (l'abbonato riceve un collegamento alla bozza tramite e-mail senza alcuna verifica) o <strong>E-mail di notifica di convalida e bozza</strong> (l'abbonato riceve un collegamento alla bozza tramite e-mail e deve fare clic sul collegamento per accedere a una bozza; lo scopo di questa opzione è verificare che l'utente abbia immesso un indirizzo e-mail corretto al quale ha accesso).</li>
        </ul><p>Nota:  Se alle bozze è allegato un flusso di lavoro automatico, tutti gli abbonamenti genereranno e-mail di conferma ai proprietari delle bozze, in modo che possano decidere a quale fase aggiungere la persona.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continua a creare la bozza.

## Configurare le impostazioni di accesso e abbonamento per una bozza esistente

Per impostare le impostazioni di accesso e abbonamento per una bozza già esistente in Workfront:

1. Nell&#39;area Documenti selezionare il documento contenente la bozza per cui si desidera configurare le impostazioni, quindi fare clic su **Dettagli documento**.
1. Nel pannello a sinistra, fai clic su **Impostazioni visualizzatore di bozze**.
1. Configura le seguenti impostazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Consenti condivisione bozze tramite URL pubblico o codice di incorporamento</strong><strong>e</strong> </td> 
      <td>Quando questa opzione è selezionata, la bozza può essere condivisa tramite un URL pubblico o un codice di incorporamento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Consenti l'iscrizione alla bozza tramite URL pubblico o codice di incorporamento</strong> </td> 
      <td>Quando questa opzione è selezionata, le persone che non sono state aggiunte esplicitamente alla bozza possono abbonarsi alla bozza. Alla persona che si abbona alla bozza vengono assegnati il ruolo e l’e-mail definiti nelle seguenti impostazioni:
       <ul>
        <li><p><strong>Ruolo del sottoscrittore:</strong> Ruolo di bozza predefinito assegnato a tutti i revisori che sottoscrivono la bozza. </p><p>Importante: se <strong>Consenti condivisione con</strong> è impostato su un valore diverso da <strong>Tutti</strong> nelle impostazioni di Workfront Proof, l'abbonamento funziona solo per gli utenti dell'organizzazione. Per ulteriori informazioni, vedere <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configurare le impostazioni di bozza in Workfront Proof</a>.</p></li>
        <li><strong>Impostazioni degli avvisi e-mail per i sottoscrittori:</strong> L'avviso e-mail predefinito assegnato a tutti i revisori che si abbonano alla bozza.</li>
       </ul><p>
        <ul>
         <li><strong>Accesso alla bozza tramite collegamento e-mail richiesto per:</strong> Configurare se il sottoscrittore riceve un'e-mail con un collegamento alla bozza. È possibile selezionare <strong>Nessuna e-mail</strong> (il collegamento e-mail non è necessario per accedere alla bozza), <strong>Solo e-mail di notifica bozza</strong> (l'abbonato riceve un collegamento alla bozza tramite e-mail senza alcuna verifica) o <strong>E-mail di notifica di convalida e bozza</strong> (l'abbonato riceve un collegamento alla bozza tramite e-mail e deve fare clic sul collegamento per accedere a una bozza; lo scopo di questa opzione è verificare che l'utente abbia immesso un indirizzo e-mail corretto al quale ha accesso).</li>
        </ul><p>Nota:  Se alle bozze è allegato un flusso di lavoro automatico, tutti gli abbonamenti genereranno e-mail di conferma ai proprietari delle bozze, in modo che possano decidere a quale fase aggiungere la persona.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.
