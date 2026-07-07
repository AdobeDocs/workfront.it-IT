---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Impostare promemoria automatici
description: Puoi impostare promemoria automatici per attivare le notifiche e-mail quando tutte le attività o i problemi sono in scadenza, in ritardo o in prossimità della data di completamento pianificata.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/sxv8RUKwTr-SABLfOrmTa0J9ToM62-1tF5rFEnu41UI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: f283a5f64062e5878373527de46b0d993b545ba7
workflow-type: tm+mt
source-wordcount: 836
ht-degree: 6%

---

# Impostare promemoria automatici

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

In qualità di amministratore di Adobe Workfront, puoi impostare promemoria automatici per attivare le notifiche e-mail quando tutte le attività, i problemi o altri elementi di lavoro assegnati sono in scadenza, in ritardo o in prossimità della data di completamento pianificata.

Dopo aver configurato queste impostazioni, gli utenti non possono disattivare i promemoria automatici. I promemoria automatici verranno inviati indipendentemente dalle impostazioni di notifica di un utente nella relativa area Impostazioni personali.

Per le notifiche in ritardo, l’e-mail viene inviata ogni notte fino al completamento dell’attività o del problema. Ciò significa che l’utente riceverà una notifica ogni giorno mentre l’attività o il problema non è completato.

Un promemoria automatico può essere inviato a uno o più dei seguenti:

* Gli utenti assegnati a un’attività o a un problema
* Responsabile immediato dell’utente
* Il manager del manager immediato

>[!NOTE]
>
>Non puoi modificare il contenuto o la riga dell’oggetto dell’e-mail attivata da un promemoria automatico.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Amministratore di sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Dettagli della funzionalità di promemoria automatico

### Distinzione da altri tipi di promemoria

I promemoria automatici sono la funzione di promemoria a livello di configurazione per le attività e i problemi di Workfront e sono separati dalla funzione di notifica dei promemoria a livello di oggetto. Per informazioni sulla differenza tra promemoria automatici e notifiche di promemoria, vedere [Promemoria automatici e notifiche di promemoria](/help/quicksilver/administration-and-setup/tips-tricks-and-troubleshooting/auto-reminders-vs-reminder-notifications.md).

Le decisioni relative a bozze e bozze non vengono inoltre gestite da promemoria automatici e seguono un processo di promemoria separato. Per informazioni dettagliate sui promemoria di decisione per bozze e bozze, vedere gli articoli in [Notifiche e promemoria per bozze](/help/quicksilver/workfront-proof/wp-emailsntfctns/wp-emails-and-notifications.md).

## Considerazioni durante l’utilizzo dei promemoria automatici

Quando si utilizzano i promemoria automatici, considera quanto segue:

* Le e-mail scadute vengono inviate come un digest e-mail per destinatario al giorno, non come e-mail separate per elemento.
* L&#39;attivazione dei promemoria automatici può causare la visualizzazione di problemi o attività già scaduti nella successiva e-mail di riepilogo Scaduto, indipendentemente da quanto tempo l&#39;elemento sia scaduto.
* I promemoria sono validi solo per i progetti in stato Corrente/Attivo.
* Per &quot;giorni&quot; nell&#39;impostazione automatica del promemoria si intendono i giorni lavorativi in base alla pianificazione, non i giorni trascorsi o l&#39;ora del calendario.



## Impostare promemoria automatici

{{step-1-to-setup}}

1. Fai clic su **E-mail** > **Promemoria automatici**.

1. Nell&#39;area **Invia una notifica in ritardo a**, selezionare una delle opzioni seguenti:

   <table>
    <tr>
        <td>L'utente "Assegnato a"</td>
        <td>Seleziona questa opzione se desideri che l’utente assegnato a un’attività o a un problema riceva una notifica in ritardo relativa al ritardo del suo elemento di lavoro.</td>
        <td></td>
    </tr>
    <tr>
        <td>Il manager dell'utente</td>
        <td>Selezionare questa opzione se si desidera che il manager dell'utente riceva una notifica di ritardo relativa al ritardo dell'elemento di lavoro del referente diretto.</td>
        <td></td>
    </tr>
    <tr>
        <td>Il manager del manager</td>
        <td>Selezionare questa opzione se si desidera che il manager immediato riceva una notifica di ritardo relativa a un elemento di lavoro di uno degli utenti del referente diretto in ritardo.</td>
        <td></td>
    </tr>
    <tr>
        <td>L'utente "Assegnato a"</td>
        <td>Nell'area <b>Invia promemoria scadenza a</b>. Selezionare questa opzione se si desidera che l'utente assegnato a un'attività o a un problema riceva una notifica relativa all'elemento di lavoro che si avvicina alla data di scadenza.</td>
        <td></td>
    </tr>
   </table>

1. Selezionare l&#39;ora per l&#39;invio del promemoria automatico selezionando la quantità di tempo precedente o successiva alla data di scadenza dell&#39;elemento di lavoro.

   L’ora viene calcolata a partire dalla Data di completamento pianificata dell’attività o del problema.

   Specifica il numero di minuti, ore, giorni, settimane o mesi per aggiungere il tempo alla data di completamento pianificata delle attività o dei problemi. Seleziona **Minuti trascorsi**, **Ore trascorse**, **Giorni trascorsi** o **Settimane trascorse** per aggiungere l&#39;ora che include i fine settimana, le festività e le ore non lavorative come indicato nella pianificazione.

   Ad esempio, se un&#39;attività viene assegnata il venerdì e ha una durata di 3 giorni, la data di completamento dell&#39;attività viene impostata per il lunedì (supponendo che sabato e domenica siano un fine settimana). Se l&#39;attività ha una durata di 3 giorni (non trascorsa), la data di completamento dell&#39;attività viene impostata su Mercoledì.

   ![Incrementi di tempo](assets/time-increments-for-automatic-reminder.png)

1. Fai clic su **Salva**.

## Ricevi promemoria automatici

Se sei l’entità designata in una notifica di Promemoria automatico, ricevi un’e-mail quando viene rispettata la scadenza specificata. Per le notifiche in ritardo, l’e-mail viene inviata ogni notte fino al completamento dell’attività o del problema.

Le attività con determinati tipi di relazione possono essere consegnate dopo la data di inizio specificata, anche se sono scadute. Ad esempio, se un&#39;attività ha un predecessore con una relazione Fine-Inizio (fs), non verrà inclusa nell&#39;e-mail, anche se è stata superata la data di inizio specificata, perché non è possibile avviare l&#39;attività fino al completamento del predecessore.

Per ulteriori informazioni sulla ricezione di e-mail di Promemoria automatici, consulta la sezione [Promemoria automatici](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) nelle [notifiche Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Invia promemoria automatici

I promemoria automatici vengono inviati non appena viene rispettata l’ora selezionata dall’amministratore di Workfront.

Se desideri attivare manualmente l’invio dei promemoria automatici, utilizza la funzione Diagnostica. Per ulteriori informazioni sull&#39;accesso e l&#39;utilizzo di Diagnostica in Workfront, vedere [Utilizzare Diagnostica per attivare i processi automatizzati](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
