---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Creazione di un account di lettura (servizio) per il Snowflake
description: Per accedere ai dati nel Data Lake di Workfront, devi innanzitutto creare un account di lettura per il Snowflake.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: e5bd25315062ad15ccd3448e008dfe94f1b616da
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Creazione di un account di lettura (servizio) per il Snowflake

Per accedere ai dati del data lake di Workfront, devi prima creare un account di lettura del Snowflake (o servizio) per ogni nuova connessione. Dopo aver creato una connessione, puoi trovarne l’URL e il nome utente associati facendo clic su di esso nella **Accesso ai dati** page (**Menu principale** > **Configurazione** > **Sistema** > **Accesso ai dati**) sotto **Connessioni esistenti** scheda.

Per informazioni sull’utilizzo di una connessione appena creata con un prodotto esterno, consulta [Stabilire una connessione al data lake di Workfront](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Da definire</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Creare un account di lettura

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **Configurazione**.

1. Nel pannello a sinistra, fai clic su **Sistema** > **Accesso ai dati**.

1. Clic **Crea nuova connessione**

1. Nella finestra visualizzata, inserisci un nome per la connessione in **Descrizione del riferimento di connessione** e un nome utente in **Utente di connessione**, quindi fai clic su **Genera connessione**.

   ![Crea account lettore](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. A **Password predefinita** e un URL in cui i dati possono essere visualizzati tramite il Snowflake. Dovrai utilizzare la password insieme al nome utente scelto per accedere al Snowflake per la prima volta, quindi assicurati di tenerne traccia insieme all’URL. Seleziona la casella in cui dichiara di aver effettuato questa operazione, quindi fai clic su **Chiudi**.

   ![Password account predefinita](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Apri il Snowflake utilizzando un browser per passare all’URL dal passaggio precedente, immetti il nome utente selezionato e la password predefinita del passaggio precedente, quindi fai clic su **Accedi**.

1. Dopo aver effettuato l&#39;accesso per la prima volta, verrà richiesto di scegliere una nuova password. Immettere una password di propria scelta in entrambi i **Nuova password** e **Conferma password** , quindi fai clic su **Invia**.

   ![Reimposta password Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Ora puoi utilizzare il tuo nome utente e la nuova password per accedere al tuo data lake Workfront in Snowflake o nello strumento di visualizzazione aziendale di tua scelta.

## Revoca di un account lettore

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **Configurazione**.

1. Nel pannello a sinistra, fai clic su **Sistema** > **Accesso ai dati**.

1. Fai clic sull’icona del cestino ![Icona Elimina](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) a destra dell’account che desideri revocare.

1. Nella finestra visualizzata, seleziona la casella per confermare e quindi fai clic su **Elimina**.
