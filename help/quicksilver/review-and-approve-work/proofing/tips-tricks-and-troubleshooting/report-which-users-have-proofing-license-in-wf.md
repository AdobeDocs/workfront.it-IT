---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Elencare gli utenti con una licenza di correzione in Adobe Workfront
description: È possibile visualizzare gli utenti di Adobe Workfront che dispongono attualmente dell’opzione "L’utente può generare bozze" abilitata in uno dei seguenti modi.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Elencare gli utenti con una licenza di correzione in Adobe Workfront

È possibile visualizzare gli utenti di Adobe Workfront che dispongono attualmente dell’opzione &quot;L’utente può generare bozze&quot; abilitata in uno dei seguenti modi.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Piano legacy: Seleziona o Premium</p> <p>Per ulteriori informazioni sulla verifica dell’accesso con i diversi piani, consulta <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alle funzionalità di correzione in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Modifica accesso a:</p> 
    <ul> 
     <li> <p>Creare rapporti, dashboard e calendari</p> </li> 
     <li> <p>Creare filtri, visualizzazioni e gruppi</p> </li> 
    </ul> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il ruolo o il profilo delle autorizzazioni di prova, contattare l&#39;amministratore Workfront o Workfront Proof.

## Creare un rapporto utente

Puoi creare un rapporto per gli utenti per vedere quali utenti possono generare le bozze:

1. Passa a **Reporting** area.
1. Fai clic sul pulsante **Nuovo rapporto** menu a discesa, quindi fai clic su **Report utente**.

1. Sulla **Filtri** scheda , fai clic su **Aggiungere una regola filtro**.

1. Nel campo disponibile, espandi **Utente**, quindi fai clic su **Con licenza di prova**.

1. Seleziona **Uguale** > **True**.

   ![report_prooflicenses.png](assets/report-prooflicenses-350x135.png)

1. Fai clic su **Salva e chiudi**.

   Il rapporto visualizza tutti gli utenti di Workfront a cui è stata assegnata una licenza di correzione.

## Aggiornare la visualizzazione Persone

Puoi aggiungere una nuova colonna nella vista Persone per visualizzare quali utenti possono generare le bozze:

1. Vai a **Persone** area.
1. Fai clic sul pulsante **Persone** scheda .
1. In **Visualizza** menu a discesa, effettuare una delle seguenti operazioni:

   * Per aggiungere queste informazioni a una visualizzazione esistente, selezionare la visualizzazione da personalizzare, quindi fare clic su **Personalizza visualizzazione**.
   * Per aggiungere queste informazioni a una nuova visualizzazione, fare clic su **Nuova vista**.

1. Fai clic su **Aggiungi colonna**.
1. Nel campo disponibile, espandi **Utente**, quindi fai clic su **Con licenza di prova**.

1. Fai clic su **Fine**, quindi fai clic su **Salva visualizzazione** o **Salva come nuova vista**.

   Viene visualizzata la vista **True** o **False** a seconda che l’utente disponga di una licenza di correzione.
