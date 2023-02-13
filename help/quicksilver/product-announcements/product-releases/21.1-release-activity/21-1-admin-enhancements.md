---
content-type: release-notes
keywords: note,trimestrale,aggiornamento
navigation-topic: product-releases
title: Miglioramenti dell’amministratore 21.1
description: Questa pagina descrive tutti i miglioramenti apportati dall’amministratore all’ambiente Preview con la versione 21.1. Questi miglioramenti saranno resi disponibili nell'ambiente di produzione la settimana del 15 febbraio 2021.
author: Luke
feature: Product Announcements, System Setup and Administration
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 0%

---

# Miglioramenti dell’amministratore 21.1

Questa pagina descrive tutti i miglioramenti apportati dall’amministratore all’ambiente Preview con la versione 21.1. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione la settimana del 15 febbraio 2021.

Per un elenco di tutte le modifiche disponibili con la versione 21.1, vedi [Panoramica sulla versione 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Introduzione di una nuova impostazione del livello di accesso per la copia dei progetti

Per fornire un maggiore controllo, in qualità di amministratore di sistema, sulle operazioni che i planner possono eseguire con un progetto, abbiamo reso più dettagliato l’accesso Modifica ai progetti nel livello di accesso, introducendo una nuova impostazione che consente di abilitare o disabilitare la loro capacità di copiare i progetti. Prima di questa modifica, quando gli utenti avevano abilitato l’accesso a Modifica progetti, avevano automaticamente accesso per copiarli. Con la nuova funzione, è possibile consentire a un utente di modificare i progetti senza avere necessariamente accesso per copiarli disattivando la nuova impostazione Copia.

Se prima di questa modifica gli utenti avevano accesso a Modifica progetti nel proprio livello di accesso, questa impostazione verrà automaticamente attivata al momento del rilascio della funzione.

Per informazioni sul livello di accesso al piano, consulta [Concedere l’accesso ai progetti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Per informazioni sulla copia di un progetto, consulta [Copiare un progetto](../../../manage-work/projects/manage-projects/copy-project.md).

Questa funzione è ora inclusa nella [Nozioni di base sull’amministratore nella nuova esperienza Workfront, parte 1: Organizzazione utente](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) percorso di apprendimento su Workfront One.

## In un modulo personalizzato su un oggetto, selezionare tutti gli elementi in un campo a discesa con selezione multipla

>[!NOTE]
>
>Questa funzionalità non è attualmente disponibile quando si invia una nuova richiesta.

Nella pagina Dettagli relativa a un oggetto, quando si compila un campo a discesa con più selezioni in un modulo personalizzato, è possibile fare clic su Seleziona tutto per selezionare tutte le opzioni disponibili.

Per informazioni sulla modifica dei dati in un modulo personalizzato, consultare [Modificare le informazioni nei campi modulo personalizzati](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Ricalcolare tutti i campi modulo personalizzati per un oggetto

Ora è più facile assicurarsi che tutti i dati nei campi personalizzati calcolati siano correnti per un oggetto. Una nuova opzione di menu Ricalcola espressioni consente di ricalcolare rapidamente tutti i dati presenti in questi campi.

Questa funzione è particolarmente utile dopo che un utente modifica i dati in un altro oggetto a cui fa riferimento un campo personalizzato calcolato nell’oggetto.

In precedenza, gli utenti dovevano utilizzare soluzioni alternative per assicurarsi che tutti i dati nei campi personalizzati calcolati fossero correnti. Ad esempio, hanno modificato l’oggetto insieme ad altri oggetti per utilizzare l’opzione di ricalcolo disponibile per la modifica collettiva.

Per ulteriori informazioni, consulta [Modificare le informazioni nei campi modulo personalizzati](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Sblocca attività e visualizza le preferenze relative ai problemi per gli amministratori dei gruppi

>[!NOTE]
>
>Fino al 24 giugno 2021, questa funzione era disponibile come parte di un rollout graduale solo per i clienti che hanno la possibilità di sbloccare le preferenze di progetto per gruppi. Ora è disponibile per tutti i clienti.

Gli amministratori di Adobe Workfront ora possono concedere agli amministratori di gruppo maggiore autonomia sbloccando singole attività e rilasciando preferenze per i problemi. Quando una preferenza viene sbloccata, gli amministratori di gruppo possono configurarla in modo che i gruppi soddisfino le esigenze specifiche di ciascun gruppo e i processi interni.

Per ulteriori informazioni, consulta [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

Questa funzione è ora inclusa nella [Nozioni di base sull’amministratore nella nuova esperienza Workfront, parte 2: Configurazione del progetto](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-1-project-workfl-MCTBVZ3Q3J5RHNLIPPZPFSQRLKUY) percorso di apprendimento su Workfront One.

## Configura separatamente le impostazioni del livello di accesso per portfolio e programmi

Ora è più semplice gestire l’accesso degli utenti a portfolio e programmi, in quanto è possibile configurare separatamente le relative impostazioni del livello di accesso.

In precedenza, le impostazioni del livello di accesso per portfolio e programmi venivano combinate. Ciò significa che non è stato possibile configurare le impostazioni di accesso per i programmi senza configurarli nello stesso modo per i portfolio, e lo stesso vale al contrario.

Per informazioni sulla configurazione di un livello di accesso, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Per informazioni sulle impostazioni di accesso che è possibile configurare per programmi e portfolio, consulta [Accesso configurabile alla funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

Questa funzione è ora inclusa nella [Nozioni di base sull’amministratore nella nuova esperienza Workfront, parte 1: Organizzazione utente](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) percorso di apprendimento su Workfront One.

## Selezionare tutte le caselle di controllo di una serie durante la modifica di informazioni in un modulo personalizzato

>[!NOTE]
>
>Questa funzionalità non è attualmente disponibile quando si invia una nuova richiesta.

Nella pagina Dettagli relativa a un oggetto, quando si compila un campo Modulo personalizzato contenente caselle di controllo, è possibile fare clic su Seleziona tutto per selezionare tutte le caselle di controllo disponibili.

Questa opzione viene visualizzata solo se il campo contiene più di 2 caselle di controllo.

Per ulteriori informazioni, consulta [Modificare le informazioni nei campi modulo personalizzati](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Configurare l’inserire nell&#39;elenco Consentiti di posta elettronica Workfront

Per proteggere meglio i dati, ora puoi utilizzare un inserire nell&#39;elenco Consentiti di dominio e-mail per:

* Controlla dove possono andare le e-mail di Workfront se contengono rapporti o documenti archiviati in Workfront
* I domini e-mail di controllo possono trovarsi nell’indirizzo e-mail che gli utenti possono specificare nel loro profilo utente

Ad esempio, se desideri proteggere i dati sensibili, ad esempio un report che elenca i clienti a rischio, puoi includere solo il dominio o i domini di e-mail interni nell’inserire nell&#39;elenco Consentiti e-mail. In questo modo, gli utenti non possono inviare quel rapporto (o qualsiasi altro rapporto Workfront) a un indirizzo e-mail esterno.

Per ulteriori informazioni, consulta la sezione . [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur) nell&#39;articolo [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Assegnare un amministratore di gruppo a un sottogruppo

Per facilitare il funzionamento indipendente dei livelli dell’organizzazione, abbiamo aggiunto la possibilità di assegnare un amministratore di gruppo a un sottogruppo. Ora puoi verificare di delegare la gestione dei sottogruppi alle persone giuste.

In precedenza, solo un gruppo di primo livello poteva avere Amministratori di gruppo e tali amministratori gestivano tutti i sottogruppi sotto il gruppo di primo livello.

Per ulteriori informazioni, consulta la sezione . [Amministratori di gruppo per sottogruppi](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for) nell&#39;articolo [Panoramica sui sottogruppi](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

Questa funzione è ora inclusa nella [Nozioni di base sull’amministratore nella nuova esperienza Workfront, parte 1: Organizzazione utente](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) percorso di apprendimento su Workfront One.

## Configurare le notifiche evento per i gruppi

>[!NOTE]
>
>Disponibile come parte di un rollout graduale solo per i clienti che possono sbloccare le preferenze di progetto per gruppi. Ciò include tutti i clienti dei cluster 4 e 6 e un numero ridotto di clienti di altri cluster. Questa nota verrà aggiornata man mano che la funzionalità diventa disponibile per più cluster.

Gli amministratori di Workfront possono ora concedere agli amministratori di gruppo maggiore autonomia consentendo loro di configurare le notifiche degli eventi per i gruppi di primo livello. I sottogruppi ereditano le configurazioni di notifica degli eventi dal gruppo principale.

In precedenza, le notifiche degli eventi erano configurabili solo da un amministratore Workfront a livello di sistema, il che significa che tutti i gruppi dovevano utilizzare lo stesso set di notifiche degli eventi.

Per ulteriori informazioni, consulta i seguenti articoli:

* [Sblocca o blocca la configurazione delle notifiche degli eventi per tutti i gruppi](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [Visualizzare e configurare le notifiche evento per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

Questa funzione è ora inclusa nella [Nozioni di base sull’amministratore nella nuova esperienza Workfront, parte 1: Organizzazione utente](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) percorso di apprendimento su Workfront One.

Questa funzione è ora inclusa nella [Notifiche e-mail e in-app nella nuova esperienza Workfront](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) percorso di apprendimento su Workfront One.

## Lavorare con progetti di gruppo e processi di approvazione nell&#39;area Gruppi

Se sei un amministratore di gruppo, è facile visualizzare e lavorare con i progetti e i processi di approvazione del gruppo ora che sono elencati nell&#39;area Gruppi. Dalla pagina principale di un gruppo puoi effettuare le seguenti operazioni:

* Fai clic su Progetti nel menu a sinistra per visualizzare i progetti del gruppo e crearne di nuovi per il gruppo. Se un progetto selezionato è stato condiviso con te, puoi utilizzare i pulsanti nella barra degli strumenti per modificarlo, esportarlo, copiarlo o eliminarlo.

   Per ulteriori informazioni, consulta [Creare e modificare i progetti di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

* Fai clic su Approvazioni nel menu a sinistra per visualizzare e gestire tutti i processi di approvazione associati al gruppo.

   Per ulteriori informazioni, consulta [Processi di approvazione a livello di gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

Questa funzionalità è disponibile anche per gli amministratori di Workfront.

## Visualizza il numero di licenze utilizzate e allocate in un gruppo

Per determinare la distribuzione delle licenze, è ora possibile visualizzare il numero di licenze utilizzate in un gruppo ed eventuali sottogruppi sottostanti.

Se gestisci un gruppo di livello principale, puoi visualizzare sia il numero di licenze utilizzate in un gruppo (e i relativi sottogruppi) sia il numero massimo di licenze allocate per il gruppo.

Per ulteriori informazioni, consulta [Visualizza il numero di licenze allocate e utilizzate in un gruppo nella nuova esperienza Adobe Workfront](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

