---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Stabilire una connessione a Workfront Data Connect
description: Workfront Data Connect consente di utilizzare i dati Workfront dell'organizzazione con strumenti di business intelligence o di archiviarli in un data warehouse esterno.
author: Courtney
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 10%

---

# Stabilire una connessione a Workfront Data Connect

Workfront Data Connect consente di utilizzare i dati Workfront dell&#39;organizzazione con strumenti di business intelligence o di archiviarli in un data warehouse esterno.

Per collegare il data lake Data Connect a un prodotto esterno, è necessario innanzitutto creare una connessione come descritto in [Creare un account o una connessione di lettura per Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md). È quindi necessario aggiungere tutti gli IP necessari all&#39;elenco Consentiti come descritto in [Aggiungere gli IP all&#39;elenco Consentiti](#add-ips-to-the-allowlist).

Per stabilire una connessione, la maggior parte dei prodotti richiede le seguenti informazioni sul data lake:

| Nome campo | Valore |
|---------------|-------------|
| Server | URL della connessione, senza la parte `https://` (disponibile nella pagina **Connessione dati** in Workfront*) |
| Porta | `443` |
| Database | `WORKFRONT` |
| Data warehouse | `READER_WH` |
| Schema | `WF` |
| Ruolo | `READER_ROLE` |
| Nome utente | Il nome utente scelto durante la creazione della connessione (disponibile nella pagina **Connessione dati** in Workfront*) |
| Password | La password scelta al primo accesso al Snowflake* |

*Per informazioni su dove trovare la pagina **Connessione dati** contenente le connessioni, vedere [Creazione di un account o di una connessione di lettura per il Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Una volta aggiunta una voce all’elenco degli indirizzi IP consentiti, tutti gli altri indirizzi IP non saranno più consentiti. Prima di utilizzare lo strumento di visualizzazione, assicuratevi di aver inserito tutti gli indirizzi IP necessari, sia per l’esperienza di creazione che per quella di lettura. In caso contrario, potrebbe verificarsi un errore relativo alle credenziali non valide.
>
>Se nell&#39;elenco Consentiti non sono inclusi indirizzi IP ma si verificano ancora problemi di connessione a uno strumento BI, controlla la configurazione del server proxy per lo strumento BI.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Ultimate</p>
    <p>Flusso di lavoro Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungere IP al inserisco nell&#39;elenco Consentiti di

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **Setup**.

1. Nel pannello a sinistra, fai clic su **Sistema** > **Connessione dati**.

1. Fare clic sulla scheda **IP consentiti**, quindi sul pulsante **Aggiungi un indirizzo IP all&#39;elenco indirizzi consentiti**.

1. Immettere un nome per l&#39;indirizzo IP in **Descrizione indirizzo IP** e immettere l&#39;indirizzo IP (o blocco CIDR) per lo strumento che si desidera utilizzare in **Indirizzo IP**, quindi fare clic su **Aggiungi IP all&#39;elenco Consentiti**.

   ![Aggiungi indirizzo IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Rimuovere un indirizzo IP dall&#39;elenco degli indirizzi consentiti

1. Fate clic sull&#39;icona **[!UICONTROL Menu principale]** ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fate clic sull&#39;icona **[!UICONTROL Menu principale]** ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fate clic su **Configurazione**.

1. Nel pannello a sinistra, fai clic su **Sistema** > **Connessione dati**.

1. Fai clic sulla scheda **IP consentiti**, quindi fai clic sull&#39;icona del cestino ![Icona Elimina](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) a destra dell&#39;indirizzo IP che desideri rimuovere.

1. Nella finestra visualizzata, selezionare la casella per confermare e quindi fare clic su **Elimina**.

## Condividere i dati con gli strumenti di Business Intelligence

Di seguito sono elencati alcuni strumenti comuni di business intelligence. Per ulteriori informazioni sulla connessione al data lake, visita i relativi siti di documentazione.

* Tableau
* Power BI
* Domo
* SAP HANA

## Archiviare i dati in un data warehouse esterno

Di seguito sono elencati diversi data warehouse comuni; visitare i relativi siti di documentazione per ulteriori informazioni sulla connessione al data lake.

* Databricks
* AWS Redshift
