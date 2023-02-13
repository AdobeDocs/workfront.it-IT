---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: I pulsanti di filtro non vengono visualizzati nelle intestazioni di pagina
description: Leggi questo articolo per risolvere i problemi relativi ai pulsanti del filtro che non vengono visualizzati nelle intestazioni di pagina.
feature: Get Started with Workfront
author: Lisa and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# I pulsanti di filtro non vengono visualizzati nelle intestazioni di pagina

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
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licenza</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso</strong></td> 
   <td> <p>[!UICONTROL System Administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problema

I seguenti pulsanti di filtro non vengono visualizzati nelle rispettive aree:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] area</strong></td> 
   <td><strong>Pulsanti filtro</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Projects] </p> </td> 
   <td> 
    <ul> 
     <li> <p>Progetti in corso</p> </li> 
     <li> <p>[!UICONTROL Progetti Di Proprietà]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL Timesheets]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL Approvazioni schede attività]</span> </p> </li> 
     <li> <p><span>[!UICONTROL I miei fogli presenze]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Soluzione

I pulsanti di filtro nel [!UICONTROL Progetti e schede attività] l’area non viene visualizzata perché i filtri corrispondenti non sono inclusi nel modello di layout applicato all’utente. La [!DNL Workfront] l’amministratore deve assegnare un modello di layout che includa i filtri.

>[!NOTE]
>
>A volte i filtri vengono rimossi dal [!UICONTROL Controlli elenco] area [!UICONTROL Configurazione]. La [!DNL Workfront] affinché siano disponibili nei modelli di layout, l’amministratore deve includerli negli elenchi di questa area.

1. Verifica che nel modello di layout siano visualizzati i seguenti filtri:

   * [!UICONTROL Progetti in corso] e [!UICONTROL Progetti di proprietà] in [!UICONTROL Progetti] area
   * [!UICONTROL Approvazioni foglio presenze personali] e [!UICONTROL Fogli orari personali] in [!UICONTROL Scheda attività] area

   Per eseguire questa operazione:

   1. Accedi al modello di layout.
   1. Seleziona **[!UICONTROL Elenchi]** sotto **[!UICONTROL Personalizzare ciò che gli utenti visualizzano]**.
   1. Seleziona **[!UICONTROL Progetti]** o **[!UICONTROL Schede temporali]** sotto **[!UICONTROL Selezionare un elenco da personalizzare]**.
   1. In **[!UICONTROL Filtro]** sezione , verifica che **[!UICONTROL Progetti in corso]**, **[!UICONTROL Progetti di proprietà]** (per i progetti) e **[!UICONTROL Approvazioni foglio presenze personali]** e **[!UICONTROL Fogli orari personali]** (per i fogli presenze) sono selezionati.
   1. Fai clic su **[!UICONTROL Salva]**.

   Per ulteriori informazioni, consulta [Personalizzare filtri, visualizzazioni e gruppi utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Assegna il modello di layout agli utenti, ai ruoli, ai team o ai gruppi corretti. Per informazioni, consulta [Assegnare gli utenti a un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
