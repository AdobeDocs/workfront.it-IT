---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: I pulsanti Filtro non vengono visualizzati nelle intestazioni di pagina
description: Leggi questo articolo per risolvere i problemi relativi ai pulsanti di filtro che non vengono visualizzati nelle intestazioni di pagina.
feature: Get Started with Workfront
author: Courtney
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
TQID: https://experienceleague.adobe.com/36hMJKo4unpIxvUOmBk79XlhFvFL5TgqUaoQXxrPd7c
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 287
ht-degree: 19%

---

# I pulsanti Filtro non vengono visualizzati nelle intestazioni di pagina

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table>
  <tr>
   <td>Pacchetto Adobe Workfront
   </td>
   <td>Qualsiasi</td>
  </tr>
  <tr>
   <td>Licenze Adobe Workfront
   </td>
   <td><p>Standard</p>
   <p>Piano</p>
   </td>
  </tr>
   <tr>
   <td>Configurazioni del livello di accesso
   </td>
   <td>Devi essere un amministratore [!DNL Workfront].
   </td>
  </tr>
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Problema

I seguenti pulsanti filtro non vengono visualizzati nelle rispettive aree:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] area</strong></td> 
   <td><strong>Pulsanti filtro</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Progetti] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Progetti a cui collaboro]</p> </li> 
     <li> <p>[!UICONTROL Progetti Di Cui Sono Proprietario]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL Timesheets]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL Le mie approvazioni schede orario]</span> </p> </li> 
     <li> <p><span>[!UICONTROL Le mie schede orario]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Soluzione

I pulsanti filtro nell&#39;area [!UICONTROL Progetti e schede orario] non vengono visualizzati perché i filtri corrispondenti non sono inclusi nel modello di layout applicato all&#39;utente. L&#39;amministratore [!DNL Workfront] deve assegnare un modello di layout che includa i filtri.

>[!NOTE]
>
>A volte i filtri vengono rimossi dall&#39;area [!UICONTROL Controlli elenco] in [!UICONTROL Configurazione]. L&#39;amministratore [!DNL Workfront] deve includerli negli elenchi in quest&#39;area affinché siano disponibili nei modelli di layout.

1. Verifica che nel modello di layout siano visualizzati i seguenti filtri:

   * [!UICONTROL Progetti di cui sono Responsabile] e [!UICONTROL Progetti di cui sono Proprietario] nell&#39;area [!UICONTROL Progetti]
   * [!UICONTROL Le mie approvazioni schede orario] e [!UICONTROL Le mie schede orario] nell&#39;area [!UICONTROL Scheda orario]

   Per eseguire questa operazione:

   1. Accedere al modello di layout.
   1. Seleziona **[!UICONTROL Elenchi]** in **[!UICONTROL Personalizza gli elementi visualizzati dagli utenti]**.
   1. Seleziona **[!UICONTROL Progetti]** o **[!UICONTROL Schede orario]** in **[!UICONTROL Seleziona un elenco da personalizzare]**.
   1. Nella sezione **[!UICONTROL Filtro]**, verifica che siano selezionati **[!UICONTROL Progetti di cui sono proprietario]**, **[!UICONTROL Progetti di cui sono proprietario]** (per i progetti) e **[!UICONTROL Le mie approvazioni schede orario]** e **[!UICONTROL Le mie schede orario]** (per le schede orario).
   1. Fai clic su **[!UICONTROL Salva]**.

   Per ulteriori informazioni, vedere [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Assegna il modello layout agli utenti, ai ruoli, ai team o ai gruppi appropriati. Per informazioni, vedere [Assegnare gli utenti a un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
