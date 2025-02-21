---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Inviare un rapporto nell’ambiente Sandbox di anteprima
description: Le informazioni presenti in questa pagina si riferiscono alle funzionalità disponibili solo negli ambienti Sandbox di anteprima e aggiornamento personalizzato. Questa funzionalità non è disponibile nell’ambiente di produzione.
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---

# Inviare un rapporto nell’ambiente Sandbox di anteprima

<!-- Audited: 11/2024 -->

Le informazioni presenti in questa pagina si riferiscono alle funzionalità disponibili solo negli ambienti Sandbox di anteprima e aggiornamento personalizzato. Questa funzionalità non è disponibile nell’ambiente di produzione.

Puoi impostare le opzioni di Consegna rapporti in qualsiasi ambiente di test di Adobe Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

Anche se gli ambienti di test devono funzionare il più vicino possibile all’ambiente di produzione, alcune funzionalità sono diverse da quelle dell’ambiente di produzione.

Puoi pianificare i rapporti negli ambienti di test, ma il modo in cui vengono consegnati è diverso da quello in cui vengono consegnati dall’ambiente di produzione.

Per informazioni sulla pianificazione dei report per la consegna nell&#39;ambiente di produzione, vedere [Panoramica sulla consegna dei report](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

A seconda della posizione in cui pianifichi i rapporti, la funzionalità di consegna varia tra le sandbox Anteprima e Aggiornamento personalizzato.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
      <td> 
      <p>Nuovo:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Corrente:</p>
         <ul>
         <li><p>Piano</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p></td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pianificare i rapporti nell’ambiente di anteprima

* [Pianificare i rapporti nell’ambiente di anteprima](#schedule-reports-in-the-preview-environment)

### Pianificare i rapporti nell’ambiente di anteprima

Il fatto che un report consegnato venga prodotto o meno nell&#39;ambiente di anteprima dipende dal fatto che **Ricevi e-mail da questo ambiente di test** sia abilitato o meno.

Per informazioni sull&#39;abilitazione delle e-mail dall&#39;ambiente Sandbox, vedere [Abilitare la consegna di e-mail dall&#39;ambiente Sandbox di anteprima](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![Ricevi e-mail dall&#39;opzione sandbox](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

La pianificazione dei rapporti da consegnare nell’ambiente di anteprima è identica alla pianificazione dei rapporti nell’ambiente di produzione. Per informazioni sulla pianificazione di un report per la consegna, vedere [Panoramica sulla consegna del report](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Quando pianifichi un rapporto da consegnare nell’ambiente di anteprima, si verificano i seguenti scenari:

* Quando **Ricevi e-mail da questo ambiente di test** è disabilitato per l&#39;utente che riceve il report, non viene prodotto alcun file durante la pianificazione del report per la consegna.
* Quando **Ricevi e-mail da questo ambiente di test** è abilitato per l&#39;utente che riceve il report, il file prodotto durante la pianificazione del report per la consegna viene aggiunto alla scheda Documenti dell&#39;utente.

## Pianificazione dei rapporti nell’ambiente Sandbox di aggiornamento personalizzato

Il fatto che un rapporto consegnato venga prodotto o meno nella Sandbox di aggiornamento personalizzata dipende dal fatto che l’opzione Ricevi e-mail da questo ambiente di test sia abilitata o meno.

Per informazioni sull&#39;attivazione delle e-mail dall&#39;ambiente di anteprima, vedere la sezione [Visualizzare e modificare le impostazioni delle notifiche e-mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) nell&#39;articolo [Modificare le proprie notifiche e-mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![Ricevi e-mail dall&#39;opzione sandbox](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

La pianificazione dei rapporti da consegnare nell’ambiente Sandbox di aggiornamento personalizzato è identica alla pianificazione dei rapporti nell’ambiente di produzione. Per informazioni sulla pianificazione di un report per la consegna, vedere [Panoramica sulla consegna del report](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Quando pianifichi un rapporto per la consegna nell’ambiente Sandbox di aggiornamento personalizzato, esistono i seguenti scenari:

* Quando l’opzione Ricevi e-mail da questo ambiente di test è disabilitata per l’utente che riceve il rapporto, non viene prodotto alcun file durante la pianificazione del rapporto per la consegna.
* Quando l’opzione Ricevi e-mail da questo ambiente di test è abilitata per l’utente che riceve il rapporto, questo viene inviato tramite e-mail come allegato all’indirizzo e-mail associato all’utente.

## Modalità di notifica agli utenti esterni

Gli utenti esterni non ricevono i rapporti inviati dagli ambienti di test di Workfront né una notifica e-mail.

Gli utenti esterni ricevono i rapporti e-mail solo se vengono consegnati da un ambiente di produzione.
