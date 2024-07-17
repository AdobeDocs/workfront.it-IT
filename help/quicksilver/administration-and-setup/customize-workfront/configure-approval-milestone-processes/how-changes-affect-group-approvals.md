---
title: Effetti delle modifiche al gruppo e al processo di approvazione sui processi di approvazione assegnati
user-type: administrator
content-type: reference
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Questo articolo spiega cosa accade quando un processo di approvazione è già in uso quando un amministratore di Workfront (o un utente con accesso amministrativo ai processi di approvazione) modifica la propria associazione a un gruppo.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 77b2dce2-1523-4262-a659-0d301059a54c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 1%

---

# Effetti delle modifiche al gruppo e al processo di approvazione sui processi di approvazione assegnati

Questo articolo spiega cosa accade quando un processo di approvazione è già associato ad attività, problemi, progetti, modelli o attività modello e un amministratore di Workfront (o un utente con accesso amministrativo ai processi di approvazione) esegue una delle seguenti operazioni:

* Modifica il processo di approvazione (a livello di gruppo) da un gruppo all&#39;altro
* Modifica il gruppo associato al progetto
* Modifica il processo di approvazione da livello di gruppo a livello di sistema
* Modifica il processo di approvazione a livello di sistema e di gruppo

L&#39;articolo descrive inoltre ciò che accade quando si spostano o si copiano attività o problemi associati a un processo di approvazione a livello di gruppo tra due progetti di gruppi diversi.

Per informazioni sui 3 tipi di processi di approvazione utilizzabili in Workfront, vedere [Panoramica del processo di approvazione](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

>[!NOTE]
>
>Se il progetto o le relative attività o problemi sono già associati a un processo di approvazione a livello di gruppo che utilizza stati personalizzati a livello di gruppo, la modifica del gruppo potrebbe creare un conflitto tra gli stati di approvazione del gruppo precedente e quelli esistenti a livello di sistema.
>
>Ad esempio, se un processo di approvazione contiene due percorsi, uno per uno stato a livello di sistema e uno per uno stato a livello di gruppo che equivale allo stesso stato a livello di sistema, la modifica del gruppo del progetto originale causerà problemi a Workfront nella comprensione dello stato specifico del gruppo che potrebbe non esistere nel secondo gruppo. In questo caso, si verifica un errore.
>
>Prima di aggiornare il gruppo del progetto, è consigliabile rimuovere i processi di approvazione a livello di gruppo sul progetto, le relative attività o i problemi.
>
>Per informazioni sulla creazione di processi di approvazione a livello di gruppo, vedere [Processi di approvazione a livello di gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).
>
>Per informazioni sulla creazione di uno stato personalizzato a livello di gruppo, vedere [Creare o modificare lo stato di un gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)

## Modifica di un processo di approvazione specifico per un gruppo da un gruppo a un altro

Gli scenari seguenti si verificano quando un processo di approvazione specifico del gruppo è già in uso su un oggetto e qualcuno lo riassegna a un gruppo diverso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area o oggetto a cui è stato allegato il processo di approvazione</th> 
   <th>Oggetto di approvazione</th> 
   <th>Modifica del processo di approvazione per l'oggetto o l'area</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Approvazione di un progetto o modello </td> 
   <td>Progetto</td> 
   <td>Diventa un processo di approvazione a utente singolo</td> 
  </tr> 
  <tr> 
   <td>Approvazione attività o attività modello </td> 
   <td>Attività</td> 
   <td>Diventa un processo di approvazione a utente singolo </td> 
  </tr> 
  <tr> 
   <td>Approvazione problema</td> 
   <td>Problema</td> 
   <td>Diventa un processo di approvazione a utente singolo</td> 
  </tr> 
  <tr> 
   <td>Attività nella casella Modifica progetto o Modifica modello</td> 
   <td>Attività</td> 
   <td> <p>Il campo Processo di approvazione predefinito attività viene reimpostato su N/D.</p> <p>Per impostazione predefinita, nessun processo di approvazione è associato alle nuove attività sul progetto.</p> </td> 
  </tr> 
  <tr> 
   <td>Sezione Dettagli coda di un progetto o modello</td> 
   <td>Problema</td> 
   <td> <p>Il campo Approvazione predefinita viene reimpostato su N/D.</p> <p>Per impostazione predefinita, nessun processo di approvazione è associato a nuovi problemi o richieste sul progetto.</p> </td> 
  </tr> 
  <tr> 
   <td>Sezione Argomento coda di un progetto o modello</td> 
   <td>Problema</td> 
   <td> <p>Il campo Approvazione predefinita viene reimpostato su N/D.</p> <p>Per impostazione predefinita, nessun processo di approvazione è associato a nuovi problemi o richieste sul progetto.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modifica del gruppo associato a un progetto

Quando qualcuno cambia il gruppo associato a un progetto in un gruppo diverso, si verifica quanto segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area o oggetto a cui è già associato il processo di approvazione</th> 
   <th>Oggetto di approvazione</th> 
   <th>Modifica del processo di approvazione dell'oggetto o dell'area</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Approvazione di un progetto o modello </td> 
   <td>Progetto</td> 
   <td>Diventa un processo di approvazione a utente singolo e lo stato ad esso associato viene aggiornato in modo da corrispondere a uno stato simile per il nuovo gruppo.</td> 
  </tr> 
  <tr> 
   <td>Approvazione attività o attività modello </td> 
   <td>Attività</td> 
   <td>Diventa un processo di approvazione a utente singolo e lo stato ad esso associato viene aggiornato in modo da corrispondere a uno stato simile per il nuovo gruppo.</td> 
  </tr> 
  <tr> 
   <td>Approvazione problema</td> 
   <td>Problema</td> 
   <td>Diventa un processo di approvazione a utente singolo e lo stato ad esso associato viene aggiornato in modo da corrispondere a uno stato simile per il nuovo gruppo.</td> 
  </tr> 
  <tr> 
   <td>Attività nella casella Modifica progetto o Modifica modello</td> 
   <td>Attività</td> 
   <td> <p>Il campo Processo di approvazione predefinito attività è reimpostato su N/D</p> <p>Per impostazione predefinita, nessun processo di approvazione è associato alle nuove attività sul progetto</p> </td> 
  </tr> 
  <tr> 
   <td>Sezione Dettagli coda di un progetto o modello</td> 
   <td>Problema</td> 
   <td> <p>Il campo Processo di approvazione predefinito è reimpostato su N/D</p> <p>Per impostazione predefinita, nessun processo di approvazione è associato a nuovi problemi o richieste sul progetto</p> </td> 
  </tr> 
  <tr> 
   <td>Sezione Argomento coda di un progetto o modello</td> 
   <td>Problema</td> 
   <td> <p>Il campo Processo di approvazione predefinito è reimpostato su N/D</p> <p>Per impostazione predefinita, nessun processo di approvazione è associato a nuovi problemi o richieste sul progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modifica di un processo di approvazione a livello di gruppo e di sistema

Quando qualcuno modifica l’opzione Gruppo in un processo di approvazione specifico per il gruppo in &quot;Tutti i gruppi&quot;, il processo di approvazione diventa a livello di sistema e si verifica quanto segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area o oggetto a cui è stato allegato il processo di approvazione</th> 
   <th>Oggetto di approvazione</th> 
   <th>Modifica del processo di approvazione dell'oggetto o dell'area</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Approvazione di un progetto o modello </td> 
   <td>Progetto</td> 
   <td>Nessuna modifica</td> 
  </tr> 
  <tr> 
   <td>Approvazione attività o attività modello </td> 
   <td>Attività</td> 
   <td>Nessuna modifica</td> 
  </tr> 
  <tr> 
   <td>Approvazione problema</td> 
   <td>Problema</td> 
   <td>Nessuna modifica</td> 
  </tr> 
  <tr> 
   <td>Attività nella casella Modifica progetto o Modifica modello</td> 
   <td>Attività</td> 
   <td> <p>Nessuna modifica al processo di approvazione ma, per impostazione predefinita, è associato a nuove attività nel progetto</p> </td> 
  </tr> 
  <tr> 
   <td>Sezione Dettagli coda di un progetto o modello</td> 
   <td>Problema</td> 
   <td> <p>Nessuna modifica al processo di approvazione ma, per impostazione predefinita, è associato a nuovi problemi o richieste sul progetto</p> </td> 
  </tr> 
  <tr> 
   <td>Sezione Argomento coda di un progetto o modello</td> 
   <td>Problema</td> 
   <td> <p>Nessuna modifica al processo di approvazione ma, per impostazione predefinita, è associato a nuovi problemi o richieste sul progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modifica di un processo di approvazione a livello di sistema e di gruppo

Quando qualcuno cambia la disponibilità di un processo di approvazione a livello di sistema da &quot;Tutti i gruppi&quot; a un gruppo specifico, il processo di approvazione diventa specifico per il gruppo e si verifica quanto segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area o oggetto a cui è stato allegato il processo di approvazione</th> 
   <th>Oggetto di approvazione</th> 
   <th>Modifica del processo di approvazione dell'oggetto o dell'area</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Progetto, attività, problema, modello o attività modello che appartiene al gruppo del processo di approvazione</td> 
   <td> <p>Progetto, attività o problema</p> </td> 
   <td>Nessuna modifica</td> 
  </tr> 
  <tr> 
   <td>Attività nella casella Modifica progetto o Modifica modello per un progetto o un modello che appartiene al gruppo del processo di approvazione</td> 
   <td>Attività</td> 
   <td> <p>Nessuna modifica al processo di approvazione ma, per impostazione predefinita, è associato a nuove attività nel progetto</p> </td> 
  </tr> 
  <tr> 
   <td>Sezione Dettagli coda per un progetto o un modello che appartiene al gruppo del processo di approvazione</td> 
   <td>Problema</td> 
   <td> <p>Nessuna modifica al processo di approvazione ma, per impostazione predefinita, è associato a nuovi problemi o richieste sul progetto</p> </td> 
  </tr> 
  <tr> 
   <td>Sezione Argomento coda per un progetto o un modello che appartiene al gruppo del processo di approvazione</td> 
   <td>Problema</td> 
   <td> <p>Nessuna modifica al processo di approvazione ma, per impostazione predefinita, è associato a nuovi problemi o richieste sul progetto</p> </td> 
  </tr> 
  <tr> 
   <td>Progetto, attività, problema, modello o attività modello che appartiene a un gruppo diverso dal gruppo del processo di approvazione</td> 
   <td> <p>Progetti</p> <p>Attività</p> <p>Problemi</p> </td> 
   <td>Diventa un processo di approvazione a utente singolo</td> 
  </tr> 
  <tr> 
   <td>Attività nella casella Modifica progetto o Modifica modello per un progetto o un modello che appartiene a un gruppo diverso dal gruppo del processo di approvazione</td> 
   <td>Attività</td> 
   <td> <p>Il campo Processo di approvazione predefinito attività viene reimpostato su N/D.</p> <p>Per impostazione predefinita, nessun processo di approvazione è associato alle nuove attività sul progetto.</p> </td> 
  </tr> 
  <tr> 
   <td>Sezione Dettagli coda per un progetto o un modello che appartiene a un gruppo diverso dal gruppo del processo di approvazione</td> 
   <td>Problemi</td> 
   <td> <p>Il campo Approvazione predefinita viene reimpostato su N/D.</p> <p>Per impostazione predefinita, nessun processo di approvazione è associato a nuovi problemi o richieste sul progetto.</p> </td> 
  </tr> 
  <tr> 
   <td>Sezione Argomento coda per un progetto o un modello che appartiene a un gruppo diverso dal gruppo del processo di approvazione</td> 
   <td>Problemi</td> 
   <td> <p>Il campo Approvazione predefinita viene reimpostato su N/D.</p> <p>Per impostazione predefinita, nessun processo di approvazione è associato a nuovi problemi o richieste sul progetto.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Spostamento o copia di un&#39;attività o di un problema in un progetto con un gruppo diverso da quello del processo di approvazione

Lo spostamento o la copia di un’attività o di un problema da un progetto a un altro può influire sui processi di approvazione esistenti per l’attività o il problema, a seconda dei gruppi dei due progetti. Nella tabella seguente sono illustrati gli scenari possibili:

| Processo di approvazione attività o problema originale | Gruppi dei due progetti | Modifiche nel processo di approvazione dopo lo spostamento dell’attività o del problema in un altro progetto |
|---|---|---|
| Processo di approvazione per singolo utilizzo associato a uno stato a livello di sistema | I progetti si trovano nello stesso gruppo o in gruppi diversi | Nessuna modifica |
| Processo di approvazione per singolo utilizzo associato a uno stato specifico per un gruppo | I progetti si trovano in gruppi diversi | L’approvazione rimane un processo di approvazione a utente singolo e lo stato associato agli aggiornamenti di approvazione corrisponde a uno stato simile per il nuovo gruppo. |
| Processo di approvazione a livello di sistema | I progetti si trovano nello stesso gruppo o in gruppi diversi | Nessuna modifica |
| Processo di approvazione specifico per gruppo | I progetti fanno parte dello stesso gruppo | Nessuna modifica |
| Processo di approvazione specifico per gruppo | I progetti si trovano in gruppi diversi e i gruppi hanno stati diversi specifici per ciascun gruppo | L’approvazione diventa un processo di approvazione a utente singolo e lo stato associato agli aggiornamenti dell’approvazione corrisponde a uno stato simile per il nuovo gruppo. |
| Processo di approvazione specifico per gruppo | I progetti si trovano in gruppi diversi ed è presente uno stato con la stessa chiave nel nuovo gruppo dello stato associato al processo di approvazione del primo gruppo | Nessuna modifica |
