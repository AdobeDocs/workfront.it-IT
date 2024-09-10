---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Impedisci spoofing e aggiungi [!DNL Adobe Workfront] record SPF
description: Se gli utenti non ricevono  [!DNL Adobe Workfront] notifiche e-mail, devi aggiungere [!DNL Workfront] record SPF al firewall. Per aggiungere record SPF è necessario collaborare con il team IT.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Impedisci spoofing e aggiungi [!DNL Adobe Workfront] record SPF

## Problema

Se gli utenti non ricevono [!DNL Adobe Workfront] notifiche e-mail, devi aggiungere [!DNL Workfront] record SPF al firewall. Per aggiungere record SPF è necessario collaborare con il team IT.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td>
   <p>Nuovo: Standard</p>
   <p>oppure</p>
   <p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Soluzione

Se gli indirizzi IP sono già stati aggiunti al elenco Consentiti di produzione dell&#39;ambiente di produzione come descritto in [Configurare il inserisco nell&#39;elenco Consentiti di configurazione del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) e gli utenti non ricevono ancora le e-mail:

1. Aggiungi il seguente record SPF al firewall:

   *spf.workfront.com*

   Inserire nell&#39;elenco Consentiti In questo modo, tutti gli indirizzi IP [!DNL Workfront] verranno aggiunti automaticamente al tuo sul firewall e tutti i filtri anti-spam (che utilizzano i record SPF) potranno convalidare i server [!DNL Workfront] come mittenti validi per il tuo dominio.

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

Se non riesci ad aggiungere record SPF al firewall a causa della politica aziendale, rivolgiti al tuo rappresentante di supporto [!DNL Workfront].
