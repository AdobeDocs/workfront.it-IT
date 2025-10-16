---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Formato del dominio per le chiamate API di Adobe Workfront
description: Individua il dominio da utilizzare nell’API di Adobe Workfront
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: e9a9e45720c8b9ad25e3fa9340c813a73989fb4a
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 1%

---

# Formato del dominio per le chiamate API di Adobe Workfront

Quando effettui una chiamata API all&#39;API Workfront, utilizzi il dominio della tua organizzazione nella chiamata. Il formato di questo URL di dominio varia a seconda che l’organizzazione sia stata integrata in Adobe Unified Shell.

Per sapere se la tua organizzazione si trova in Adobe Unified Shell, esamina l’URL visualizzato quando visualizzi una pagina di Workfront.

| L’URL di Workfront inizia con: | URL per chiamate API: |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


Per individuare il dominio:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic sull&#39;icona **[!UICONTROL Setup]** ![Setup](/help/_includes/assets/gear-icon-setup.png).
1. Seleziona **Sistema**, quindi seleziona **Informazioni cliente**.

   Il dominio è elencato a destra della schermata.

   ![Dominio](assets/domain.png)

