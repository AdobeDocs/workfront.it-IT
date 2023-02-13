---
content-type: tips-tricks-troubleshooting
product-area: documents
keywords: disable, pubblico, condivisione, prova, pubblico, url
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Disattiva la prova di condivisione tramite URL pubblico o codice di incorporamento
description: Puoi disattivare la possibilità di condividere una bozza con un URL pubblico o con un codice di incorporamento su una bozza in base a prove o per singoli utenti.
author: Courtney
feature: Digital Content and Documents
exl-id: 73f08e12-f70d-4347-8a5b-441f94d24590
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Disattiva la prova di condivisione tramite URL pubblico o codice di incorporamento

Puoi disattivare la possibilità di condividere una bozza con un URL pubblico o con un codice di incorporamento su una bozza in base a prove o per singoli utenti.

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
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il ruolo o il profilo delle autorizzazioni di prova, contattare l&#39;amministratore Workfront o Workfront Proof.

## Disattiva per prova

Devi essere il proprietario o il creatore della bozza, oppure devi disporre del ruolo di bozza Autore o Moderatore .

1. Nel progetto che contiene la bozza, fai clic su **Documenti** nel pannello a sinistra.
1. Passa il puntatore del mouse sulla bozza e seleziona **Dettagli documento** .
1. Nel pannello a sinistra, fai clic su **Impostazioni del visualizzatore di correzione**, quindi disattiva il **Consenti condivisione di prove tramite URL pubblico o codice di incorporamento** casella di controllo.

   ![](assets/proofing-viewer-settings-350x200.png)

1. Fai clic su **Salva**.

## Disattiva per utente

Puoi disattivare l’impostazione Prova pubblica per i singoli utenti nell’istanza di Workfront. Per apportare questa modifica, è necessario disporre di un profilo di autorizzazione di prova dell’amministratore.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Copertura**.
1. Fai clic su **Impostazioni account** nell&#39;angolo in alto a destra.
1. Fai clic sul pulsante **Utenti** , quindi fai clic sul nome di un utente.
1. In **Impostazioni predefinite della bozza** disattivare la sezione **Condivisione pubblica** casella di controllo.

   ![](assets/default-proof-settings--public-sharing-350x210.png)
