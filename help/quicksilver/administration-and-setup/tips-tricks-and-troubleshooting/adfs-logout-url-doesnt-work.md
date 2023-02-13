---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: L'URL di logout ADFS non funziona
description: La procedura descritta in questa pagina si applica solo alle organizzazioni non ancora integrate in Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# L&#39;URL di logout ADFS non funziona

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni non ancora integrate [!UICONTROL Adobe Admin Console].
>
>Se la tua organizzazione è stata integrata nel [!UICONTROL Adobe Admin Console], vedi [Differenze di amministrazione basate su piattaforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problema

Quando utilizzi l’URL di logout ADFS (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0), ricevi una pagina di messaggio con l’errore: &quot;Si è verificato un problema durante l&#39;accesso al sito. Prova a sfogliare di nuovo il sito.&quot;

Se il problema persiste, contattare l&#39;amministratore del sito e fornire il seguente numero di riferimento per identificare il problema: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Requisiti di accesso

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
   <td role="rowheader">Adobe [!DNL Workfront] licenza</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Soluzione

1. Nel server di gestione ADFS, vai a **[!UICONTROL Relazioni di trust]** > **[!UICONTROL Fiducia nel partito]** > `<your party trust>` proprietà.

1. Sotto la **[!UICONTROL Endpoint]** scheda , fai clic su **[!UICONTROL Aggiungi]**.

1. **[!UICONTROL Tipo endpoint]** = Logout SAML, Binding = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   Puoi impostare un URL di risposta se desideri che venga reindirizzato a un’altra pagina. Si consiglia tuttavia il sito ADFS perché avverte che sei disconnesso, ma dovresti comunque chiudere il browser.
