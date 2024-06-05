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

Per collegare i dati del data lake di Workfront a un prodotto esterno, devi prima aggiungere tutti gli IP richiesti al inserisco nell&#39;elenco Consentiti come descritto in [Aggiungere IP al inserisco nell&#39;elenco Consentiti di](#add-ips-to-the-allowlist) di seguito. Inoltre, la maggior parte dei prodotti richiede informazioni aggiuntive sul data lake per stabilire una connessione:

| Nome campo | Valore |
|---------------|-------------|
| Server | L&#39;URL per la connessione, senza `https://` porzione (trovata sul **Accesso ai dati** in Workfront*) |
| Porta | `443` |
| Database | `WORKFRONT` |
| Data warehouse | `READER_WH` |
| Schema | `WF` |
| Ruolo | `READER_ROLE` |
| Nome utente | Il nome utente scelto durante la creazione della connessione (disponibile nella **Accesso ai dati** in Workfront*) |
| Password | La password scelta al primo accesso al Snowflake* |

*Per informazioni su dove trovare **Accesso ai dati** pagina contenente le connessioni al data lake, consulta [Creazione di un account di lettura (servizio) per il Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Una volta aggiunta una voce al inserisco nell&#39;elenco Consentiti di, tutti gli altri indirizzi IP non sono più consentiti. Prima di utilizzare lo strumento, assicurati di aver inserito tutti gli indirizzi IP richiesti, sia per la creazione che per la lettura dello strumento di visualizzazione. In caso contrario, potrebbe verificarsi un errore relativo alle credenziali non valide.
>
>Se nel elenco Consentiti non è incluso alcun indirizzo IP ma si verificano ancora problemi di connessione a uno strumento BI, controllare la configurazione del server proxy per lo strumento BI.


## Aggiungere IP al inserisco nell&#39;elenco Consentiti di

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **Configurazione**.

1. Nel pannello a sinistra, fai clic su **Sistema** > **Accesso ai dati**.

1. Fai clic sul pulsante **IP consentiti** , quindi fare clic sul pulsante **Aggiungere un indirizzo IP al Inserisco nell&#39;elenco Consentiti di** pulsante.

1. Immetti un nome per l’indirizzo IP in **Descrizione indirizzo IP** e immetti l’indirizzo IP (o blocco CIDR) dello strumento che desideri utilizzare in **Indirizzo IP**, quindi fai clic su **Aggiungi IP al Inserisco nell&#39;elenco Consentiti di**.

   ![Aggiungi indirizzo IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Rimozione di un indirizzo IP dal inserisco nell&#39;elenco Consentiti di

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **Configurazione**.

1. Nel pannello a sinistra, fai clic su **Sistema** > **Accesso ai dati**.

1. Fai clic sul pulsante **IP consentiti** , quindi fai clic sull’icona del cestino ![Icona Elimina](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) a destra dell’indirizzo IP che desideri rimuovere.

1. Nella finestra visualizzata, seleziona la casella per confermare e quindi fai clic su **Elimina**.

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
