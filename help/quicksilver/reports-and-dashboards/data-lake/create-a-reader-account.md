---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Creazione di un account di lettura (servizio) per il Snowflake
description: Per accedere ai dati di Data Connect, è necessario innanzitutto creare un account lettore di Snowflake.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: 16809b2d1801dd7aa4ab1f452e4687601fc1ac59
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Creazione di un account di lettura (servizio) per il Snowflake

Per accedere ai dati di Data Connect, è necessario innanzitutto creare un account lettore di Snowflake (o servizio) per ogni nuova connessione. Dopo aver creato una connessione, puoi trovare l&#39;URL e il nome utente associati facendo clic su di esso nella pagina **Accesso ai dati** (**Menu principale** > **Configurazione** > **Sistema** > **Accesso ai dati**) nella scheda **Connessioni esistenti**.

Per informazioni sull&#39;utilizzo di una connessione appena creata con un prodotto esterno, vedere [Stabilire una connessione a Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

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

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **Setup**.

1. Nel pannello a sinistra, fai clic su **Sistema** > **Accesso ai dati**.

1. Fai clic su **Crea nuova connessione**

1. Nella finestra visualizzata, immetti un nome per la connessione in **Descrizione riferimento connessione** e un nome utente in **Utente connessione**, quindi fai clic su **Genera connessione**.

   ![Crea account lettore](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. Verrà generata una **password predefinita** e un URL per la visualizzazione dei dati tramite il Snowflake. Dovrai utilizzare la password insieme al nome utente scelto per accedere al Snowflake per la prima volta, quindi assicurati di tenerne traccia insieme all’URL. Selezionare la casella in cui si dichiara di averlo fatto, quindi fare clic su **Chiudi**.

   ![Password account predefinita](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Apri il Snowflake utilizzando un browser per passare all&#39;URL del passaggio precedente, immetti il nome utente selezionato e la password predefinita del passaggio precedente, quindi fai clic su **Accedi**.

1. Dopo aver effettuato l&#39;accesso per la prima volta, verrà richiesto di scegliere una nuova password. Immetti una password a tua scelta nei campi **Nuova password** e **Conferma password**, quindi fai clic su **Invia**.

   ![Reimposta password Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Ora puoi utilizzare il tuo nome utente e la nuova password per accedere al data lake Data Connect in Snowflake o nello strumento di visualizzazione aziendale di tua scelta.

## Revoca di un account lettore

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **Setup**.

1. Nel pannello a sinistra, fai clic su **Sistema** > **Accesso ai dati**.

1. Fai clic sull&#39;icona del cestino ![icona Elimina](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) a destra dell&#39;account che desideri revocare.

1. Nella finestra visualizzata, selezionare la casella per confermare e quindi fare clic su **Elimina**.
