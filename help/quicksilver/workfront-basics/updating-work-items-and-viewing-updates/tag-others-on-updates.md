---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Assegna tag ad altri utenti in caso di aggiornamenti
description: Quando si forniscono commenti di aggiornamento su un oggetto Adobe Workfront, tutti gli utenti del progetto possono visualizzare le informazioni inviate. Tuttavia, in alcuni casi gli utenti che non fanno parte del progetto potrebbero trarre vantaggio dalla visualizzazione di tali informazioni. Invece di includere tali utenti nel progetto, puoi assegnare loro tag nell’aggiornamento per condividerlo con loro. Gli utenti taggati ricevono una notifica dell’evento.
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 4b6d14559f776ed5484a67fcc5f461f154cc5e30
workflow-type: tm+mt
source-wordcount: '1577'
ht-degree: 0%

---

# Assegna tag ad altri utenti in caso di aggiornamenti

<!--take "Beta" references out when we remove the beta and change "current" to "legacy" after October 26-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>\
<span class="preview">Per informazioni sulle versioni rapide, consulta [Abilitare o disabilitare le versioni rapide per la tua organizzazione](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>

<span class="preview">Per informazioni sulla pianificazione della versione corrente, consulta [Panoramica sulla versione del quarto trimestre 2023](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span>

>[!IMPORTANT]
>
>Attualmente stiamo riprogettando l’esperienza di aggiunta di commenti in Adobe Workfront.
>A seconda dell’ambiente e degli oggetti da cui accedi all’esperienza di commento, nella sezione Aggiornamenti potrebbero essere presenti funzionalità diverse.
>
>Per ulteriori informazioni sulla nuova esperienza di commento e sulla sua disponibilità, consulta [Nuova esperienza di commento](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>La nuova esperienza di aggiunta di commenti è disponibile solo per la sezione Aggiornamenti e non per le seguenti aree:
>
> * Home
> * Pannello Riepilogo negli elenchi
> * Pannello Riepilogo nelle schede orario


<!--old note before August 17: 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>For more information about the new commenting experience, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>You can access the new experience for the following objects:
> * Issues, projects, tasks, and documents.
>
>     This is available when you enable the commenting Beta experience.
>
>     This functionality is available only for the Updates section, and it is not available for the following areas:
>
>     * Home
>     * Summary panel in lists
>     * Summary panel in timesheets
>
> * Goals, cards in the Boards area
>
>   The new commenting experience is the only experience for goals and cards. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 
>
>     You can add and view updates to cards in the Boards area when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md).

-->

È possibile assegnare tag agli utenti quando si esegue un aggiornamento a un oggetto se si desidera attirare la loro attenzione su un oggetto che altrimenti potrebbero non seguire.
Invece di includere tali utenti nell’oggetto assegnandoli a esso o imponendo loro di abbonarsi ad esso, puoi assegnare loro tag nell’aggiornamento per condividerlo con loro. Gli utenti taggati ricevono una notifica sull’aggiornamento immesso.

>[!NOTE]
>
>Per poter ricevere la notifica e-mail, l’utente deve abilitare una notifica personale nel proprio profilo. Per ulteriori informazioni, consulta [Attiva o disattiva le notifiche degli eventi](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>

Per informazioni sull&#39;aggiunta di aggiornamenti agli oggetti di Workfront, vedere [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Quando un problema viene convertito in un progetto o in un’attività, gli aggiornamenti vengono copiati nel nuovo progetto o attività, ma non negli utenti taggati. Per continuare la conversazione, è necessario assegnare nuovamente i tag ai partecipanti.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Richiedi o superiore per problemi e documenti; rivedi o superiore per tutti gli altri oggetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>Richiedente o superiore per problemi e documenti; revisore o superiore per tutti gli altri oggetti</p> 
   <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Accesso di visualizzazione all'oggetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront.

## Assegna tag ad altri utenti in caso di aggiornamenti

L’assegnazione di tag ad altri in un aggiornamento varia a seconda dell’esperienza e dell’oggetto selezionato.

### Assegna tag ad altri utenti in caso di aggiornamenti nella sezione Aggiornamenti corrente

<!--change "current" to "legacy" at the October 26, 2023 release-->

Puoi assegnare tag agli utenti manualmente nella sezione Aggiornamenti corrente.

1. Inizia ad aggiornare un elemento di lavoro, come descritto in [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In **Notifica** , digitare il nome dell&#39;utente o del team che si desidera includere, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   Oppure

   Digita il simbolo @ nella **Avvia un nuovo aggiornamento** , digitare il nome dell&#39;utente o del team che si desidera includere nell&#39;aggiornamento, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   >[!TIP]
   >
   >Per identificare l’utente corretto quando ci sono utenti con nomi simili o identici, nota l’avatar, il Ruolo principale dell’utente o il suo indirizzo e-mail.
   >
   >Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono tag in un aggiornamento.
   >
   >Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, consulta [Concedere l’accesso agli utenti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-users-in-update.png)

1. (Facoltativo) Per rendere l’aggiornamento privato, abilita **Privato per la mia azienda** nell&#39;angolo inferiore destro della casella di aggiornamento. In questo modo l’aggiornamento è visibile solo agli utenti della tua azienda. Il **Privato per la mia azienda** L’opzione è disponibile solo quando una società è specificata nel tuo profilo Workfront.

   >[!NOTE]
   >
   >Gli utenti taggati esterni all’azienda potrebbero comunque ricevere una notifica o un’e-mail in-app, anche se non vedranno i commenti privati nella scheda Aggiornamenti. È consigliabile non assegnare tag agli utenti esterni in un aggiornamento se non si desidera condividere le informazioni con loro.

1. (Facoltativo) Per aggiungere più utenti e team, ripeti il passaggio 2.

   >[!NOTE]
   >
   >Tutti gli utenti e i membri del gruppo elencati nel campo Notify (Notifica) ricevono una notifica in-app per l’aggiornamento e potrebbero ricevere un’e-mail, a seconda della configurazione delle impostazioni di notifica e-mail. Gli utenti che si assegnano i tag in un commento o in una risposta ricevono una notifica per quel commento o risposta e possono vedere il proprio nome nel campo Notify (Notifica) per il resto del thread, ma non ricevono un’altra notifica a meno che non si assegnino nuovamente i tag. Per ulteriori informazioni, consulta [Attiva o disattiva le notifiche degli eventi](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) e [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Clic **Aggiorna**.\
   Agli utenti inclusi nell&#39;aggiornamento viene automaticamente concessa l&#39;autorizzazione Visualizzazione per l&#39;oggetto e possono visualizzare e rispondere agli aggiornamenti apportati all&#39;oggetto.

   Puoi vedere chi è stato taggato in ogni risposta nella parte superiore del thread di aggiornamento. Questi utenti, insieme a tutti gli utenti abbonati all’oggetto, ricevono una notifica ogni volta che viene effettuato un aggiornamento o una risposta sull’oggetto.

   ![](assets/tagging-transparency-350x192.png)

   Per informazioni sulle funzionalità aggiuntive disponibili durante l&#39;aggiornamento di un elemento di lavoro, vedere [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

### Assegnare tag ad altri utenti sugli aggiornamenti nella nuova esperienza di commento

Puoi assegnare tag ad altri utenti per gli aggiornamenti nella nuova esperienza di commento nei seguenti modi:

* **Automaticamente**: quando un utente aggiunge un commento o una risposta, viene automaticamente taggato e aggiunto all’area Tag persone o team della casella di commento.
* **Manualmente**: quando si aggiunge manualmente un utente all’area Tag persone della casella di commento.

È inoltre possibile rimuovere gli utenti a cui vengono assegnati tag per errore quando si modifica o si risponde a un commento.

1. Inizia ad aggiornare un elemento di lavoro, come descritto in [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). In qualità di proprietario del commento, riceverai automaticamente i tag e verrai aggiunto all’area Tag persone o team della casella di commento.

   >[!TIP]
   >
   >Il proprietario del commento non può visualizzare il proprio nome nell’area Tag persone o team della casella di commento.

1. In **Assegna tag a persone o team** , digitare il nome dell&#39;utente o del team che si desidera includere, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   Oppure

   Digita il simbolo @ nella **Scrivi un commento** , digitare il nome dell&#39;utente o del team che si desidera includere nell&#39;aggiornamento, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   >[!TIP]
   > 
   >Per identificare l’utente corretto quando ci sono utenti con nomi simili o identici, nota l’avatar, il Ruolo principale dell’utente o il suo indirizzo e-mail.
   > 
   >Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono tag in un aggiornamento.
   > 
   >Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, consulta [Concedere l’accesso agli utenti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-others-unified-commenting.png)

1. (Facoltativo) Per rendere l’aggiornamento privato, abilita **Privato per la mia azienda** nell&#39;angolo inferiore destro della casella di aggiornamento. In questo modo l’aggiornamento è visibile solo agli utenti della tua azienda. Il **Privato per la mia azienda** L’opzione è disponibile solo quando una società è specificata nel tuo profilo Workfront.

   >[!NOTE]
   >
   >* Questa opzione viene visualizzata solo quando l’utente è associato a una società.
   >* Gli utenti taggati esterni all’azienda potrebbero comunque ricevere una notifica o un’e-mail in-app, anche se non vedranno i commenti privati nella scheda Aggiornamenti. È consigliabile non assegnare tag agli utenti esterni in un aggiornamento se non si desidera condividere le informazioni con loro.

1. (Facoltativo) Per aggiungere più utenti e team, ripeti il passaggio 2. <!--insure this stays accurate-->

   >[!NOTE]
   >
   >Tutti gli utenti e i membri del gruppo elencati nel campo &quot;Assegna tag a persone o team&quot; ricevono una notifica in-app per l’aggiornamento e potrebbero ricevere un’e-mail, a seconda della configurazione delle impostazioni di notifica e-mail. Gli utenti che si applicano il tag in un commento o in una risposta ricevono una notifica per tale commento o risposta e possono vedere il proprio nome in elencato come membro del thread per il resto del thread, ma non ricevono un’altra notifica a meno che non si assegnino nuovamente il tag. Per ulteriori informazioni, consulta [Attiva o disattiva le notifiche degli eventi](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) e [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Clic **Invia**.\
   Agli utenti inclusi nell&#39;aggiornamento viene automaticamente concessa l&#39;autorizzazione Visualizzazione per l&#39;oggetto e possono visualizzare e rispondere agli aggiornamenti apportati all&#39;oggetto.

   <span class="preview">I nomi delle entità con tag vengono visualizzati accanto ai relativi avatar, fino a due entità. Se vengono assegnate tag a più di due entità, viene visualizzato il nome della prima entità, oltre a un numero di quelle aggiuntive.</span>

   ![](assets/members-icons-expanded-unshimmed.png)

   Per informazioni sulle funzionalità aggiuntive disponibili durante l&#39;aggiornamento di un elemento di lavoro, vedere [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Facoltativo) Fai clic su **Altro** menu ![](assets/more-menu.png) <span class="preview">nell’angolo superiore destro del commento</span>, quindi fai clic su **Modifica**. Rimuovi gli utenti taggati, quindi fai clic su **Invia**. È possibile modificare un commento solo entro 15 minuti dall&#39;immissione. Puoi modificare solo i commenti aggiunti.