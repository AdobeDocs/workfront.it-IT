---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Aggiungere un utente a un’organizzazione in Adobe Workfront Fusion
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Aggiungere un utente a un’organizzazione o a un team in Adobe Workfront Fusion

>[!IMPORTANT]
>
>Questo articolo verrà rimosso nel prossimo futuro, poiché tutte le organizzazioni verranno spostate in Adobe Admin Console.

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state caricate in [!DNL Adobe Admin Console]. Se la tua organizzazione è stata integrata in [!DNL Adobe Admin Console], devi eseguire questa azione tramite [!DNL Adobe Admin Console].
>
>Per istruzioni sull&#39;aggiunta di un utente dopo che l&#39;organizzazione è stata spostata in [!DNL  Adobe Admin Console] e nell&#39;esperienza unificata di Adobe, vedi [Aggiungere utenti a [!DNL Adobe Workfront Fusion] tramite il [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md).
>
>Per un elenco delle procedure che differiscono a seconda che l&#39;organizzazione sia stata integrata in Adobe Admin Console, vedi [Differenze di amministrazione basate su Platform (Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

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
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> 
     <p>Devi essere un amministratore [!DNL Workfront Fusion] per la tua organizzazione.</p>
     <p>Devi essere un amministratore [!DNL Workfront Fusion] per il tuo team.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Aggiungere utenti a un’organizzazione


<!--
<p>The procedure to add a user to your Fusion organization differs based on whether your organization has been onboarded to the Adobe Business Platform. </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Add a user to an organization that has been onboarded to the Adobe Business Platform</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Add a user to an organization that has not been onboarded to the Adobe Business Console</a> </p> </li>
</ul>
<div>
<p><strong>Add a user to an organization that has been onboarded to the Adobe Business Platform</strong></p>
<p>If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.</p>
<p>For instructions on adding a user in the Adobe Admin Console:</p>
<ul>
<li> <p>See <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Create users in Workfront with the Adobe Admin Console</a></p> </li>
<li> <p>See the section "Add users" in the article <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li>
<li> <p>Contact your Adobe Admin Console Administrator.</p> </li>
</ul>
<p>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Platform-based administration differences (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>Add a user to an organization that has not been onboarded to the Adobe Business Console</strong></p>

-->
>[!NOTE]
>
>Se la tua organizzazione è attualmente in fase di trasferimento al Adobe Admin Console, non puoi gestire gli utenti in Workfront (aggiunta o eliminazione di utenti). Puoi eseguire queste azioni in Adobe Admin Console al termine della migrazione.

Per aggiungere utenti all’organizzazione, devi essere un amministratore dell’organizzazione a cui desideri aggiungere gli utenti. Per informazioni sui ruoli, vedere [Ruoli organizzazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

Per aggiungere un utente all&#39;organizzazione:

1. Passa a **[!UICONTROL Organizzazioni]** nel menu e seleziona l&#39;organizzazione a cui desideri aggiungere un utente.
1. Apri la scheda **[!UICONTROL Utenti]** nel dashboard.
1. Fai clic su **[!UICONTROL Invita un nuovo utente]**.e invia l&#39;invito facendo clic su **[!UICONTROL Invia]**.

   >[!NOTE]
   >
   >   
   >Se non trovi il pulsante [!UICONTROL Invita un nuovo utente], significa che la tua organizzazione è stata integrata in [!DNL Adobe Business Platform.]
   >
   >  Per istruzioni sull&#39;aggiunta di un utente a un&#39;organizzazione di cui è stato effettuato l&#39;onboarding in [!DNL Adobe Business Platform], vedere [Aggiungere utenti a [!DNL Adobe Workfront Fusion] tramite il [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)

1. Compila il modulo.

   <table style="table-layout:auto">
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Email address]</td>
      <td>
        Inserisci l’indirizzo e-mail dell’utente
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>
        <p>Inserisci il nome completo dell'utente</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Role] </td>
      <td>Selezionare il ruolo dell'utente. Per una spiegazione dei ruoli, vedere <a href="/help/quicksilver/workfront-fusion/organizations/organization-roles.md">Ruoli organizzazione e team.</a></p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Team</td>
      <td>Seleziona tutti i team di cui vuoi che l’utente sia membro.</td>
    </tr>
    <tr>
      <td role="rowheader">Nota</td>
      <td>Immettere una nota per l'utente. Questa nota verrà visualizzata nell'e-mail di invito dell'utente.</td>
    </tr>
  </tbody>
</table>

L’utente riceve un messaggio e-mail di invito in cui può accettare l’invito.

## Aggiungere un utente a un team

Gli utenti vengono assegnati ai team quando vengono creati. Se è necessario aggiungere un utente esistente a un team, è possibile aggiungerlo nella pagina Utenti del team.

L’aggiunta di un utente a un team viene gestita dalla pagina relativa a tale team.

1. Vai al team a cui desideri aggiungere l&#39;utente selezionando **Organizzazioni** nel pannello a sinistra, facendo clic sulla scheda **Team** nella pagina dell&#39;organizzazione e selezionando il team.

   Oppure

   Se ti trovi nella pagina per un altro team, fai clic sul menu a discesa del team nella parte superiore della pagina.

1. Nella pagina del team (con il nome del team nella parte superiore della pagina), seleziona la scheda **Utenti**.
1. Individua l’utente sulla pagina. Gli utenti dell’organizzazione vengono visualizzati in questa pagina anche se non sono membri del team.
1. Fai clic su **Nessuno** a destra del nome dell&#39;utente, quindi seleziona il ruolo che desideri assegnare al team.

L’utente viene aggiunto al team.