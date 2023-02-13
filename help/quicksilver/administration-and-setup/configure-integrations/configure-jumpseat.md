---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configurare l’integrazione JumpSeat
description: È possibile integrare [!DNL JumpSeat] con [!DNL Workfront] per creare indicazioni personalizzate interne al prodotto.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 2%

---

# Configurare l’integrazione JumpSeat

È possibile integrare [!DNL JumpSeat] con [!DNL Workfront] per creare indicazioni personalizzate interne al prodotto.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano*</strong></td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Prodotto</strong></td> 
   <td>Devi avere un attivo [!DNL JumpSeat] piano.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p> Devi essere un [!DNL Workfront] amministratore. Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Prerequisiti

Prima di iniziare, devi

* Aggiungi e attiva [!DNL Workfront] come applicazione in [!DNL JumpSeat]. Per ulteriori informazioni, consulta [Come Aggiungere O Eliminare Un’Applicazione](https://support.jumpseat.io/article/how-to-add-an-application/).

## Configura le [!DNL JumpSeat] integrazione

Consigliamo di configurare un [!DNL JumpSeat] integrazione sia negli ambienti di anteprima che di produzione.

>[!TIP]
>
>È necessario aggiungere e attivare due [!DNL Workfront] applicazioni in [!DNL JumpSeat]- uno per Anteprima e uno per Produzione. Vedi [Come Aggiungere O Eliminare Un’Applicazione](https://support.jumpseat.io/article/how-to-add-an-application/) per ulteriori informazioni.

Per configurare le [!DNL JumpSeat] integrazione:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]**.
1. Nel pannello a sinistra, fai clic su **[!UICONTROL Sistema]** > **[!UICONTROL [!DNL JumpSeat]Integrazione]**.
1. Inserisci il tuo **[!UICONTROL [!DNL JumpSeat]URL]**.

   **Esempio:** [!DNL https]://{mycompanyname}.jumpseduta.io

1. Inserisci il **[!UICONTROL [!DNL JumpSeat]token di integrazione]**. Puoi trovarlo nella **[!UICONTROL Configurazione]** in [!DNL JumpSeat].

   **Esempio:** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. Fai clic su **[!UICONTROL Verificare la configurazione]**.
1. Scegli se desideri che l’integrazione sia **[!UICONTROL Attivo]** o **[!UICONTROL Inattivo]**.

   >[!IMPORTANT]
   >
   >Il test di configurazione eseguito al punto 5 deve essere superato per attivare l&#39;integrazione.

   ![Pagina di integrazione JumpSeat](assets/jumpseat-integration-page.png)

1. Fai clic su **[!UICONTROL Salva]**.
