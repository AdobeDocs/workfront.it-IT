---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Inviare un rapporto nell’ambiente Sandbox di anteprima
description: Le informazioni presenti in questa pagina fanno riferimento a funzionalità disponibili solo negli ambienti Sandbox di anteprima e aggiornamento personalizzato. Questa funzionalità non è disponibile nell’ambiente di produzione.
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Inviare un rapporto nell’ambiente Sandbox di anteprima

Le informazioni presenti in questa pagina fanno riferimento a funzionalità disponibili solo negli ambienti Sandbox di anteprima e aggiornamento personalizzato. Questa funzionalità non è disponibile nell’ambiente di produzione.

Puoi impostare le opzioni di consegna dei rapporti in qualsiasi ambiente di test di Adobe Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

Anche se gli ambienti di test devono funzionare il più vicino possibile all’ambiente di produzione, alcune funzionalità sono diverse dall’ambiente di produzione.

È possibile pianificare i rapporti negli ambienti di test, ma il modo in cui vengono consegnati differisce da come vengono consegnati dall’ambiente di produzione.

Per informazioni sulla pianificazione dei rapporti per la consegna nell’ambiente di produzione, consulta [Panoramica sulla consegna dei rapporti](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

A seconda della posizione in cui vengono pianificati i rapporti, la funzionalità di consegna è diversa tra le sandbox Anteprima e Aggiornamento personalizzato.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Pianificare rapporti nell’ambiente Anteprima

* [Pianificare rapporti nell’ambiente Anteprima](#schedule-reports-in-the-preview-environment)

### Pianificare rapporti nell’ambiente Anteprima

Il fatto che un rapporto consegnato venga prodotto o meno nell’ambiente Anteprima dipende dal fatto se **Ricevi e-mail da questo ambiente di test** è abilitato o meno.

Per informazioni sull’abilitazione delle e-mail dall’ambiente Sandbox, consulta [Abilitare la consegna di e-mail dall’ambiente Sandbox di anteprima](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

La pianificazione dei rapporti per la consegna nell’ambiente Anteprima è identica alla pianificazione dei rapporti nell’ambiente Produzione. Per informazioni sulla pianificazione di un rapporto per la consegna, vedi [Panoramica sulla consegna dei rapporti](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Quando pianifichi una consegna di un rapporto nell’ambiente Anteprima, sono presenti i seguenti scenari:

* Quando **Ricevi e-mail da questo ambiente di test** è disabilitato per l’utente che riceve il rapporto, non viene prodotto alcun file durante la pianificazione del rapporto per la consegna.
* Quando **Ricevi e-mail da questo ambiente di test** è abilitato per l’utente che riceve il rapporto; il file prodotto durante la pianificazione del rapporto per la consegna viene aggiunto nella scheda Documenti dell’utente.

## Pianificare rapporti nell’ambiente Sandbox di aggiornamento personalizzato

Il fatto che un rapporto consegnato venga prodotto o meno nella Sandbox di aggiornamento personalizzato dipende dal fatto che l’impostazione Ricevi e-mail da questo ambiente di test sia abilitata o meno.

Per informazioni sull’abilitazione delle e-mail dall’ambiente di anteprima, consulta la sezione . [Visualizza e modifica le impostazioni delle notifiche e-mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) nell&#39;articolo [Attivare o disattivare le notifiche degli eventi personali](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

La pianificazione dei rapporti per la consegna nell’ambiente Sandbox di aggiornamento personalizzato è identica alla pianificazione dei rapporti nell’ambiente Produzione. Per informazioni sulla pianificazione di un rapporto per la consegna, vedi [Panoramica sulla consegna dei rapporti](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Quando pianifichi un rapporto per la consegna nell’ambiente Sandbox di aggiornamento personalizzato, esistono i seguenti scenari:

* Quando l’utente che riceve il rapporto riceve e-mail da questo ambiente di test è disabilitato, non viene generato alcun file durante la pianificazione del rapporto per la consegna.
* Quando l’utente che riceve il rapporto riceve e-mail da questo ambiente di test è abilitato, questo viene inviato come allegato all’indirizzo e-mail associato all’utente.

## Notifiche agli utenti esterni

Gli utenti esterni non ricevono rapporti inviati dagli ambienti di test di Workfront, né ricevono una notifica e-mail.

Gli utenti esterni ricevono i rapporti e-mail solo se vengono consegnati da un ambiente di produzione.
