---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Definire i tipi di ora e la disponibilità per i fogli presenze
description: Un tipo di ora è un’etichetta che consente di categorizzare l’immissione di ora. A seconda dei requisiti di reporting dell’organizzazione per ore, questo può essere una parte essenziale del tempo di registrazione.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---

# Definire i tipi di ora e la disponibilità per i fogli presenze

Un tipo di ora è un’etichetta che consente di categorizzare l’immissione di ora. A seconda dei requisiti di reporting dell’organizzazione per ore, questo può essere una parte essenziale del tempo di registrazione.

In Adobe Workfront sono disponibili due set di tipi di ora:

* **Orario generale:** Ore che non sono associate a un progetto, ad esempio il momento di malattia o l’amministrazione. È possibile registrare le ore generali solo nella scheda attività.
* **Orari specifici del progetto:** Ore di accesso a progetti, attività e problemi. Puoi registrare ore specifiche per il progetto da qualsiasi posizione in cui puoi registrare il tempo.

Durante l’accesso in Workfront, i tipi di ora specifici del progetto disponibili dipendono dalle opzioni di configurazione impostate a livello di sistema, progetto e utente. I seguenti tipi di ora predefiniti per specifici progetti sono sempre disponibili: Ora progetto, Ora attività e Ora problema.)

I tipi di ora disponibili per la selezione del tempo di registrazione (su progetti, attività e problemi) sono determinati in primo luogo dai tipi di ora resi disponibili a livello di sistema dall&#39;amministratore di sistema, quindi dai tipi di ora selezionati a livello di progetto e utente.

Dopo aver configurato i tipi di ora appropriati, puoi registrare il tempo da più posizioni in Workfront, come descritto in [Tempo di log](../../timesheets/create-and-manage-timesheets/log-time.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso dell'amministratore di sistema per definire i tipi di ora per l'intero sistema e per modificare tutti gli utenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Gestisci l’accesso al progetto per definire i tipi di ora in un progetto</td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Definire la disponibilità a livello di sistema

L’amministratore di sistema determina quali tipi di ora specifici del progetto vengono resi disponibili a livello di sistema, come descritto in [Gestione dei tipi di ora](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md) sezione  [Gestione dei tipi di ora](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Definire la disponibilità a livello di progetto {#define-availability-at-the-project-level}

Il proprietario del progetto determina se nel progetto sono disponibili tutti i tipi di ora definiti a livello di sistema (attività e problemi all’interno del progetto) o se è disponibile solo un sottoinsieme di tali tipi di ora. 

1. Passa al progetto in cui desideri determinare la disponibilità dei tipi di ora.
1. Fai clic sul pulsante **Altro** accanto al nome dell&#39;attività, quindi fare clic su **Modifica**.

1. Fai clic su **Modifica progetto**.
1. In **Impostazioni** , individua la sezione **Tipi di ora filtro** opzione .

1. Seleziona **No** per rendere disponibili nel progetto tutti i tipi di ora specifici per il progetto.

   Oppure

   Seleziona **Sì** per rendere disponibile nel progetto solo un sottoinsieme dei tipi di ora specifici del progetto, seleziona i tipi di ora che desideri rendere disponibili. Tenete premuto il tasto Maiusc per selezionare più tipi di ora.

   Se selezioni questa opzione, solo i tipi di ora selezionati vengono resi disponibili per selezionare durante la registrazione delle ore sul progetto (o su attività e problemi all’interno del progetto). Se selezioni questa opzione e non selezioni alcun tipo di ora, nel progetto vengono visualizzati solo i tipi di ora generali.

   Le stesse selezioni devono essere effettuate a livello di singolo utente per consentire all’utente di visualizzare queste opzioni relative al tipo di ora nel progetto.

1. Fai clic su **Salva modifiche**.

## Definire la disponibilità a livello di utente

È possibile registrare ore per un determinato tipo di ora su progetti, attività e problemi solo se tale tipo di ora è stato reso disponibile a livello di sistema, di progetto e di utente.

Se rendi disponibile un tipo di ora a livello utente come descritto in questa sezione, ma non lo si vede quando si registra il tempo su un progetto, un&#39;attività o un problema, tale tipo di ora non è disponibile nel progetto (come descritto in [Definire la disponibilità a livello di progetto](#define-availability-at-the-project-level)).

Per definire i tipi di ora disponibili per un utente:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic sull’avatar dell’utente nell’angolo in alto a sinistra.
1. Fai clic sul pulsante **Altro** accanto al nome utente, quindi fai clic su **Modifica**.

1. Solo un amministratore di sistema può modificare altri utenti. Se disponi di una licenza Plan, puoi modificare i tipi di ora nel tuo profilo.
1. In **Pianificazione delle risorse** nella sezione **Tipi di ora disponibili** scegliere una delle seguenti operazioni dal menu a discesa, a seconda dei tipi di ora che si desidera rendere disponibili quando si registra il tempo su un progetto, un&#39;attività o un problema:

   * **Per rendere disponibili all’utente tutti i tipi di ora:** Seleziona tutti i tipi di ora.\
      Se non selezioni tutti i tipi di ora, tecnicamente equivale a selezionare tutti i tipi di ora. Tuttavia, in questo caso, tutto il tipo di ora è disponibile per l’utente solo per progetti, attività e problemi in cui **No** è selezionato in **Tipi di ora filtro** durante la modifica del progetto, come descritto in [Definire la disponibilità a livello di progetto](#define-availability-at-the-project-level).
   * **Per rendere disponibile solo un sottoinsieme dei tipi di ora all’utente:** Seleziona solo i tipi di ora che desideri rendere disponibili.

      Affinché i tipi di ora selezionati a livello di utente siano disponibili per progetti, attività e problemi, questi tipi di ora devono essere selezionati anche nel **Tipi di ora filtro** durante la modifica del progetto, come descritto in [Definire la disponibilità a livello di progetto](#define-availability-at-the-project-level).

1. Fai clic su **Salva modifiche**.

   Ora, quando si eseguono le ore di accesso a un progetto, un&#39;attività o un problema, i tipi di ora selezionati sono disponibili se a livello di progetto sono stati resi disponibili gli stessi tipi di ora.
