---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-2-0
title: Metadati di connessione in Adobe Workfront Fusion
description: Adobe Workfront Fusion richiede una licenza Adobe Workfront Fusion oltre a una licenza Adobe Workfront.
author: Becky
feature: Workfront Fusion
source-git-commit: 3a7983279a38c30cb58078d129ea22dee137d9a5
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Metadati di connessione in Adobe Workfront Fusion

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] richiede un [!DNL Adobe Workfront Fusion] licenza oltre a un [!DNL Adobe Workfront] licenza.

Non tutte le connessioni sono uguali. Comprendere le differenze tra le connessioni è molto importante per conoscere il contesto aziendale. Fusion utilizza i metadati per identificare gli attributi importanti di una connessione.

È possibile impostare i metadati della connessione durante la creazione di una nuova connessione. Questi attributi si trovano nella stessa finestra di dialogo utilizzata per impostare una connessione:

![Metadati di connessione](assets/connection-metadata-setup.png)

Gli utenti di Fusion possono visualizzare e modificare le connessioni dall&#39;area Connessioni.

![Metadati di connessione nell’area Connessioni](assets/connections-area-metadata.png)

## Tipo di ambiente

Le connessioni di fusione possono essere utilizzate sia da sistemi di produzione che da sistemi non di produzione. Conoscere la differenza è molto importante per proteggere gli ambienti di produzione. Tieni presente che il tipo di ambiente, come altri metadati di connessione, viene utilizzato solo a scopo informativo. Gli utenti sono ancora responsabili dell’impostazione accurata di questo attributo.

## Tipo di autenticazione

Le connessioni Fusion possono essere utilizzate sia per gli account di servizio che per gli account personali. Gli account di servizio vengono utilizzati per l’autenticazione quando uno scenario si automatizza come Fusion. Gli account personali sono autenticazioni basate su una persona specifica. Il tipo di autenticazione utilizzato dipende dai requisiti dello scenario. Gli account personali devono essere utilizzati per azioni utente automatizzate. Ad esempio, se uno scenario Fusion automatizza l’approvazione da parte di una persona specifica, il tipo di autenticazione deve essere per tale persona. In caso contrario, Fusion agisce come Fusion e il tipo deve essere &quot;Account di servizio&quot;.

Tieni presente che il tipo, come altri metadati di connessione, viene utilizzato solo a scopo informativo. Gli utenti sono ancora responsabili dell’impostazione manuale accurata di questo attributo.

Per ulteriori informazioni sui tipi di autenticazione, consulta [Autenticazione](https://developer.adobe.com/developer-console/docs/guides/authentication/) nella guida all’autenticazione di Adobe.



