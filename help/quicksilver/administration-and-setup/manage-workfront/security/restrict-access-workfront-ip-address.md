---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Limitare l’accesso ad Adobe Workfront per indirizzo IP
description: Puoi configurare un inserire nell'elenco Consentiti IP Adobe Workfront che limiti l’accesso a Workfront a 45 indirizzi IP o intervalli di indirizzi IP specificati. Questo fornisce un ulteriore livello di sicurezza per l'applicazione Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 1%

---

# Limitare l’accesso ad Adobe Workfront per indirizzo IP

Puoi configurare un inserire nell&#39;elenco Consentiti IP Adobe Workfront che limiti l’accesso a Workfront a 45 indirizzi IP o intervalli di indirizzi IP specificati. Questo fornisce un ulteriore livello di sicurezza per l&#39;applicazione Workfront.

Gli indirizzi IP o gli intervalli di indirizzi IP devono essere forniti dall’amministratore di rete.

## Requisiti di accesso

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Altri inserire nell&#39;elenco Consentiti

Se il firewall o il server di posta elettronica è configurato per consentire l’accesso solo a determinati fornitori, è necessario aggiungere alcuni indirizzi IP al relativo inserire nell&#39;elenco Consentiti. Questo apre la comunicazione tra l’ambiente e i server Adobe Workfront. Per informazioni, consulta [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Inoltre, se la tua organizzazione utilizza il piano Enterprise, puoi configurare l’inserire nell&#39;elenco Consentiti e-mail di Workfront per controllare quali domini e-mail possono accettare e-mail da Workfront e quali domini e-mail possono essere inclusi nell’indirizzo e-mail specificato dagli utenti nel loro profilo utente Workfront. Per ulteriori informazioni, consulta [Configurare l’inserire nell&#39;elenco Consentiti e-mail](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## Aggiunta di indirizzi IP all’inserire nell&#39;elenco Consentiti

Dopo aver aggiunto gli indirizzi IP all’inserire nell&#39;elenco Consentiti Workfront, solo questi possono essere utilizzati per accedere ad Workfront. Gli utenti che tentano di accedere a Workfront da un altro indirizzo IP ricevono un messaggio di errore che indica che l’indirizzo IP è bloccato.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Sistema** > **Informazioni sul cliente.**

1. In **inserire nell&#39;elenco Consentiti IP** sezione , seleziona **Abilita l&#39;inserire nell&#39;elenco Consentiti IP.**

   Questa opzione è disabilitata per impostazione predefinita.

1. Specifica l&#39;indirizzo IP che stai utilizzando per accedere al sistema Workfront.

   Oppure

   Specifica un intervallo di indirizzi IP che include quello attualmente utilizzato per accedere al sistema Workfront.

   L’indirizzo IP utilizzato per accedere a Workfront deve essere aggiunto all’inserire nell&#39;elenco Consentiti prima che l’inserire nell&#39;elenco Consentiti sia abilitato.

1. Fai clic su **Aggiungi intervallo IP,** quindi specifica l’indirizzo IP o l’intervallo di indirizzi IP a cui desideri poter accedere in Workfront.
1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri indirizzi IP o intervalli di indirizzi IP.

   Puoi aggiungere fino a 45 indirizzi o intervalli.

1. Fai clic su **Salva.**
