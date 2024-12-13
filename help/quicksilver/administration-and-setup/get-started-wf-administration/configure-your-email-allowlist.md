---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurare Il Inserisco nell'elenco Consentiti Di Email Di
description: Se l'organizzazione utilizza il piano WorkfrontEnterprise, è possibile creare un Workfront di gestione delle e-mail di inserire nell'elenco Consentiti per controllare quali domini e-mail sono autorizzati ad accettare e-mail da Workfront e quali domini e-mail possono trovarsi nell'indirizzo e-mail specificato dagli utenti nel loro profilo utente. Questa opzione è utile se i criteri di sicurezza dell'organizzazione impediscono agli utenti di inviare i dati memorizzati in Workfront a indirizzi e-mail esterni. Per assicurarsi che tali criteri vengano rispettati, è possibile includere nel elenco Consentiti di gestione della sicurezza solo i domini aziendali interni.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: 937965ad495453e185504d53f9d9c88c3cd7e201
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Configurare la inserisce nell&#39;elenco Consentiti di e-mail per l’e-mail

Se l&#39;organizzazione utilizza il piano aziendale di Workfront, è possibile creare un inserisco nell&#39;elenco Consentiti di gestione delle e-mail di Workfront per controllare:

* Quali domini e-mail possono accettare e-mail da Workfront?
* Quali domini e-mail possono trovarsi nell’indirizzo e-mail specificato dagli utenti nel loro profilo utente.

Questa opzione è utile se i criteri di sicurezza dell&#39;organizzazione impediscono agli utenti di inviare i dati memorizzati in Workfront a indirizzi e-mail esterni. Per assicurarsi che tali criteri vengano rispettati, è possibile includere nel elenco Consentiti di gestione della sicurezza solo i domini aziendali interni.

>[!IMPORTANT]
>
>Il tuo team IT deve assicurarsi che le e-mail in arrivo da `notifications@my.workfront.com` non siano bloccate nel sistema della tua organizzazione.
>
>Tutte le e-mail provenienti da Workfront vengono inviate da tale indirizzo per aumentare la consegna delle e-mail e per eliminare lo spoofing delle e-mail. Ciò include sia gli avvisi automatici che la comunicazione utente-utente.
>
>Ad esempio, la riga Da di un&#39;e-mail Workfront ricevuta da un utente di nome Joan Harris sarà simile alla seguente:
>`Joan Harris <notifications@my.workfront.com>`

Per informazioni sulla configurazione del firewall dell&#39;organizzazione per aprire la comunicazione tra l&#39;ambiente e i server Adobe Workfront, vedere [Configurare il inserisco nell&#39;elenco Consentiti di del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront. Per ulteriori informazioni, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Inserire nell&#39;elenco Consentiti Altri

Se la tua organizzazione dispone del piano Enterprise, puoi configurare un Adobe Workfront di inserire nell&#39;elenco Consentiti IP che limita l’accesso a Workfront a 75 indirizzi IP o intervalli di indirizzi IP specificati. Questo fornisce un ulteriore livello di sicurezza per l’applicazione Workfront. Per ulteriori informazioni, vedere [Limitare l&#39;accesso ad Adobe Workfront per indirizzo IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

Inoltre, se il firewall o il server di posta è configurato in modo da consentire l&#39;accesso solo a determinati fornitori, è necessario aggiungere determinati indirizzi IP al relativo inserisco nell&#39;elenco Consentiti di. Questo apre la comunicazione tra l’ambiente e i server Adobe Workfront. Per ulteriori informazioni, vedere [Configurare il inserisco nell&#39;elenco Consentiti di configurazione del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configurare la inserisce nell&#39;elenco Consentiti di e-mail per l’e-mail

{{step-1-to-setup}}

1. Fai clic su **Sistema** > **Informazioni cliente**.
1. Nella sezione **Inserisce nell&#39;elenco Consentiti messaggio di posta elettronica**, seleziona **Abilita il dominio di cui è stato eseguito il Inserisco nell&#39;elenco Consentiti di**, quindi fai clic su **Aggiungi dominio**.
1. Nella casella visualizzata digitare un dominio che si desidera consentire, ad esempio `ourcompany.com`, quindi fare clic su **Aggiungi dominio**.
1. Ripeti il passaggio precedente per aggiungere altri domini che desideri consentire.
1. Al termine, fare clic su **Salva**.
