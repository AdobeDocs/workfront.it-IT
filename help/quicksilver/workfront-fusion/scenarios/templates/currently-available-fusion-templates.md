---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Modelli di Adobe Workfront Fusion attualmente disponibili
description: In Adobe Workfront Fusion sono attualmente disponibili i seguenti modelli pubblici.
author: Becky
feature: Workfront Fusion
exl-id: 29d95b93-ab54-416d-b0d5-ff12634951b2
source-git-commit: b87a3777fb3f3c873a197eea1ffb051cec50aa93
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# Modelli di Adobe Workfront Fusion attualmente disponibili

In Adobe Workfront Fusion sono attualmente disponibili i seguenti modelli pubblici.

È possibile che nel team o nell&#39;organizzazione siano disponibili altri modelli creati dal team.

Per visualizzare i modelli disponibili, fai clic su **Modelli** icona ![](assets/fusion-template-icon.png) nel menu di navigazione laterale.

## Modelli Workfront

Questi modelli automatizzano i processi e i flussi di lavoro di Workfront.

### Workfront: copia dei dati di campo e del Forms personalizzato del programma nei nuovi progetti associati

Questa automazione controlla i nuovi progetti nei programmi con moduli personalizzati. Quindi aggiunge i moduli e i campi personalizzati del programma ai nuovi progetti.

### Workfront - Conversione del problema approvato in progetto

Questo modello converte i problemi in progetti. Puoi modificarlo per soddisfare gli standard della tua organizzazione.

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

### APILayer > Workfront - Aggiornamento del tasso di cambio giornaliero (EUR)

Questo modello crea uno scenario che automatizza l&#39;aggiornamento di un tasso di cambio in un determinato momento. Questo scenario richiama il tasso di euro (EUR) al dollaro statunitense (USD) da un’API APIlayers.com e aggiorna il tasso in Workfront.

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
