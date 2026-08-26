---
title: Creare app App Builder con Claude Code
description: Utilizza un set di Claude Code per creare app Adobe Workfront App Builder personalizzate descrivendo cosa desideri, invece di eseguire autonomamente i passaggi di configurazione e distribuzione.
author: Becky
feature: Digital Content and Documents
hide: true
source-git-commit: 366cc4ffea48295b00389b5ee36f2df42b2c8a07
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 4%

---


# Creare app App Builder con Claude Code

Un pacchetto di abilità consente a [!DNL Claude] (o a qualsiasi cablaggio preassemblato di codifica IA che supporta le abilità in formato Claude, ad esempio [!DNL Claude Code] o [!DNL OpenAI Codex]) di creare app [!DNL Adobe App Builder] personalizzate per [!DNL Workfront]. Se hai accesso a uno di questi strumenti, puoi creare un’estensione dell’interfaccia utente descrivendo cosa desideri in inglese semplice, senza richiedere esperienza di sviluppo o passaggi di configurazione manuali.

Le estensioni dell’interfaccia utente di Workfront, basate su Adobe App Builder, consentono alla clientela e ai partner di creare esperienze utente personalizzate. Le estensioni dell’interfaccia utente consentono di modificare l’esperienza Workfront dell’organizzazione per soddisfare al meglio le sue esigenze, il che può migliorare l’efficienza, fornire esperienze senza soluzione di continuità e connesse, migliorare in modo significativo la soddisfazione degli utenti e aiutare la tua organizzazione a realizzare la sua visione unica.

Per ulteriori informazioni sulle estensioni dell&#39;interfaccia utente di Workfront, vedere [Creare applicazioni personalizzate per Workfront con Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Competenze di estensibilità dell’interfaccia utente

Le competenze di estensibilità dell’interfaccia utente consentono a un cablaggio preassemblato della codifica AI di gestire la creazione di estensioni dell’interfaccia utente in Workfront. Descrivi la funzione che desideri e svolge il lavoro pratico, ad esempio la configurazione degli strumenti, la creazione del progetto in [!DNL Adobe App Builder], la creazione dell&#39;app, la distribuzione nel cloud di Adobe e l&#39;esecuzione in Workfront. Sei coinvolto nel processo solo quando una decisione o un accesso richiede l’intervento dell’utente. In questo articolo viene utilizzato [!DNL Claude] come esempio, ma le istruzioni sono valide per qualsiasi cablaggio preassemblato di codifica AI con supporto per Claude Skills.

## Prerequisiti

Prima di iniziare, assicurati di avere:

* **Un cablaggio preassemblato di codifica IA che supporta Claude Skills**, ad esempio [!DNL Claude Code].

  Per ulteriori informazioni sulle abilità Claude, vedere [Che cosa sono le abilità?](https://support.claude.com/en/articles/12512176-what-are-skills) nella documentazione di Claude.

* **Accesso alle abilità**.

  * Puoi trovare le abilità in [https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md).

    Se il collegamento non si apre, chiedere all&#39;amministratore di concederti l&#39;accesso.
  * Le abilità sono pubblicate nel marketplace delle abilità pubbliche di Adobe ([adobe/skills](https://github.com/adobe/skills)). In [!DNL Claude Code], eseguire:

    ```
    /plugin marketplace add adobe/skills
    ```

    ```
    /plugin install app-builder@adobe-skills
    ```

* Accesso **[!DNL Adobe App Builder], con ruolo Sviluppatore**. La tua organizzazione Adobe ha bisogno di una licenza App Builder e devi essere aggiunto come sviluppatore al suo interno. Questo è ciò che consente a [!DNL Claude] di aprire Adobe Developer Console e creare il progetto.

  Per verificare che questo prerequisito sia soddisfatto:

  1. Apri [Adobe Developer Console](https://developer.adobe.com/console).
  1. Verifica che l’organizzazione mostrata nell’angolo in alto a destra sia corretta.
  1. Fai clic su **Crea nuovo progetto** > **Crea progetto da modello**.
  1. Verifica se **App Builder** è presente nell&#39;elenco.

     * Se nell&#39;elenco sono presenti **App Builder**, è possibile accedere a.
     * Se non è presente alcuna opzione **Crea progetto da modello** o nessuna opzione **App Builder**, non si dispone ancora dell&#39;accesso. Chiedi all’amministratore di Workfront o Adobe di aggiungerti come sviluppatore (in Adobe Admin Console > Utenti > Sviluppatori) e conferma che la tua organizzazione disponga di una licenza App Builder.
* **Il server Workfront MCP è connesso**, quindi [!DNL Claude] utilizza l&#39;API Workfront reale invece di indovinare i tipi di dati, i campi e i comandi.

  Per verificare se il server Workfront MCP è già connesso, chiedere a [!DNL Claude]: *&quot;Visualizzare le risorse Workfront MCP?&quot;*

  Per ulteriori informazioni e istruzioni, vedere [Connettere Workfront a Claude](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#connect-workfront-to-claude)nell&#39;articolo Configurare il server Adobe Workfront MCP.
