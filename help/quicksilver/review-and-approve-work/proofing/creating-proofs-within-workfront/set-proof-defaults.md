---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Configurare i valori predefiniti per la verifica personale
description: Puoi definire le impostazioni predefinite della bozza personali che si applicano alle bozze create. Queste impostazioni predefinite vengono applicate ogni volta che si genera una bozza iniziale o si carica una nuova versione di bozza in Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 278bff89-0305-407b-9def-d06820d908de
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Configurare i valori predefiniti per la verifica personale

Puoi definire le impostazioni predefinite della bozza personali che si applicano alle bozze create. Queste impostazioni predefinite vengono applicate ogni volta che si genera una bozza iniziale o si carica una nuova versione di bozza in Workfront.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Piano corrente: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Seleziona o superiore</p> <p>Per ulteriori informazioni sulla verifica dell'accesso con i diversi piani, vedere <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alla funzionalità di verifica in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano corrente: Lavoro o Piano</p> <p>Piano legacy: qualsiasi (per l’utente deve essere abilitata la verifica)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, la mansione o il profilo di autorizzazione della bozza di cui si dispone, contattare l&#39;amministratore di Workfront o Workfront Proof.

## Configurare i valori predefiniti per la verifica personale

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Strumenti di correzione**.

1. Nell&#39;angolo superiore destro fare clic sull&#39;avatar e selezionare **Impostazioni personali**.
1. Scegliere la scheda **Impostazioni predefinite bozza**, quindi specificare le informazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td colspan="2"><strong>Impostazioni predefinite notifiche e-mail</strong> </td> 
     </tr> 
     <tr> 
      <td>Avviso e-mail predefinito</td> 
      <td>Seleziona la frequenza con cui l’utente riceve gli aggiornamenti e-mail. Selezionare Tutte le attività, Risposte ai commenti, Decisioni, Decisione finale, Riepilogo orario, Riepilogo giornaliero o Disabilitato.</td> 
     </tr> 
     <tr> 
      <td>Avviso e-mail predefinito per i nuovi revisori ospiti</td> 
      <td>Seleziona la frequenza con cui i revisori guest ricevono gli aggiornamenti e-mail. Le opzioni sono le stesse dell’avviso e-mail predefinito.</td> 
     </tr> 
     <tr> 
      <td>Notifica nuova bozza</td> 
      <td>Scegli di ricevere una notifica quando vieni aggiunto a una bozza.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>Impostazioni messaggio</strong> </td> 
     </tr> 
     <tr> 
      <td>Modello oggetto bozza</td> 
      <td>Digita cosa vuoi che gli utenti vedano nell’oggetto di un’e-mail quando condividi una bozza con loro.</td> 
     </tr> 
     <tr> 
      <td>Modello di messaggio bozza</td> 
      <td>Digita cosa desideri che gli utenti vedano nel corpo di un’e-mail quando condividi una bozza con loro.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>Impostazioni bozza predefinite</strong> </td> 
     </tr> 
     <tr> 
      <td>Blocca la bozza quando vengono prese tutte le decisioni</td> 
      <td>Scegli di bloccare automaticamente la bozza da ulteriori modifiche dopo aver preso tutte le decisioni.</td> 
     </tr> 
     <tr> 
      <td>Richiedi una sola decisione</td> 
      <td>Scegli di richiedere una sola decisione su una bozza.</td> 
     </tr> 
     <tr> 
      <td>Accesso richiesto</td> 
      <td> <p>Scegli di rendere la bozza disponibile solo agli utenti con credenziali di accesso di Workfront Proof.</p> <p>Nota: le credenziali di Workfront Proof possono essere diverse dalle credenziali di Workfront, a meno che l’azienda non utilizzi l’SSO. È consigliabile utilizzare questa funzione solo se l’SSO degli utenti della tua azienda è valido.</p> </td> 
     </tr> 
     <tr> 
      <td>Abbonamento abilitato</td> 
      <td>Consenti ai revisori esterni all’organizzazione di registrarsi per la bozza tramite l’URL pubblico o il codice di incorporamento. Quando questa opzione è selezionata, l’abbonato deve fare clic su un collegamento in un’e-mail per accedere a una bozza. Seleziona questa opzione per richiedere al revisore esterno di fare clic su un collegamento nell’e-mail per accedere alla bozza. Questa opzione è abilitata per impostazione predefinita se l’opzione Condivisione pubblica è selezionata e viene applicata a tutte le bozze create da questo utente. </td> 
     </tr> 
     <tr> 
      <td>Ruolo predefinito per i nuovi revisori ospiti</td> 
      <td>Seleziona un ruolo di bozza predefinito per i revisori ospiti. Le opzioni sono le stesse del ruolo Bozza predefinita.</td> 
     </tr> 
     <tr> 
      <td>Blocca download del file originale</td> 
      <td>Scegliere questa opzione per impedire agli utenti di scaricare il file originale. </td> 
     </tr> 
     <tr> 
      <td>Il mio ruolo di bozza predefinito</td> 
      <td>Scegli il tuo ruolo di bozza predefinito. </td> 
     </tr> 
     <tr> 
      <td>Colore markup predefinito</td> 
      <td>Scegliere il colore di markup predefinito. </td> 
     </tr> 
    </tbody> 
   </table>
