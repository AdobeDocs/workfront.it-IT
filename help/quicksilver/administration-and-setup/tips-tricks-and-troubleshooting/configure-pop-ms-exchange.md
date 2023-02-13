---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Configurare POP in Microsoft Exchange
description: Un account e-mail POP in [!DNL Microsoft Exchange] è disabilitato.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Configura POP in [!DNL Microsoft Exchange]

## Problema

Un account e-mail POP in [!DNL Microsoft Exchange] è disabilitato.

## Soluzione

Prima di risolvere il problema, assicurati che l’account POP dell’utente sia configurato correttamente. Se si verificano ancora problemi dopo aver confermato che l’account POP è configurato correttamente, contattare [!DNL Microsoft] Supporto o uno dei loro partner per ulteriore assistenza.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configura POP in [!DNL Microsoft Exchange]

>[!NOTE]
>
>I seguenti passaggi possono essere utilizzati come guida generale per la configurazione di POP in [!DNL Microsoft Exchange] per una produzione [!DNL Workfront] sistema. I passaggi possono variare notevolmente a seconda della versione di Exchange o delle modifiche al codice apportate da Microsoft.

1. Avviare e abilitare il servizio POP3 sul server Exchange 2010.

   >[!NOTE]
   >
   >Per impostazione predefinita, il servizio POP3 non viene avviato.

   1. Inizio [!DNL Microsoft]Server Manager di .
   1. Naviga: **[!UICONTROL Server Manager]** > **[!UICONTROL Configurazione]** >**[!UICONTROL Windows Firewall con protezione avanzata]** > **[!UICONTROL Servizi]**.

   1. Fai clic con il pulsante destro del mouse **[!DNL Microsoft Exchange]POP3**, quindi fai clic su **[!UICONTROL Proprietà]**.

   1. (Condizionale) Per garantire l&#39;avvio automatico del servizio POP, nella **[!UICONTROL Generale]** imposta la **[!UICONTROL Avvio]** digitare [!UICONTROL Automatico].

1. Configurare POP3 per il server.

   1. Avvia la [!DNL Microsoft Exchange] Console di gestione.
   1. Naviga: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configurazione server]** > **[!UICONTROL Accesso client]**.

   1. Scegli **[!UICONTROL POP3]**.

      POP3 è nell&#39;elenco [!UICONTROL POP3] e [!UICONTROL IMAP4] schede.

   1. Sul lato destro sotto **[!UICONTROL Azioni]**, seleziona **[!UICONTROL POP3]**, quindi scegli **[!UICONTROL Proprietà]**.

   1. Fai clic su **[!UICONTROL Proprietà POP3]**, quindi apri la **[!UICONTROL Binding]** scheda .

      Vengono visualizzati tutti gli indirizzi IP disponibili e i numeri di porta configurati per la visualizzazione del server POP3. La casella in alto mostra i non crittografati e la casella in basso mostra gli IP e le porte per le connessioni SSL/TLS.

   1. Fai clic su **[!UICONTROL Proprietà POP3]**, quindi apri la **[!UICONTROL Autenticazione]** scheda .

   1. **[!UICONTROL Seleziona protetto]** accesso.

      Per l’autenticazione del client al server è necessaria una connessione TLS.

1. Abilitare o consentire agli utenti di connettersi a POP.

   1. Avvia la [!DNL Microsoft Exchange] Console di gestione.
   1. Naviga: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configurazione destinatario]** > **[!UICONTROL Cassetta postale]**.

      Viene visualizzato un elenco di cassette postali o utenti.

   1. Evidenzia l’e-mail utilizzata in [!DNL Workfront].
   1. Sul lato destro sotto **[!UICONTROL Azioni]**, seleziona **[!UICONTROL Proprietà]**, quindi apri la **[!UICONTROL Caratteristiche della cassetta postale]** scheda .

   1. (Condizionale) Se POP3 è disattivato, fare clic su **[!UICONTROL POP3]**, quindi fai clic su **[!UICONTROL Abilita]**.

      Viene visualizzato un elenco di cassette postali o utenti.

1. Configura i connettori di ricezione.

   1. Inizio [!DNL Microsoft Exchange] Console di gestione.
   1. Naviga: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configurazione server]** > **[!UICONTROL Trasporto Hub]**.

      Viene visualizzato un elenco di connettori di ricezione.

   1. Conferma il connettore di ricezione *Client* *EX01* è abilitato.

      Dove *Client* *EX01* è il nome del server Exchange.

   1. Seleziona *Client EX01*, poi a destra sotto **[!UICONTROL Azioni]**, seleziona **[!UICONTROL Proprietà]**.

   1. Apri **[!UICONTROL Autenticazione]** , quindi assicurati **[!UICONTROL Transport Layer Security (TLS)]** è controllata.

      >[!NOTE]
      >
      >Per poter disporre dell’autenticazione di base, potrebbe essere necessario avviare TLS e l’autenticazione integrata di Windows.
