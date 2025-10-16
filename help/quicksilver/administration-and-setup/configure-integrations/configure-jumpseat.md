---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configurare l’integrazione JumpSeat
description: Puoi integrare  [!DNL JumpSeat] con [!DNL Workfront] per creare guide personalizzate interne al prodotto.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Nolan, Becky
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 6%

---

# Configurare l’integrazione JumpSeat

È possibile integrare [!DNL JumpSeat] con [!DNL Workfront] per creare linee guida personalizzate interne al prodotto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table>
  <tr>
   <td>Pacchetto Adobe Workfront
   </td>
    <p>Flusso di lavoro Ultimate</p>
   <td> <p>PRIME o ULTIMATE</p>
   </td>
  </tr>
    <tr>
   <td>Licenze Adobe Workfront
   </td>
   <td>Standard
   <p>Piano</p>
   </td>
  </tr>
  </tr>
  <tr>
   <td>Prodotto
   </td>
   <td>È necessario disporre di un piano [!DNL JumpSeat] attivo.
   </td>
  </tr>
   <tr>
   <td>Configurazioni del livello di accesso
   </td>
   <td>Devi essere un amministratore [!DNL Workfront].
   </td>
  </tr>
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare, è necessario

* Aggiungere e attivare [!DNL Workfront] come applicazione in [!DNL JumpSeat]. Per ulteriori informazioni, vedere [Come aggiungere o eliminare un&#39;applicazione](https://support.jumpseat.io/article/how-to-add-an-application/).

>[!IMPORTANT]
>
>Se utilizzi Adobe Unified Experience, devi utilizzare il seguente URL applicazione: `.workfront.adobe.com`.



## Configurare l&#39;integrazione di [!DNL JumpSeat]

È consigliabile impostare un&#39;integrazione di [!DNL JumpSeat] sia negli ambienti di anteprima che in quelli di produzione.

>[!TIP]
>
>È necessario aggiungere e attivare due applicazioni [!DNL Workfront] separate in [!DNL JumpSeat], una per l&#39;anteprima e una per la produzione. Per ulteriori informazioni, vedere [Come aggiungere o eliminare un&#39;applicazione](https://support.jumpseat.io/article/how-to-add-an-application/).

Per configurare l&#39;integrazione di [!DNL JumpSeat]:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Sistema]** > Integrazione **[!UICONTROL [!DNL JumpSeat]]**.
1. Immetti l&#39;URL **[!UICONTROL [!DNL JumpSeat]]**, che si trova sull&#39;icona dell&#39;estensione in [!DNL JumpSeat].

>[!BEGINSHADEBOX]

**Esempio:**

https://{mycompanyname}.jumpseat.io

&#x200B;>>

>[!ENDSHADEBOX]

1. Immettere il token di integrazione **[!UICONTROL [!DNL JumpSeat]]**. Puoi trovarlo nella pagina **[!UICONTROL Configurazione]** in [!DNL JumpSeat].

   **Esempio:** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. Fare clic su **[!UICONTROL Verifica configurazione]**.
1. Scegli se vuoi che l&#39;integrazione sia **[!UICONTROL Attiva]** o **[!UICONTROL Inattiva]**.

   >[!IMPORTANT]
   >
   >Per attivare l’integrazione, deve essere superato il test di configurazione eseguito nel passaggio 5.

   ![Pagina di integrazione JumpSeat](assets/jumpseat-integration-page.png)

1. Fai clic su **[!UICONTROL Salva]**.

>[!TIP]
>
>Per ulteriori informazioni sulla configurazione dell&#39;integrazione di [!DNL JumpSeat], vedere la documentazione di [!DNL JumpSeat] per [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
