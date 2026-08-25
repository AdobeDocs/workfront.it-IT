---
title: Creare app App Builder con Claude Code
description: Utilizza un set di Claude Code per creare app Adobe Workfront App Builder personalizzate descrivendo cosa desideri, invece di eseguire autonomamente i passaggi di configurazione e distribuzione.
author: Becky
feature: Digital Content and Documents
hide: true
source-git-commit: e5a288dcac20be9176d1541d531edaf0d8c99a8c
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 5%

---


# Creare app App Builder con Claude Code

Un set di abilità [!DNL Claude Code] consente a [!DNL Claude] di creare app [!DNL Adobe App Builder] personalizzate per [!DNL Workfront]. Ciò significa che puoi crearne una descrivendo ciò che desideri in inglese semplice, senza essere uno sviluppatore o scrivendo personalmente i passaggi di configurazione.

Le estensioni dell’interfaccia utente di Workfront, basate su Adobe App Builder, consentono alla clientela e ai partner di creare esperienze utente personalizzate. Le estensioni dell’interfaccia utente consentono di modificare l’esperienza Workfront dell’organizzazione per soddisfare al meglio le sue esigenze, il che può migliorare l’efficienza, fornire esperienze senza soluzione di continuità e connesse, migliorare in modo significativo la soddisfazione degli utenti e aiutare la tua organizzazione a realizzare la sua visione unica.

Per ulteriori informazioni sulle estensioni dell&#39;interfaccia utente di Workfront, vedere [Creare applicazioni personalizzate per Workfront con Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Interfaccia utente Competenze di estensibilità per Claude

L&#39;utilizzo di [!DNL Adobe App Builder] può essere piuttosto tecnico, il che può creare barriere se un utente non ha familiarità con la procedura o le tecniche. Le abilità di estensibilità dell&#39;interfaccia utente semplificano questo processo utilizzando [!DNL Claude]. Descrivi la funzione desiderata e [!DNL Claude] esegue le operazioni pratiche, ad esempio la configurazione degli strumenti, la creazione del progetto in [!DNL Adobe App Builder], la creazione dell&#39;app, la distribuzione nel cloud di Adobe e l&#39;esecuzione in Workfront. Sei coinvolto nel processo solo quando una decisione o un accesso richiede l’intervento dell’utente.

## Prerequisiti

Prima di iniziare, assicurati di avere:

* Installazione di **[!DNL Claude Code]** completata.
* **Accesso alle abilità**.

  * Puoi trovare le abilità in [https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md).

    Se il collegamento non si apre, chiedere all&#39;amministratore di concederti l&#39;accesso.
  * Dopo aver scaricato le abilità, esegui i seguenti comandi per configurarle.

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
