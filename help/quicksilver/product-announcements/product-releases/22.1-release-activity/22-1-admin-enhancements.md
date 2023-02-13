---
title: Miglioramenti dell’amministratore 2.1
description: Miglioramenti dell’amministratore 2.1
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 0%

---

# Miglioramenti dell’amministratore 2.1

Questa pagina descrive tutti i miglioramenti apportati dall’amministratore all’ambiente di anteprima con la versione 22.1. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la settimana del 17 gennaio 2022.

Per un elenco di tutte le modifiche disponibili con la versione 22.1, vedi [Panoramica sulla versione 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Download di documenti registrati nell’area Aggiornamenti

Per consentire agli utenti di tenere traccia dei download dei documenti archiviati in Workfront, il sistema ora registra una voce nell’area Aggiornamenti di un documento quando qualcuno lo scarica.

>[!NOTE]
>
>È consigliabile testare questa funzione in Anteprima su un nuovo documento caricato.

Per informazioni sul modo in cui Workfront registra gli aggiornamenti automatici sugli oggetti, consulta [Aggiornamenti tracciati dal sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Concedere l’accesso ai team utilizzando i livelli di accesso

Una nuova sezione dell’area Livelli di accesso offre controlli più granulari per la gestione dell’accesso degli utenti ai team. Ora è possibile determinare chi può creare, modificare e visualizzare i team.

Questo non modifica l’accesso esistente degli utenti ai team.

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## La mappatura dei gruppi è ora disponibile nelle blueprint

Alcune blueprint ora includono gruppi, che è possibile personalizzare prima di installare la blueprint. Puoi mappare un gruppo nella blueprint a un gruppo esistente nella tua istanza Workfront, oppure crearne uno nuovo, se necessario.

Per ulteriori informazioni, consulta [Configurare una blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Aggiornamenti dello stile nell’area Custom Forms

L’area Personalizzato di Forms ha un nuovo aspetto e un nuovo aspetto che lo aggiorna con molte altre aree della nuova esperienza Workfront.

Per informazioni sulla creazione di un modulo personalizzato, vedere [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Molti miglioramenti per la creazione di campi personalizzati calcolati

La creazione di campi personalizzati calcolati è ora molto più semplice con queste aggiunte nel nuovo Editor di calcolo:

* Puoi passare il cursore sopra un’espressione del calcolo per visualizzare informazioni su di essa, inclusa una descrizione, un esempio di come può essere utilizzata e un collegamento per ulteriori informazioni in un articolo della guida.
* Ogni espressione aggiunta è codificata in colori, a seconda del tipo. In questo modo è più facile individuare le espressioni e riconoscerne immediatamente il tipo.
* I numeri di riga consentono di identificare e fare riferimento a funzioni in un calcolo lungo.
* Quando si inizia a digitare un&#39;espressione o un nome di campo, viene visualizzato un elenco di elementi disponibili, in modo da poter scegliere quello desiderato. E quando si digita una parentesi aperta, la parentesi di chiusura viene aggiunta automaticamente.
* È possibile visualizzare in anteprima il risultato del calcolo utilizzando un oggetto esistente senza uscire dall&#39;editor di calcolo.

Inoltre, nel testo personalizzato &quot;Istruzioni&quot; al passaggio del mouse per un campo personalizzato calcolato, è possibile visualizzare o nascondere la formula del campo. Questa funzione è utile se si ritiene che gli utenti che compileranno il modulo personalizzato non avranno bisogno di tali informazioni.

Per ulteriori informazioni sulla creazione di un campo personalizzato calcolato, consulta [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Visualizza informazioni del registro di controllo su stati e aziende

Ora è possibile risolvere più facilmente gli incidenti che coinvolgono stati e aziende visualizzandone le informazioni nell’area Registri di controllo in Configurazione.

Ad esempio:

* È possibile scoprire chi ha rinominato, bloccato o nascosto uno stato e quando lo ha fatto.
* Puoi scoprire chi ha rimosso alcuni membri o ruoli di lavoro da un&#39;azienda e quando l&#39;ha fatto.

Per informazioni sulla visualizzazione delle informazioni del registro di controllo, consulta [Visualizzare ed esportare i registri di controllo](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Mappatura aziendale Blueprint e altri miglioramenti

Sono ora disponibili i seguenti miglioramenti alla blueprint:

* Alcuni progetti ora includono aziende, che è possibile personalizzare prima di installare il modello. Puoi mappare una società nel blueprint a una società esistente nella tua istanza Workfront, oppure crearne una nuova se necessario.
* È ora disponibile un nuovo tipo di blueprint, Struttura organizzativa . Alcuni progetti includono elementi di più tipi (ad esempio, Modello di progetto e Struttura organizzativa). Puoi filtrare per tipo di blueprint nella pagina del catalogo.
* Le sezioni &quot;Preferenze di installazione&quot; e &quot;Proprietà modello&quot; nella pagina di configurazione sono state combinate in &quot;Preferenze modello&quot; per semplicità.

Per ulteriori informazioni, consulta [Configurare una blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Gestire più facilmente le iscrizioni aziendali

Nell’area Aziende, una barra degli strumenti aggiornata semplifica l’aggiunta di utenti Workfront esistenti a un’azienda e la rimozione di membri dell’azienda.

In precedenza, queste azioni erano disponibili solo nella casella Modifica società .

La barra degli strumenti aggiornata contiene anche tutte le azioni disponibili nella barra degli strumenti precedente, ad esempio la modifica delle informazioni sul profilo utente dei membri e la loro disattivazione nel sistema.

Per ulteriori informazioni, consulta [Gestire le iscrizioni aziendali](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Selezionare espressioni e campi nella nuova finestra campo calcolata

Stiamo continuando a semplificare la creazione di un campo calcolato in un modulo personalizzato. Ora, quando fai clic su Massimizza per aprire il nuovo editor di calcolo, puoi trovare e selezionare le espressioni e i campi necessari.

Per ulteriori informazioni, consulta [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## I gruppi possono configurare le proprie preferenze per la scheda attività e l&#39;ora

>[!NOTE]
>
>Questa funzione era inizialmente disponibile come parte di un rollout graduale solo per i clienti del cluster 4 come parte della versione 21.4. Questa funzione sarà disponibile per tutti i cluster rimanenti in Produzione l’8 novembre 2021.

In un&#39;organizzazione di grandi dimensioni, alcuni gruppi potrebbero dover configurare le preferenze relative alla scheda attività e alle ore in modo indipendente per adattarsi ai flussi di lavoro univoci, anziché ereditare le preferenze configurate da un amministratore a livello di sistema. Ora gli amministratori di Workfront possono sbloccare una scheda attività e una preferenza oraria per tutti i gruppi del sistema in modo che possano configurarla autonomamente.

Questa funzionalità è stata aggiunta di recente anche per le preferenze del progetto e per le preferenze relative a attività ed emissioni.

Per informazioni su come un amministratore di Workfront sblocca una scheda attività e una preferenza oraria, consulta la sezione . [Sblocca le preferenze della scheda attività e dell&#39;ora per i gruppi](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) nell&#39;articolo [Configurare le preferenze relative a schede attività e ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Per informazioni su come un amministratore di gruppo configura l&#39;attività sbloccata e genera le preferenze per un gruppo, consulta [Configurare le preferenze relative a schede attività e ora per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Seleziona più notifiche da sbloccare o bloccare nuovamente per i gruppi

È ora più rapido e semplice sbloccare o bloccare nuovamente le notifiche e-mail per i gruppi. Ora è possibile selezionare più notifiche, controllare le selezioni per verificare che siano corrette, quindi fare clic sul nuovo pulsante Sblocca o Blocca che viene visualizzato nella barra degli strumenti.

In precedenza, era necessario sbloccare e bloccare nuovamente le notifiche una alla volta. Workfront dispone attualmente di 95 notifiche, quindi ci è voluto un po&#39; se lo si dovesse fare per tutti o molti di loro.

Per ulteriori informazioni, consulta [Sblocca o blocca la configurazione delle notifiche degli eventi per tutti i gruppi](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## Per gli amministratori dei gruppi: Selezione più semplice di un gruppo di sostituzione quando si elimina un gruppo

Durante l&#39;eliminazione di un gruppo, due miglioramenti nella casella Elimina gruppo consentono di selezionare più facilmente il gruppo di sostituzione che si desidera mantenere gli utenti, gli elementi di lavoro e i sottogruppi del gruppo eliminato:

* È possibile iniziare a digitare il nome del gruppo per individuarlo rapidamente. In precedenza, non era possibile digitare alcun elenco a discesa. Questo problema si verificava per le organizzazioni con molti gruppi perché era necessario scorrere l&#39;elenco per trovare il gruppo desiderato. Inoltre, l&#39;elenco a discesa aveva un limite di elementi, quindi era possibile che il gruppo desiderato non fosse visualizzato.
* Puoi usare la nuova icona info per assicurarti di selezionare il gruppo di sostituzione desiderato. Passando il puntatore sull’icona viene visualizzata una descrizione comandi con informazioni sul gruppo, ad esempio la gerarchia dei gruppi al di sopra di esso e i nomi dei relativi amministratori.

Per ulteriori informazioni, consulta [Eliminare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## Area più grande per la creazione di campi calcolati

È ora più semplice creare campi calcolati complessi in un modulo personalizzato. Fai clic sul nuovo pulsante Massimizza per aprire una grande finestra di modifica per creare il calcolo. Al termine, fare clic su Riduci a icona per continuare a utilizzare il modulo personalizzato.

Per ulteriori informazioni, consulta [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Aggiungi moduli personalizzati ai gruppi

I moduli personalizzati sono ora supportati per l’oggetto Group . In questo modo i gruppi della tua organizzazione possono acquisire e condividere informazioni che soddisfano le loro esigenze e i loro flussi di lavoro specifici in modo più semplice. Gli utenti possono effettuare le seguenti operazioni per un gruppo, come per altri oggetti Workfront:

* Creazione di un modulo personalizzato
* Allegare un modulo personalizzato
* Salvare i dati del modulo personalizzato
* Rimuovere un modulo personalizzato
* Modificare dati personalizzati dagli elenchi e, nella nuova esperienza Workfront, dalla pagina Gruppo

Per informazioni sui moduli personalizzati, consulta [Moduli personalizzati](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## Creare app OAuth2 per integrare applicazioni con Workfront

Ora è possibile integrare Workfront con altre applicazioni per le quali Workfront non offre un’integrazione integrata. Creando un’app OAuth2 per l’applicazione con cui desideri eseguire l’integrazione, puoi consentire a tale applicazione di accedere a Workfront, pur sapendo che i tuoi dati sono protetti dal protocollo di autenticazione OAuth2, standard di settore e sicuro.

In precedenza era possibile effettuare l’integrazione solo con altre applicazioni tramite integrazioni integrate, Workfront Fusion o l’API Workfront.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Miglioramenti al testo dell&#39;interfaccia nell&#39;area Aziende

Nell’area Aziende in Configurazione, nuovi messaggi di conferma e lievi modifiche di formulazione facilitano la gestione delle iscrizioni aziendali. Ad esempio, il nome della sezione &quot;Persone&quot; nel pannello a sinistra è ora &quot;Membri dell&#39;azienda&quot;.

Per informazioni sulla gestione delle appartenenze aziendali, vedi [Gestire le iscrizioni aziendali](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
