---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: I pulsanti Filtro non vengono visualizzati nelle intestazioni di pagina
description: Leggi questo articolo per risolvere i problemi relativi ai pulsanti di filtro che non vengono visualizzati nelle intestazioni di pagina.
feature: Get Started with Workfront
author: Nolan and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# I pulsanti Filtro non vengono visualizzati nelle intestazioni di pagina

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe [!DNL Workfront]</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso</strong></td> 
   <td> <p>[!UICONTROL Amministratore di sistema]</p> </td> 
  </tr> 
 </tbody> 
</table>

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
