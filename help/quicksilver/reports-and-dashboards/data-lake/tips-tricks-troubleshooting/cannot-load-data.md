---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: 'Tableau Desktop: impossibile stabilire una connessione'
description: Quando si tenta di collegare Tableau Desktop a Data Connect, viene visualizzato un errore.
author: Courtney
feature: Reports and Dashboards
source-git-commit: e8b1d553ac4761e2b6eae79ae384956105939d90
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Tableau Desktop: impossibile stabilire una connessione

## Problema

Quando tenti di collegare Tableau Desktop a Data Connect, viene visualizzato il seguente errore:

`Cannot load data into PowerBI. Receiving an HY000 [Microsoft][Snowflake] (25) message`

## Causa

Questo errore è causato da un&#39;impostazione proxy nel computer locale che impedisce il caricamento dei dati da Data Connect.

Data Connect viene fornito tramite i servizi cloud di Snowflake di terze parti. Tableau richiede una rete aperta per comunicare con Snowflake.

## Soluzione

Per risolvere il problema, procedere come segue:

* **Risolvere i problemi disabilitando lo strumento di sicurezza**: disattivare lo strumento di sicurezza, ad esempio Zscaler o Cisco, per verificare se risolve il problema di connettività. Se il problema di connessione viene risolto, verificare che lo strumento di sicurezza sia aggiornato alla versione più recente, aggiungere l&#39;indirizzo IP di Data Connect (Snowflake) al elenco Consentiti di VPN con il team della rete interna.

* **Aggiungi indirizzi IP al Inserisco nell&#39;elenco Consentiti di**: assicurati che le impostazioni del firewall consentano gli indirizzi IP utilizzati da Data Connect. Utilizzare il comando `SYSTEM$ALLOWLIST()` per ottenere l&#39;indirizzo IP, che può quindi essere inserito nell&#39;elenco Consentiti nella VPN.

* **Verifica impostazioni firewall e proxy**: verifica se alcune configurazioni firewall o proxy nella rete stanno bloccando l&#39;accesso agli endpoint di Snowflake. Potrebbe essere necessario contattare l&#39;amministratore di rete per aggiungere gli indirizzi IP e le porte Snowflake richiesti al inserisco nell&#39;elenco Consentiti di gestione dei sistemi della società.

* **Soluzione alternativa**: creare un&#39;estrazione da una schermata del foglio di lavoro anziché dal riquadro Source dati in Tableau. La connessione non viene persa e il processo di estrazione viene completato.

