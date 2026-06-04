---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Stabilire una connessione a Workfront Data Connect
description: Workfront Data Connect consente di utilizzare i dati Workfront della propria organizzazione con strumenti di business intelligence o di memorizzarli in un data warehouse esterno.
author: Courtney
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/pPk3qt9-o3QhAajyI4eGhwe0J2tRphXDstrJxmdW8Ww
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 1489
ht-degree: 4%

---

# Stabilire una connessione a Workfront Data Connect

Workfront Data Connect consente di utilizzare i dati Workfront della propria organizzazione con strumenti di business intelligence o di memorizzarli in un data warehouse esterno.

Per collegare il data lake Data Connect a un prodotto esterno, è necessario innanzitutto creare una connessione come descritto in [Creare un account o una connessione di lettura per Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md). Quindi, devi aggiungere tutti gli IP richiesti al inserisco nell&#39;elenco Consentiti di come descritto in [Aggiungere gli IP al inserisco nell&#39;elenco Consentiti di](#add-ips-to-the-allowlist) di seguito.

La maggior parte dei prodotti richiede le seguenti informazioni sul data lake per stabilire una connessione:

| Nome campo | Valore |
|---------------|-------------|
| Server | L&#39;URL per la connessione, senza la porzione `https://` (trovata nella pagina **Connessione dati** in Workfront*) |
| Porta | `443` |
| Database | `WORKFRONT` |
| Data warehouse | `READER_WH` |
| Schema | `WF` |
| Ruolo | `READER_ROLE` |
| Nome utente | Il nome utente scelto durante la creazione della connessione (trovato nella pagina **Connessione dati** in Workfront*) |
| Password | La password scelta al primo accesso a Snowflake* |

*Per informazioni su dove trovare la pagina **Connessione dati** contenente le connessioni, vedere [Creare un account o una connessione di lettura per Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Una volta aggiunta una voce all’elenco Consentiti di IP, tutti gli altri indirizzi IP non sono più consentiti. Prima di utilizzare lo strumento, assicurati di aver inserito tutti gli indirizzi IP richiesti, sia per la creazione che per la lettura dello strumento di visualizzazione. In caso contrario, potrebbe verificarsi un errore relativo alle credenziali non valide.
>
>Se non si dispone di indirizzi IP inclusi nel inserisco nell&#39;elenco Consentiti di accesso a un server di business intelligence, ma si verificano ancora problemi durante la connessione a uno strumento di business intelligence, controllare la configurazione del server proxy per lo strumento di business intelligence.

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
   <td> <p>Devi essere un amministratore di Workfront</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungere IP al inserisco nell&#39;elenco Consentiti di

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **Setup**.

1. Nel pannello a sinistra, fai clic su **Sistema** > **Connessione dati**.

1. Fai clic sulla scheda **IP consentiti**, quindi fai clic sul pulsante **Aggiungi un indirizzo IP alla tua Inserisce nell&#39;elenco Consentiti di**.

1. Immettere un nome per l&#39;indirizzo IP in **Descrizione indirizzo IP** e immettere l&#39;indirizzo IP (o blocco CIDR) per lo strumento che si desidera utilizzare in **Indirizzo IP**, quindi fare clic su **Aggiungi IP all&#39;Elenco Consentiti**.

   ![Aggiungi indirizzo IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Trova intervalli IP di Azure per Microsoft Power BI

Il traffico Microsoft Power BI verso Data Connect non proviene da un singolo indirizzo fisso. Microsoft pubblica gli intervalli IP come blocchi CIDR in un file JSON di grandi dimensioni. Questa sezione spiega come trovare i blocchi per le aree effettivamente utilizzate.

### Fonte ufficiale Microsoft per gli intervalli IP e i codici di matricola di Azure

Microsoft pubblica l&#39;elenco nella [pagina di download degli intervalli IP e dei codici di matricola di Azure &#x200B;](https://www.microsoft.com/en-us/download/details.aspx?id=56519). Scaricare il file JSON corrente (il nome file è in genere simile a `ServiceTags_Public_YYYYMMDD.json`). Aggiorna il inserisco nell&#39;elenco Consentiti di aggiornamento del file di Microsoft quando questo viene aggiornato o quando si verificano problemi di connettività dopo una modifica di Microsoft.

>[!NOTE]
>
>Il file JSON è molto grande, spesso oltre le 100.000 righe. Questo è previsto. Le sezioni necessarie sono piccole; non è necessario leggere l&#39;intero file a mano.

### Confronto tra Power BI e Power Query Online

Talvolta i clienti segnalano &quot;Power BI&quot; quando il traffico proviene effettivamente da componenti Power Query che Microsoft considera come un servizio Azure separato nell’elenco dei codici di matricola.

| Se gli utenti... | Cerca questo codice di matricola nel codice JSON |
|----------------|---------------------------------------|
| Utilizza il servizio Power BI, i set di dati in hosting in Azure o i gateway nel contesto cloud | `PowerBI` (voci globali o regionali come `PowerBI.EastUS`) |
| Utilizzare Power Query Online, flussi di dati cloud ed esperienze simili | `PowerQueryOnline` (voci globali o regionali come `PowerQueryOnline.EastUS`) |

Se l&#39;organizzazione utilizza entrambe le esperienze, aggiungere blocchi CIDR di `PowerBI` e `PowerQueryOnline` per le stesse aree geografiche. Se ne aggiungi solo uno, alcuni utenti potrebbero essere ancora bloccati mentre altri riescono a farlo.

### Scegli i tag regionali, non l’aggregato globale

Il file JSON contiene una singola voce per tutte le aree per `PowerBI` (e in modo simile per `PowerQueryOnline`) che aggrega molte aree e può contenere centinaia di blocchi CIDR, oltre a molte voci per aree geografiche più piccole come `PowerBI.WestUS`, `PowerBI.WestUS2` e `PowerBI.WestUS3`. Ogni oggetto regionale elenca solo i prefissi per quell&#39;area, in genere decine di righe al massimo. È consigliabile non aggiungere la voce globale, a meno che non si disponga di un requisito documentato per consentire ogni area geografica di Azure. Per la maggior parte dei clienti di Data Connect, le voci internazionali sono l’impostazione predefinita corretta. Aggiungere le aree in cui vengono eseguiti i tenant e gli utenti di Power BI, oltre a un piccolo buffer per la ridondanza (ad esempio, un&#39;area di disaster recovery secondaria utilizzata dalla società).

### Scegli le aree geografiche

I nomi delle aree geografiche di Microsoft nel file sono simili a `EastUS`, `WestEurope`, `GermanyWestCentral` e così via. Utilizza le aree in cui sono ospitati la capacità e gli utenti di Power BI, non dove si trova il tuo ufficio, anche se spesso sono allineati.

| Scenario | Cosa aggiungere per primo |
|----------|-------------------|
| Utilizzo negli Stati Uniti | Inizia con le aree degli Stati Uniti utilizzate dal tenant (esempi: `EastUS`, `EastUS2`, `WestUS`, `WestUS2`, `WestUS3`, `CentralUS`, `SouthCentralUS`). Non è necessaria alcuna regione degli Stati Uniti a meno che l’amministratore di Microsoft non confermi l’hosting per più regioni. |
| Utilizzo nell’Unione europea o nel Regno Unito | Inizia con le aree utilizzate dal tenant (esempi: `WestEurope`, `NorthEurope`, `FranceCentral`, `GermanyWestCentral`, `SwedenCentral`, `UKSouth`). Aggiungi altro solo se gli utenti si estendono su altre aree geografiche di Microsoft. |
| Utilizzo per l’Asia Pacifico | Aggiungi le aree geografiche confermate dall&#39;amministratore Power BI o Azure (ad esempio: `SoutheastAsia`, `EastAsia`, `AustraliaEast`). |
| Più aree geografiche | Aggiungere entrambi i set di tag regionali (ad esempio, UE e USA) per ciascun servizio (`PowerBI` e `PowerQueryOnline` se entrambi sono in uso). |
| Area geografica sconosciuta | Chiedi all’amministratore di Microsoft 365 o Power BI quali aree geografiche di Azure ospitano le risorse Power BI, oppure controlla le impostazioni del tenant dell’amministratore di Power BI. Se è necessario sbloccare rapidamente per il test, aggiungere una coppia di aree note (ad esempio, `EastUS` e `WestUS`) e monitorare, quindi restringere l&#39;elenco dopo la conferma. |

### Trova intervalli IP e aggiungili al inserisco nell&#39;elenco Consentiti di

Per raccogliere gli intervalli IP da Microsoft e aggiungerli all’elenco Consentiti di Workfront:

1. Apri la [pagina di download degli intervalli IP e dei tag di servizio di Azure - Cloud pubblico](https://www.microsoft.com/en-us/download/details.aspx?id=56519), scarica il file JSON dei tag di servizio e salvalo localmente (ad esempio, `Downloads\ServiceTags_Public_YYYYMMDD.json`).

1. Apri il file in qualsiasi editor che gestisca bene il codice JSON di grandi dimensioni, ad esempio Visual Studio Code.

1. Utilizzare la funzionalità Trova dell&#39;editor (`Ctrl+F` in Windows o `Cmd+F` in macOS) per individuare oggetti JSON il cui campo `"name"` è uguale a un codice di matricola come `PowerBI.EastUS` o `PowerQueryOnline.WestEurope`. Ricerche utili:

   * `"name": "PowerBI.WestUS"` - Passa alla Power BI degli Stati Uniti occidentali.
   * `"name": "PowerQueryOnline.WestUS"` - Passare a West US Power Query Online.
   * `PowerBI.` — elenca tutti i tag regionali di Power BI, quindi perfeziona in base al nome della tua area geografica.

1. In ogni oggetto corrispondente, trovare l&#39;array denominato `addressPrefixes`. Ogni stringa nell&#39;array è un blocco CIDR (ad esempio, `20.59.79.96/27` o un prefisso IPv6). Questi sono i valori che aggiungerai al tuo Workfront di inserire nell&#39;elenco Consentiti.

1. Aggiungere ogni CIDR al Workfront di inserire nell&#39;elenco Consentiti come descritto in [Aggiungere IP al inserisco nell&#39;elenco Consentiti di](#add-ips-to-the-allowlist) in questo articolo. Se l’ambiente memorizza nella cache le regole, attendere alcuni minuti per la propagazione dei criteri.

1. Da Power BI o Power Query Online eseguire una piccola query di prova su Data Connect per convalidare la connessione. In caso di errore, acquisisci l’ora approssimativa e chiedi al team di rete se nega l’allineamento con gli intervalli mancanti. Controlla di nuovo se hai saltato `PowerQueryOnline` quando è stato aggiunto solo `PowerBI`, il che è un gap comune.

Se, ad esempio, l&#39;amministratore di Microsoft conferma che i carichi di lavoro di Power BI utilizzano Stati Uniti occidentali, Stati Uniti occidentali 2 e Stati Uniti occidentali 3 e che gli utenti utilizzano sia Power BI che Power Query Online, verranno aperti sei oggetti: `PowerBI.WestUS`, `PowerBI.WestUS2`, `PowerBI.WestUS3` e `PowerQueryOnline.<Region>` corrispondenti per ciascuno, quindi verrà eseguita la copia di `addressPrefixes` da tutti e sei.

### Riferimento struttura JSON

Ogni blocco di codice di matricola ha un aspetto concettualmente simile al seguente. I file reali includono più metadati.

```json
{
  "name": "PowerBI.WestUS2",
  "id": "PowerBI.WestUS2",
  "properties": {
    "region": "westus2",
    "systemService": "PowerBI",
    "addressPrefixes": [
      "203.0.113.0/24",
      "2001:db8::/32"
    ],
    "networkFeatures": ["API", "NSG", "UDR", "FW"]
  }
}
```

L&#39;array `addressPrefixes` contiene i blocchi CIDR che verranno aggiunti a Workfront. Altri campi sono per scenari di rete Azure e non sono applicabili qui.

### Mantieni il inserisco nell&#39;elenco Consentiti di

* Microsoft cambia gli intervalli IP nel tempo. Quando Microsoft pubblica un file JSON aggiornato, aggiorna o confronta periodicamente il tuo inserire nell&#39;elenco Consentiti, specialmente dopo un problema di connettività.
* Se l&#39;ambiente in uso supporta IPv6 in Snowflake e Microsoft elenca i prefissi IPv6, includerli se i criteri di protezione consentono IPv6. In caso contrario, assicurati di coordinarti con il tuo team di rete.

## Rimuovere un indirizzo IP dal inserisco nell&#39;elenco Consentiti di

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **Setup**.

1. Nel pannello a sinistra, fai clic su **Sistema** > **Connessione dati**.

1. Fai clic sulla scheda **IP consentiti**, quindi fai clic sull&#39;icona cestino ![icona Elimina](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) a destra dell&#39;indirizzo IP che desideri rimuovere.

1. Nella finestra visualizzata, selezionare la casella per confermare e quindi fare clic su **Elimina**.

## Condividere i dati con gli strumenti di Business Intelligence

Di seguito sono elencati alcuni strumenti comuni di business intelligence. Per ulteriori informazioni sulla connessione al data lake, visita i relativi siti di documentazione.

* Tableau
* Power BI
* Domo
* SAP HANA

## Archiviare dati in un data warehouse esterno

Di seguito sono elencati alcuni data warehouse comuni; visita i relativi siti di documentazione per ulteriori informazioni sulla connessione al data lake.

* Databricks
* AWS Redshift
