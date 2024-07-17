---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Configurare POP in Microsoft Exchange
description: Un account di posta elettronica POP in [!DNL Microsoft Exchange]  è disabilitato.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

# Configura POP in [!DNL Microsoft Exchange]

## Problema

Un account di posta elettronica POP in [!DNL Microsoft Exchange] è disabilitato.

## Soluzione

Prima di dedicare del tempo alla risoluzione del problema, assicurati che l’account POP dell’utente sia configurato correttamente. Se si continuano a riscontrare problemi dopo aver confermato che l&#39;account POP è configurato correttamente, contattare il supporto di [!DNL Microsoft] o uno dei loro partner per ulteriore assistenza.

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
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore [!DNL Workfront]. Per ulteriori informazioni, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configura POP in [!DNL Microsoft Exchange]

>[!NOTE]
>
>I passaggi seguenti possono essere utilizzati come guida generale per la configurazione di POP in [!DNL Microsoft Exchange] per un sistema di produzione [!DNL Workfront]. I passaggi possono variare in modo significativo a seconda della versione di Exchange o delle modifiche apportate al codice da Microsoft.

1. Avviare e abilitare il servizio POP3 sul server Exchange 2010.

   >[!NOTE]
   >
   >Per impostazione predefinita, il servizio POP3 non è avviato.

   1. Avvia Server Manager di [!DNL Microsoft].
   1. Accedi a: **[!UICONTROL Server Manager]** > **[!UICONTROL Configurazione]** >**[!UICONTROL Windows Firewall con sicurezza avanzata]** > **[!UICONTROL Servizi]**.

   1. Fare clic con il pulsante destro del mouse su **[!DNL Microsoft Exchange]POP3**, quindi scegliere **[!UICONTROL Proprietà]**.

   1. (Condizionale) Per garantire l&#39;avvio automatico del servizio POP, nella scheda **[!UICONTROL Generale]** impostare il tipo **[!UICONTROL Avvio]** su [!UICONTROL Automatico].

1. Configurare POP3 per il server.

   1. Avviare la console di gestione [!DNL Microsoft Exchange].
   1. Naviga: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configurazione server]** > **[!UICONTROL Accesso client]**.

   1. Scegliere **[!UICONTROL POP3]**.

      POP3 è incluso nell&#39;elenco delle schede [!UICONTROL POP3] e [!UICONTROL IMAP4].

   1. Sul lato destro in **[!UICONTROL Azioni]**, seleziona **[!UICONTROL POP3]**, quindi scegli **[!UICONTROL Proprietà]**.

   1. Fai clic su **[!UICONTROL Proprietà POP3]**, quindi apri la scheda **[!UICONTROL Associazione]**.

      Vengono visualizzati tutti gli indirizzi IP disponibili e i numeri di porta configurati per il server POP3. La casella superiore mostra la voce Non crittografato, mentre la casella inferiore mostra l’IP e le porte per le connessioni SSL/TLS.

   1. Fai clic su **[!UICONTROL POP3 Properties]**, quindi apri la scheda **[!UICONTROL Authentication]**.

   1. **[!UICONTROL Seleziona accesso protetto]**.

      È necessaria una connessione TLS per consentire al client di eseguire l&#39;autenticazione al server.

1. Attiva o consente agli utenti di connettersi al POP.

   1. Avviare la console di gestione [!DNL Microsoft Exchange].
   1. Naviga: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configurazione destinatario]** > **[!UICONTROL Cassetta postale]**.

      Viene visualizzato un elenco di cassette postali o utenti.

   1. Evidenziare l&#39;indirizzo e-mail utilizzato in [!DNL Workfront].
   1. Sul lato destro in **[!UICONTROL Azioni]**, seleziona **[!UICONTROL Proprietà]**, quindi apri la scheda **[!UICONTROL Caratteristiche cassetta postale]**.

   1. (Condizionale) Se POP3 è disabilitato, fare clic su **[!UICONTROL POP3]**, quindi su **[!UICONTROL Abilita]**.

      Viene visualizzato un elenco di cassette postali o utenti.

1. Configurare i connettori di ricezione.

   1. Avviare la console di gestione [!DNL Microsoft Exchange].
   1. Naviga: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configurazione server]** > **[!UICONTROL Trasporto Hub]**.

      Viene visualizzato un elenco di connettori di ricezione.

   1. Verificare che il connettore di ricezione *Client* *EX01* sia abilitato.

      Dove *Client* *EX01* è il nome del server Exchange.

   1. Seleziona *Client EX01*, quindi a destra in **[!UICONTROL Azioni]**, seleziona **[!UICONTROL Proprietà]**.

   1. Apri la scheda **[!UICONTROL Autenticazione]**, quindi assicurati che **[!UICONTROL Transport Layer Security (TLS)]** sia selezionato.

      >[!NOTE]
      >
      >Per disporre dell&#39;autenticazione di base, potrebbe essere necessario avviare l&#39;autenticazione TLS e l&#39;autenticazione integrata di Windows.
