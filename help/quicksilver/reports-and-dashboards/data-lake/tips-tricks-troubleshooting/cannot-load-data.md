---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Tableau Desktop non può stabilire una connessione
description: Quando si tenta di collegare Tableau Desktop a Data Connect, viene visualizzato un errore.
author: Courtney
feature: Reports and Dashboards
exl-id: 2a25d99a-a05e-4f60-ae1a-51ee137ad5f3
TQID: https://experienceleague.adobe.com/-V1TT-X0FjMm2PIKDy0JVFkvt-A-a7f8fRbVzGzy1jg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 253
ht-degree: 5%

---

# Tableau Desktop non può stabilire una connessione

## Problema

Quando tenti di collegare Tableau Desktop a Data Connect, viene visualizzato il seguente errore:

`Cannot load data into PowerBI. Receiving an HY000 [Microsoft][Snowflake] (25) message`

## Causa

Questo errore è causato da un&#39;impostazione proxy nel computer locale che impedisce il caricamento dei dati da Data Connect.

Data Connect viene fornito tramite i servizi cloud di Snowflake di terze parti. Tableau richiede una rete aperta per comunicare con Snowflake.

## Soluzione

Per risolvere il problema, procedere come segue:

* **Risolvere i problemi disabilitando lo strumento di sicurezza**: disattivare lo strumento di sicurezza, ad esempio Zscaler o Cisco, per verificare se risolve il problema di connettività. Se il problema di connessione viene risolto, verificare che lo strumento di sicurezza sia aggiornato alla versione più recente, aggiungere l&#39;indirizzo IP di Data Connect (Snowflake) all&#39;elenco Consentiti di VPN con il team della rete interna.

* **Aggiungi indirizzi IP al Inserisco nell&#39;elenco Consentiti di**: verifica che le impostazioni del firewall consentano gli indirizzi IP utilizzati da Data Connect. Utilizzare il comando `SYSTEM$ALLOWLIST()` per ottenere l&#39;indirizzo IP, che è quindi possibile inserire nell&#39;elenco Consentiti nella VPN. L&#39;indirizzo IP può essere utilizzato solo per i collegamenti di rete.

* **Verifica impostazioni firewall e proxy**: verifica se alcune configurazioni firewall o proxy nella rete stanno bloccando l&#39;accesso agli endpoint di Snowflake. Potrebbe essere necessario contattare l&#39;amministratore di rete per aggiungere gli indirizzi IP e le porte Snowflake richiesti all&#39;elenco Consentiti della società.

* **Soluzione alternativa**: creare un&#39;estrazione da una schermata del foglio di lavoro anziché dal riquadro Source dati in Tableau. La connessione non viene persa e il processo di estrazione viene completato.
