---
title: Concedere l’accesso ai portfolio
user-type: administrator
product-area: system-administration;portfolios
navigation-topic: configure-access-to-workfront
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ai portfolio in Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f4a9c4f3-8ed4-4629-aced-9cc09b8acd3f
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# Concedere l’accesso ai portfolio

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ai portfolio, come descritto in [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurare l’accesso degli utenti ai portfolio utilizzando un livello di accesso personalizzato

1. Inizia a creare o modificare il livello di accesso, come spiegato in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) il **Visualizza** o **Modifica** a destra dei Portfoli, quindi seleziona le abilità che desideri concedere **Metti a punto le impostazioni**.

   ![](assets/fine-tune-portfolios.png)

   >[!NOTE]
   >
   >Quando si configura un&#39;impostazione del livello di accesso per un determinato tipo di oggetto, tale configurazione non influisce sull&#39;accesso degli utenti agli oggetti di livello inferiore. Ad esempio, è possibile impedire agli utenti di eliminare i portfolio nel proprio livello di accesso, ma ciò non impedisce loro di eliminare i progetti, che sono di livello inferiore rispetto ai portfolio.Per ulteriori informazioni sulla gerarchia degli oggetti, vedere la sezione [Interdipendenza e gerarchia degli oggetti](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) nell’articolo [Comprendere gli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui si sta lavorando, continuare con uno degli articoli elencati in [Configurare l’accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), ad esempio [Concedere l’accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fai clic su **Salva**.

   Dopo aver creato il livello di accesso, puoi assegnarlo a un utente. Per ulteriori informazioni, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accesso ai portfolio per tipo di licenza

Per informazioni sulle operazioni che gli utenti di ogni livello di accesso possono eseguire con i portfolio, consulta la sezione [Portfoli](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#portfoli) nell’articolo [Funzionalità disponibile per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accesso ai portfolio condivisi

In qualità di proprietario o creatore di un portfolio, puoi condividere con altri utenti concedendo loro le autorizzazioni necessarie, come spiegato in [Condividere un portfolio](../../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

Quando si condivide un oggetto con un altro utente, i diritti del destinatario su di esso sono determinati da una combinazione di due fattori:

* Autorizzazioni concesse al destinatario per l&#39;oggetto
* Impostazioni del livello di accesso del destinatario per il tipo di oggetto

Per informazioni sulle autorizzazioni che gli utenti possono concedere a un portfolio quando lo condividono, consulta [Condividere un portfolio](../../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md).
