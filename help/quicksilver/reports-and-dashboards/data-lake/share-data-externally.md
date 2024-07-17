---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data lake
title: Stabilire una connessione al data lake di Workfront
description: Workfront data lake consente di utilizzare i dati Workfront della tua organizzazione con i più diffusi strumenti di business intelligence o di memorizzarli in un data warehouse esterno.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 91371c862be6f3b99f0450ff359f601dc913dc0c
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 1%

---

# Stabilire una connessione al data lake di Workfront

Workfront data lake consente di utilizzare i dati Workfront della tua organizzazione con strumenti di business intelligence o archiviarli in un data warehouse esterno.

Per collegare i dati del data lake di Workfront a un prodotto esterno, è necessario innanzitutto aggiungere tutti gli IP necessari al inserisco nell&#39;elenco Consentiti come descritto in [Aggiungere gli IP al inserisco nell&#39;elenco Consentiti di](#add-ips-to-the-allowlist). Inoltre, la maggior parte dei prodotti richiede informazioni aggiuntive sul data lake per stabilire una connessione:

| Nome campo | Valore |
|---------------|-------------|
| Server | L&#39;URL per la connessione, senza la porzione `https://` (trovata nella pagina **Accesso ai dati** in Workfront*) |
| Porta | `443` |
| Database | `WORKFRONT` |
| Data warehouse | `READER_WH` |
| Schema | `WF` |
| Ruolo | `READER_ROLE` |
| Nome utente | Il nome utente scelto durante la creazione della connessione (trovato nella pagina **Accesso ai dati** in Workfront*) |
| Password | La password scelta al primo accesso al Snowflake* |

*Per informazioni su dove trovare la pagina **Accesso ai dati** contenente le connessioni al data lake, vedere [Creazione di un account lettore (di servizio) per il Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Una volta aggiunta una voce al inserisco nell&#39;elenco Consentiti di, tutti gli altri indirizzi IP non sono più consentiti. Prima di utilizzare lo strumento, assicurati di aver inserito tutti gli indirizzi IP richiesti, sia per la creazione che per la lettura dello strumento di visualizzazione. In caso contrario, potrebbe verificarsi un errore relativo alle credenziali non valide.
>
>Se nel elenco Consentiti non è incluso alcun indirizzo IP ma si verificano ancora problemi di connessione a uno strumento BI, controllare la configurazione del server proxy per lo strumento BI.


## Aggiungere IP al inserisco nell&#39;elenco Consentiti di

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **Setup**.

1. Nel pannello a sinistra, fai clic su **Sistema** > **Accesso ai dati**.

1. Fai clic sulla scheda **IP consentiti**, quindi fai clic sul pulsante **Aggiungi un indirizzo IP al tuo Inserisco nell&#39;elenco Consentiti di**.

1. Immettere un nome per l&#39;indirizzo IP in **Descrizione indirizzo IP** e immettere l&#39;indirizzo IP (o blocco CIDR) per lo strumento che si desidera utilizzare in **Indirizzo IP**, quindi fare clic su **Aggiungi IP da Inserire nell&#39;elenco Consentiti**.

   ![Aggiungi indirizzo IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Rimozione di un indirizzo IP dal inserisco nell&#39;elenco Consentiti di

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **Setup**.

1. Nel pannello a sinistra, fai clic su **Sistema** > **Accesso ai dati**.

1. Fai clic sulla scheda **IP consentiti**, quindi fai clic sull&#39;icona cestino ![icona Elimina](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) a destra dell&#39;indirizzo IP che desideri rimuovere.

1. Nella finestra visualizzata, selezionare la casella per confermare e quindi fare clic su **Elimina**.

## Condividere i dati con gli strumenti di Business Intelligence

Di seguito sono elencati alcuni strumenti di business intelligence comuni. I collegamenti ti porteranno al sito della documentazione del servizio per ulteriori informazioni sulla connessione al data lake.

* [Tableau](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [Power BI](https://learn.microsoft.com/power-query/connectors/snowflake)
* [Domo](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## Archiviare dati in un data warehouse esterno

Di seguito sono elencati alcuni data warehouse comuni; i collegamenti ti porteranno al sito della documentazione di ciascun servizio, dove puoi saperne di più sulla connessione al tuo data lake.

* [Database](https://docs.databricks.com/en/connect/index.html)
* [AWS Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
