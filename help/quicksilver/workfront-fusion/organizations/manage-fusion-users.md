---
filename: manage-fusion-users
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Gestisci [!DNL Adobe Workfront Fusion] utenti della tua organizzazione
description: Gestisci [!DNL Adobe Workfront Fusion] utenti della tua organizzazione
author: Becky
feature: Workfront Fusion
exl-id: fbb858a6-1230-41b4-892a-4ffeb2711922
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Gestisci [!DNL Adobe Workfront Fusion] utenti della tua organizzazione

[!DNL Adobe Workfront Fusion] gli amministratori possono gestire i ruoli utente all&#39;interno di [!DNL Workfront Fusion].

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on adding a user in the Adobe Admin Console:
>
>* See [Add a user to an organization in Adobe Workfront Fusion](../../workfront-fusion/organizations/add-user-to-an-organization.md#create)
>* See the section "Add users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront Fusion/Adobe Business Platform)](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

-->

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!DNL Pro] o superiore</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">Licenza [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration,</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> 
     <p>Devi essere un [!DNL Workfront Fusion] amministratore della tua organizzazione.</p>
     <p>Devi essere un [!DNL Workfront Fusion] amministratore del team.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Visualizzare o modificare i ruoli utente {#view}

[!DNL Adobe Workfront Fusion] gli amministratori possono visualizzare e aggiornare i ruoli utente.

1. Durante l&#39;accesso come [!DNL Workfront Fusion] amministratore, seleziona **[!UICONTROL Utenti]** nella navigazione a sinistra.
1. Fai clic su **[!UICONTROL Dettagli]** nella riga dell’utente che si desidera visualizzare.
1. (Facoltativo) Per aggiornare il ruolo dell’utente, fai clic sul menu a discesa nel **[!DNL Role]** nella riga dell&#39;organizzazione in cui si desidera modificare il ruolo dell&#39;utente, quindi selezionare il nuovo ruolo.

## Visualizzare o modificare i dettagli utente {#view2}

[!DNL Adobe Workfront Fusion] gli amministratori possono visualizzare e aggiornare i dettagli utente.

1. Durante l&#39;accesso come [!DNL Workfront Fusion] amministratore, seleziona **[!UICONTROL Utenti]** nella navigazione a sinistra.
1. Fai clic su **[!UICONTROL Dettagli]** nella riga dell’utente che si desidera visualizzare.
1. (Facoltativo) Per aggiornare i dettagli dell&#39;utente, fai clic su **[!UICONTROL Opzioni]** nell’angolo superiore destro dello schermo, quindi seleziona **[!UICONTROL Dettagli sulle modifiche]**.

## Eliminare un utente {#delete}

[!DNL Adobe Workfront Fusion] gli amministratori possono eliminare gli utenti.

1. Durante l&#39;accesso come [!DNL Workfront Fusion] amministratore, seleziona [!UICONTROL Utenti] nella navigazione a sinistra.
1. Fai clic su **[!UICONTROL Dettagli]** nella riga dell’utente che si desidera visualizzare.
1. (Facoltativo) Per aggiornare i dettagli dell&#39;utente, fai clic su **[!UICONTROL Opzioni]** nell’angolo superiore destro dello schermo, quindi seleziona **[!UICONTROL Elimina]**.

### Considerazioni sull&#39;eliminazione di un utente in Workfront Fusion

* Quando un utente viene eliminato, le connessioni, le chiavi e i webhook dell&#39;utente vengono rimossi. Tutti gli scenari appartenenti all&#39;utente vengono trasferiti al proprietario dell&#39;organizzazione. Le connessioni in questi scenari devono essere aggiornate perché le connessioni appartenenti all&#39;utente non sono più valide.
* Se l&#39;utente eliminato possiede applicazioni o modelli pubblici, le applicazioni o i modelli pubblici vengono trasferiti al proprietario dell&#39;organizzazione. Se non è presente un proprietario organizzazione, le applicazioni o i modelli pubblici vengono trasferiti a un altro utente.
