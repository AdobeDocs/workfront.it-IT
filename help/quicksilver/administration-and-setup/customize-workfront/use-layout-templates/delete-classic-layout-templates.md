---
title: Elimina modelli di layout classici
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: I modelli layout dell’esperienza Workfront classica non sono più disponibili nell’interfaccia di Workfront, ma possono comunque influire sui dati di Workfront. Questo può causare incongruenze nei campi interessati dai modelli layout (ad esempio Condiviso con), nei rapporti o nelle dashboard.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c6d33d5d-da93-4aba-8897-f177c1171595
TQID: 'https://experienceleague.adobe.com/AcxOFTyZbrQakRoeBlslCoLJgrgY4HS41vaYLOx5i-I'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 70%
---
# Elimina modelli di layout classici

I modelli layout dell’esperienza Workfront classica non sono più disponibili nell’interfaccia di Workfront, ma possono comunque influire sui dati di Workfront. Questo può causare incongruenze nei campi interessati dai modelli layout (ad esempio Condiviso con), nei rapporti o nelle dashboard.

È possibile risolvere queste incoerenze eliminando i modelli di layout Classic. Poiché non sono disponibili nell’interfaccia di Workfront, per eliminarle utilizza l’API Workfront.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.</p>
        <p>Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminare i modelli layout classici utilizzando una chiamata API

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
