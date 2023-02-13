---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Impedire lo spoofing e aggiungere [!DNL Adobe Workfront] Record SPF
description: Se gli utenti non ricevono [!DNL Adobe Workfront] notifiche e-mail, è necessario aggiungere [!DNL Workfront] L'SPF registra sul firewall. Devi collaborare con il tuo team IT per aggiungere record SPF.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Impedire lo spoofing e aggiungere [!DNL Adobe Workfront] Record SPF

## Problema

Se gli utenti non ricevono [!DNL Adobe Workfront] notifiche e-mail, è necessario aggiungere [!DNL Workfront] L&#39;SPF registra sul firewall. Devi collaborare con il tuo team IT per aggiungere record SPF.

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

## Soluzione

Se hai già aggiunto gli indirizzi IP al tuo inserire nell&#39;elenco Consentiti per l’ambiente di produzione come descritto in [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) e gli utenti non ricevono ancora le e-mail:

1. Aggiungi il seguente record SPF al firewall:

   *spf.workfront.com*

   Questo aggiunge automaticamente tutto [!DNL Workfront] Indirizzi IP al tuo inserire nell&#39;elenco Consentiti sul firewall e consente a tutti i filtri di posta indesiderata (che utilizzano record SPF) di convalidare [!DNL Workfront] server come mittenti validi per il dominio.

   >[!NOTE]
   >
   > Un record SPF è un record TXT che fa parte di un file di zona DNS. Non è supportata la modifica del file di zona DNS.

1. È necessario specificare il tipo di record SPF da configurare. Questi sono i tipi validi di record SPF:

   * all (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * esiste (https://dmarcian.com/spf-syntax-table/#exists)
   * include (https://dmarcian.com/spf-syntax-table/#include)

   Ad esempio, &quot;v=spf1 a mx include: [spf.workfront.com](http://spf.workfront.com/) -all&quot;

Se non puoi aggiungere record SPF al firewall a causa della politica aziendale, collabora con il tuo [!DNL Workfront] Rappresentante del supporto.
