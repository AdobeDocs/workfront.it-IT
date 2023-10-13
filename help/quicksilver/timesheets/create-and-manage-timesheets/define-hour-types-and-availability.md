---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Definire i tipi di ore e la disponibilità per le schede orario
description: Un Tipo di Ora è un’etichetta che consente di categorizzare l’immissione dell’ora. A seconda dei requisiti di reporting della tua organizzazione per ore, questo può essere una parte essenziale del tempo di registrazione.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '1240'
ht-degree: 0%

---

# Definire i tipi di ore e la disponibilità per le schede orario

Un Tipo di Ora è un’etichetta che consente di categorizzare l’immissione dell’ora. A seconda dei requisiti di reporting della tua organizzazione per ore, questo può essere una parte essenziale del tempo di registrazione.

In Adobe Workfront sono disponibili due set di tipi di ore:

* **Ore generali:** Ore non associate a un progetto, ad esempio malattia o amministrazione. Puoi registrare le ore generali solo sulla scheda orario.
* **Ore specifiche del progetto:** Le ore registrate per progetti, attività e problemi. È possibile registrare le ore specifiche del progetto da qualsiasi posizione in cui è possibile registrare il tempo.

Quando si registra l’ora in Workfront, i tipi di ora specifici per il progetto disponibili dipendono dalle opzioni di configurazione impostate a livello di sistema, progetto e utente. Sono sempre disponibili i seguenti tipi di ore predefiniti specifici per il progetto: Ora progetto, Ora attività e Ora problema.

I tipi di ore disponibili per la selezione durante la registrazione del tempo (su progetti, attività e problemi) sono determinati innanzitutto dai tipi di ore disponibili a livello di sistema dall&#39;amministratore di sistema e quindi dai tipi di ore selezionati a livello di progetto e utente.

Dopo aver configurato i tipi di ora appropriati, è possibile registrare il tempo da più posizioni in Workfront, come descritto in [Tempo di connessione](../../timesheets/create-and-manage-timesheets/log-time.md).

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
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso amministratore di sistema per definire i tipi di lavoro a livello di sistema e modificare tutti gli utenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Gestire l’accesso al progetto per definire i tipi di ore su un progetto</td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza di cui si dispone, contattare l&#39;amministratore Workfront.

## Definire la disponibilità a livello di sistema

L’amministratore di sistema determina quali tipi di ore specifiche per il progetto vengono rese disponibili a livello di sistema, come descritto nel [Gestire i tipi di lavoro](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Definire la disponibilità a livello di progetto {#define-availability-at-the-project-level}

Il proprietario del progetto determina se tutti i tipi di ore definiti a livello di sistema sono disponibili nel progetto (e le attività e i problemi all’interno del progetto) o se è disponibile solo un sottoinsieme di tali tipi di ore. 

1. Vai al progetto in cui desideri determinare la disponibilità dei tipi di ore.
1. Fai clic su **Altro** accanto al nome dell&#39;attività, quindi fare clic su **Modifica**.

1. Clic **Modifica Progetto**.
1. In **Impostazioni** , individuare la sezione **Filtra Tipi di Ora** opzione.

1. Seleziona **No** per rendere disponibili nel progetto tutti i tipi di ore specifici del progetto.

   Oppure

   Seleziona **Sì** per rendere disponibile nel progetto solo un sottoinsieme dei tipi di ora specifici del progetto, seleziona i tipi di ora che desideri rendere disponibili. (Tenere premuto il tasto Maiusc per selezionare più tipi di ore).

   Se selezioni questa opzione, solo i tipi di ore selezionati saranno disponibili per la selezione durante la registrazione delle ore sul progetto (o sulle attività e sui problemi all’interno del progetto). Se si seleziona questa opzione e non si seleziona alcun tipo di ora, nel progetto verranno visualizzati solo i tipi di ora generali.

   Le stesse selezioni devono essere effettuate a livello del singolo utente affinché l’utente possa visualizzare queste opzioni del tipo di ora sul progetto.

1. Clic **Salva modifiche**.

## Definire la disponibilità a livello di utente

È possibile registrare le ore per un determinato tipo di ora su progetti, attività e problemi solo se tale tipo di ora è stato reso disponibile a livello di sistema, di progetto e a livello di utente.

Se si rende disponibile un tipo di ora a livello utente come descritto in questa sezione, ma tale tipo non viene visualizzato quando si registra l&#39;ora in un progetto, attività o problema, tale tipo di ora non è stato reso disponibile nel progetto (come descritto in [Definire la disponibilità a livello di progetto](#define-availability-at-the-project-level)).

Per definire i tipi di ore disponibili per un utente:

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront.

1. Fai clic sull’avatar utente nell’angolo in alto a sinistra.
1. Fai clic su **Altro** accanto al nome utente, quindi fai clic su **Modifica**.

1. Solo un amministratore di sistema può modificare altri utenti. Se si dispone di una licenza Pianificazione, è possibile modificare i tipi di ore nel proprio profilo.
1. In **Pianificazione delle risorse** , nella sezione **Tipi di lavoro disponibili** eseguire una delle operazioni seguenti, a seconda dei tipi di ore che si desidera rendere disponibili quando si registra l&#39;ora di un progetto, un&#39;attività o un problema:

   * **Per rendere disponibili all&#39;utente tutti i tipi di ora:** Seleziona tutti i tipi di ore.\
     Se si lascia deselezionati tutti i tipi di ore, ciò equivale tecnicamente a selezionare tutti i tipi di ore. Tuttavia, in questo caso, tutti i tipi di lavoro sono disponibili per l’utente solo nei progetti, attività e problemi in cui **No** è selezionato in **Filtra Tipi di Ora** durante la modifica del progetto, come descritto in [Definire la disponibilità a livello di progetto](#define-availability-at-the-project-level).
   * **Per rendere disponibile per l&#39;utente solo un sottoinsieme dei tipi di ora:** Selezionare solo i tipi di ore che si desidera rendere disponibili.

     Affinché i tipi di lavoro selezionati a livello di utente siano disponibili per progetti, attività e problemi, è necessario che questi stessi tipi di lavoro siano selezionati anche nel **Filtra Tipi di Ora** durante la modifica del progetto, come descritto in [Definire la disponibilità a livello di progetto](#define-availability-at-the-project-level).

1. Clic **Salva modifiche**.

   Ora, quando si registrano le ore per un progetto, un&#39;attività o un problema, i tipi di ore selezionati sono disponibili se tali tipi di ore sono stati resi disponibili a livello di progetto.


## Collaborazione tra i tipi di lavoro a livello di utente e di progetto

Nell&#39;elenco seguente vengono descritti i tipi di ore visualizzati in un oggetto dopo aver personalizzato e filtrato sia i tipi di ore a livello di utente che quelli a livello di progetto:

* Per impostazione predefinita, quando si apre un oggetto per registrare l&#39;ora, il menu a discesa Tipo di ora visualizza i Tipi di ora predefiniti associati all&#39;utente. Ciò si verifica quando non hai personalizzato i tipi di lavoro.

* Dopo aver personalizzato i Tipi di lavoro e definito i Tipi di lavoro disponibili per l&#39;utente o aver filtrato i Tipi di lavoro per un progetto, si possono verificare i seguenti scenari:

   * Se hai selezionato tutti i tipi di ore per il campo Tipo di ora disponibile nel profilo dell&#39;utente e i Tipi di ora del progetto non sono filtrati, vedrai tutti i tipi di ora disponibili al momento della registrazione dell&#39;ora.
   * Se hai selezionato solo un sottoinsieme di tipi di ore per il campo Tipo di ora disponibile nel profilo dell&#39;utente e i Tipi di ora del progetto non sono filtrati, vedrai solo i tipi di ora dell&#39;utente quando registri l&#39;ora.
   * Se hai selezionato tutti i tipi di ora per il campo Tipo di ora disponibile nel profilo dell&#39;utente e i Tipi di ora del progetto sono filtrati, vedrai solo i tipi di ora del progetto e i tipi di ora predefiniti come Ora del progetto, Ora dell&#39;attività, Ora del problema a seconda dell&#39;oggetto.
   * Se nel profilo dell&#39;utente è stato selezionato solo un sottoinsieme di tipi di ore per il campo Tipo di ora disponibile e i Tipi di ora del progetto sono filtrati, verranno visualizzati solo i tipi di ora comuni all&#39;utente e al progetto. Se nessun tipo di ora è comune all&#39;utente e al progetto, vengono visualizzati solo i tipi di ora predefiniti (Ora progetto, Ora attività, Ora problema).

>[!TIP]
>
>   Se selezioni un Tipo di Ora diverso invece del tipo di Ora predefinito per un oggetto, il tipo di Ora diventa fisso. La prossima volta che accedi allo stesso oggetto, per impostazione predefinita il Tipo di Ora viene impostato automaticamente sull&#39;ultimo oggetto selezionato.

