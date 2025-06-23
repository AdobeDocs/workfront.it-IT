---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Definire i tipi di lavoro e la disponibilità
description: Un Tipo di Ora è un’etichetta che consente di categorizzare l’immissione dell’ora. A seconda dei requisiti di reporting della tua organizzazione per ore, questo può essere una parte essenziale del tempo di registrazione.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '1487'
ht-degree: 0%

---

# Definire i tipi di ore e la disponibilità

<!--Audited: 6/2025-->

Un Tipo di Ora è un’etichetta che consente di categorizzare l’immissione dell’ora. A seconda dei requisiti di reporting dell’organizzazione per le ore, questa può essere una parte essenziale del tempo di registrazione.

In Adobe Workfront sono disponibili 2 set di tipi di ore:

* **Ore generali**: ore non associate a un progetto, ad esempio ore di malattia o amministrazione. Puoi registrare solo le ore generali sulla scheda orario.
* **Ore specifiche per il progetto**: ore connesse a progetti, attività e problemi. È possibile registrare le ore specifiche del progetto da qualsiasi posizione in cui è possibile registrare il tempo.

Quando si registra l’ora in Workfront, i tipi di ora specifici per il progetto disponibili dipendono dalle opzioni di configurazione impostate a livello di sistema, progetto e utente. Sono sempre disponibili i seguenti tipi di ore predefiniti specifici per il progetto: Ora progetto, Ora attività e Ora problema.

I tipi di ore disponibili per la selezione durante la registrazione del tempo (su progetti, attività e problemi) sono determinati innanzitutto dai tipi di ore disponibili a livello di sistema dall&#39;amministratore di sistema e quindi dai tipi di ore selezionati a livello di progetto e utente.

Una volta configurati i tipi di ora appropriati, è possibile registrare il tempo da più posizioni in Workfront. Per ulteriori informazioni, vedere [Tempo di connessione](../../timesheets/create-and-manage-timesheets/log-time.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Nuovo: Standard</p> 
   <p>Corrente: Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso amministratore di sistema per definire i tipi di lavoro a livello di sistema e modificare tutti gli utenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Gestire l’accesso al progetto per definire i tipi di ore su un progetto</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Definire la disponibilità a livello di sistema

L’amministratore di sistema determina quali tipi di ore specifiche per il progetto vengono rese disponibili a livello di sistema. Per ulteriori informazioni, vedere [Gestire i tipi di lavoro](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Definire la disponibilità a livello di progetto {#define-availability-at-the-project-level}

Il proprietario del progetto determina se tutti i tipi di ore definiti a livello di sistema sono disponibili nel progetto (e le attività e i problemi all’interno del progetto) o se è disponibile solo un sottoinsieme di tali tipi di ore.

{{step1-to-projects}}

1. Nella pagina **Progetti** selezionare il progetto per il quale si desidera determinare la disponibilità dei tipi di ore.
1. Fai clic sull&#39;icona **Altro** ![Altro icona](assets/more-icon.png) accanto al nome del progetto nell&#39;intestazione, quindi fai clic su **Modifica**. Viene aperto il pannello **Modifica progetto**.

1. Nella sezione **Impostazioni progetto**, individua l&#39;impostazione **Filtra tipi di lavoro**.

1. Selezionare **No** per rendere disponibili nel progetto tutti i tipi di lavoro specifici del progetto.

   Oppure

   Seleziona **Sì** per rendere disponibile nel progetto solo un sottoinsieme dei tipi di lavoro specifici del progetto, quindi seleziona i **Tipi di lavoro** che desideri rendere disponibili. È possibile selezionare più tipi di ore.

   >[!NOTE]
   >
   >   Considera quanto segue:
   >   
   >   * Se si seleziona **Sì**, solo i tipi di ore selezionati saranno disponibili per la selezione quando si registrano le ore nel progetto (o per attività e problemi all&#39;interno del progetto).
   >   
   >   * Se si seleziona **Sì** e non si seleziona alcun tipo di ora, nel progetto verranno visualizzati solo i tipi di ora generali.
   >
   >   * Le stesse selezioni devono essere effettuate a livello del singolo utente affinché l’utente possa visualizzare queste opzioni del tipo di ora sul progetto.
   >
   >   * Quando il Tipo di Ora Predefinito dell’Utente e un Tipo di Ora Filtrato del Progetto corrispondono, quel tipo di Ora è selezionato per impostazione predefinita durante la registrazione dell’Ora.

1. Fai clic su **Salva**.

## Definire la disponibilità a livello di utente

È possibile registrare le ore per un determinato tipo di ora su progetti, attività e problemi solo se tale tipo di ora è stato reso disponibile a livello di sistema, di progetto e di utente.

Se si rende disponibile un tipo di ora a livello di utente come descritto in questa sezione, ma tale tipo non viene visualizzato durante la registrazione dell&#39;ora in un progetto, attività o problema, tale tipo di ora non è stato reso disponibile nel progetto. Per ulteriori informazioni, vedere la sezione seguente in questo articolo: [Definire la disponibilità a livello di progetto](#define-availability-at-the-project-level).

Per definire i tipi di ore disponibili per un utente:

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic sul tuo avatar utente nell&#39;angolo superiore sinistro.

   Oppure

   Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/adobe-main-menu.png) nell&#39;angolo superiore destro, se disponibile, quindi fai clic su **Workfront Profile**.

1. Fai clic sull&#39;icona **Altro** ![Altro icona](assets/more-icon.png) accanto al nome utente, quindi fai clic su **Modifica**. Viene visualizzata la casella **Modifica persona**.

   >[!IMPORTANT]
   >
   >Solo un amministratore di sistema può modificare altri utenti. Se si dispone di una licenza Pianificazione, è possibile modificare i tipi di ore nel proprio profilo.


1. Nella sezione **Pianificazione risorse**, nel menu a discesa **Tipi di ore disponibili**, eseguire una delle operazioni seguenti, a seconda dei tipi di ore che si desidera rendere disponibili quando si registra l&#39;ora in un progetto, un&#39;attività o un problema:

   * **Per rendere disponibili tutti i tipi di lavoro per l&#39;utente:** Selezionare tutti i tipi di lavoro.\
     Se si lascia deselezionati tutti i tipi di ore, ciò equivale tecnicamente a selezionare tutti i tipi di ore. Tuttavia, in questo caso, tutti i tipi di lavoro sono disponibili per l&#39;utente solo per i progetti, le attività e i problemi in cui **No** è selezionato nell&#39;opzione **Filtra tipi di lavoro** durante la modifica del progetto, come descritto in [Definire la disponibilità a livello di progetto](#define-availability-at-the-project-level).
   * **Per rendere disponibile per l&#39;utente solo un sottoinsieme dei tipi di ore:** Selezionare solo i tipi di ore che si desidera rendere disponibili.

     Affinché i tipi di lavoro selezionati a livello utente siano disponibili per progetti, attività e problemi, è necessario selezionare questi stessi tipi di lavoro anche nell&#39;opzione **Filtra tipi di lavoro** durante la modifica del progetto, come descritto in [Definire la disponibilità a livello di progetto](#define-availability-at-the-project-level).

1. (Facoltativo) Nel menu a discesa **Tipo di ora predefinito**, seleziona un tipo di ora. Quando il Tipo di Ora Predefinito dell’Utente e un Tipo di Ora Filtrato del Progetto corrispondono, quel tipo di Ora è selezionato per impostazione predefinita durante la registrazione dell’Ora.

1. Fai clic su **Salva modifiche**. Ora, quando si registrano le ore per un progetto, un&#39;attività o un problema, i tipi di ore selezionati sono disponibili se tali tipi di ore sono stati resi disponibili a livello di progetto.

## Collaborazione tra i tipi di lavoro a livello di utente e di progetto

Nell&#39;elenco seguente vengono descritti i tipi di ore visualizzati in un oggetto dopo aver personalizzato e filtrato sia i tipi di ore a livello di utente che quelli a livello di progetto al momento dell&#39;accesso all&#39;oggetto:

* Dopo aver personalizzato il Tipo di Ora predefinito per l&#39;utente e i Tipi di Ora progetto filtrati, il menu a discesa Tipo di Ora visualizza uno dei seguenti tipi di ora:

   * Quando l’utente ha un Tipo di Ora Predefinito sul proprio profilo e il progetto ha lo stesso Tipo di Ora Filtrato, questo Tipo di Ora viene visualizzato come impostazione predefinita selezionata durante la registrazione dell’ora; il Progetto, l’Attività o l’Ora del Problema vengono visualizzati come opzioni aggiuntive.

   * Se l’utente non dispone di un Tipo di Ora predefinito e il progetto dispone di Tipi di Ora filtrati, il Tipo di Ora predefinito per la registrazione è Progetto, Attività o Ora problema, ma vengono visualizzati anche i Tipi di Ora filtrati del progetto come opzioni aggiuntive.

   * Se l&#39;utente non ha un Tipo di Ora Predefinito e il progetto non ha Tipi di Ora Filtrati, vengono visualizzati come valori predefiniti solo i tipi di Ora Progetto, Attività o Ora problema, a seconda dell&#39;oggetto a cui stai effettuando l&#39;accesso.

   * Se l&#39;utente dispone di un Tipo di Ora Predefinito e il progetto non dispone di Tipi di Ora Filtrati, il Progetto, l&#39;Attività o il Tempo del Problema vengono visualizzati come valori predefiniti quando si registra il tempo sugli oggetti e non sono disponibili altri Tipi di Ora come opzioni, incluso il Tipo di Ora Predefinito dell&#39;utente.

* Dopo aver personalizzato i Tipi di lavoro e definito i Tipi di lavoro disponibili per l&#39;utente o aver filtrato i Tipi di lavoro per un progetto, si possono verificare i seguenti scenari:

   * Quando hai selezionato tutti i tipi di ore per il campo Tipo di ora disponibile nel profilo dell&#39;utente e i Tipi di ora del progetto non sono filtrati, vedrai tutti i tipi di ora disponibili quando registri l&#39;ora.
   * Quando hai selezionato solo un sottoinsieme di tipi di ore per il campo Tipo di ora disponibile nel profilo dell&#39;utente e i Tipi di ora del progetto non sono filtrati, vedrai solo i tipi di ora dell&#39;utente quando registri l&#39;ora.
   * Quando hai selezionato tutti i tipi di ora per il campo Tipo di ora disponibile nel profilo dell&#39;utente e i Tipi di ora del progetto sono filtrati, vedrai solo i tipi di ora del progetto e i tipi di ora predefiniti come Ora del progetto, Ora dell&#39;attività, Ora del problema a seconda dell&#39;oggetto.
   * Quando hai selezionato solo un sottoinsieme di tipi di ore per il campo Tipo di ora disponibile nel profilo dell&#39;utente e i Tipi di ora del progetto sono filtrati, vedrai solo i tipi di ora comuni all&#39;utente e al progetto. Se nessun tipo di ora è comune all&#39;utente e al progetto, vengono visualizzati solo i tipi di ora predefiniti (Ora progetto, Ora attività, Ora problema).

>[!TIP]
>
>   Se selezioni un Tipo di Ora diverso da quello predefinito per un oggetto, il tipo di Ora diventa permanente. La prossima volta che accedi allo stesso oggetto, per impostazione predefinita il Tipo di Ora viene impostato automaticamente sull&#39;ultimo oggetto selezionato.

