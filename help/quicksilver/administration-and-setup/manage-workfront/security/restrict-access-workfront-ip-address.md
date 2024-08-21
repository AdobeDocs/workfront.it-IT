---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Limita l’accesso ad Adobe Workfront per indirizzo IP
description: È possibile configurare un Adobe Workfront di di inserire nell'elenco Consentiti che limiti l’accesso a Workfront a 45 indirizzi IP o intervalli di indirizzi IP specificati. Questo fornisce un ulteriore livello di sicurezza per l’applicazione Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 2%

---

# Limita l’accesso ad Adobe Workfront per indirizzo IP

È possibile configurare un Adobe Workfront di di inserire nell&#39;elenco Consentiti che limiti l’accesso a Workfront a 45 indirizzi IP o intervalli di indirizzi IP specificati. Questo fornisce un ulteriore livello di sicurezza per l’applicazione Workfront.

Questi indirizzi IP o intervalli di indirizzi IP devono essere forniti dall&#39;amministratore di rete.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Enterprise</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Inserire nell&#39;elenco Consentiti Altri

Se il firewall o il server di posta è configurato in modo da consentire l&#39;accesso solo a determinati fornitori, è necessario aggiungere determinati indirizzi IP al relativo inserisco nell&#39;elenco Consentiti di posta elettronica. Questo apre la comunicazione tra l’ambiente e i server Adobe Workfront. Per ulteriori informazioni, vedere [Configurare il inserisco nell&#39;elenco Consentiti di configurazione del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Inoltre, se la tua organizzazione utilizza il piano Enterprise, puoi configurare il Workfront di gestione delle e-mail di inserire nell&#39;elenco Consentiti per controllare quali domini e-mail sono autorizzati ad accettare e-mail da Workfront e quali domini e-mail possono trovarsi nell’indirizzo e-mail specificato dagli utenti nel profilo utente di Workfront. Per ulteriori informazioni, consulta [Configurare il tuo inserisco nell&#39;elenco Consentiti di e-mail di accesso ai messaggi di posta elettronica](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## Aggiunta di indirizzi IP al inserisco nell&#39;elenco Consentiti di

Dopo l&#39;aggiunta degli indirizzi IP al Workfront di di inserire nell&#39;elenco Consentiti, è possibile utilizzare solo tali indirizzi IP per accedere a Workfront. Gli utenti che tentano di accedere a Workfront da un altro indirizzo IP ricevono un messaggio di errore che indica che il loro indirizzo IP è bloccato.

{{step-1-to-setup}}

1. Fai clic su **Sistema** > **Informazioni cliente**

1. Nella sezione **inserisco nell&#39;elenco Consentiti IP** selezionare **Abilita inserisco nell&#39;elenco Consentiti IP.**

   Questa opzione è disabilitata per impostazione predefinita.

1. Specificare l&#39;indirizzo IP attualmente utilizzato per accedere al sistema Workfront.

   Oppure

   Specifica un intervallo di indirizzi IP che includa quello attualmente in uso per accedere al sistema Workfront.

   L&#39;indirizzo IP che si sta utilizzando per accedere a Workfront deve essere aggiunto al inserisco nell&#39;elenco Consentiti di prima di abilitare il inserisco nell&#39;elenco Consentiti.

1. Fare clic su **Aggiungi intervallo IP,** quindi specificare l&#39;indirizzo IP o l&#39;intervallo di indirizzi IP a cui si desidera accedere in Workfront.
1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri indirizzi IP o intervalli di indirizzi IP.

   Puoi aggiungere fino a 45 indirizzi o intervalli.

1. Fai clic su **Salva.**
