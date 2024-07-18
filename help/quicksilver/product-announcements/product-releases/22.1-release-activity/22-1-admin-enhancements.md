---
title: 22.1 Miglioramenti per gli amministratori
description: 22.1 Miglioramenti per gli amministratori
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '1452'
ht-degree: 0%

---

# 22.1 Miglioramenti per gli amministratori

Questa pagina descrive tutti i miglioramenti per gli amministratori apportati con la versione 22.1 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la settimana del 17 gennaio 2022.

Per un elenco di tutte le modifiche disponibili con la versione 22.1, consulta la [panoramica sulla versione 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Download dei documenti registrati nell’area Aggiornamenti

Per consentire agli utenti di tenere traccia dei download dei documenti archiviati in Workfront, il sistema registra ora una voce nell&#39;area Aggiornamenti per un documento quando viene scaricato.

>[!NOTE]
>
>È consigliabile testare questa funzione in Anteprima su un documento appena caricato.

Per informazioni su come Workfront registra gli aggiornamenti automatici sugli oggetti, vedere [Aggiornamenti monitorati dal sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Concedere l’accesso ai team utilizzando i livelli di accesso

Una nuova sezione nell’area Livelli di accesso offre controlli più granulari per la gestione dell’accesso degli utenti ai team. Ora è possibile determinare chi può creare, modificare e visualizzare i team.

Ciò non modifica l’accesso esistente degli utenti ai team.

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## La mappatura dei gruppi è ora disponibile nei blueprint

Alcuni blueprint ora includono gruppi che puoi personalizzare prima di installarli. Puoi mappare un gruppo nella blueprint a un gruppo esistente nella tua istanza di Workfront, oppure puoi creare un nuovo gruppo, se necessario.

Per ulteriori informazioni, vedere [Configurare una blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Aggiornamenti degli stili nell’area Forms personalizzata

L’area Personalizza Forms ha un nuovo aspetto che lo rende aggiornato a molte altre aree della nuova esperienza Workfront.

## Numerosi miglioramenti per la creazione di campi personalizzati calcolati

La creazione di campi personalizzati calcolati è ora molto più semplice con queste aggiunte nel nuovo Editor di calcolo:

* È possibile passare il cursore del mouse su qualsiasi espressione del calcolo per visualizzarne le informazioni, incluse una descrizione, un esempio di come è possibile utilizzarla e un collegamento a ulteriori informazioni in un articolo della Guida.
* Ogni espressione aggiunta viene codificata in base al colore, a seconda del tipo. In questo modo è più semplice individuare le espressioni e riconoscerne immediatamente il tipo.
* I numeri di riga consentono di identificare e fare riferimento a funzioni in un calcolo lungo.
* Quando inizi a digitare un’espressione o un nome di campo, viene visualizzato un elenco di elementi disponibili in modo da poter scegliere quello desiderato. Quando si digita una parentesi aperta, la parentesi chiusa viene aggiunta automaticamente.
* È possibile visualizzare in anteprima il risultato del calcolo utilizzando un oggetto esistente senza uscire dall&#39;editor di calcolo.

Inoltre, nel testo personalizzabile delle &quot;Istruzioni&quot; al passaggio del mouse per un campo personalizzato calcolato, puoi visualizzare o nascondere la formula del campo. Questa opzione è utile se si ritiene che gli utenti che compileranno il modulo personalizzato non avranno bisogno di tali informazioni.

## Visualizzare le informazioni del registro di controllo relative agli stati e alle società

Ora è possibile risolvere più facilmente i problemi relativi a stati e aziende visualizzando le relative informazioni nell’area Registri di controllo in Configurazione.

Ad esempio:

* Puoi scoprire chi ha rinominato, bloccato o nascosto uno stato e quando lo ha fatto.
* Puoi scoprire chi ha rimosso alcuni membri o ruoli da un’azienda e quando lo ha fatto.

Per informazioni sulla visualizzazione delle informazioni del registro di controllo, vedere [Visualizzare ed esportare i registri di controllo](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Mappatura aziendale dei blueprint e altri miglioramenti

Sono ora disponibili i seguenti miglioramenti ai blueprint:

* Alcuni blueprint ora includono aziende, che puoi personalizzare prima di installare la blueprint. Puoi mappare una società nel blueprint a una società esistente nella tua istanza di Workfront, oppure puoi creare una nuova società, se necessario.
* È ora disponibile un nuovo tipo di blueprint, Struttura organizzativa. Alcuni blueprint includono elementi di più tipi (ad esempio, Modello di progetto e Struttura organizzativa). Puoi filtrare per tipo di blueprint nella pagina del catalogo.
* Le sezioni &quot;Preferenze di installazione&quot; e &quot;Proprietà del modello&quot; nella pagina di configurazione sono state unite in &quot;Preferenze modello&quot; per semplicità.

Per ulteriori informazioni, vedere [Configurare una blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Gestire più facilmente l&#39;iscrizione a una società

Nell’area Società, una barra degli strumenti aggiornata semplifica l’aggiunta di utenti Workfront esistenti a un’azienda e la rimozione dei membri dell’azienda.

In precedenza, queste azioni erano disponibili solo nella casella Modifica società.

La barra degli strumenti aggiornata contiene inoltre tutte le azioni disponibili nella barra degli strumenti precedente, ad esempio la modifica delle informazioni sul profilo utente dei membri e la loro disattivazione nel sistema.

Per ulteriori informazioni, vedere [Gestire le appartenenze alle società](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Selezionare espressioni e campi nella finestra Nuovo campo calcolato

Stiamo continuando a semplificare la creazione di un campo calcolato in un modulo personalizzato. Ora, quando si fa clic su Ingrandisci per aprire il nuovo Editor di calcolo, è possibile trovare e selezionare le espressioni e i campi necessari.

## I gruppi possono configurare le proprie preferenze per le ore e le schede orario

>[!NOTE]
>
>Questa funzione era inizialmente disponibile nell’ambito di un rollout graduale solo per i clienti nel cluster 4 come parte della versione 21.4. Questa funzione sarà disponibile per tutti i cluster rimanenti in Produzione l’8 novembre 2021.

In un’organizzazione di grandi dimensioni, alcuni gruppi potrebbero dover configurare le preferenze delle ore e delle schede orario in modo indipendente per adattarsi ai propri flussi di lavoro univoci, anziché ereditare le preferenze configurate da un amministratore a livello di sistema. Ora gli amministratori di Workfront possono sbloccare una scheda orario e una preferenza per le ore per tutti i gruppi del sistema in modo da poterla configurare autonomamente.

Questa funzionalità è stata aggiunta di recente anche per le preferenze del progetto e per le preferenze di attività e problemi.

Per informazioni su come un amministratore di Workfront sblocca una preferenza di tipo scheda orario e ora, vedere la sezione [Sbloccare le preferenze di tipo scheda orario e ora per i gruppi](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) nell&#39;articolo [Configurare le preferenze di tipo scheda orario e ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Per informazioni su come un amministratore di gruppo configura le attività sbloccate e le preferenze relative ai problemi per un gruppo, vedere [Configurare le preferenze relative alle ore e alle schede orario per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Seleziona più notifiche da sbloccare o ribloccare per i gruppi

Ora sbloccare o bloccare nuovamente le notifiche e-mail per i gruppi è più rapido e semplice. Ora è possibile selezionare più notifiche, verificare che le selezioni siano corrette, quindi fare clic sul nuovo pulsante Sblocca o Blocca visualizzato nella barra degli strumenti.

In precedenza, era necessario sbloccare e bloccare nuovamente le notifiche una alla volta. Workfront al momento ha 95 notifiche, quindi ci è voluto un po’ di tempo se dovevi farlo per tutte o per molte di esse.

Per ulteriori informazioni, vedere [Sbloccare o bloccare la configurazione delle notifiche degli eventi per tutti i gruppi](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## Per gli amministratori di gruppi: selezionare più facilmente un gruppo sostitutivo quando si elimina un gruppo

Quando si elimina un gruppo, due miglioramenti nella casella Elimina gruppo consentono di selezionare più facilmente il gruppo sostitutivo di cui si desidera mantenere gli utenti, gli elementi di lavoro e i sottogruppi del gruppo eliminato:

* È possibile iniziare a digitare il nome del gruppo per individuarlo rapidamente. In precedenza era disponibile solo un elenco a discesa che non era possibile digitare. Questo era problematico per le organizzazioni con molti gruppi, perché era necessario scorrere l’elenco per trovare il gruppo desiderato. Inoltre, l’elenco a discesa conteneva un limite di elementi, pertanto era possibile che il gruppo desiderato non venisse visualizzato.
* Puoi usare la nuova icona info per assicurarti di selezionare il gruppo sostitutivo desiderato. Passando il puntatore del mouse sull&#39;icona viene visualizzata una descrizione che elenca le informazioni sul gruppo, ad esempio la gerarchia dei gruppi al di sopra di esso e i nomi dei relativi amministratori.

Per ulteriori informazioni, vedere [Eliminare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## Area più ampia per la creazione di campi calcolati

Ora è più semplice creare campi calcolati complessi in un modulo personalizzato. Fare clic sul nuovo pulsante Ingrandisci per aprire una grande finestra di modifica per la creazione del calcolo. Al termine, fare clic su Riduci a icona per continuare a lavorare sul modulo personalizzato.

## Aggiungere moduli personalizzati ai gruppi

I moduli personalizzati sono ora supportati per l’oggetto Gruppo. In questo modo i gruppi dell&#39;organizzazione possono acquisire e condividere più facilmente le informazioni che soddisfano le esigenze e i flussi di lavoro specifici. Gli utenti possono eseguire le operazioni seguenti per un gruppo, come per altri oggetti di Workfront:

* Creare un modulo personalizzato
* Allegare un modulo personalizzato
* Salvare i dati del modulo personalizzato
* Rimuovere un modulo personalizzato
* Modificare i dati personalizzati dagli elenchi e, nella nuova esperienza Workfront, dalla pagina Gruppo

Per informazioni sui moduli personalizzati, vedere [Moduli personalizzati](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## Creazione di app OAuth2 per integrare le applicazioni con Workfront

Ora è possibile integrare Workfront con altre applicazioni per le quali Workfront non offre un&#39;integrazione incorporata. Creando un’app OAuth2 per l’applicazione con cui desideri essere integrato, puoi consentire all’applicazione di accedere a Workfront, sapendo al contempo che i tuoi dati sono protetti dal protocollo di autenticazione OAuth2 sicuro e standard del settore.

In precedenza, era possibile eseguire l’integrazione con altre applicazioni solo tramite integrazioni integrate, Workfront Fusion o l’API Workfront.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Miglioramenti al testo dell’interfaccia nell’area Società

Nell’area Società in Configurazione, i nuovi messaggi di conferma e le leggere modifiche redazionali semplificano la gestione delle appartenenze all’azienda. Ad esempio, il nome di sezione &quot;Persone&quot; nel pannello a sinistra è ora &quot;Membri dell’azienda&quot;.

Per informazioni sulla gestione delle appartenenze a società, vedere [Gestire le appartenenze a società](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
