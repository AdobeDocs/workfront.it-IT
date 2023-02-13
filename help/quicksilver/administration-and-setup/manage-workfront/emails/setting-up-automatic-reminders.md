---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Imposta promemoria automatici
description: Imposta promemoria automatici
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 1%

---

# Imposta promemoria automatici

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

In qualità di amministratore di Adobe Workfront, puoi impostare promemoria automatici per attivare le notifiche e-mail quando tutte le attività o i problemi sono dovuti, in ritardo o in prossimità della data di completamento pianificata. Dopo aver configurato queste impostazioni, gli utenti non possono disattivare i promemoria automatici.

Per le notifiche in ritardo, l’e-mail viene inviata ogni notte fino al completamento dell’attività o del problema.

È possibile inviare un promemoria automatico a uno o più dei seguenti elementi:

* Utenti assegnati a un’attività o a un problema
* Il responsabile diretto dell&#39;utente
* Il responsabile del responsabile diretto

>[!NOTE]
>
>Non puoi modificare il contenuto o l’oggetto dell’e-mail attivato da un promemoria automatico.

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
   <td> <p>Amministratore di sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

## Imposta promemoria automatici

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **E-mail** >**Promemoria automatica**.

1. In **Invia una notifica in ritardo a** selezionare una delle seguenti opzioni:

   <table>
    <tr>
        <td>Utente "Assegnato a"</td>
        <td>Selezionare questa opzione se si desidera che l'utente assegnato a un'attività o a un problema riceva una notifica tardiva del proprio elemento di lavoro in ritardo.</td>
        <td></td>
    </tr>
    <tr>
        <td>Il manager dell'utente</td>
        <td>Selezionare questa opzione se si desidera che il responsabile dell'utente riceva una notifica tardiva del ritardo dell'elemento di lavoro del rapporto diretto.</td>
        <td></td>
    </tr>
    <tr>
        <td>Il manager del manager</td>
        <td>Selezionare questa opzione se si desidera che il responsabile immediatamente del responsabile riceva una notifica tardiva relativa a un elemento di lavoro in ritardo di uno degli utenti del rapporto diretto.</td>
        <td></td>
    </tr>
    <tr>
        <td>Utente "Assegnato a"</td>
        <td>(Nel <b>Invia promemoria scadenza a</b> area.) Selezionare questa opzione se si desidera che l'utente assegnato a un'attività o a un problema riceva una notifica relativa al proprio elemento di lavoro che si avvicina alla data di scadenza.</td>
        <td></td>
    </tr>
</table>

1. Selezionare l&#39;ora di invio del promemoria automatico selezionando la quantità di tempo prima o dopo la data di scadenza dell&#39;elemento di lavoro.

   L&#39;ora viene calcolata dalla data di completamento pianificata dell&#39;attività o del problema.

   Specificare il numero di minuti, ore, giorni, settimane o mesi da aggiungere alla data di completamento pianificata delle attività o dei problemi. Seleziona **Minuti trascorsi**, **Ore trascorse**, **Giorni trascorsi** oppure **Settimane trascorse** per aggiungere un orario che includa i fine settimana, le festività e gli orari non lavorativi, come indicato nella pianificazione.

   Ad esempio, se un’attività viene assegnata il venerdì e ha una durata di 3 giorni trascorsi, la data di completamento dell’attività viene impostata per il lunedì (partendo dal presupposto che il sabato e la domenica siano weekend). Se l&#39;attività ha una durata di 3 giorni (non trascorsi), la data di completamento dell&#39;attività è impostata per mercoledì.

   ![](assets/time-increments-for-automatic-reminder.png)

1. Fai clic su **Salva**.

## Ricevere promemoria automatici

Se sei l&#39;entità designata in una notifica di promemoria automatico, riceverai un&#39;e-mail quando verrà rispettata la scadenza specificata. Per le notifiche in ritardo, l’e-mail viene inviata ogni notte fino al completamento dell’attività o del problema.

Le attività con determinati tipi di dipendenza possono essere consegnate dopo la data di inizio specificata, anche se scadute. Ad esempio, se un&#39;attività ha un predecessore con una dipendenza Fine-Inizio (fs), non verrà inclusa nell&#39;e-mail, anche se viene trascorsa la data di inizio specificata, perché non è possibile avviare l&#39;attività fino al completamento del predecessore.

Per ulteriori informazioni sulla ricezione delle e-mail di promemoria automatici, consulta la sezione [promemoria automatici](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) sezione [Notifiche Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Invia promemoria automatici

I promemoria automatici vengono inviati non appena viene soddisfatta l’ora selezionata dall’amministratore di Workfront.

Se desideri attivare l&#39;invio manuale delle e-mail di promemoria automatico, puoi farlo utilizzando Diagnostica. Per ulteriori informazioni sull&#39;accesso e l&#39;utilizzo di Diagnostica in Workfront, vedi [Utilizzare Diagnostica per attivare i processi automatizzati](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
