---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Organizzazioni e team di Adobe Workfront Fusion
description: Le funzioni Organizzazione e Team di Adobe Workfront Fusion consentono alle aziende di controllare l'accesso a scenari e altre funzioni all'interno di Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: 063c4a885d43b41ba6ff72ac22a1552486531fa6
workflow-type: tm+mt
source-wordcount: '1239'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] organizzazioni e team

Le funzionalità Organizzazione e Team di [!DNL Adobe Workfront Fusion] consentono alle aziende di controllare l&#39;accesso a scenari e altre funzionalità in Fusion.

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

<p>**Per informazioni sulle licenze [!DNL Adobe Workfront Fusion], vedere <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] licenze</a></p>


## Organismi

[!DNL Workfront Fusion] utenti appartengono a un&#39;organizzazione.

* [Ruoli organizzazione](#organization-roles)
* [Invito di utenti a un&#39;organizzazione](#inviting-users-to-an-organization)
* [Passare da un’organizzazione all’altra](#switch-between-organizations)

### Ruoli organizzazione

Un utente ha uno dei seguenti ruoli in un’organizzazione:

* **[!UICONTROL Proprietario]**: il proprietario dispone di tutte le autorizzazioni disponibili nell&#39;organizzazione.
* **[!UICONTROL Amministratore]**: il ruolo di amministratore consente a un utente di creare e gestire team e utenti per l&#39;organizzazione.
* **[!UICONTROL Membro]**: i membri possono utilizzare [!DNL Workfront Fusion], ma non possono apportare modifiche organizzative.
* **[!UICONTROL Contabile]**: un ruolo di contabile consente agli utenti di visualizzare solo le informazioni sulle licenze nel dashboard dell&#39;organizzazione.
* **[!UICONTROL Sviluppatore app]**: la funzionalità per questo ruolo non è attualmente disponibile e lo sarà prossimamente. Non è consigliabile assegnare gli utenti a questo ruolo in questo momento.

Per informazioni sulle azioni specifiche disponibili per gli utenti in ogni ruolo dell&#39;organizzazione, vedere [Ruoli dell&#39;organizzazione e del team](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### Invito di utenti a un&#39;organizzazione

Per impostazione predefinita, il proprietario di un’organizzazione (o l’utente autorizzato) può invitare un’altra persona a partecipare all’organizzazione.

Per invitare un utente a partecipare a un&#39;organizzazione:

1. Fai clic su **[!UICONTROL Modifica dettagli]** nell&#39;angolo superiore destro della schermata.
1. Selezionare **[!UICONTROL Invita un nuovo utente]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. Inserisci l’indirizzo e-mail e il nome dell’utente.
1. Selezionare un ruolo per l&#39;utente. Per ulteriori informazioni sui ruoli, vedere [Ruoli organizzazione](#organization-roles) in questo documento.
1. (Facoltativo) Aggiungi una nota. Questa nota viene visualizzata nell&#39;e-mail di invito ricevuta dall&#39;utente.
1. Fai clic su **[!UICONTROL Salva]**.

[!DNL Fusion] invia un&#39;e-mail con un invito all&#39;organizzazione specifica e un pulsante [!UICONTROL Accetta il ruolo].

Quando il destinatario fa clic sul pulsante, viene reindirizzato alla pagina dell’invito, dove può accettare l’invito.

L&#39;invito scadrà tra un giorno.

>[!NOTE]
>
>Se l&#39;utente è nuovo a [!DNL Fusion], [!DNL Fusion] crea automaticamente un account per l&#39;utente e invia un&#39;e-mail con una password temporanea, indirizzando al nuovo utente l&#39;accesso e la modifica della password.

### Passare da un’organizzazione all’altra

È possibile far parte di più organizzazioni in Fusion. Le risorse non sono condivise tra le organizzazioni.

Per cambiare organizzazione all’interno dell’esperienza unificata di Adobe, fai clic sul nome dell’organizzazione nell’angolo in alto a destra e seleziona la nuova organizzazione dal menu a discesa. Solo le organizzazioni con un account di Fusion verranno visualizzate nel menu a discesa, anche se sei membro di altre organizzazioni in Adobe.

## Team

I team sono gruppi di utenti che condividono l’accesso a risorse specifiche. Tali risorse possono includere:

* Scenari
* Connessioni
* Webhook
* Chiavi
* Archivi di dati
* Strutture di dati
* Impostazioni delle notifiche e-mail

>[!NOTE]
>
>Poiché i team controllano l’accesso alle risorse, a volte è utile che abbiano un solo membro. Ad esempio, gli utenti in formazione possono creare connessioni ai loro singoli account [!DNL Google]. Tutti i membri del team potranno connettersi al singolo account [!DNL Google]. In questo caso, è consigliabile che l&#39;utente sia l&#39;unico membro di un team di formazione.

Le organizzazioni possono disporre di tutti i team necessari e gli utenti possono appartenere a uno o più team.

Gli utenti possono selezionare il proprio team dall’elenco a discesa nel pannello di navigazione a sinistra. Gli utenti visualizzano solo i team di cui sono membri. La selezione di un team consente a un utente di accedere alle risorse del team.

* [Ruoli di team](#team-roles)
* [Gestione team](#team-management)

### Ruoli di team

Un utente ha uno dei seguenti ruoli in ciascuno dei propri team:

* **[!UICONTROL Amministratore team]**: oltre alle funzionalità degli altri ruoli del team, il ruolo Amministratore consente all&#39;utente di aggiungere, rimuovere o modificare il ruolo di un membro del team.
* **[!UICONTROL Membro team]**: il ruolo del membro del team consente agli utenti di creare ed eseguire scenari.
* **[!UICONTROL Monitoraggio team]**: il ruolo [!UICONTROL monitoraggio] consente agli utenti di accedere alle informazioni sull&#39;esecuzione per gli scenari, ma non è possibile progettare scenari o modificare lo stato &quot;Attivo&quot;.
* **[!UICONTROL Operatore team]**: il ruolo [!UICONTROL operatore] consente agli utenti di visualizzare i dati di esecuzione e di modificare lo stato &quot;Attivo&quot; degli scenari.
* **[!UICONTROL Membro con restrizioni team]**: la funzionalità per questo ruolo non è attualmente disponibile e sarà disponibile prossimamente. Non è consigliabile assegnare gli utenti a questo ruolo in questo momento.

Per informazioni sulle azioni specifiche disponibili per gli utenti in ogni ruolo del team, vedere [Ruoli organizzazione e team](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### Gestione team

* [Creare un team](#create-a-team)
* [Imposta opzioni di notifica team](#set-team-notification-options)

#### Creare un team

I proprietari e gli amministratori dell’organizzazione possono creare dei team.

Per creare un team:

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Organizzazione]**
1. Selezionare la scheda **[!UICONTROL Team]**.
1. Fai clic su **[!UICONTROL Aggiungi un nuovo team]** nell&#39;elenco dei team.
1. Immettere un nome per il nuovo team e fare clic su **Aggiungi**.

#### Imposta opzioni di notifica team

>[!NOTE]
>
>Se l’organizzazione è stata spostata in Unified Shell, riceverai notifiche tramite l’area Notifiche di Adobe. Per visualizzare le notifiche nell’area Notifiche di Adobe, è necessario utilizzare l’esperienza Unified Shell.
>
>Per utilizzare l’esperienza Unified Shell, inclusa l’area Notifiche dell’Adobe, fai clic sul pulsante Prova nuova interfaccia utente di Fusion in Esperienza unificata nella parte superiore della pagina. Questo pulsante è disponibile solo se l’organizzazione è stata spostata in Unified Shell.
>
>Per ulteriori informazioni, vedere [Accedere alle notifiche](/help/quicksilver/workfront-fusion/fusion-in-admin-console/fusion-unified-experience.md#access-your-notifications) in [!DNL Adobe Unified Experience] per [!DNL Workfront Fusion].

Le opzioni di notifica e-mail sono impostate a livello di team.

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Team]**
1. Selezionare la scheda **[!UICONTROL Opzioni di notifica]**.
1. Abilitare le notifiche che si desidera vengano ricevute dal team.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">'[!UICONTROL Warning in esecuzione scenario]'</td> 
      <td> <p>Ricevi un’e-mail quando viene visualizzato un avviso in un’esecuzione di uno scenario</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Errori nell'esecuzione dello scenario]</td> 
      <td>Ricevi un’e-mail quando si verifica un errore in un’esecuzione di uno scenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Disattivazione scenario]</p> </td> 
      <td><p>Ricevi un’e-mail quando uno scenario si disattiva.</p><p><b>Nota:</b> ricevi una notifica relativa alla disattivazione dello scenario solo quando lo scenario è stato disattivato automaticamente a causa di errori. Non ricevi notifiche su scenari disattivati manualmente.</p><p>In alcuni casi, uno scenario potrebbe essere disattivato dal team di progettazione [!DNL Workfront Fusion] perché causa problemi di prestazioni o di altro tipo. In questi casi, non si ricevono notifiche in [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

Le modifiche alle opzioni di notifica vengono salvate automaticamente

#### Passa da un team all’altro

È possibile far parte di più team in Fusion. Poiché i team non condividono le risorse, potrebbe essere necessario cambiare team per accedere a scenari specifici o ad altre risorse.

Se la tua organizzazione non fa parte dell’esperienza unificata di Adobe, puoi cambiare team facendo clic sul nome del team nell’area di navigazione a sinistra, quindi selezionando un team dal menu a discesa.

Se il tuo team fa parte dell’esperienza unificata di Adobe, puoi selezionare un nuovo team facendo clic sul nome del team nell’intestazione e selezionando un team dal menu a discesa. Questa opzione è disponibile in tutte le pagine specifiche di un determinato team, ad esempio la pagina di uno scenario o la pagina Connessioni.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->