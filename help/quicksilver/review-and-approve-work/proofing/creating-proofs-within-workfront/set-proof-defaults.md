---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Configurare le impostazioni predefinite di correzione personali
description: Puoi definire le impostazioni predefinite per la bozza personale da applicare alle bozze create. Queste impostazioni predefinite vengono applicate ogni volta che si genera una bozza per la prima volta o si carica una nuova versione di bozza in Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 278bff89-0305-407b-9def-d06820d908de
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Configurare le impostazioni predefinite di correzione personali

Puoi definire le impostazioni predefinite per la bozza personale da applicare alle bozze create. Queste impostazioni predefinite vengono applicate ogni volta che si genera una bozza per la prima volta o si carica una nuova versione di bozza in Workfront.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Piano attuale: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Seleziona o superiore</p> <p>Per ulteriori informazioni sulla verifica dell’accesso con i diversi piani, consulta <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alle funzionalità di correzione in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano attuale: Lavoro o piano</p> <p>Piano legacy: Qualsiasi (è necessario che la correzione sia attivata per l’utente)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il ruolo o il profilo delle autorizzazioni di prova, contattare l&#39;amministratore Workfront o Workfront Proof.

## Configurare le impostazioni predefinite di correzione personali

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Copertura**.

1. Nell&#39;angolo in alto a destra, fai clic sull&#39;avatar e seleziona **Impostazioni personali**.
1. Scegli la **Valori predefiniti di correzione** , quindi specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td colspan="2"><strong>Impostazioni predefinite delle notifiche e-mail</strong> </td> 
     </tr> 
     <tr> 
      <td>Avviso e-mail predefinito</td> 
      <td>Seleziona la frequenza con cui l’utente riceve gli aggiornamenti e-mail. Seleziona Tutte le attività, Risposte ai miei commenti, Decisioni, Decisioni finali, Riepilogo orario, Riepilogo giornaliero o Disabilitato.</td> 
     </tr> 
     <tr> 
      <td>Avviso e-mail predefinito per i nuovi revisori ospiti</td> 
      <td>Seleziona la frequenza con cui i revisori ricevono gli aggiornamenti e-mail. Le opzioni sono le stesse di quelle per l’avviso e-mail predefinito.</td> 
     </tr> 
     <tr> 
      <td>Notifica a prova nuova</td> 
      <td>Scegli di ricevere una notifica quando vieni aggiunto a una bozza.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>Impostazioni messaggio</strong> </td> 
     </tr> 
     <tr> 
      <td>Modello del soggetto di prova</td> 
      <td>Digita ciò che vuoi che gli utenti vedano nell’oggetto di un messaggio e-mail quando condividi una bozza con loro.</td> 
     </tr> 
     <tr> 
      <td>Modello di messaggio di bozza</td> 
      <td>Digita ciò che vuoi che gli utenti vedano nel corpo di un’e-mail quando condividi una bozza con loro.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>Impostazioni predefinite della bozza</strong> </td> 
     </tr> 
     <tr> 
      <td>Blocca la prova quando vengono prese tutte le decisioni</td> 
      <td>Scegli di bloccare automaticamente la bozza da ulteriori modifiche dopo che tutte le decisioni sono state prese.</td> 
     </tr> 
     <tr> 
      <td>Solo una decisione</td> 
      <td>Scegli di richiedere una sola decisione su una bozza.</td> 
     </tr> 
     <tr> 
      <td>Accesso richiesto</td> 
      <td> <p>Scegli di rendere la bozza disponibile solo agli utenti con le credenziali di accesso di Workfront Proof.</p> <p>Nota: Le credenziali di Workfront Proof possono essere diverse dalle credenziali di Workfront, a meno che gli utenti della tua azienda non siano SSO. Si consiglia di utilizzare questa funzione solo se l’utente della tua azienda utilizza SSO.</p> </td> 
     </tr> 
     <tr> 
      <td>Sottoscrizione abilitata</td> 
      <td>Consenti ai revisori esterni all'organizzazione di registrarsi per la bozza tramite l'URL pubblico o il codice di incorporamento. Quando questa opzione è selezionata, l’utente iscritto deve fare clic su un collegamento in un messaggio e-mail per accedere a una bozza che è anche disponibile. Seleziona questa opzione per richiedere al revisore esterno di fare clic su un collegamento all’interno dell’e-mail per accedere alla bozza. Questa opzione è attivata per impostazione predefinita se l’opzione Condivisione pubblica è selezionata e viene applicata a tutte le bozze create dall’utente. </td> 
     </tr> 
     <tr> 
      <td>Ruolo predefinito per i nuovi revisori ospiti</td> 
      <td>Seleziona un ruolo di bozza predefinito per i revisori ospiti. Le opzioni sono le stesse di quelle nel ruolo di bozza predefinito.</td> 
     </tr> 
     <tr> 
      <td>Blocco del download del file originale</td> 
      <td>Scegli di impedire agli utenti di scaricare il file originale. </td> 
     </tr> 
     <tr> 
      <td>Ruolo di bozza predefinito</td> 
      <td>Scegli il ruolo di bozza predefinito. </td> 
     </tr> 
     <tr> 
      <td>Colore di markup predefinito</td> 
      <td>Scegliere il colore di marcatura predefinito. </td> 
     </tr> 
    </tbody> 
   </table>
