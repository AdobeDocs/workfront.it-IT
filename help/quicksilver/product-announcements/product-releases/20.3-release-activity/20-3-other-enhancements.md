---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 altri miglioramenti
description: Questa pagina descrive tutti gli altri miglioramenti effettuati con la versione 20.3 nell’ambiente di produzione. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana del 10 agosto 2020.
author: Luke
feature: Product Announcements
exl-id: 6fef7261-114f-4c26-861e-61a4acb22d40
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1510'
ht-degree: 0%

---

# 20.3 altri miglioramenti

Questa pagina descrive tutti gli altri miglioramenti effettuati con la versione 20.3 nell’ambiente di produzione. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana del 10 agosto 2020.

Per un elenco di tutte le modifiche disponibili con la versione 20.3, vedi [Panoramica sulla versione 20.3](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## Condividere un calendario con un collegamento privato

Per semplificare la condivisione dei calendari in Workfront, puoi condividere un collegamento privato che porta gli utenti direttamente al calendario. Il calendario deve essere condiviso con l&#39;utente e deve accedere per visualizzarlo.

In precedenza, era possibile condividere un URL pubblico che non richiedeva un accesso per la visualizzazione.

Per ulteriori informazioni, consulta [Condivisione di un rapporto calendario](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

## Nuova area Bozze durante la creazione di richieste

Per offrirti maggiore flessibilità quando lavori con le richieste, Workfront ora salva automaticamente ogni richiesta creata come bozza nella nuova area Bozze. Se non disponi di tutte le informazioni necessarie per completare la nuova richiesta, puoi lasciarla come bozza, tornare ad essa e finirla in seguito. Workfront salva una richiesta per argomento della coda nella nuova area Bozze. Le bozze di richiesta possono essere salvate per tutto il tempo necessario fino a quando non saranno pronte per essere completate e inviate. È inoltre possibile rimuovere o riposizionare l’area Bozze nel pannello a sinistra utilizzando un modello di layout.

Per ulteriori informazioni sulla creazione delle richieste, vedi [Creare e inviare richieste Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

>[!NOTE]
>
>Per la versione Anteprima, se ti è stato assegnato un modello di layout personalizzato, dovrai aggiungere l’area Bozze delle richieste modificando il modello di layout.

## Espandere o comprimere gli elementi nella scheda attività

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront

Per gestire facilmente i fogli presenze con diversi elementi, ora puoi espandere o comprimere tutti gli elementi facendo clic su un pulsante.

In precedenza era necessario fare clic su ogni elemento singolarmente.

Per ulteriori informazioni, consulta [Tempo di log](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Ignora date effettive nei calendari Workfront

>[!NOTE]
>
>Questa funzione è stata rilasciata nell’ambiente Preview il 5 giugno 2020. Sarà disponibile nell’ambiente Produzione il 19 giugno 2020.

Per avere un maggiore controllo sulla modalità di visualizzazione degli oggetti nei Rapporti calendario, puoi scegliere di ignorare le date effettive anche quando sono disponibili.

In precedenza, il calendario utilizzava automaticamente le date effettive una volta disponibili.

Per ulteriori informazioni, consulta [Panoramica dei rapporti sul calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Utilizzare campi data personalizzati nei rapporti calendario

>[!NOTE]
>
>Questa funzione è stata rilasciata nell’ambiente Preview il 29 maggio 2020. Sarà disponibile nell’ambiente Produzione il 12 giugno 2020.

Per visualizzare e gestire meglio il lavoro quotidiano con i calendari, i campi data personalizzati sono ora disponibili come opzione data.

In precedenza, era possibile gestire il calendario solo con le date previste e pianificate quando le date effettive non erano disponibili.

Per ulteriori informazioni, consulta [Utilizzare campi data personalizzati in un rapporto calendario](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md) (o se utilizzi Workfront Classic, consulta [Utilizzare campi data personalizzati in un rapporto calendario](https://one.workfront.com/s/article/Use-custom-date-fields-in-a-calendar-report-432597950?language=en_US)).

## Modifiche e-mail

**Modifiche e-mail in uscita:** Tutte le e-mail da Workfront verranno inviate da notifications@my.workfront.com. Ciò include avvisi automatizzati e comunicazioni da utente a utente.

In precedenza, gli amministratori di sistema potevano aggiungere un indirizzo e-mail personalizzato nell’area Configurazione e-mail.

**Modifiche alla risposta POP in entrata:** Gli amministratori di sistema non potranno più configurare un server e-mail POP personalizzato per le risposte e-mail in arrivo alle notifiche.

Per ulteriori informazioni, consulta [Modifiche e-mail di spoofing e risposta POP](https://one.workfront.com/s/article/Email-spoofing-and-POP-reply-email-changes?language=en_US).

## DomainKeys Identified Mail (DKIM) ora incluso nelle e-mail Workfront in uscita

Una tecnica di autenticazione e-mail (DKIM) sarà inclusa in tutte le e-mail in uscita. Questa firma DKIM non è visibile all’utente finale, ma consente la convalida a livello di server e rafforza il framework di autenticazione esistente.

## Aggiornamenti alla registrazione nella nuova esperienza Workfront

Per rendere più gestibile l’iscrizione degli utenti alla nuova esperienza Workfront, gli amministratori dei gruppi possono ora accedere all’iscrizione e all’annullamento dell’iscrizione degli utenti appartenenti ai gruppi gestiti.

È disponibile anche un collegamento Dettagli utente che visualizza le seguenti informazioni utente:

* Nome
* Ruolo
* Indirizzo e-mail
* Immagine del profilo

## Novità per gli amministratori: Brand Workfront per gruppi, team, ruoli e utenti specifici

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront

Ora è possibile utilizzare un modello di layout per modificare i loghi nell’area di navigazione superiore e nel menu principale per gruppi, team, ruoli di lavoro e utenti con un proprio marchio.

Per ulteriori informazioni, consulta [Brand your Adobe Workfront instance](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

## Gli amministratori dei gruppi possono creare e gestire i processi di approvazione

Per consentire maggiore autonomia e controllo dei flussi di lavoro dei gruppi, un amministratore di gruppo può ora accedere all&#39;area Processo di approvazione in Configurazione e creare e modificare i processi di approvazione per un gruppo gestito. Questi processi di approvazione si basano sugli stati di quel gruppo.

Per garantire che gli amministratori dei gruppi non modifichino inavvertitamente i processi di approvazione utilizzati in tutto il sistema o creati da altri gruppi, possono accedere solo ai processi di approvazione associati ai gruppi gestiti.

Per ulteriori informazioni, consulta [Creazione di un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Per gli amministratori: La nuova pagina Gruppi facilita la creazione e la gestione dei gruppi

Gli amministratori dei gruppi possono gestire più facilmente i gruppi ora che tutto ciò di cui hanno bisogno si trova nella nuova pagina Gruppi . Non è più necessario navigare tra le varie caselle di sovrapposizione e le pagine di configurazione per creare e modificare i gruppi.

Ecco i principali punti salienti:

* Dettagli gruppo: Visualizzare e modificare le informazioni di base sul gruppo, ad esempio il nome, la descrizione, i nomi degli amministratori del gruppo e se il gruppo è pubblico o privato.
* Elenco dei membri del gruppo: Visualizzare tutti i membri del gruppo e utilizzare la nuova barra degli strumenti per aggiungere, rimuovere, esportare, attivare e disattivare rapidamente le appartenenze. È inoltre possibile modificare i profili dei membri e inviare loro i commenti relativi all’aggiornamento.
* Campo Amministratore gruppo nell’intestazione: Quando si visualizza un gruppo gestito, assegnare o annullare rapidamente l&#39;assegnazione di un membro del gruppo come amministratore del gruppo. Puoi eseguire questa operazione anche nell’elenco dei membri del gruppo utilizzando la nuova colonna Ruolo gruppo .
* Elenco dei sottogruppi: Visualizzare, modificare, copiare, esportare ed eliminare i sottogruppi in un gruppo gestito.
* Elenco stati: Visualizza e gestisci gli stati del gruppo.

Per ulteriori informazioni, consulta [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Novità per gli amministratori: Creare fino a 14 livelli di sottogruppi

Per organizzare più facilmente i gruppi Workfront in modo che corrispondano alla gerarchia aziendale, sono stati aumentati i livelli di sottogruppi che è possibile creare all’interno di un gruppo da 3 a 14.

Per ulteriori informazioni, consulta [Panoramica sui gruppi](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Novità per gli amministratori: Nuova barra laterale di configurazione

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront

La barra laterale sinistra in Configurazione è ora più veloce e facile da utilizzare e sfrutta il layout e le funzionalità di base già noti. Insieme a un look e una sensazione più moderni, ecco cos&#39;altro è nuovo:

* Il nuovo sfondo bianco nella barra laterale facilita la differenziazione dal resto dell&#39;area di configurazione.
* Le icone nella barra laterale sono un po&#39; più grandi e alcune sono riprogettate per suggerire più chiaramente cosa fa l&#39;opzione.
* Uno spazio verticale maggiore tra gli elementi della barra laterale facilita la lettura.
* È possibile comprimere la barra laterale quando è necessario spazio nell&#39;area principale per visualizzare e fare di più, ad esempio per visualizzare ulteriori colonne. E potete espandere nuovamente la barra laterale quando avete bisogno di vedere i nomi delle feature.
* Quando la barra laterale viene ridotta, vengono visualizzate solo le icone per ogni feature. Per visualizzare le voci secondarie sotto una voce della barra laterale principale, posiziona il cursore del mouse sulla relativa icona per visualizzarle in un menu a comparsa. Ad esempio, passa il puntatore sull’icona Processi per visualizzare un menu contenente Approvazioni e Percorsi cardine.
* Puoi accedere alle due opzioni di avvio rapido (Importa dati ed Esporta dati) con un clic più veloce. Si sono spostati da sotto Sistema per visualizzare il livello principale della barra laterale.

Per informazioni sull&#39;utilizzo dell&#39;area Configurazione, consulta [Amministrazione e configurazione](../../../administration-and-setup/administration-and-setup.md).

## Includi il numero del cluster nell&#39;area Informazioni cliente

In qualità di amministratore di Workfront, è ora possibile trovare facilmente il numero del cluster all&#39;interno di Workfront, senza dover spendere tempo e sforzi aggiuntivi per ottenerlo dal nostro team di supporto. È stato aggiunto un campo Configurazione cluster nell&#39;area Informazioni cliente di Configurazione.

Per informazioni sull&#39;area Informazioni cliente, consulta [Configurare le informazioni di base per il sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

## Codifica Base64 per sottoscrizioni di eventi

Il campo base64Encoding è un campo facoltativo utilizzato per abilitare la codifica Base64 dei payload di abbonamento agli eventi. Se una richiesta viene effettuata utilizzando il campo base64Encoding impostato su true, gli oggetti newState e oldState nel payload vengono consegnati come stringhe di codifica Base64. Questa funzione può essere utile se la rete è configurata in modo da non consentire l’uso di caratteri speciali nelle sottoscrizioni di eventi.

Per ulteriori informazioni, consulta [API iscrizione agli eventi](../../../wf-api/general/event-subs-api.md).

## È stata rimossa la possibilità di creare sottoscrizioni di eventi duplicate

Per evitare la consegna di messaggi duplicati, non puoi più creare sottoscrizioni duplicate. Inoltre, tutte le sottoscrizioni duplicate create in precedenza sono state rimosse.

Per ulteriori informazioni, consulta [Domande frequenti - Abbonamenti agli eventi](../../../wf-api/general/event-subs-faq.md).
