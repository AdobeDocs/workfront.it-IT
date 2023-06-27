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
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Gestisci [!DNL Adobe Workfront Fusion] utenti della tua organizzazione

[!DNL Adobe Workfront Fusion] gli amministratori possono gestire i ruoli utente all’interno di [!DNL Workfront Fusion].

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
   <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> 
     <p>Devi essere un [!DNL Workfront Fusion] per la tua organizzazione.</p>
     <p>Devi essere un [!DNL Workfront Fusion] amministratore del team.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Visualizzare o modificare i ruoli utente {#view}

[!DNL Adobe Workfront Fusion] gli amministratori possono visualizzare e aggiornare i ruoli utente.

1. Durante l’accesso come [!DNL Workfront Fusion] amministratore, seleziona **[!UICONTROL Utenti]** nel menu di navigazione a sinistra.
1. Clic **[!UICONTROL Dettagli]** nella riga dell’utente che desideri visualizzare.
1. (Facoltativo) Per aggiornare il ruolo dell’utente, fai clic sul menu a discesa nella **[!DNL Role]** nella riga dell’organizzazione in cui desideri modificare il ruolo dell’utente, quindi seleziona il nuovo ruolo.

## Visualizzare o modificare i dettagli utente {#view2}

[!DNL Adobe Workfront Fusion] gli amministratori possono visualizzare e aggiornare i dettagli degli utenti.

1. Durante l’accesso come [!DNL Workfront Fusion] amministratore, seleziona **[!UICONTROL Utenti]** nel menu di navigazione a sinistra.
1. Clic **[!UICONTROL Dettagli]** nella riga dell’utente che desideri visualizzare.
1. (Facoltativo) Per aggiornare i dettagli dell’utente, fai clic su **[!UICONTROL Opzioni]** nell’angolo superiore destro dello schermo, quindi seleziona **[!UICONTROL Modifica dettagli]**.

## Eliminare un utente {#delete}

[!DNL Adobe Workfront Fusion] gli amministratori possono eliminare gli utenti.

1. Durante l’accesso come [!DNL Workfront Fusion] amministratore, seleziona [!UICONTROL Utenti] nel menu di navigazione a sinistra.
1. Clic **[!UICONTROL Dettagli]** nella riga dell’utente che desideri visualizzare.
1. (Facoltativo) Per aggiornare i dettagli dell’utente, fai clic su **[!UICONTROL Opzioni]** nell’angolo superiore destro dello schermo, quindi seleziona **[!UICONTROL Elimina]**.

### Considerazioni durante l’eliminazione di un utente in Workfront Fusion

* Quando un utente viene eliminato, le connessioni, le chiavi e i webhook dell’utente vengono rimossi. Eventuali scenari appartenenti all’utente vengono trasferiti al proprietario dell’organizzazione. Le connessioni in questi scenari devono essere aggiornate, perché le connessioni appartenenti all’utente non sono più valide.
* Se l’utente eliminato è proprietario di applicazioni o modelli pubblici, le applicazioni o i modelli pubblici vengono trasferiti al proprietario dell’organizzazione. Se non è presente un proprietario dell’organizzazione, le applicazioni o i modelli pubblici vengono trasferiti a un altro utente.
