---
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: emails-administration
title: Configurare i modelli e-mail
description: In qualità di amministratore di Adobe Workfront, puoi configurare modelli e-mail per supportare le notifiche dei promemoria.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2ebc3be5-2734-4012-9277-86176c070137
source-git-commit: 1129f8ab93d349325bed56bc2b3ba94c2600c03f
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 1%

---

# Configurare i modelli e-mail

In qualità di amministratore di Adobe Workfront, puoi configurare modelli e-mail per supportare le notifiche dei promemoria.

I modelli di e-mail contengono il messaggio inviato agli utenti quando viene avviata una notifica di promemoria.\
Senza un modello e-mail, la notifica del promemoria verrà consegnata come contenuto vuoto nel corpo dell’e-mail.

I modelli e-mail possono essere associati a notifiche di promemoria per problemi, attività, progetti e schede orario. Durante la creazione dei modelli e-mail, l’amministratore di Workfront può fornire il contenuto dell’e-mail e una riga dell’oggetto.

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
   <td> <p>Amministratore di sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

## Crea un nuovo modello e-mail {#create-a-new-email-template}

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **E-mail** > **Notifiche**> **Modelli e-mail**.

![](assets/email-templates-tab-under-setup-email-notifications-area.png)

1. Clic **Nuovo modello e-mail**.

1. In **Nuovo modello e-mail** nella casella visualizzata, specificare le informazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td>Titolo del modello e-mail (obbligatorio).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo oggetto</td> 
      <td>Specifica il tipo di oggetto a cui associare il modello (obbligatorio, sarà impostato su "Problema" per impostazione predefinita).</td> 
     </tr>
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Descrizione del modello.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Oggetto </td> 
      <td>Oggetto visualizzato all’invio del messaggio e-mail (obbligatorio).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Corpo </td> 
      <td> <p>Contenuto visualizzato all’invio del messaggio e-mail.</p> <p>Puoi utilizzare la formattazione HTML per il contenuto dell’e-mail, come descritto in <a href="#add-html-formatting-to-an-email-template" class="MCXref xref">Aggiungere formattazione HTML a un modello e-mail</a> in questo articolo.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

## Aggiungere formattazione HTML a un modello e-mail {#add-html-formatting-to-an-email-template}

Per generare notifiche personalizzate, puoi aggiungere HTML ai modelli e-mail.\
Inizia a creare il modello e-mail come descritto in [Crea un nuovo modello e-mail](#create-a-new-email-template).

La formattazione HTML può arricchire i modelli e-mail, come illustrato nelle sezioni seguenti.

* [Collegamento a oggetti Workfront](#link-to-workfront-objects)
* [Collegamento a campi personalizzati con HTML](#link-to-custom-fields-with-html)
* [Esempi di e-mail su HTML](#html-email-examples)

### Collegamento a oggetti Workfront {#link-to-workfront-objects}

È possibile includere collegamenti ai campi di Workfront utilizzando `$$` carattere jolly per indicare al generatore di e-mail di cercare valori dal database associato a un oggetto specifico.

Ad esempio, il corpo dell’e-mail di una notifica che avvisa l’assegnatario dell’attività che l’attività sta per iniziare può seguire questa struttura:

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><a href="https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which is due to start on $$plannedStartDate$$.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b><strong>HEADING</b></td>
<td>$$WILDCARD$$</td>
</tr>
<tr>
<td><b>HEADING</b></td>
<td>$$WILDCARD$$</td>
</tr>
<tr>
<td><b>HEADING</b></td>
<td>$$WILDCARD$$</td></tr>
</table>
</html>
```

Per ottenere il valore &quot;jolly&quot; per un oggetto, effettuare una delle seguenti operazioni:

<!-- Refer to the API Explorer and select the names of your objects from the Fields tab of any object. For more information about the API Explorer, see [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

* Utilizza il valore &quot;valuefield&quot; presente all’interno della visualizzazione in modalità testo di un rapporto. Per ulteriori informazioni sui valori della modalità testo, consulta [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

  Il valore &quot;intestazione&quot; può essere il nome dell’oggetto, come desideri che appaia nel corpo dell’e-mail.

### Collegamento a campi personalizzati con HTML {#link-to-custom-fields-with-html}

È possibile includere collegamenti a utenti e campi personalizzati utilizzando **$$** carattere jolly per indicare al generatore di e-mail di cercare i valori dal database associato all’oggetto. Devono essere presenti su entrambi i lati del riferimento dell’attributo del database.

Se ad esempio si aggiunge come HTML il testo seguente, il nome dell&#39;utente assegnato verrà aggiunto alla notifica di promemoria associata a un&#39;attività:

`assignedTo:firstName`

Per aggiungere campi personalizzati con la stessa formattazione, puoi aggiungere quanto segue nella notifica e-mail:

`DE:Custom Field As It Appears in Workfront`

Ad esempio, si tratta di un modello e-mail che include un riferimento a un campo personalizzato denominato Data di consegna e presuppone che il campo Data di consegna appartenga a un’attività.

Sostituisci `<your domain>` con il dominio Workfront della tua azienda, senza le parentesi:

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><a href="https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which has a Delivery Date of $$DE:Task:Delivery Date$$.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
<tr>
<td><b>Description:</b></td>
<td>$$description$$</td>
<tr>
<td><b>Estimated Effort:</b></td>
<td>$$work$$ hours</td>
</tr>
<tr>
<td><b>Planned Completion Date:</b></td>
<td>$$plannedCompletionDate$$</td>
<td><b>Delivery Date:</b></td>
<td>$$DE:Task:Delivery Date$$</td>
</tr>
</table>
</html>
```

>[!NOTE]
>
>Se il campo appartiene a un progetto, sostituisci attività con progetto:
>
>`DE:Project:Delivery Date`

### Esempi di e-mail su HTML {#html-email-examples}

* [Notifica di promemoria per progetto in ritardo (esempio)](#late-project-reminder-notification-example)
* [Promemoria Attività o Problema in procinto di iniziare (esempio)](#task-or-issue-about-to-start-reminder-example)

#### Notifica di promemoria per progetto in ritardo (esempio) {#late-project-reminder-notification-example}

Per modificare un modello e-mail per un promemoria per un progetto in ritardo, considera queste informazioni per i campi Oggetto e Contenuto.

Sostituisci `<your domain>` con il dominio Workfront della tua azienda, senza le parentesi.

**Oggetto:**

Un Progetto Gestito È In Ritardo

**ContentContenuto:**

```html
<html>
<p>The <b><a href="https://<your domain>.my.workfront.com/project/view?ID=$$ID$$">$$name$$</a></b> project you are assigned as the owner of just became late.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
</tr>
<tr>
<td><b>Planned Completion Date:</b></td>
<td>$$plannedCompletionDate$$</td>
</tr>
</table>
<p>Please review the task plan and bring it up to date to reflect the progress made so far. If it is necessary to update the plan to bring it reflect reality going forward, be sure to speak to $$sponsor:name$$ for approval before make these changes to the work breakdown structure.</p>
</html>
```

Questo genera un’e-mail simile alla seguente:

![](assets/screen-shot-2016-09-16-at-3.52.54-pm-350x103.png)

#### Promemoria attività o problema in procinto di iniziare {#task-or-issue-about-to-start-reminder-example}

Puoi anche creare una notifica di promemoria per un’attività o un problema imminente.

Il seguente codice può essere incluso in un modello e-mail da utilizzare per le notifiche di promemoria su attività e problemi inviate un numero qualsiasi di giorni prima della data di inizio pianificata dell’attività o del problema.

Sostituisci `<your domain>` con il dominio Workfront della tua azienda, senza le parentesi.

Per utilizzare questa proprietà per un messaggio e-mail relativo a un problema, modifica il `/task/view.` valore nel collegamento all’elemento di lavoro per `/issue/view`.

**Oggetto:**

`$$name$$ to start on $$plannedStartDate$$`

**ContentContenuto:**

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><ahref=https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which is due to start on $$plannedStartDate$$.</p>
<tablewidth=350"style=font-size:12px;">
<tr>
<td><b>Task Name:</b></td>
<td>$$name$$</td>
</tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
</tr>
<td><b>Created on:</b></td>
<td>$$entryDate$$</td>
</tr>
<tr>
<td><b>Project Manager:</b></td>
<td>$$project:owner:name$$</td>
<tr>
<td><b>Priority:</b></td>
<td>$$priority$$</td>
</tr>
<tr>
<td><b>Who is assigned to:</b></td>
<td>$$assignedTo:name$$</td>
</tr>
<tr>
<td><b>When it's due:</b></td>
<td>$$estCompletionDate$$</td>
</tr>
</table>
</html>
```

![email_template_delivered.png](assets/email-template-delivered.png)

Dopo aver creato un modello e-mail, gli utenti possono associarlo alle notifiche di promemoria, come descritto in [Configurare le notifiche di promemoria](../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
