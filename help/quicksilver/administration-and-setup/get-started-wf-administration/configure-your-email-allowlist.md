---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurare l’inserire nell'elenco Consentiti e-mail
description: Se la tua organizzazione utilizza il piano WorkfrontEnterprise, puoi creare un inserire nell'elenco Consentiti e-mail Workfront per controllare quali domini e-mail possono accettare e-mail da Workfront e quali domini e-mail possono trovarsi nell’indirizzo e-mail specificato dagli utenti nel loro profilo utente. Questo è utile se la politica di sicurezza della tua organizzazione limita l’invio da parte degli utenti di dati archiviati in Workfront ad indirizzi e-mail esterni. Puoi includere solo i domini aziendali interni nell’inserire nell'elenco Consentiti per garantire che questa policy sia rispettata.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Configurare l’inserire nell&#39;elenco Consentiti e-mail

Se la tua organizzazione utilizza il piano WorkfrontEnterprise, puoi creare un inserire nell&#39;elenco Consentiti e-mail Workfront per controllare:

* Quali domini e-mail possono accettare e-mail da Workfront.
* Quali domini e-mail possono essere inclusi nell’indirizzo e-mail specificato dagli utenti nel loro profilo utente.

Questo è utile se la politica di sicurezza della tua organizzazione limita l’invio da parte degli utenti di dati archiviati in Workfront ad indirizzi e-mail esterni. Puoi includere solo i domini aziendali interni nell’inserire nell&#39;elenco Consentiti per garantire che questa policy sia rispettata.

>[!IMPORTANT]
>
>Il team IT deve assicurarsi che le e-mail in arrivo da `notifications@my.workfront.com` non è bloccato nel sistema della tua organizzazione.
>
>Tutte le e-mail da Workfront vengono inviate da tale indirizzo per aumentare la consegna e-mail di successo ed eliminare lo spoofing delle e-mail. Ciò include sia gli avvisi automatizzati che la comunicazione utente-utente.
>
>Ad esempio, la riga Da in un&#39;e-mail Workfront che ricevi da un utente chiamato Joan Harris apparirebbe così:
>
```
>Joan Harris <notifications@my.workfront.com>
>```

Per informazioni sulla configurazione del firewall dell’organizzazione per aprire la comunicazione tra l’ambiente e i server Adobe Workfront, consulta [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisiti di accesso

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront. Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Altri inserire nell&#39;elenco Consentiti

Se la tua organizzazione dispone del piano Enterprise, puoi configurare un inserire nell&#39;elenco Consentiti IP Adobe Workfront che limiti l’accesso a Workfront a 45 indirizzi IP o intervalli di indirizzi IP specificati. Questo fornisce un ulteriore livello di sicurezza per l&#39;applicazione Workfront. Per ulteriori informazioni, consulta [Limitare l’accesso ad Adobe Workfront per indirizzo IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

Inoltre, se il firewall o il server di posta elettronica sono configurati per consentire l’accesso solo a determinati fornitori, è necessario aggiungere alcuni indirizzi IP al relativo inserire nell&#39;elenco Consentiti. Questo apre la comunicazione tra l’ambiente e i server Adobe Workfront. Per informazioni, consulta [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configurare l’inserire nell&#39;elenco Consentiti e-mail

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Sistema** > **Informazioni cliente**.

1. In **Inserire nell&#39;elenco Consentiti e-mail** sezione , seleziona **Abilita Inserire nell&#39;elenco Consentiti dominio**, quindi fai clic su **Aggiungi dominio**.
1. Nella casella visualizzata, digita un dominio che desideri consentire, ad esempio `ourcompany.com`, quindi fai clic su **Aggiungi dominio**.

1. Ripeti il passaggio precedente per aggiungere altri domini che desideri consentire.
1. Al termine, fai clic su **Salva**.
