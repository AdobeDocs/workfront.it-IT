---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: L'URL di disconnessione ADFS non funziona
description: La procedura descritta in questa pagina si applica solo alle organizzazioni che non hanno ancora effettuato l’onboarding in Adobe Admin Console.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 0%

---

# L&#39;URL di disconnessione ADFS non funziona

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state caricate in [!UICONTROL Adobe Admin Console].
>
>Se la tua organizzazione è stata integrata in [!UICONTROL Adobe Admin Console], vedi [Differenze di amministrazione basate su Platform ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problema

Quando si utilizza l&#39;URL di disconnessione ADFS (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0), viene visualizzata una pagina con il messaggio di errore: &quot;Si è verificato un problema di accesso al sito. Prova a passare di nuovo al sito.&quot;

Se il problema persiste, contattare l&#39;amministratore del sito e fornire il seguente numero di riferimento per identificare il problema: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

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
   <td role="rowheader">Licenza Adobe [!DNL Workfront]</td> 
   <td> 
   <p>Nuovo: Standard</p>
   Oppure
   <p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>  
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Soluzione

1. Nel server di gestione ADFS, passare a **[!UICONTROL Relazioni di trust]** > **[!UICONTROL Trust tra entità]** > `<your party trust>` proprietà.

1. Nella scheda **[!UICONTROL Endpoints]**, fai clic su **[!UICONTROL Aggiungi]**.

1. **[!UICONTROL Tipo endpoint]** = Disconnessione SAML, Binding = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   Puoi impostare un URL di risposta se desideri che venga reindirizzato a un’altra pagina. Tuttavia, è consigliabile utilizzare il sito ADFS perché avverte che è stata eseguita la disconnessione, ma è comunque necessario chiudere il browser.
