---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Modifica impostazioni bozza
description: Puoi modificare le impostazioni della bozza in qualsiasi momento dopo aver creato una bozza.
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 7%

---

# Modifica impostazioni bozza

Puoi modificare le impostazioni della bozza in qualsiasi momento dopo aver creato una bozza.

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
   <td role="rowheader">Ruolo bozza</td> 
   <td>Autore o moderatore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il ruolo o il profilo delle autorizzazioni di prova, contattare l&#39;amministratore Workfront o Workfront Proof.

## Modifica impostazioni bozza

Alcune impostazioni possono essere bloccate se l’amministratore di Workfront le ha disattivate a livello di account.

1. Vai al progetto, all&#39;attività o al problema in cui desideri ottenere la bozza, quindi fai clic sul pulsante **Documenti** scheda .
1. Passa il puntatore del mouse sulla bozza, quindi fai clic su **Dettagli documento**.
1. Nel pannello a sinistra, fai clic su **Impostazioni del visualizzatore di correzione**.
1. Regola le seguenti impostazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Login richiesto. Questa bozza non puÚ essere condivisa con utenti guest</td> 
      <td> <p>Se hai bisogno di livelli di sicurezza più elevati per il processo di revisione e approvazione, puoi utilizzare l’accesso alla bozza. Questo significa che solo gli utenti Workfront possono essere aggiunti alla bozza. Devono immettere la propria e-mail e password prima di potervi accedere.</p> <p>Nota: <em style="font-style: normal;">Se l’accesso richiesto è abilitato, le sottoscrizioni non possono essere abilitate.</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Richiedi la firma elettronica per le decisioni</td> 
      <td> <p>È possibile richiedere una firma elettronica di qualsiasi revisore che prenda una decisione sulla bozza. Quando un revisore prende una decisione, viene visualizzato un prompt che chiede loro di inserire la propria e-mail e password e di confermare la propria decisione. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information, see 
          <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Blocca la prova quando vengono prese tutte le decisioni necessarie</td> 
      <td> <p>Puoi impostare uno stato di bozza da bloccare quando l’Approvatore finale prenderà la sua decisione. È utile se desideri che i revisori non siano in grado di tornare alla bozza e aggiungere altri commenti o modificare le loro decisioni.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti il download del file originale</td> 
      <td> <p>È possibile consentire ai revisori di una bozza di scaricare il file originale da cui è stata creata una bozza. Questa opzione è attivata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti la condivisione bozza tramite URL pubblico o codice integrato</td> 
      <td>Puoi consentire agli utenti di condividere la bozza con un URL pubblico o un codice di incorporamento. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti l'iscrizione alla bozza tramite URL pubblico o codice integrato</td> 
      <td> <p>L’abilitazione dell’abbonamento sulla bozza consente alle persone che non sono state aggiunte esplicitamente alla bozza di sottoscriversi alla bozza (ad esempio, aggiungersi alla bozza). Gli verranno quindi assegnati il ruolo e l’avviso e-mail selezionati per tali utenti nelle impostazioni di abbonamento.</p> <p>Se l’opzione Abbonamento è stata abilitata su una bozza, i campi seguenti diventeranno attivi:</p> 
       <ul> 
        <li><strong>Convalida del sottoscrittore obbligatoria</strong> - L’utente con sottoscrizione deve fare clic su un collegamento in un messaggio e-mail per accedere a una bozza<br>Selezionando questa opzione, la persona che si abbona non avrà accesso immediato alla bozza, ma riceverà un collegamento alla bozza in un messaggio e-mail. Lo scopo della convalida dell'utente con sottoscrizione è quello di garantire che l'utente abbia inserito un indirizzo e-mail corretto al quale ha accesso.</li> 
        <li><strong>Ruolo predefinito per i nuovi abbonati -</strong> Questo è il ruolo di bozza predefinito che verrà assegnato a tutti i revisori che si abbonano alla bozza.</li> 
        <li><strong>Avviso e-mail predefinito per i nuovi abbonati</strong> - Questo è l’avviso e-mail predefinito che verrà assegnato a tutti i revisori che si abbonano alla bozza.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

 
