---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Configurare il server MCP di Adobe Workfront
description: Configura l’istanza di Workfront e l’assistente AI in modo da poter lavorare con Workfront tramite una conversazione in linguaggio naturale.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 4%

---


# Configurare il server MCP di Adobe Workfront

Il server MCP [!DNL Adobe Workfront] consente di utilizzare i dati Workfront tramite conversazioni in linguaggio naturale in un assistente di intelligenza artificiale supportato come Claude o ChatGPT.

Prima di poter collegare un assistente AI a Workfront, un amministratore Workfront deve abilitare l’accesso al server MCP nell’istanza Workfront. I passaggi esatti per connettere un assistente AI sono diversi per ogni assistente AI supportato.

Per ulteriori informazioni sul server Workfront MCP, vedere [Panoramica del server Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Assistenti AI supportati

Il server MCP di Workfront supporta attualmente i seguenti assistenti AI:

* [!DNL Claude]

<!-- NEEDS DETAIL: Update this list as Adobe adds support for additional AI assistants (for example, [!DNL Gemini], or [!DNL Microsoft Copilot]). -->

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront package requirement (Select, Prime, Ultimate, Any?) --></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront license requirement (Standard, Work, etc.) --></p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di poter collegare Workfront a un assistente AI, è necessario:

* Avere un account [!DNL Adobe Workfront] attivo con l&#39;autorizzazione per accedere ai dati che si desidera utilizzare.
* Avere accesso a un assistente di intelligenza artificiale come [!DNL Claude].

  <!-- NEEDS DETAIL: Confirm which Claude tiers are supported. Claude Enterprise is confirmed; Claude Pro and Claude Team support is unconfirmed. -->

### Prerequisiti per l’amministrazione

L&#39;accesso al server MCP è gestito da due amministratori distinti. Entrambi devono abilitare l’accesso prima di poter connettersi.

* **L&#39;amministratore di Workfront** deve abilitare l&#39;accesso al server MCP nella tua istanza di Workfront.

* Se utilizzi una versione Enterprise di un assistente AI, l&#39;amministratore dell&#39;assistente AI deve abilitare il connettore [!DNL Adobe Workfront] per la tua organizzazione.


## Connettere Workfront a Claude

La connessione a Workfront viene eseguita una volta per ogni account [!DNL Claude]. La connessione consente di eseguire l&#39;autenticazione a una specifica istanza di Workfront e si rimane connessi fino a quando non si sceglie di disconnettersi.


>[!IMPORTANT]
>
>Se utilizzi [!DNL Claude] Enterprise, **l&#39;amministratore [!DNL Claude] Enterprise** deve abilitare il connettore [!DNL Adobe Workfront] per la tua organizzazione. Finché non lo faranno, il connettore [!DNL Adobe Workfront] non verrà visualizzato quando lo si cerca in [!DNL Claude]. Contatta prima l&#39;amministratore [!DNL Claude].


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

### Verifica la connessione

Per confermare che [!DNL Claude] è connesso a Workfront, chiedere a [!DNL Claude] di elencare le azioni rese disponibili dal server Workfront MCP. Ad esempio:

* *Quali azioni puoi intraprendere Workfront?*
* *Elenca gli strumenti di Workfront a cui hai accesso.*

[!DNL Claude] restituisce l&#39;elenco delle azioni disponibili.

<!-- NEEDS DETAIL: Add a screenshot of the tool-list response. -->

### Passa a un’altra istanza di Workfront

Ogni connessione autentica [!DNL Claude] in una singola istanza di Workfront. Per utilizzare un&#39;istanza diversa, disconnettiti e riconnettiti.

Per connettersi a un&#39;altra istanza di Workfront:

1. In [!DNL Claude], disconnettere il connettore [!DNL Adobe Workfront].
1. Ricollegare il connettore.
1. Esegui l’autenticazione alla nuova istanza di Workfront.

>[!NOTE]
>
>La disconnessione da [!DNL Claude] non cambia l&#39;istanza di Workfront. È necessario disconnettere e ricollegare il connettore.

## Personalizzare il comportamento di Claude con le abilità

<!-- NEEDS DETAIL: Confirm whether Adobe is shipping any pre-built Claude skills alongside the MCP server. If yes, list them and link to download or installation guidance. If no, decide whether to mention skills as a user-driven workaround at all, or remove this section. -->

[!DNL Claude] supporta set di istruzioni creati dall&#39;utente denominati skill. È possibile utilizzare un&#39;abilità per personalizzare il comportamento di [!DNL Claude] con Workfront. È possibile, ad esempio, creare un&#39;abilità che indica a [!DNL Claude] di recuperare sempre dati aggiornati da Workfront anziché basarsi sui risultati precedenti.

## Risoluzione dei problemi di configurazione e autenticazione

| Problema | Probabile causa | Correggi |
|---|---|---|
| Impossibile trovare il connettore [!DNL Adobe Workfront] in [!DNL Claude]. | L&#39;amministratore [!DNL Claude] non l&#39;ha abilitato. | Contattare l&#39;amministratore [!DNL Claude] (non l&#39;amministratore Workfront) e richiedere l&#39;attivazione del connettore [!DNL Adobe Workfront]. |
| Ti sei connesso, ma non puoi vedere i tuoi dati. | Hai eseguito l’autenticazione nell’istanza di Workfront errata. | Scollegare il connettore, riconnettersi e autenticarsi nell&#39;istanza corretta. |
| Autenticazione non riuscita o connessione interrotta. | La sessione di autenticazione è scaduta o si è verificato un errore di connessione. | Scollegare e ricollegare il connettore. |
| Desideri passare a un’istanza di Workfront diversa. | Una singola connessione ti collega a un’istanza. | Disconnetti, riconnetti e autentica la nuova istanza. |

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

Per la risoluzione dei problemi quotidiani dopo la connessione (ad esempio, risultati non aggiornati o comportamenti imprevisti), vedere [Utilizzare il server Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).

## Domande frequenti sulla configurazione

### È possibile connettersi a più istanze di Workfront contemporaneamente?

No. Ogni connessione collega un assistente AI a una singola istanza Workfront. Per passare, disconnettersi e riconnettersi, eseguire l&#39;autenticazione nella nuova istanza.

### Questo funziona con Claude Pro o Claude Team, o solo Claude Enterprise?

<!-- NEEDS DETAIL: Confirm Claude tier support and answer this directly. -->

### Quale amministratore abilita questa impostazione?

Sia l’amministratore di Workfront che l’amministratore dell’assistente AI. L&#39;amministratore di Workfront abilita l&#39;accesso al server MCP sul lato Workfront. L’amministratore dell’assistente AI abilita l’accesso a Workfront sul lato dell’assistente AI. Per [!DNL Claude], l&#39;amministratore Enterprise di [!DNL Claude] abilita il connettore [!DNL Adobe Workfront].
