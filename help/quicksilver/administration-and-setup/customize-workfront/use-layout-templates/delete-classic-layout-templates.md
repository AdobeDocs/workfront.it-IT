---
title: Elimina modelli di layout classici
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: I modelli layout dell’esperienza Workfront classica non sono più disponibili nell’interfaccia di Workfront, ma possono comunque influire sui dati di Workfront. Questo può causare incongruenze nei campi interessati dai modelli stessi (ad esempio Condiviso con), nei rapporti o nelle dashboard.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c6d33d5d-da93-4aba-8897-f177c1171595
source-git-commit: a8214d9e10363881afbc2bd71f78f46cb6a25880
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 56%

---

# Concedere l’accesso amministrativo per un modello di layout

I modelli layout dell’esperienza Workfront classica non sono più disponibili nell’interfaccia di Workfront, ma possono comunque influire sui dati di Workfront. Questo può causare incongruenze nei campi interessati dai modelli stessi (ad esempio Condiviso con), nei rapporti o nelle dashboard.

È possibile risolvere queste incoerenze eliminando i modelli di layout Classic. Poiché non sono disponibili nell’interfaccia di Workfront, per eliminarle utilizza l’API Workfront.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Eliminare i modelli di layout classici utilizzando una chiamata API

Puoi immettere chiamate API nella barra URL del browser e premere Invio. La risposta API viene visualizzata nel browser.

>[!NOTE]
>
>Non è possibile eliminare i modelli layout di sistema e globali.

1. Accedi a Workfront.
1. Individua il modello layout da eliminare utilizzando la seguente chiamata API:
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. Prendi nota dell’ID del modello layout che desideri eliminare.
1. Individua l’ID sessione utilizzando la seguente chiamata API:
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >Non condividere mai il tuo ID sessione con nessuno.

1. Inserisci l’ID del modello layout e l’ID sessione nella seguente chiamata API:
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. Incolla la chiamata API dal passaggio 4 nella barra degli URL del browser e premi Invio.

   Questa azione eliminerà il modello layout.
