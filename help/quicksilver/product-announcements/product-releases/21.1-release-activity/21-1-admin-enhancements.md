---
content-type: release-notes
keywords: note,trimestrale,aggiornamento
navigation-topic: product-releases
title: 21.1 Miglioramenti per gli amministratori
description: Questa pagina descrive tutti i miglioramenti per gli amministratori apportati con la versione 21.1 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione la settimana del 15 febbraio 2021.
author: Luke
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: 6fe1a2c71f53d6b314c2b1402a547f9c934bfbea
workflow-type: tm+mt
source-wordcount: '1347'
ht-degree: 0%

---

# 21.1 Miglioramenti per gli amministratori

Questa pagina descrive tutti i miglioramenti per gli amministratori apportati con la versione 21.1 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione la settimana del 15 febbraio 2021.

Per un elenco di tutte le modifiche disponibili con la versione 21.1, consulta la [panoramica sulla versione 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Introduzione di una nuova impostazione del livello di accesso per la copia dei progetti

Per consentirti di controllare meglio, in qualità di amministratore di sistema, le operazioni che i responsabili della pianificazione possono eseguire con un progetto, abbiamo reso più granulare l’accesso di modifica ai progetti nel livello di accesso, introducendo una nuova impostazione che consente di abilitare o disabilitare la possibilità di copiare i progetti. Prima di questa modifica, quando abilitavi l’accesso degli utenti a Modifica progetti, questi potevano automaticamente copiarli. Con la nuova funzione, puoi consentire a un utente di modificare i progetti senza necessariamente averne accesso alla copia disabilitando la nuova impostazione Copia.

Se gli utenti disponevano dell’accesso Modifica progetti nel proprio livello di accesso prima di questa modifica, questa impostazione veniva abilitata automaticamente al momento del rilascio di questa funzione.

Per informazioni sul livello di accesso Piano, vedere [Concedere l&#39;accesso ai progetti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Per informazioni sulla copia di un progetto, vedere [Copiare un progetto](../../../manage-work/projects/manage-projects/copy-project.md).

Questa funzionalità è ora inclusa in [Nozioni di base per gli amministratori nella nuova esperienza Workfront, parte 1: percorso di apprendimento Organizzazione utente](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) in Workfront One.

## In un modulo personalizzato su un oggetto, seleziona tutti gli elementi in un campo a discesa a selezione multipla

>[!NOTE]
>
>Questa funzionalità non è attualmente disponibile quando si invia una nuova richiesta.

Nella pagina Dettagli di un oggetto, quando si compila un campo a discesa a selezione multipla in un modulo personalizzato, è possibile fare clic su Seleziona tutto se è necessario selezionare tutte le opzioni disponibili.

Per informazioni sulla modifica dei dati in un modulo personalizzato, vedere [Modificare le informazioni nei campi modulo personalizzato](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Ricalcolare tutti i campi modulo personalizzato per un oggetto

Ora è più facile assicurarsi che tutti i dati nei campi personalizzati calcolati siano correnti per un oggetto. Una nuova opzione di menu Ricalcola espressioni consente di ricalcolare rapidamente tutti i dati contenuti in questi campi.

Questa funzione è particolarmente utile quando qualcuno modifica dati in un altro oggetto a cui fa riferimento un campo personalizzato calcolato nell’oggetto.

In precedenza, gli utenti dovevano utilizzare soluzioni alternative per assicurarsi che tutti i dati nei campi personalizzati calcolati fossero correnti. Ad esempio, hanno modificato l’oggetto insieme ad altri oggetti per utilizzare l’opzione di ricalcolo disponibile per la modifica in serie.

Per ulteriori informazioni, vedere [Modificare le informazioni nei campi modulo personalizzato](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Sblocca le preferenze per attività e problemi per gli amministratori di gruppi

>[!NOTE]
>
>Fino al 24 giugno 2021, questo era disponibile come parte di un rollout graduale solo per i clienti che possono sbloccare le preferenze di progetto per i gruppi. Ora è disponibile per tutti i clienti.

Gli amministratori di Adobe Workfront ora possono dare agli amministratori di gruppi più autonomia sbloccando le preferenze di singole attività e problemi. Quando una preferenza viene sbloccata, gli amministratori di gruppi possono configurarla per i propri gruppi in modo da soddisfare le esigenze specifiche e i processi interni di ciascun gruppo.

Per ulteriori informazioni, consulta [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

Questa funzionalità è ora inclusa in [Nozioni di base per gli amministratori nella nuova esperienza Workfront, parte 2: Percorso di apprendimento per la configurazione del progetto](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) in Workfront One.

## Configurare separatamente le impostazioni del livello di accesso per portfolio e programmi

Ora è più semplice gestire l’accesso degli utenti a portfolio e programmi, in quanto è possibile configurare separatamente le impostazioni del livello di accesso.

In precedenza, venivano combinate le impostazioni del livello di accesso per portfolio e programmi. Non era quindi possibile configurare le impostazioni di accesso per i programmi senza configurarle allo stesso modo per i portfolio, e lo stesso si verificava al contrario.

Per informazioni sulla configurazione di un livello di accesso, vedere [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Per informazioni sulle impostazioni di accesso che è possibile configurare per programmi e portfolio, vedere [Accesso configurabile alle funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

Questa funzionalità è ora inclusa in [Nozioni di base per gli amministratori nella nuova esperienza Workfront, parte 1: percorso di apprendimento Organizzazione utente](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) in Workfront One.

## Selezionare tutte le caselle di controllo di una serie durante la modifica delle informazioni in un modulo personalizzato

>[!NOTE]
>
>Questa funzionalità non è attualmente disponibile quando si invia una nuova richiesta.

Nella pagina Dettagli di un oggetto, quando si compila un campo Modulo personalizzato contenente caselle di controllo, è possibile fare clic su Seleziona tutto se è necessario selezionare tutte le caselle di controllo disponibili.

Questa opzione viene visualizzata solo se il campo contiene più di 2 caselle di controllo.

Per ulteriori informazioni, vedere [Modificare le informazioni nei campi modulo personalizzato](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Configurare il Workfront di e-mail di inserire nell&#39;elenco Consentiti

Per una migliore protezione dei dati, ora puoi utilizzare un dominio e-mail in modo che si inserisca nell&#39;elenco Consentiti a:

* Controlla dove possono andare le e-mail di Workfront se contengono rapporti o documenti memorizzati in Workfront
* I domini e-mail di controllo possono trovarsi nell’indirizzo e-mail che gli utenti possono specificare nel loro profilo utente

Ad esempio, se desideri proteggere i dati sensibili, ad esempio un rapporto che elenca i clienti a rischio, puoi includere nel inserisco nell&#39;elenco Consentiti di gestione delle e-mail solo il dominio o i domini e-mail interni. In questo modo, gli utenti non possono inviare tale rapporto (o qualsiasi altro rapporto di Workfront) a un indirizzo e-mail esterno.

Per ulteriori informazioni, vedere la sezione [Configurare il inserisco nell&#39;elenco Consentiti di  del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur) nell&#39;articolo [Configurare il inserisco nell&#39;elenco Consentiti di  del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Assegnare un amministratore di gruppo a un sottogruppo

Per facilitare il funzionamento indipendente dei livelli dell’organizzazione, è stata aggiunta la possibilità di assegnare un amministratore di gruppo a un sottogruppo. A questo punto è possibile assicurarsi di delegare la gestione dei sottogruppi alle persone giuste.

In precedenza, solo un gruppo di primo livello poteva avere Amministratori di gruppo e questi amministratori gestivano tutti i sottogruppi al di sotto del gruppo di primo livello.

Per ulteriori informazioni, vedere la sezione [Amministratori di gruppi per i sottogruppi](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for) nell&#39;articolo [Panoramica sui sottogruppi](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

Questa funzionalità è ora inclusa in [Nozioni di base per gli amministratori nella nuova esperienza Workfront, parte 1: percorso di apprendimento Organizzazione utente](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) in Workfront One.

## Configurare le notifiche degli eventi per i gruppi

>[!NOTE]
>
>Disponibile come parte di un rollout graduale solo per i clienti che hanno la possibilità di sbloccare le preferenze di progetto per i gruppi. Questo include tutti i clienti dei cluster 4 e 6 e un numero limitato di clienti di altri cluster. Questa nota verrà aggiornata man mano che la funzionalità sarà disponibile per più cluster.

Gli amministratori di Workfront ora possono dare maggiore autonomia agli amministratori di gruppi consentendo loro di configurare le notifiche degli eventi per i loro gruppi di livello superiore. I sottogruppi ereditano le configurazioni di notifica degli eventi dal gruppo padre principale.

In precedenza, le notifiche degli eventi potevano essere configurate solo da un amministratore Workfront a livello di sistema, il che significa che tutti i gruppi dovevano utilizzare lo stesso set di notifiche degli eventi.

Per ulteriori informazioni, consulta i seguenti articoli:

* [Sblocca o blocca la configurazione delle notifiche degli eventi per tutti i gruppi](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [Visualizzare e configurare le notifiche degli eventi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

<!--This feature is now included in the [Administrator Fundamentals in the new Workfront experience, Part 1: User Organization](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) learning path on Workfront One.

This feature is now included in the [Email and In-App Notifications in the new Workfront experience](https://experienceleague.adobe.com/en/docs/workfront/using/home://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) learning path on Workfront One.-->

## Utilizzare progetti di gruppo e processi di approvazione nell&#39;area Gruppi

Gli amministratori di gruppi possono visualizzare e utilizzare facilmente i progetti e i processi di approvazione del gruppo ora che sono elencati nell&#39;area Gruppi. Dalla pagina principale di un gruppo è possibile:

* Fate clic su Progetti (Projects) nel menu a sinistra per visualizzare i progetti del gruppo e crearne di nuovi. Se un progetto selezionato è stato condiviso con te, puoi utilizzare i pulsanti nella barra degli strumenti per modificarlo, esportarlo, copiarlo o eliminarlo.

  Per ulteriori informazioni, vedere [Creare e modificare i progetti di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

* Fai clic su Approvazioni nel menu a sinistra per visualizzare e gestire tutti i processi di approvazione associati al gruppo.

  Per ulteriori informazioni, vedere [Processi di approvazione a livello di gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

Questa funzionalità è disponibile anche per gli amministratori di Workfront.

## Visualizza il numero di licenze utilizzate e assegnate in un gruppo

Per determinare il livello di distribuzione delle licenze, è ora possibile visualizzare il numero di licenze utilizzate in un gruppo ed eventuali sottogruppi al di sotto di esso.

Se si gestisce un gruppo di primo livello, è possibile visualizzare sia il numero di licenze utilizzate in un gruppo (e nei relativi sottogruppi) sia il numero massimo di licenze allocate per il gruppo.

Per ulteriori informazioni, consulta [Visualizzare il numero di licenze allocate e utilizzate in un gruppo nella nuova esperienza Adobe Workfront](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

