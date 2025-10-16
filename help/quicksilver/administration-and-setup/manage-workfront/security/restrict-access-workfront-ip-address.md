---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Limita l’accesso ad Adobe Workfront per indirizzo IP
description: È possibile configurare un Adobe Workfront di di inserire nell'elenco Consentiti che limiti l’accesso a Workfront a 75 indirizzi IP o intervalli di indirizzi IP specificati. Questo fornisce un ulteriore livello di sicurezza per l’applicazione Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 22ae8b489c63ba6eea1472cf415f95e375a94773
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 2%

---

# Limita l’accesso ad Adobe Workfront per indirizzo IP

<!--
>[!IMPORTANT]
>
>This functionality is not currently available to organizations that have been onboarded to the Adobe Admin Console. It will be available in the Adobe Admin Console in a future release. -->

È possibile configurare un Adobe Workfront di di inserire nell&#39;elenco Consentiti che limiti l’accesso a Workfront a 75 indirizzi IP o intervalli di indirizzi IP specificati. Questo fornisce un ulteriore livello di sicurezza per l’applicazione Workfront.

Questi indirizzi IP o intervalli di indirizzi IP devono essere forniti dall&#39;amministratore di rete.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Standard</p><p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

   Puoi aggiungere fino a 75 indirizzi o intervalli.

1. Fai clic su **Salva.**
