---
navigation-topic: notifications
title: Personalizzare gli oggetti e-mail per le notifiche degli eventi
description: Puoi personalizzare la riga dell’oggetto delle e-mail attivate dalle notifiche dell’evento.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 2f39a091-aec2-4013-a835-0ab1c8789dc3
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 4%

---

# Personalizzare gli oggetti e-mail per le notifiche degli eventi

Puoi personalizzare la riga dell’oggetto delle e-mail attivate dalle notifiche dell’evento:

La modifica dell&#39;oggetto ha effetto su tutti gli utenti del sistema, indipendentemente dal livello di accesso del destinatario. Gli utenti visualizzano tutti gli oggetti e i campi inclusi nell’oggetto dell’e-mail.

Alcune notifiche di eventi hanno più righe dell’oggetto, il che significa che tali notifiche di eventi possono avere più oggetti e-mail in base alle loro funzionalità.

>[!IMPORTANT]
>
>Presta attenzione quando elimini i campi predefiniti per i casi in cui le righe dell’oggetto si riferiscono a più oggetti. Di seguito è riportato l’elenco delle notifiche di eventi che contengono tali righe dell’oggetto:
>
>* Qualcuno mi include in un aggiornamento diretto
>* Qualcuno include il mio team in un aggiornamento diretto
>* Commento elemento lavoro a Partecipanti argomento
>* Commento sull&#39;elemento di lavoro ad assegnatario elemento di lavoro
>

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Planner o versione successiva, con accesso amministrativo per notifiche promemoria</p> <p>Per informazioni su come concedere a un utente del piano l'accesso amministrativo, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Personalizzare le righe dell’oggetto dell’e-mail per le notifiche dell’evento {#customize-email-subject-lines-for-event-notifications}

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **E-mail** > **Notifiche**.

1. Fai clic su **Notifiche evento** scheda.
1. Fare clic sul nome della notifica dell&#39;evento che si desidera personalizzare per aprire **Notifica evento** casella.
1. In **Riga dell’oggetto dell’e-mail** , modificare il testo e i campi, inclusi i campi personalizzati, nell&#39;oggetto dell&#39;e-mail.

   I nomi dei campi aggiunti devono corrispondere alla sintassi Camel Case della struttura del nostro database. <!--For more information about how our objects and their fields are named in the Workfront database, see the [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

1. Clic **Aggiorna** per salvare le nuove righe dell’oggetto nelle e-mail.

## Personalizzare le righe dell’oggetto dell’e-mail per le e-mail con più oggetti

Alcune notifiche di eventi hanno più righe dell’oggetto, a seconda degli oggetti che attivano.

Ad esempio, &quot;Qualcuno mi include in un aggiornamento diretto&quot; ha due diverse righe di oggetti: il primo è per attività, problemi, attività modello e documenti (noto anche come &quot;referenceObject&quot;) e il secondo è per oggetti che consentono agli utenti di fare commenti, come portfolio, programma e così via (noto anche come &quot;topReferenceObject&quot;).

![](assets/Ev-not-mult-subj-lines.png)

Se un utente viene incluso in una conversazione sull’attività, sul problema, sull’attività modello o sul documento, viene generato un messaggio e-mail con la prima riga dell’oggetto. L&#39;oggetto contiene &quot;referenceObject:name&quot; e il sistema definisce l&#39;oggetto e visualizza il nome appropriato nel campo dell&#39;oggetto. L’oggetto dell’e-mail sarà simile al seguente: &quot;Commento sull’attività 123 nel progetto ABC&quot;.

Se aggiunta a una conversazione di progetto, verrà generata un’e-mail con il secondo oggetto. Qui l&#39;oggetto contiene &quot;topReferenceObject:name&quot; e di nuovo Workfront identifica l&#39;oggetto a cui si è fatto riferimento e restituirà il nome dell&#39;oggetto invece di &quot;topReferenceObject:name&quot; nell&#39;oggetto. L’oggetto dell’e-mail sarà simile al seguente: &quot;Commento sul progetto ABC&quot;.

Per modificare l’oggetto dell’e-mail e aggiungere campi aggiuntivi a una delle righe dell’oggetto, consulta [Personalizzare le righe dell’oggetto dell’e-mail per le notifiche dell’evento](#customize-email-subject-lines-for-event-notifications) in questo articolo.

## Personalizzare le righe dell’oggetto dell’e-mail per le e-mail con più azioni

Alcune notifiche di eventi hanno anche più oggetti e-mail per delineare le diverse azioni che vengono eseguite sugli oggetti.

Ad esempio, la richiesta di aggiungere un documento a un problema è un evento che può attivare due e-mail diverse: una per quando il documento viene aggiunto e una per quando il documento viene modificato.

![](assets/ev-not-mult-subj-lines-diff-actions.png)

Per modificare l’oggetto dell’e-mail e aggiungere campi aggiuntivi a una delle righe dell’oggetto, consulta [Personalizzare le righe dell’oggetto dell’e-mail per le notifiche dell’evento](#customize-email-subject-lines-for-event-notifications) in questo articolo.
