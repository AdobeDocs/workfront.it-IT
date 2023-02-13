---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Organizzazioni e team Adobe Workfront Fusion
description: Le funzionalità di Adobe Workfront Fusion Organization e Team consentono alle aziende di controllare l'accesso agli scenari e ad altre funzionalità di Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] organizzazioni e team

[!DNL Adobe Workfront Fusion]Le funzionalità di organizzazione e team consentono alle aziende di controllare l&#39;accesso a scenari e altre caratteristiche all&#39;interno di Fusion.

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

<p>**Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] licenze</a></p>


## Organizzazioni

[!DNL Workfront Fusion] gli utenti appartengono a un&#39;organizzazione. Le [!DNL Fusion] La licenza determina quanti scenari e connettori attivi sono disponibili nell’organizzazione.

[!DNL Fusion] la licenza determina il numero di scenari attivi e app attive disponibili per un&#39;organizzazione. [!DNL Fusion] visualizza il conteggio &quot;Scenari attivi&quot; e &quot;App attive&quot; correnti nel dashboard dell&#39;organizzazione.

* [Ruoli dell&#39;organizzazione](#organization-roles)
* [Invitare gli utenti a un&#39;organizzazione](#inviting-users-to-an-organization)

### Ruoli dell&#39;organizzazione

Un utente ha uno dei seguenti ruoli in un&#39;organizzazione:

* **[!UICONTROL Proprietario]**: Il proprietario dispone di tutte le autorizzazioni disponibili nell&#39;organizzazione.
* **[!UICONTROL Amministratore]**: Il ruolo di amministratore consente a un utente di creare e gestire team e utenti per l&#39;organizzazione.
* **[!UICONTROL Membro]**: I membri possono utilizzare [!DNL Workfront Fusion] ma non è in grado di apportare modifiche organizzative.
* **[!UICONTROL Ragioniere]**: Un ruolo contabile consente solo agli utenti di visualizzare le informazioni sulla licenza nel dashboard dell&#39;organizzazione.
* **[!UICONTROL Sviluppatore di app]**: La funzionalità per questo ruolo non è al momento disponibile e verrà resa disponibile prossimamente. Al momento non è consigliabile assegnare gli utenti a questo ruolo.

### Invitare gli utenti a un&#39;organizzazione

Per impostazione predefinita, un proprietario organizzazione (o utente autorizzato) può invitare un’altra persona a partecipare alla propria organizzazione.

Per invitare un utente a unirsi a un&#39;organizzazione:

1. Fai clic su **[!UICONTROL Modifica dettagli]** nell&#39;angolo superiore destro dello schermo.
1. Seleziona **[!UICONTROL Invitare un nuovo utente]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. Compila l’indirizzo e-mail e il nome dell’utente.
1. Seleziona un ruolo per l’utente. Per ulteriori informazioni sui ruoli, consulta [Ruoli dell&#39;organizzazione](#organization-roles) in questo documento.
1. (Facoltativo) Aggiungi una nota. Questa nota viene visualizzata nell’e-mail di invito che l’utente riceve.
1. Fai clic su **[!UICONTROL Salva]**.

[!DNL Fusion] invia un’e-mail con un invito all’organizzazione specifica e un [!UICONTROL Accettare Il Ruolo] pulsante .

![](assets/accept-the-role.png)

Quando il destinatario fa clic sul pulsante , viene reindirizzato alla pagina dell’invito, dove può accettare l’invito.

L’invito scade in un giorno.

>[!NOTE]
>
>Se l’utente è nuovo a [!DNL Fusion], [!DNL Fusion] crea automaticamente un account e invia un&#39;e-mail con una password temporanea, indirizzando il nuovo utente all&#39;accesso e alla modifica della password.

## Team

I team sono gruppi di utenti che condividono l’accesso a risorse specifiche. Tali risorse possono comprendere:

* Scenari
* Connessioni
* Webhook
* Chiavi
* Archiviazione dati
* Strutture dati
* Impostazioni delle notifiche e-mail

>[!NOTE]
>
>Poiché i team controllano l’accesso alle risorse, a volte è utile che un team abbia un solo membro. Ad esempio, gli utenti in formazione possono creare connessioni al proprio individuo [!DNL Google] conti. Tutti i membri del team potranno inoltre connettersi al singolo [!DNL Google] quindi in questo caso è meglio che l’utente sia l’unico membro di un team di formazione.

Le organizzazioni possono avere il numero di team necessario e gli utenti possono appartenere a uno o più team.

Gli utenti possono selezionare il proprio team dall’elenco a discesa nel pannello di navigazione a sinistra. Gli utenti vedono solo i team di cui sono membri. Selezionando un team, un utente potrà accedere alle risorse del team.

* [Ruoli team](#team-roles)
* [Gestione team](#team-management)

### Ruoli team

Un utente ha uno dei seguenti ruoli in ciascuno dei propri team:

* **[!UICONTROL Amministratore del team]**: Oltre alle funzionalità degli altri ruoli del team, il ruolo Amministratore consente all’utente di aggiungere, rimuovere o modificare il ruolo di un membro del team.
* **[!UICONTROL Membro del team]**: Il ruolo di membro del team consente agli utenti di creare ed eseguire scenari.
* **[!UICONTROL Monitoraggio del team]**: La [!UICONTROL monitoraggio] Il ruolo consente agli utenti di accedere alle informazioni di esecuzione per gli scenari, ma non possono progettare scenari o modificare il loro stato &quot;Attivo&quot;.
* **[!UICONTROL Operatore team]**: La [!UICONTROL operatore] Il ruolo consente agli utenti di visualizzare i dati di esecuzione e di modificare lo stato &quot;Attivo&quot; degli scenari.
* **[!UICONTROL Membro con restrizioni del team]**: La funzionalità per questo ruolo non è al momento disponibile e verrà resa disponibile prossimamente. Al momento non è consigliabile assegnare gli utenti a questo ruolo.

### Gestione team

* [Creare un team](#create-a-team)
* [Imposta opzioni di notifica del team](#set-team-notification-options)

#### Creare un team

I proprietari e gli amministratori dell&#39;organizzazione possono creare dei team.

Per creare un team:

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Organizzazione]**
1. Seleziona la **[!UICONTROL Team]** scheda .
1. Fai clic su **[!UICONTROL Aggiungi un nuovo team]** nell’elenco delle squadre.
1. Immettere un nome per il nuovo team e fare clic su **Aggiungi**.

#### Imposta opzioni di notifica del team

Le opzioni di notifica e-mail sono impostate a livello di team.

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Team]**
1. Seleziona la **[!UICONTROL Opzioni di notifica]** scheda .
1. Abilita le notifiche che desideri ricevere dal team.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">'[!UICONTROL Avviso nell'esecuzione dello scenario''</td> 
      <td> <p>Ricevi un messaggio e-mail quando è presente un avviso in un’esecuzione di uno scenario</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Errori nell'esecuzione dello scenario]</td> 
      <td>Ricevi un'e-mail quando si verifica un errore in uno scenario eseguito.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Disattivazione dello scenario]</p> </td> 
      <td><p>Ricevi un’e-mail quando uno scenario si disattiva.</p><p><b>Nota:</b> Viene visualizzata una notifica sulla disattivazione dello scenario solo quando lo scenario è stato disattivato automaticamente a causa di errori. Non si ricevono notifiche su scenari disattivati manualmente.</p><p>In alcuni casi, uno scenario potrebbe essere disattivato dal [!DNL Workfront Fusion] team di progettazione perché lo scenario sta causando prestazioni o altri problemi. In questi casi, non ricevi notifiche in [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

Modifiche alle opzioni di notifica salvate automaticamente

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->