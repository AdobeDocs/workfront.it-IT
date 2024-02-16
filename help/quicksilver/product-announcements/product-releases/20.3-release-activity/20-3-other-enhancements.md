---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 altri miglioramenti
description: Questa pagina descrive tutti gli altri miglioramenti apportati con la versione 20.3 all’ambiente di produzione. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana del 10 agosto 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6fef7261-114f-4c26-861e-61a4acb22d40
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 0%

---

# 20.3 altri miglioramenti

Questa pagina descrive tutti gli altri miglioramenti apportati con la versione 20.3 all’ambiente di produzione. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana del 10 agosto 2020.

Per un elenco di tutte le modifiche disponibili con la versione 20.3, consulta [Panoramica sulla versione 20.3](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Condividere un calendario con un collegamento privato

Per semplificare la condivisione dei calendari in Workfront, è possibile condividere un collegamento privato che porta gli utenti direttamente al calendario. Il calendario deve essere condiviso con l’utente che deve effettuare l’accesso per visualizzarlo.

In precedenza, era possibile condividere un URL pubblico che non richiedeva l’accesso per la visualizzazione.

Per ulteriori informazioni, consulta [Condivisione di un report calendario](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

## Nuova area Bozze durante la creazione di richieste

Per offrire maggiore flessibilità nell&#39;utilizzo delle richieste, Workfront salva automaticamente ogni richiesta creata come bozza nella nuova area Bozze. Se non disponi di tutte le informazioni necessarie per completare la nuova richiesta, puoi lasciarla come bozza, tornarci sopra e terminarla in un secondo momento. Workfront salva una richiesta per argomento della coda nella nuova area Bozze. Le bozze di richieste possono essere salvate per il tempo necessario fino a quando non si è pronti a completarle e inviarle. Potete anche rimuovere o riposizionare l&#39;area Bozze nel pannello sinistro utilizzando un modello di layout.

Per ulteriori informazioni sulla creazione delle richieste, consulta [Creare e inviare richieste Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

>[!NOTE]
>
>Per la versione di anteprima, se è stato assegnato un modello di layout personalizzato, sarà necessario aggiungere l’area Bozze delle richieste modificando il modello di layout.

## Espandere o comprimere gli elementi nella scheda orario

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront

Per gestire facilmente le schede orario con diversi elementi, ora puoi espandere o comprimere tutti gli elementi facendo clic su un pulsante.

In precedenza era necessario fare clic su ogni elemento singolarmente.

Per ulteriori informazioni, consulta [Tempo di connessione](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Ignora date effettive nei calendari Workfront

>[!NOTE]
>
>Questa funzione è stata rilasciata nell’ambiente di anteprima il 5 giugno 2020. Sarà disponibile nell’ambiente di produzione il 19 giugno 2020.

Per avere un maggiore controllo sulla visualizzazione degli oggetti nei Report calendario, è possibile scegliere di ignorare le date effettive anche quando sono disponibili.

In precedenza, il calendario utilizzava automaticamente le date effettive una volta disponibili.

Per ulteriori informazioni, consulta [Panoramica dei rapporti sul calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Utilizzare campi data personalizzati nei report calendario

>[!NOTE]
>
>Questa funzione è stata rilasciata nell’ambiente di anteprima il 29 maggio 2020. Sarà disponibile nell’ambiente di produzione il 12 giugno 2020.

Per aiutarti a visualizzare e gestire meglio il tuo lavoro quotidiano con i calendari, i campi data personalizzati sono ora disponibili come opzione data.

In precedenza, era possibile gestire il calendario solo con date pianificate e previste quando le date effettive non erano disponibili.

Per ulteriori informazioni, consulta [Utilizzare campi data personalizzati in un report calendario](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md) (o se utilizzi Workfront Classic, consulta [Utilizzare campi data personalizzati in un report calendario](https://one.workfront.com/s/article/Use-custom-date-fields-in-a-calendar-report-432597950?language=en_US)).

## Modifiche e-mail

**Modifiche e-mail in uscita:** Tutte le e-mail da Workfront verranno inviate da notifications@my.workfront.com. Ciò include avvisi automatizzati e comunicazione tra utenti.

In precedenza, gli amministratori di sistema potevano aggiungere un indirizzo e-mail personalizzato nell’area Email Setup (Configurazione e-mail).

**Modifiche alla risposta POP e-mail in entrata:** Gli amministratori di sistema non potranno più configurare un server e-mail POP personalizzato per le risposte e-mail in arrivo alle notifiche.

Per ulteriori informazioni, consulta [Modifiche e-mail di spoofing e risposta POP](https://one.workfront.com/s/article/Email-spoofing-and-POP-reply-email-changes?language=en_US).

## DKIM (DomainKeys Identified Mail) ora incluso nelle e-mail Workfront in uscita

In tutte le e-mail in uscita verrà inclusa una tecnica di autenticazione e-mail (DKIM). Questa firma DKIM non è visibile all’utente finale, ma consente la convalida a livello di server e rafforza il framework di autenticazione esistente.

## Aggiornamenti all’iscrizione alla nuova esperienza Workfront

Per rendere più gestibile l’iscrizione degli utenti alla nuova esperienza Workfront, gli amministratori di gruppi ora possono iscrivere e annullare l’iscrizione degli utenti che appartengono ai gruppi da essi gestiti.

È inoltre disponibile un collegamento Dettagli utente che consente di visualizzare le seguenti informazioni utente:

* Nome
* Ruolo
* Indirizzo e-mail
* Immagine del profilo

## Novità per gli amministratori: Brand Workfront per gruppi, team, ruoli e utenti specifici

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront

Ora è possibile utilizzare un modello di layout per modificare i loghi nell’area di navigazione superiore e nel menu principale per gruppi, team, mansioni e utenti specifici che dispongono di un proprio marchio.

Per ulteriori informazioni, consulta [Personalizza l’istanza di Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

## Gli amministratori di gruppi possono creare e gestire i processi di approvazione

Per consentire una maggiore autonomia e un maggiore controllo dei flussi di lavoro dei gruppi, un amministratore di gruppo può ora accedere all’area Processo di approvazione in Configurazione e creare e modificare i processi di approvazione per un gruppo che gestisce. Questi processi di approvazione si basano sugli stati del gruppo.

Per evitare che gli amministratori di gruppi modifichino inavvertitamente i processi di approvazione utilizzati nel sistema o creati da altri gruppi, possono accedere solo ai processi di approvazione associati ai gruppi che gestiscono.

Per ulteriori informazioni, consulta [Creare un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Per gli amministratori: la pagina Nuovi gruppi semplifica la creazione e la gestione dei gruppi

Gli amministratori di gruppi possono gestire i gruppi più facilmente ora che tutto ciò di cui hanno bisogno si trova nella nuova pagina Gruppi. Non è più necessario spostarsi tra le varie caselle di sovrapposizione e le pagine di impostazione per creare e modificare i gruppi.

Di seguito sono riportati i punti salienti:

* Dettagli gruppo: visualizza e modifica le informazioni di base sul gruppo, ad esempio il nome, la descrizione, i nomi degli amministratori del gruppo e se il gruppo è pubblico o privato.
* Elenco dei membri del gruppo: visualizza tutti i membri del gruppo e utilizza la nuova barra degli strumenti per aggiungere, rimuovere, esportare, attivare e disattivare rapidamente le appartenenze. È inoltre possibile modificare i profili dei membri e inviare loro commenti di aggiornamento.
* Campo Amministratore gruppo nell&#39;intestazione: quando visualizzi un gruppo che gestisci, assegna o rimuovi rapidamente l&#39;assegnazione di un membro del gruppo come amministratore. È possibile eseguire questa operazione anche nell&#39;elenco dei membri del gruppo utilizzando la nuova colonna Ruolo gruppo.
* Elenco sottogruppi: consente di visualizzare, modificare, copiare, esportare ed eliminare i sottogruppi di un gruppo gestito dall&#39;utente.
* Elenco stati: consente di visualizzare e gestire gli stati del gruppo.

Per ulteriori informazioni, consulta [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Novità per gli amministratori: creare fino a 14 livelli di sottogruppi

Per facilitare l’organizzazione dei gruppi Workfront in base alla gerarchia dell’organizzazione, sono stati aumentati da 3 a 14 i livelli dei sottogruppi che è possibile creare all’interno di un gruppo.

Per ulteriori informazioni, consulta [Panoramica sui gruppi](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Novità per gli amministratori: nuova barra laterale Configura

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront

La barra laterale sinistra in Configurazione è ora più veloce e facile da usare e sfrutta il layout di base e le funzionalità già note. Oltre a un look and feel più moderno, ecco le altre novità:

* Un nuovo sfondo biancastro nella barra laterale semplifica la differenziazione dal resto dell’area Setup.
* Le icone nella barra laterale sono un po&#39; più grandi e alcune sono riprogettate per suggerire più chiaramente cosa fa l&#39;opzione.
* Uno spazio verticale maggiore tra gli elementi della barra laterale ne facilita la lettura.
* È possibile comprimere la barra laterale quando è necessario spazio nell’area principale per visualizzare e fare di più, ad esempio per visualizzare colonne aggiuntive. Inoltre, è possibile espandere nuovamente la barra laterale quando è necessario visualizzare i nomi delle funzioni.
* Quando la barra laterale è compressa, vengono visualizzate solo le icone per ogni funzione. Per visualizzare le voci secondarie sotto una voce della barra laterale principale, posiziona il cursore del mouse sulla relativa icona per visualizzarle in un menu a comparsa. Ad esempio, passa il cursore del mouse sull’icona Processi per visualizzare un menu contenente Approvazioni e Percorsi milestone.
* È possibile accedere alle due opzioni Kick-Start (Importa dati ed Esporta dati) un clic più velocemente. Si sono spostati da sotto Sistema per visualizzare sul livello principale della barra laterale.

Per informazioni su come utilizzare l’area Configurazione, consulta [Amministrazione e configurazione](../../../administration-and-setup/administration-and-setup.md).

## Includi numero cluster nell&#39;area Informazioni cliente

In qualità di amministratore di Workfront, è ora possibile trovare facilmente il numero del cluster all&#39;interno di Workfront, senza dover dedicare più tempo e fatica a ottenerlo dal team di supporto. È stato aggiunto un campo Cluster Setup (Configurazione cluster) nell’area Customer Info (Informazioni cliente) di Setup.

Per informazioni sull&#39;area Informazioni cliente, vedere [Configurare le informazioni di base per il sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

## Codifica Base64 per sottoscrizioni eventi

Il campo base64Encoding è un campo facoltativo utilizzato per abilitare la codifica Base64 dei payload di abbonamento agli eventi. Se viene effettuata una richiesta utilizzando il campo base64Encoding impostato su true, gli oggetti newState e oldState nel payload vengono consegnati come stringhe di codifica Base64. Questa funzione può essere utile se la rete è configurata in modo da non consentire l&#39;utilizzo di caratteri speciali nelle sottoscrizioni di eventi.

Per ulteriori informazioni, consulta [API di abbonamento agli eventi](../../../wf-api/general/event-subs-api.md).

## È stata rimossa la possibilità di creare sottoscrizioni di eventi duplicate

Per evitare il recapito di messaggi duplicati, non è più possibile creare sottoscrizioni duplicate. Inoltre, tutte le sottoscrizioni duplicate create in precedenza sono state rimosse.

Per ulteriori informazioni, consulta [Domande frequenti - Abbonamenti agli eventi](../../../wf-api/general/event-subs-faq.md).
