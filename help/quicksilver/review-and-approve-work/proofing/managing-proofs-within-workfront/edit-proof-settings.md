---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Modifica impostazioni bozza
description: Puoi modificare le impostazioni della bozza in qualsiasi momento dopo aver creato una bozza.
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 7%

---

# Modifica impostazioni bozza

Puoi modificare le impostazioni della bozza in qualsiasi momento dopo aver creato una bozza.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td role="rowheader">Ruolo bozza</td> 
   <td>Autore o moderatore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, la mansione o il profilo di autorizzazione della bozza di cui si dispone, contattare l&#39;amministratore di Workfront o Workfront Proof.

+++

## Modifica impostazioni bozza

Alcune impostazioni potrebbero essere bloccate se l’amministratore di Workfront le ha disabilitate a livello di account.

1. Vai al progetto, all&#39;attività o al problema in cui desideri la bozza, quindi fai clic sulla scheda **Documenti**.
1. Passa il puntatore del mouse sulla bozza, quindi fai clic su **Dettagli documento**.
1. Nel pannello a sinistra, fai clic su **Impostazioni visualizzatore di bozze**.
1. Regola le seguenti impostazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Login richiesto. Questa bozza non puÚ essere condivisa con utenti guest</td> 
      <td> <p>Se hai bisogno di livelli di sicurezza più elevati per il processo di revisione e approvazione, puoi utilizzare l’opzione per richiedere l’accesso alla bozza. Ciò significa che solo gli utenti Workfront possono essere aggiunti alla bozza. Per accedervi, è necessario immettere l'indirizzo e-mail e la password.</p> <p>Nota: <em style="font-style: normal;">Se l'accesso richiesto è abilitato, le sottoscrizioni non possono essere abilitate.</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Richiedi la firma elettronica per le decisioni</td> 
      <td> <p>Puoi richiedere una firma elettronica di qualsiasi revisore che prenda una decisione sulla bozza. Quando un revisore prende una decisione, viene visualizzato un messaggio che chiede di inserire la propria e-mail e password e di confermare la decisione. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information, see 
          <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Blocca la bozza quando vengono prese tutte le decisioni necessarie</td> 
      <td> <p>Puoi impostare uno stato di bozza da bloccare quando l’approvatore finale prende la sua decisione. Questa opzione è utile se desideri che i revisori non possano tornare alla bozza e aggiungere ulteriori commenti o modificare le loro decisioni.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti il download del file originale</td> 
      <td> <p>Puoi consentire ai revisori di una bozza di scaricare il file originale da cui è stata creata una bozza. Questa opzione è attivata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti la condivisione bozza tramite URL pubblico o codice integrato</td> 
      <td>Puoi consentire agli utenti di condividere la bozza con un URL pubblico o un codice di incorporamento. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti l'iscrizione alla bozza tramite URL pubblico o codice integrato</td> 
      <td> <p>L’abilitazione dell’abbonamento sulla bozza consente alle persone che non sono state aggiunte esplicitamente alla bozza di abbonarsi alla bozza (ad esempio, aggiungersi alla bozza). A questi verranno quindi assegnati il ruolo e l’avviso e-mail selezionati nelle impostazioni dell’abbonamento.</p> <p>Se l’abbonamento è stato abilitato su una bozza, i campi seguenti diventano attivi:</p> 
       <ul> 
        <li><strong>È richiesta la convalida del sottoscrittore</strong>. Per accedere a una bozza, il sottoscrittore deve fare clic su un collegamento in un messaggio e-mail<br>La selezione di questa opzione indica che il sottoscrittore non otterrà l'accesso immediato alla bozza, ma riceverà un collegamento alla bozza in un messaggio e-mail. Lo scopo della convalida dell’abbonato è garantire che la persona abbia inserito un indirizzo e-mail corretto al quale ha accesso.</li> 
        <li><strong>Ruolo predefinito per i nuovi abbonati -</strong> Questo è il ruolo di bozza predefinito che verrà assegnato a tutti i revisori che si abbonano alla bozza.</li> 
        <li><strong>Avviso e-mail predefinito per i nuovi abbonati</strong>: questo è l'avviso e-mail predefinito che verrà assegnato a tutti i revisori che si abbonano alla bozza.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

 
