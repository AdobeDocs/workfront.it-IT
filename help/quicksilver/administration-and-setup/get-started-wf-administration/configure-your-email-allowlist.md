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
source-git-commit: 15ea03bf586054f7ef421f8cacede6f42835a6e4
workflow-type: tm+mt
source-wordcount: '399'
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
>>`Joan Harris <notifications@my.workfront.com>`

Per informazioni sulla configurazione del firewall dell&#39;organizzazione per aprire la comunicazione tra l&#39;ambiente e i server Adobe Workfront, vedere [Configurare il inserisco nell&#39;elenco Consentiti di del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Standard</p> <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Devi essere un amministratore di Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Inserire nell&#39;elenco Consentiti Altri

Se il firewall o il server di posta è configurato in modo da consentire l&#39;accesso solo a determinati fornitori, è necessario aggiungere determinati indirizzi IP al relativo inserisco nell&#39;elenco Consentiti di posta elettronica. Questo apre la comunicazione tra l’ambiente e i server Adobe Workfront. Per ulteriori informazioni, vedere [Configurare il inserisco nell&#39;elenco Consentiti di configurazione del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configurare la inserisce nell&#39;elenco Consentiti di e-mail per l’e-mail

{{step-1-to-setup}}

1. Fai clic su **Sistema** > **Informazioni cliente**.
1. Nella sezione **Inserisce nell&#39;elenco Consentiti messaggio di posta elettronica**, seleziona **Abilita il dominio di cui è stato eseguito il Inserisco nell&#39;elenco Consentiti di**, quindi fai clic su **Aggiungi dominio**.
1. Nella casella visualizzata digitare un dominio che si desidera consentire, ad esempio `ourcompany.com`, quindi fare clic su **Aggiungi dominio**.
1. Ripeti il passaggio precedente per aggiungere altri domini che desideri consentire.
1. Al termine, fare clic su **Salva**.
