---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configurare l’integrazione JumpSeat
description: È possibile integrare [!DNL JumpSeat] con [!DNL Workfront] per creare guide personalizzate interne al prodotto.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# Configurare l’integrazione JumpSeat

È possibile integrare [!DNL JumpSeat] con [!DNL Workfront] per creare guide personalizzate interne al prodotto.

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
   <td>È necessario disporre di un [!DNL JumpSeat] piano.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p> Devi essere un [!DNL Workfront] amministratore. Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Prerequisiti

Prima di iniziare, è necessario

* Aggiungi e attiva [!DNL Workfront] come applicazione in [!DNL JumpSeat]. Per ulteriori informazioni, consulta [Aggiungere O Eliminare Un’Applicazione](https://support.jumpseat.io/article/how-to-add-an-application/).

## Configurare [!DNL JumpSeat] integrazione

È consigliabile impostare un [!DNL JumpSeat] integrazione negli ambienti di anteprima e produzione.

>[!TIP]
>
>È necessario aggiungere e attivare due [!DNL Workfront] applicazioni in [!DNL JumpSeat]- uno per l&#39;anteprima e uno per la produzione. Consulta [Aggiungere O Eliminare Un’Applicazione](https://support.jumpseat.io/article/how-to-add-an-application/) per ulteriori informazioni.

Per configurare [!DNL JumpSeat] integrazione:

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]**.
1. Nel pannello a sinistra, fai clic su **[!UICONTROL Sistema]** > **[!UICONTROL [!DNL JumpSeat]Integrazione]**.
1. Immetti il **[!UICONTROL [!DNL JumpSeat]URL]**, disponibile sull’icona dell’estensione in [!DNL JumpSeat].

   **Esempio:** [!DNL https]://{mycompanyname}.jumpseat.io

1. Inserisci il **[!UICONTROL [!DNL JumpSeat]token di integrazione]**. Puoi trovarlo sulla scheda **[!UICONTROL Configurazione]** pagina in [!DNL JumpSeat].

   **Esempio:** $2 anni$10$BevsKeQ8....OYR.LurSg2U64O

1. Clic **[!UICONTROL Verifica configurazione]**.
1. Scegli se desideri che l’integrazione sia **[!UICONTROL Attivo]** o **[!UICONTROL Inattivo]**.

   >[!IMPORTANT]
   >
   >Per attivare l’integrazione, deve essere superato il test di configurazione eseguito nel passaggio 5.

   ![Pagina Integrazione JumpSeat](assets/jumpseat-integration-page.png)

1. Fai clic su **[!UICONTROL Salva]**.

>[!TIP]
>
>Per ulteriori informazioni sulla configurazione di [!DNL JumpSeat] integrazione, vedi la sezione [!DNL JumpSeat] documentazione per [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
