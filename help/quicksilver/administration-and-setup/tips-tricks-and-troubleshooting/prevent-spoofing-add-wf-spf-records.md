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
TQID: https://experienceleague.adobe.com/6VnF205aiahPEWdP2kPk-YXF8UfPwSJ0-yJ6nGq3-FM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 292
ht-degree: 9%

---

# Impedisci spoofing e aggiungi [!DNL Adobe Workfront] record SPF

## Problema

Se gli utenti non ricevono [!DNL Adobe Workfront] notifiche e-mail, devi aggiungere [!DNL Workfront] record SPF al firewall. Per aggiungere record SPF è necessario collaborare con il team IT.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Soluzione

Se hai già aggiunto gli indirizzi IP al tuo elenco Consentiti di per l&#39;ambiente di produzione come descritto in [Configurare il inserisco nell&#39;elenco Consentiti di del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) e gli utenti non ricevono ancora le e-mail:

1. Aggiungi il seguente record SPF al firewall:

   *spf.workfront.com*

   In questo modo tutti gli indirizzi IP [!DNL Workfront] verranno aggiunti automaticamente al tuo elenco Consentiti di sul firewall e tutti i filtri anti-spam (che utilizzano record SPF) potranno convalidare i server [!DNL Workfront] come mittenti validi per il tuo dominio.

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
