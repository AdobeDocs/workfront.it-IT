---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Installare il visualizzatore di correzione desktop per la propria organizzazione
description: Desktop Proofing Viewer, progettato principalmente per la correzione dei contenuti interattivi, è un’applicazione che deve essere installata sul computer locale di ciascun utente. In qualità di amministratore di Adobe Workfront o amministratore di Workfront Proof, puoi eseguire questa installazione.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: c89b21c6-fe70-4f46-aebd-5b82a667db72
source-git-commit: 58f976d9f4245e528a4ddf23d39b92d9fa405311
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 0%

---

# Installare il visualizzatore di correzione desktop per la propria organizzazione

Desktop Proofing Viewer, progettato principalmente per la correzione dei contenuti interattivi, è un’applicazione che deve essere installata sul computer locale di ciascun utente. In qualità di amministratore di Adobe Workfront o amministratore di Workfront Proof, puoi eseguire questa installazione.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Piano attuale: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Premium o Select</p> <p>Per ulteriori informazioni sulla verifica dell’accesso con i diversi piani, consulta <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alle funzionalità di correzione in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano attuale: Lavoro o piano</p> <p>Piano legacy: Qualsiasi (è necessario che la correzione sia attivata per l’utente)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>È necessario che l’amministratore sia selezionato nel profilo delle autorizzazioni di prova. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configurare l’accesso per la correzione di un utente</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Requisiti di sistema

Il visualizzatore per correzione desktop è supportato nei seguenti sistemi operativi:

* Windows 7 e versioni successive, a 32 bit e a 64 bit
* Mac OS X 10.9 e versioni successive, 64 bit

## Prerequisiti

Per consentire agli utenti di utilizzare il visualizzatore di correzione desktop, è necessario

* Configura il sistema per avviare il visualizzatore di correzione desktop come visualizzazione predefinita per le bozze interattive prima dell’installazione.

## Configurare il visualizzatore di correzione desktop come predefinito per le bozze interattive

Dopo aver installato il visualizzatore di correzione desktop per la propria organizzazione, è possibile impostarlo come visualizzatore predefinito per le bozze interattive.

1. In Workfront, fai clic sul menu principale ![](assets/main-menu-icon.png), quindi fai clic su Proofing ![](assets/proofing-in-main-menu.png) per accedere a Workfront Proof.

1. Fai clic su **Impostazioni account** nell&#39;angolo in alto a destra di Workfront Proof, quindi fai clic sul pulsante **Impostazioni** scheda .

1. Sotto **Valori predefiniti di prova**, alla fine del **Visualizzatore di correzione desktop per correzione interattiva** riga, fai clic su **Configurazione**.

   ![](assets/proof-defaults-350x265.png)

1. Fai clic su **Abilitato e predefinito**, quindi fai clic su **Salva**.

## Installazione del visualizzatore di correzione del desktop per gli utenti

* [Installazione del visualizzatore di correzione desktop in Mac](#installing-the-desktop-proofing-viewer-on-mac)
* [Installazione del visualizzatore di correzione desktop in Windows](#installing-the-desktop-proofing-viewer-on-windows)

### Installazione del visualizzatore di correzione desktop in Mac {#installing-the-desktop-proofing-viewer-on-mac}

1. Sul computer dell’utente, effettua una delle seguenti operazioni per scaricare l’app:

   * Se utilizzi l’ambiente Produzione, fai clic su  [Download di produzione Mac per visualizzatore di correzione desktop.](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof-2.1.19.pkg)
   * Se utilizzi l’ambiente Anteprima, fai clic su  [Mac Preview Download per il visualizzatore di correzione desktop.](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview-2.1.19.pkg)
)

1. Apri il file appena scaricato per avviare l&#39;installazione.
1. Nella casella di installazione visualizzata, fai clic su **Continua**, quindi fai clic su **Installa**.

   ![00000776.png](assets/00000776-350x244.png)

1. Assicurati che ogni utente completi l&#39;installazione aprendo una bozza interattiva dall&#39;area Documenti di Workfront.

### Installazione del visualizzatore di correzione desktop in Windows {#installing-the-desktop-proofing-viewer-on-windows}

1. Sul computer dell’utente, effettua una delle seguenti operazioni per scaricare l’app:

   * Nell’ambiente di produzione, fai clic su [Download di Windows Production per il visualizzatore di correzione desktop.](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Setup+2.1.19.exe)
   * Nell’ambiente Anteprima, fai clic su [Download di anteprima di Windows per il visualizzatore di correzione desktop](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview+Setup+2.1.19.exe).

1. Apri il file appena scaricato per avviare l&#39;installazione.
1. Nella finestra di avviso di protezione visualizzata, fare clic su **Esegui**.

   ![Screen_Shot_2018-05-02_at_10.56.55_AM.png](assets/screen-shot-2018-05-02-at-10.56.55-am-350x271.png)

   Viene installato ed eseguito il Visualizzatore di correzione desktop.

1. (Condizionale) Se installi l&#39;applicazione utilizzando Internet Explorer, aggiorna la pagina di avvio nel browser dopo l&#39;installazione dell&#39;applicazione.
1. Assicurati che ogni utente completi l&#39;installazione aprendo una bozza interattiva dall&#39;area Documenti di Workfront.
