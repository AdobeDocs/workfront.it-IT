---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Informazioni sulla migrazione di Workfront a Adobe Admin Console
description: Questo articolo descrive in termini generali il processo di spostamento di un’organizzazione in Adobe Admin Console, in modo che tu come amministratore Workfront possa sapere cosa aspettarti.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1114'
ht-degree: 0%

---

# Informazioni sulla migrazione di Workfront a Adobe Admin Console

Adobe sta modificando il modo in cui gestisci gli utenti Adobe Workfront, aumentando la produttività per te e la tua organizzazione. Come parte di questa modifica, Adobe sta eseguendo la migrazione dell’istanza Workfront e degli utenti a Adobe Admin Console. Si tratta di una migrazione necessaria e non influirà su rapporti, percorsi di approvazione, contenuti o risorse. Questo influirà su come gestisci l’accesso degli utenti e come accedono gli utenti.

Questo articolo descrive in termini generali il processo di spostamento di un’organizzazione in Adobe Admin Console, in modo che tu come amministratore Workfront possa sapere cosa aspettarti.

Per informazioni su come utilizzare Adobe Admin Console per gestire i diritti Adobe in tutta l&#39;organizzazione, consulta [Gestione degli utenti in Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## Cosa sta cambiando?

Come parte della migrazione, la gestione degli utenti passerà dall’applicazione Workfront a Adobe Admin Console con i seguenti ruoli amministrativi:

* **Gli amministratori di sistema** sono utenti con privilegi avanzati di tutti gli amministratori. Assegnano tutti i ruoli amministrativi e gestiscono gli utenti dell’intera organizzazione per tutti i prodotti.

* **Amministratori del profilo di prodotto (amministratori di sistema di Workfront)** gestiscono quali utenti dell&#39;organizzazione hanno accesso a Workfront.

* **Gli utenti accederanno con Adobe Identity.Adobe** Dopo la migrazione degli utenti esistenti a Adobe Admin Console, gli utenti effettueranno l&#39;accesso alle proprie istanze di Workfront utilizzando la nuova identità Adobe, Adobe ID o Adobe Federated ID (SSO).

* **Non è stata modificata la modalità di gestione di tutte le altre funzionalità** all&#39;interno dell&#39;applicazione Workfront stessa, inclusa la gestione di funzionalità, ruoli utente, aree di lavoro, funzionalità e comportamento.

## Timeline del Percorso di migrazione

Adobe eseguirà prima la migrazione dell’istanza Workfront a Adobe Admin Console, quindi eseguirà la migrazione di tutti gli utenti esistenti con indirizzi e-mail verificati. Se sei un amministratore di sistema o un amministratore del profilo di prodotto di Workfront (amministratore di sistema di Workfront), riceverai e-mail che ti guidano attraverso il percorso di migrazione. Ecco una cronologia di ciò che puoi aspettarti:

### Migrazione di Workfront a Adobe Admin Console completata

Gli amministratori di sistema riceveranno un’e-mail al termine della migrazione di Workfront a Adobe Admin Console. Al momento, gli amministratori di sistema potrebbero dover completare alcuni passaggi obbligatori **prima dell&#39;avvio della migrazione degli utenti**, per ridurre al minimo l&#39;impatto sugli utenti di Workfront.

* **Se gli utenti di Workfront al momento effettuano l&#39;accesso con SSO**, è necessario configurare SSO in Adobe Admin Console in modo che gli utenti possano continuare ad accedere con SSO. Se gli utenti di Workfront al momento non utilizzano l’SSO, ma desideri configurarlo su Adobe Admin Console, puoi farlo a questo punto nel percorso di migrazione.
* **Se gestisci già altri prodotti Adobe nel tuo Adobe Admin Console**, Adobe potrebbe richiedere il tuo consenso per eseguire automaticamente la migrazione degli utenti alla console esistente. Fai clic sul pulsante **Inizia** nell&#39;e-mail per passare alla pagina del consenso.
* **Se in precedenza hai eliminato il tipo di licenza Requestor**, verrà aggiunto al sistema. A questo tipo di licenza non verrà assegnato alcun utente, ma è necessario per la sincronizzazione tra Workfront e Adobe Admin Console. Non è richiesta alcuna azione da parte dell&#39;utente per quanto riguarda il tipo di licenza del richiedente.

Al momento non vi sono modifiche alla gestione degli utenti. Gli amministratori di Workfront continueranno a gestire gli utenti in Workfront e gli utenti continueranno ad accedere con il proprio Workfront ID o SSO fino al completamento della migrazione degli utenti.

### Pianifica migrazione utenti

Dopo che l’amministratore di sistema avrà soddisfatto i prerequisiti descritti nella sezione precedente, Adobe pianificherà automaticamente la migrazione utente per 30 giorni dopo il completamento di tali prerequisiti e comunicherà con gli amministratori del profilo di prodotto di Workfront (amministratori di sistema di Workfront) per gestire la migrazione degli utenti.

Gli amministratori dei profili di prodotto di Workfront (amministratori di sistema di Workfront):

* Ricevi un’e-mail con la data di inizio della migrazione utente pianificata (circa 30 giorni dopo il completamento di questi prerequisiti)
* Accedere alla console dell&#39;amministratore Workfront designata, dove è possibile modificare la data di migrazione

  >[!NOTE]
  >
  >A causa della complessità della migrazione, le modifiche della data sono limitate a non più di 30 giorni oltre la data pianificata. Contatta l’assistenza se hai bisogno di una data successiva.

* Ricevi un messaggio e-mail di promemoria 1 giorno prima della data di inizio della migrazione utente

### Prepara utenti per il giorno della migrazione

In qualità di amministratore del profilo di prodotto di Workfront (amministratore di sistema di Workfront), è responsabile di assicurare che tutti gli utenti siano pronti per la migrazione il giorno stesso.

* Prepara tutti gli utenti alla prossima migrazione ad Adobe Identity inviando loro le seguenti notifiche:

   * Durante la migrazione, gli utenti riceveranno un’e-mail da Adobe per informarli della modifica della modalità di accesso a Workfront. Gli utenti saranno invitati ad accettare un invito ad accedere utilizzando Adobe Identity per la prima volta, effettuando l’accesso con un Adobe ID esistente o configurandone uno nuovo utilizzando lo stesso indirizzo e-mail.

### Cosa aspettarsi il giorno della migrazione

* **La migrazione degli utenti inizierà alla mezzanotte del centro dati Workfront del cliente che ospita.**

* **Adobe eseguirà prima automaticamente la migrazione degli amministratori di Workfront.** Quando gli amministratori di Workfront verranno trasferiti ad Adobe Identity, avranno il ruolo di amministratore del profilo di prodotto di Adobe (amministratore di sistema di Workfront). Eventuali ruoli esistenti di un utente prima della migrazione non saranno interessati.

  >[!NOTE]
  >
  >Non si verificherà alcuna perdita di accesso al prodotto durante la migrazione degli utenti. Se un utente ha effettuato l’accesso durante il periodo di migrazione del suo utente, non ci sarà alcun impatto. Tuttavia, al prossimo accesso verrà richiesto di utilizzare la propria identità Adobe.



* **Durante la migrazione, gli utenti riceveranno un&#39;e-mail da Adobe per informarli della modifica della modalità di accesso a Workfront.** Gli utenti saranno invitati ad accettare un invito ad accedere con Adobe Identity per la prima volta, effettuando l&#39;accesso con un Adobe ID esistente o configurando un nuovo Adobe ID utilizzando lo stesso indirizzo e-mail.

  Per informazioni su come accedere a Workfront con un Adobe ID, vedere [Accedere a Adobe Experience Cloud](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud).

### Migrazione utente completata

Dopo la migrazione di tutti gli amministratori di sistema e gli utenti, Adobe invierà una notifica via e-mail a tutti gli amministratori di sistema e agli amministratori dei profili di prodotto (amministratori di sistema Workfront). In questo momento, tutti gli utenti di Workfront per tale istanza accederanno a Workfront utilizzando Adobe Identity. Gli amministratori di sistema di Workfront e gli amministratori dei profili di prodotto (amministratori di sistema di Workfront) possono gestire l’accesso degli utenti all’interno di Adobe Admin Console. Se i clienti non utilizzano una forma di sincronizzazione delle directory all’interno della console dell’amministratore, possono continuare a gestire l’accesso a Workfront all’interno dell’applicazione Workfront.

## Ottieni supporto

Per domande o dubbi, seguire i passaggi descritti nell&#39;articolo [Contattare l&#39;Assistenza clienti](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).




