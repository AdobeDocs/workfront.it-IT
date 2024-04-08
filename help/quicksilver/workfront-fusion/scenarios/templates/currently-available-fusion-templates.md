---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Modelli di Adobe Workfront Fusion attualmente disponibili
description: In Adobe Workfront Fusion sono attualmente disponibili i seguenti modelli pubblici.
author: Becky
feature: Workfront Fusion
exl-id: 29d95b93-ab54-416d-b0d5-ff12634951b2
source-git-commit: 2b2424a26ba903cda8f03c468da733732bf6d434
workflow-type: tm+mt
source-wordcount: '1162'
ht-degree: 0%

---

# Modelli di Adobe Workfront Fusion attualmente disponibili

In Adobe Workfront Fusion sono attualmente disponibili i seguenti modelli pubblici.

È possibile che nel team o nell&#39;organizzazione siano disponibili altri modelli creati dal team.

Per visualizzare i modelli disponibili, fai clic su **Modelli** icona ![](assets/fusion-template-icon.png) nel menu di navigazione laterale in Fusion.

## Modelli Workfront

Questi modelli automatizzano i processi e i flussi di lavoro di Workfront.

### Workfront - Creazione di progetti da CSV

Questa automazione crea nuovi progetti in Workfront in base a Nome, Portfolio, Stato, Data inizio pianificata e Dettagli modello specificati in un file CSV.

### Workfront - Richieste di pulizia senza nuovi appunti negli ultimi 30 giorni

Utilizza questo modello per applicare un aggiornamento della nota di 30 giorni alle richieste. Lo stato delle richieste non aggiornate in 30 giorni viene modificato e chiuso a 60 giorni.

### Workfront - Modifica lo stato del progetto impostandolo su Completato al 100%.

Questa automazione aggiorna i progetti allo stato Completato che hanno tutte le attività completate a 1005. I progetti con problemi o attività aperte o approvazioni di progetti riceveranno un aggiornamento e, una volta risolti, i progetti passeranno allo stato Completato.

### Workfront: avvisa e tenta di chiudere i progetti non aggiornati

Utilizza questo scenario per automatizzare l’avviso e la chiusura dei progetti che soddisfano i criteri di progetto non aggiornati della tua organizzazione.

### Workfront: copia nuove note e risposte dal problema/richiesta di origine al progetto o all’attività già convertiti

Utilizzare questo modello per copiare le note e le risposte da un problema o una richiesta in un progetto o un&#39;attività già convertiti.

### Workfront: copia dei dati di campo e del Forms personalizzato del programma nei nuovi progetti associati

Questa automazione controlla i nuovi progetti nei programmi con moduli personalizzati. Quindi aggiunge i moduli e i campi personalizzati del programma ai nuovi progetti.

### Workfront: copia dati di campo e Forms personalizzati del Portfolio nei nuovi progetti associati

Questa automazione controlla nuovi progetti in portfolio con moduli personalizzati. Quindi aggiunge i moduli e i campi personalizzati del portfolio ai nuovi progetti.

### Workfront - Conversione del problema approvato in progetto

Questo modello converte i problemi in progetti. Puoi modificarlo per soddisfare gli standard della tua organizzazione.

### Workfront: copia i documenti da problemi/richieste in progetti o attività già convertiti

Questo scenario flessibile consente di copiare i documenti da problemi o richieste a progetti o attività convertiti in precedenza.

### Notifica personalizzata in base alla modifica del campo

Questo modello crea aggiornamenti personalizzati (e relative notifiche) per i singoli utenti che lavorano su un progetto Workfront, in base a un evento univoco, ad esempio una modifica del valore di un campo. Lo scenario controlla Workfront per quando un campo specificato cambia in un’attività o in un problema. Quando si verifica, lo scenario valuta le informazioni nel progetto correlato e crea un aggiornamento personalizzato per una persona assegnata a un ruolo specifico nel progetto.

### Workfront: aggiunta in blocco al nome del progetto con convenzione

Questo modello di aggiornamento in blocco rinomina tutti i progetti che soddisfano i criteri di una ricerca (rientrano in un portfolio) e li rinomina con un formato standard.

### Workfront - Rinomina progetti con convenzione

Questo modello individua tutti i progetti che soddisfano i criteri di un filtro (rientrano in un portfolio) e li rinomina con un formato standard.

### Workfront - Crea baseline in caso di modifica dello stato

Questo modello acquisisce una baseline del progetto in seguito a qualsiasi modifica dello stato del progetto indicata nei moduli &quot;switch&quot; e crea un aggiornamento nel flusso di aggiornamento per la registrazione.

### Workfront - Creazione della linea di base settimanale

Questo modello acquisisce una previsione del progetto su base settimanale ogni lunedì alle 6 (ora legale) sui progetti filtrati in base al portfolio e crea un aggiornamento nel flusso di aggiornamento per la registrazione.

### Trova modelli di progetto non utilizzati in fase di definizione del criterio e invia una notifica

Una volta al mese, rivedi i modelli di progetto utilizzando il tuo criterio con questo modello facile da gestire che notifica agli utenti appropriati i modelli che violano il criterio.

## Workfront - Modelli di bozza Workfront

Questi modelli automatizzano i flussi di lavoro che combinano Workfront con Workfront Proof.

### Workfront Proof > Workfront - Decisione di aggiornamento progetto su bozza

Quando si prende una decisione su una bozza aggiunta direttamente a un progetto, questa automazione raccoglie informazioni sulla decisione della bozza, ad esempio chi ha preso la decisione, e quindi riflette questo progresso nel progetto Workfront corrispondente come aggiornamento.

### Workfront Proof > Workfront - Aggiornamento e completamento attività (se approvato) sulla decisione della bozza

Se le singole bozze sono associate a singole attività, questo scenario chiude l’attività associata quando viene presa una decisione di approvazione sulla bozza. Se approvato, completa l’attività e aggiorna il progetto.

## HTTP - Modelli Workfront

Questi modelli recuperano le informazioni da un servizio web e le inseriscono in Workfront.

>[!NOTE]
>
> Per utilizzare i modelli in questa sezione è necessario disporre di una licenza Workfront Fusion for Work Automation and Integration.

### Connessione tramite JWT (JSON Web Token)

Stabilisci l’autorizzazione JWT per un’API client.

### APILayer > Workfront - Aggiornamento del tasso di cambio giornaliero (EUR)

Questo modello crea uno scenario che automatizza l&#39;aggiornamento di un tasso di cambio in un determinato momento. Questo scenario richiama il tasso di euro (EUR) al dollaro statunitense (USD) da un’API APIlayers.com e aggiorna il tasso in Workfront.

## Modelli Workfront-Marketo

Questi modelli supportano l&#39;integrazione Workfront-Marketo.

>[!NOTE]
>
> Per utilizzare i modelli in questa sezione è necessario disporre di una licenza Workfront Fusion for Work Automation and Integration.

### Approvare la bozza e-mail del Marketo Engage con i flussi di lavoro di approvazione di Workfront

Questo fa parte dell’integrazione Revisione e approvazione tra Workfront e Marketi Engage. Questo modello rileva se è stata approvata una bozza e-mail in Workfront, quindi aggiorna l’e-mail corrispondente nel Marketo Engage in base all’approvazione.

### Acquisisci le richieste delle campagne di marketing in Workfront e automatizza la creazione di campagne in Marketi Engage

Questo scenario offre un modo programmatico per creare campagne e-mail e webinar in Marketo Engage da una richiesta effettuata in Workfront. Utilizzando l’automazione per creare, organizzare e configurare le campagne, i team sono in grado di migliorare l’efficienza.

### Verifica una bozza e-mail del Marketo Engage in Workfront

Questo modello rileva se un’attività di Workfront è stata impostata sullo stato Pronto per la revisione, quindi esporta la bozza e-mail dal Marketo Engage per salvarla come bozza in Workfront.

## Modelli Workfront-SharePoint

Questi modelli consentono di collegare Workfront e SharePoint.

>[!NOTE]
>
> Per utilizzare i modelli in questa sezione è necessario disporre di una licenza Workfront Fusion for Work Automation and Integration.

### Guarda le modifiche apportate alla cartella SharePoint

Questo modello consente di verificare se è stata apportata una modifica a una cartella di SharePoint.


## Modelli Workfront-Anaplan

Questi modelli supportano l’integrazione Workfront-Anaplan e prevedono una configurazione specifica sia in Anaplan che in Workfront. Per informazioni su questi modelli e sulle relative configurazioni richieste, consulta gli articoli relativi ai singoli modelli.

Per ulteriori informazioni sull’integrazione Workfront-Anaplan, consulta [Adobe Workfront con Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

>[!NOTE]
>
> Per utilizzare i modelli in questa sezione è necessario disporre di una licenza Workfront Fusion for Work Automation and Integration.

### Flussi di lavoro di ottimizzazione della spesa

* [Invia [!DNL Adobe Workfront] aggiornamenti del progetto a un [!DNL Anaplan] voce di elenco](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [Invia [!DNL Adobe Workfront] spese per un [!DNL Anaplan] voce di elenco](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
* [Invia [!DNL Adobe Workfront] aggiornamenti ore effettive di un [!DNL Anaplan] voce di elenco](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

### Flussi di lavoro per collegare le richieste di budget

* [Creare un [!DNL Anaplan] voce di elenco da un [!DNL Adobe Workfront] richiesta budget](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [Applicare un [!DNL Anaplan] allocazione budget a un [!DNL Adobe Workfront] progetto](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

### Flussi di lavoro per collegare le richieste delle campagne

* [Creare un [!DNL Anaplan] voce di elenco da un [!DNL Adobe Workfront] richiesta campagna](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [Applicare un [!DNL Anaplan] allocazione budget a un [!DNL Adobe Workfront] richiesta campagna o progetto campagna](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)


<!--[!BADGE New!]{type=Informative} -->