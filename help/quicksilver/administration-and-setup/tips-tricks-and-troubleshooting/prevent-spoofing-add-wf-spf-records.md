---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Impedisci spoofing e aggiunta [!DNL Adobe Workfront] Record SPF
description: Se gli utenti non ricevono [!DNL Adobe Workfront] notifiche e-mail, devi aggiungere [!DNL Workfront] Record SPF nel firewall. Per aggiungere record SPF è necessario collaborare con il team IT.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Impedisci spoofing e aggiunta [!DNL Adobe Workfront] Record SPF

## Problema

Se gli utenti non ricevono [!DNL Adobe Workfront] notifiche e-mail, devi aggiungere [!DNL Workfront] Record SPF nel firewall. Per aggiungere record SPF è necessario collaborare con il team IT.

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
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Soluzione

Se hai già aggiunto gli indirizzi IP al inserisco nell&#39;elenco Consentiti di per l’ambiente di produzione come descritto in [Configurare il inserisco nell&#39;elenco Consentiti di configurazione del firewall per l’accesso a un sistema di protezione da attacchi di tipo](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) e gli utenti non ricevono ancora le e-mail:

1. Aggiungi il seguente record SPF al firewall:

   *spf.workfront.com*

   Questo aggiunge automaticamente tutto [!DNL Workfront] Indirizzi IP al tuo di inserire nell&#39;elenco Consentiti sul firewall e consente a tutti i filtri anti-spam (che utilizzano i record SPF) di convalidare [!DNL Workfront] server come mittenti validi per il dominio.

   >[!NOTE]
   >
   > Un record SPF è un record TXT che fa parte di un file di zona DNS. La modifica del file della zona DNS non è supportata.

1. È necessario specificare il tipo di record SPF da configurare. Di seguito sono riportati i tipi validi di record SPF:

   * tutti (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * esiste (https://dmarcian.com/spf-syntax-table/#exists)
   * includi (https://dmarcian.com/spf-syntax-table/#include)

   Ad esempio, &quot;v=spf1 a mx include: spf.workfront.com -all&quot;

Se non riesci ad aggiungere record SPF al firewall a causa della politica aziendale, rivolgiti al tuo [!DNL Workfront] Rappresentante del supporto.
