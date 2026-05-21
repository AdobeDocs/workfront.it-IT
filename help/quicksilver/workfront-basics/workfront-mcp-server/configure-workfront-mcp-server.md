---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Configurare il server MCP di Adobe Workfront
description: Configura l’istanza di Workfront e la piattaforma di intelligenza artificiale in modo da poter lavorare con Workfront attraverso una conversazione in linguaggio naturale.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 98d5b93bcb99c468de2ad107a2aca3a9a1995429
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 0%

---


# Configurare il server MCP di Adobe Workfront

Il server MCP [!DNL Adobe Workfront] ti consente di utilizzare i dati di Workfront tramite conversazioni in linguaggio naturale in una piattaforma di intelligenza artificiale supportata come Claude o ChatGPT.

Prima di poter collegare una piattaforma di agenti di intelligenza artificiale a Workfront, un amministratore Workfront deve abilitare l’accesso al server MCP nell’istanza di Workfront. I passaggi esatti per connettere una piattaforma AI agente sono diversi per ogni piattaforma AI agente supportata.

Per ulteriori informazioni sul server Workfront MCP, vedere [Panoramica del server Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Piattaforme di IA agente supportate

Il server MCP di Workfront supporta attualmente le seguenti piattaforme AI:

* [!DNL Claude]
* [!DNL ChatGPT]

## Prerequisiti

Prima di poter collegare Workfront a una piattaforma di intelligenza artificiale, è necessario:

* Avere un account [!DNL Adobe Workfront] attivo con l&#39;autorizzazione per accedere ai dati che si desidera utilizzare.
* Avere accesso a una piattaforma agente di IA come [!DNL Claude].

### Prerequisiti per l’amministrazione

L&#39;accesso al server MCP è gestito da due amministratori distinti.

* **L&#39;amministratore di Workfront** controlla l&#39;accesso al server MCP per l&#39;istanza di Workfront. L&#39;accesso è abilitato per impostazione predefinita in Preferenze di sistema, pertanto non è richiesta alcuna azione a meno che l&#39;amministratore non abbia scelto di disabilitarlo. <!-- TODO: link to the System Preferences AI preferences article once the Enable MCP toggle is documented there. -->

* Se utilizzi una versione Enterprise di una piattaforma AI agente, l&#39;amministratore di tale piattaforma deve abilitare il connettore [!DNL Adobe Workfront] per la tua organizzazione.


## Connettere Workfront a Claude

La connessione a Workfront viene eseguita una volta per ogni account [!DNL Claude]. La connessione consente di eseguire l&#39;autenticazione a una specifica istanza di Workfront e si rimane connessi fino a quando non si sceglie di disconnettersi.

### Connettersi dalla directory dei connettori

+++ Espandere per visualizzare istruzioni dettagliate per la connessione di Workfront a [!DNL Claude].

Per connettere Workfront a [!DNL Claude]:

1. Apri [!DNL Claude].

1. Passare all&#39;area connettori.

   <!-- NEEDS DETAIL: Exact menu path (for example, "Click Settings, then click Connectors"). -->

1. Trovare **[!DNL Adobe Workfront]** nell&#39;elenco dei connettori.

   Se non lo vedi, vedi [Prerequisiti di amministratore](#admin-prerequisites) in questo articolo.

1. Fai clic su **Connetti**.

   <!-- NEEDS DETAIL: Confirm the exact button label. -->

1. Quando richiesto, accedi all’istanza di Workfront.

   <!-- NEEDS DETAIL: Describe the auth flow — does it open a new browser tab, an in-app window, prompt for a Workfront domain? -->

1. Al termine dell’autenticazione, sei connesso.

   <!-- NEEDS DETAIL: Add a screenshot of the connected state in Claude. -->

+++

### Connettersi con un URL

+++ Espandere per visualizzare istruzioni dettagliate per la connessione di Workfront a [!DNL Claude] con un URL.

Per connettere Workfront a [!DNL Claude] con un URL:

1. Accedi a [Claude](https://claude.ai) utilizzando le tue credenziali.
1. Nel menu a sinistra, seleziona l&#39;icona **Personalizza**.
1. Seleziona **Connettori**, quindi seleziona l&#39;icona **+** per aggiungere un connettore.
1. Seleziona il pulsante **Crea app**.
1. Assegnare al connettore un nome desiderato (ad esempio &quot;Workfront&quot;) e immettere l&#39;URL del server MCP desiderato: `https://mcp.workfront.adobe.com/mcp/v1/workfront`

1. Una volta creato il connettore, viene visualizzata una finestra di accesso. Esegui l’autenticazione utilizzando le credenziali di Adobe ID. Se appartieni a più istanze, assicurati di selezionare l’istanza Workfront desiderata.

+++

### Personalizzare il comportamento di Claude con le abilità

[!DNL Claude] supporta set di istruzioni creati dall&#39;utente denominati skill. È possibile utilizzare un&#39;abilità per personalizzare il comportamento di [!DNL Claude] con Workfront. È possibile, ad esempio, creare un&#39;abilità che indica a [!DNL Claude] di recuperare sempre dati aggiornati da Workfront anziché basarsi sui risultati precedenti.

Per ulteriori informazioni sulle [!DNL Claude] abilità, consulta la [documentazione per l&#39;utente Claude](https://code.claude.com/docs/en/skills) o chiedi aiuto a Claude per le abilità.

## Connetti a ChatGPT

1. Accedi a [ChatGPT](https://chatgpt.com) utilizzando le tue credenziali.
1. In basso a sinistra, seleziona **il tuo nome** → **Impostazioni**.
1. Seleziona **App**, quindi abilita **Modalità sviluppatore**.
1. Seleziona il pulsante **Crea app**.
1. Assegnare all&#39;app il nome desiderato (ad esempio &quot;Workfront&quot;) e immettere l&#39;URL del server MCP desiderato: `https://mcp.workfront.adobe.com/mcp/v1/workfront`
1. Verificare che l&#39;autenticazione sia impostata su **OAuth** (impostazione predefinita) e selezionare la casella di controllo Accettazione per continuare.
1. Una volta creata l’app, viene visualizzata una finestra di accesso. Esegui l’autenticazione utilizzando le credenziali di Adobe ID. Se appartieni a più istanze, assicurati di selezionare l’istanza Workfront desiderata.

### Personalizzare il comportamento di ChatGPT con GPT personalizzati

ChatGPT supporta gli assistenti creati dall’utente denominati GPT personalizzati. Puoi utilizzare un GPT personalizzato per personalizzare il comportamento di ChatGPT con il connettore. Ad esempio, puoi creare un GPT personalizzato che comunichi a ChatGPT di recuperare sempre dati aggiornati dal servizio connesso, invece di fare affidamento sui risultati precedenti.

Per ulteriori informazioni sugli GPT personalizzati, consulta la [documentazione utente di ChatGPT](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts) o chiedi a ChatGPT di fornire assistenza sugli GPT personalizzati.

## Verifica la connessione

Per verificare che la piattaforma di gestione dell’intelligenza artificiale sia connessa a Workfront, chiedi alla piattaforma di gestione dell’intelligenza artificiale di elencare le azioni che il server Workfront MCP rende disponibili. Ad esempio:

* *Quali azioni puoi intraprendere Workfront?*
* *Elenca gli strumenti di Workfront a cui hai accesso.*

È inoltre possibile visualizzare l&#39;elenco completo degli strumenti in [Strumenti server Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

## Strumenti disponibili

Il server MCP di Workfront espone un set di strumenti richiamati dalla piattaforma dell’agente di intelligenza artificiale connesso, ad esempio strumenti per cercare in Workfront, creare elementi, aggiornare campi e gestire le approvazioni. Per l&#39;elenco completo dei riferimenti, raggruppati per area Workfront, vedere [Strumenti server MCP di Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

## Passa a un’altra istanza di Workfront

Ogni connessione autentica la piattaforma dell’agente di intelligenza artificiale in una singola istanza di Workfront. Per utilizzare un&#39;istanza diversa, disconnettiti e riconnettiti.

Per connettersi a un&#39;altra istanza di Workfront:

1. Nella piattaforma dell’agente di intelligenza artificiale, disconnetti il server MCP di Workfront.
1. Ricollegare il connettore.
1. Esegui l’autenticazione alla nuova istanza di Workfront.

>[!NOTE]
>
>La disconnessione da sola non cambia l’istanza di Workfront. È necessario disconnettere e ricollegare il connettore.

<!--

## Connect to Gemini

>[!IMPORTANT]
>
>You must be an administrator on the Gemini platform to set up the MCP server. If you aren't an administrator, share these instructions with your administrator so they can set up the connection for you.


To set up the connection between Gemini and the Workfront MCP server, follow the instructions provided by Google for [connecting Gemini to external tools using MCP](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server). 

When prompted for the MCP Server URL, enter the following URL for your Workfront MCP server: `https://mcp.workfront.adobe.com/mcp/v1/workfront`
-->

<!--
## Connect to Microsoft Copilot

✅ 1) Copilot Studio (most common for agents / enterprise use)
This is the cleanest "paste a URL" flow.
Steps
1. Open your Copilot Studio agent
2. Go to Tools
3. Click:
    * Add a tool → New tool → Model Context Protocol
4. In the wizard, fill in:
    * Server name (anything)
    * Server description
    * ✅ Server URL (your MCP endpoint)
5. Choose auth (if needed):
    * None / API key / OAuth
6. Click Create
👉 That's it—your MCP server is now attached to the agent.
This flow is explicitly documented:
* You add MCP via Tools → Add tool → Model Context Protocol
* Then provide Server name, description, and URL ￼
￼
What happens next
* Copilot discovers tools automatically from the MCP server
* You can enable/disable tools per agent
* The agent calls them when relevant

-->

## Risoluzione dei problemi di configurazione e autenticazione

+++ Espandere per visualizzare suggerimenti per la risoluzione dei problemi relativi alla configurazione e all&#39;autenticazione del server Workfront MCP.

| Problema | Probabile causa | Correggi |
|---|---|---|
| Impossibile trovare il connettore [!DNL Adobe Workfront] in [!DNL Claude]. | L&#39;amministratore [!DNL Claude] non l&#39;ha abilitato. | Contattare l&#39;amministratore [!DNL Claude] (non l&#39;amministratore Workfront) e richiedere l&#39;attivazione del connettore [!DNL Adobe Workfront]. |
| Ti sei connesso, ma non puoi vedere i tuoi dati. | Hai eseguito l’autenticazione nell’istanza di Workfront errata. | Scollegare il connettore, riconnettersi e autenticarsi nell&#39;istanza corretta. |
| Autenticazione non riuscita o connessione interrotta. | La sessione di autenticazione è scaduta o si è verificato un errore di connessione. | Scollegare e ricollegare il connettore. |
| Desideri passare a un’istanza di Workfront diversa. | Una singola connessione ti collega a un’istanza. | Disconnetti, riconnetti e autentica la nuova istanza. |
| Non è possibile connettersi a Workfront oppure viene visualizzato un messaggio che indica che l&#39;accesso al server MCP è disabilitato. | L&#39;amministratore di Workfront ha disattivato l&#39;accesso al server MCP per l&#39;istanza. | Contattare l&#39;amministratore di Workfront e chiedere di abilitare l&#39;accesso al server MCP in Preferenze di sistema. |

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

Per la risoluzione dei problemi quotidiani dopo la connessione (ad esempio, risultati non aggiornati o comportamenti imprevisti), vedere [Utilizzare il server Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).


+++


<!--
+++

## Frequently asked questions about setup

+++ Expand to view frequently asked questions about setting up the Workfront MCP server.

### Can I connect to multiple Workfront instances at once?

No. Each connection ties an AI agentic platform to a single Workfront instance. To switch, disconnect and reconnect, authenticating to the new instance.

### Which administrator enables this?

Both your Workfront administrator and the administrator for your AI agentic platform. Your Workfront administrator enables MCP server access on the Workfront side. The administrator for your AI agentic platform enables Workfront access on that platform's side. For [!DNL Claude], the [!DNL Claude] Enterprise administrator enables the [!DNL Adobe Workfront] connector.

+++

-->