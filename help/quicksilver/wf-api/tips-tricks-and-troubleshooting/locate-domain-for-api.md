---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Formato del dominio per le chiamate API di Adobe Workfront
description: Individua il dominio da utilizzare nell’API di Adobe Workfront
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---

# Formato del dominio per le chiamate API di Adobe Workfront

Quando effettui una chiamata API all&#39;API Workfront, utilizzi il dominio della tua organizzazione nella chiamata. Il formato di questo URL di dominio varia a seconda che l’organizzazione sia stata integrata nell’Adobe Unified Shell.

Per verificare se l’organizzazione si trova nell’Adobe Unified Shell, esamina l’URL visualizzato quando visualizzi una pagina di Workfront.

| L’URL di Workfront inizia con: | URL per chiamate API: |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

Per individuare il dominio:

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **[!UICONTROL Configurazione]** ![Icona Configurazione](/help/_includes/assets/gear-icon-setup.png).
1. Seleziona **Sistema**, quindi seleziona **Informazioni Cliente**.

   Il dominio è elencato a destra della schermata.

   ![Dominio](assets/domain.png)

