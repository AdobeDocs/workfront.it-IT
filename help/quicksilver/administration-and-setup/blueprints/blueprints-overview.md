---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Panoramica delle blueprint
description: Le blueprint forniscono elementi di base per aiutarti a creare un sistema di gestione del lavoro che cresce con te.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

# Panoramica delle blueprint

Le blueprint forniscono elementi di base per aiutarti a creare un sistema di gestione del lavoro che cresce con te. Gli amministratori di sistema possono sfogliare il catalogo delle blueprint e installare modelli di progetto pronti all’uso. Altri utenti possono consultare il catalogo e richiedere l’installazione di un blueprint. Per ulteriori informazioni, consulta [Sfoglia il catalogo dei progetti e richiedi l&#39;installazione dei progetti](../../administration-and-setup/blueprints/browse-catalog.md).

Ogni blueprint è destinato a un reparto e a un livello di maturità specifico per aiutarti a implementare le best practice comprovate nel tuo sistema più velocemente. I livelli di scadenza indicati di seguito sono indicati nella carta di catalogo del progetto e nei dettagli.

**[!UICONTROL Gestito]:** I modelli di progetto gestiti aiutano a supportare l&#39;adozione di un nuovo processo aziendale prima che le attività e gli adempimenti siano completamente accettati come procedura standard. Essi contengono attività per garantire che ogni fase del nuovo processo sia seguita.

**[!UICONTROL Integrato]:** I modelli di progetto integrati presuppongono il supporto delle funzioni aziendali attraverso una procedura operativa standard. I collaboratori del processo conoscono i passaggi e le attività da completare per seguire il processo. I modelli di progetto per supportare questo processo contengono meno attività per tenere traccia solo delle tappe principali e di altri risultati finali necessari a scopo di reporting.

## Trova il modello corretto

È possibile sfogliare i progetti per caso d’uso, livello di scadenza, stato dell’installazione e digitare i filtri sul lato destro del catalogo. Una volta trovato un modello che ti interessa, puoi visualizzare i dettagli nella pagina dei dettagli.

### Tipi di blueprint

Il tipo di blueprint mostra ciò che è incluso nel blueprint. Il tipo è elencato nella parte inferiore della blueprint card del catalogo. Tieni presente che una blueprint può avere più di un tipo.

Sono disponibili i seguenti tipi di blueprint:

* Modelli di progetto: Include gli oggetti standard associati a un modello di progetto (attività, problemi, ruoli e team) e alcune preferenze relative a tali oggetti. Per ulteriori informazioni, consulta [Configurare una blueprint](../../administration-and-setup/blueprints/configure-template-package.md).
* Strutture organizzative: Include gli oggetti associati alla struttura di un&#39;organizzazione (aziende, gruppi, ruoli e team). Per ulteriori informazioni, consulta [Configurare una blueprint](../../administration-and-setup/blueprints/configure-template-package.md).
* Dashboard: Include una o più dashboard per un caso d’uso specifico, ad esempio i servizi di implementazione.

<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

Per rivedere i progetti correnti, vedi [Elenco dei progetti disponibili](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).

### Visualizza dettagli di 

Ogni blueprint contiene una pagina dei dettagli. Da questa pagina puoi:

* Visualizzare un riepilogo del contenuto del flusso di lavoro
* Leggi un breve riepilogo della blueprint
* Visualizza la cronologia di installazione (fare clic su **[!UICONTROL Vedere Dettagli]** per visualizzare l&#39;elenco completo degli oggetti installati con la blueprint)
* Consultare le descrizioni di ruoli, team, società e gruppi
* Vedi un esempio visivo della blueprint specifica, ad esempio un modello di progetto (puoi visualizzare l’anteprima dell’immagine completa nel browser o scaricarla)

![[!UICONTROL Dettagli blueprint] page](assets/blueprint-details-page-2022.png)

## Installare una blueprint

L’amministratore di sistema può eseguire l’installazione direttamente nell’ambiente di produzione o in ambienti sandbox. Per ulteriori informazioni, consulta [Installare una blueprint](../../administration-and-setup/blueprints/blueprints-install.md) o [Configurare una blueprint](../../administration-and-setup/blueprints/configure-template-package.md).

Dopo l’installazione, potrebbe non essere sicuro delle migliori azioni da intraprendere. Per informazioni, consulta [Azioni da intraprendere dopo l’installazione di una blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

## Note aggiuntive su blueprint e modelli

Le blueprint non sostituiscono la funzionalità dei modelli di progetto in [!DNL Adobe Workfront]. Le blueprint sono un modo per creare nuovi modelli più rapidamente per organizzare più del tuo lavoro in [!DNL Workfront].

Non è possibile copiare o modificare una blueprint. Tuttavia, una volta installata la soluzione da una blueprint, puoi modificare il modello di progetto, i ruoli o i team creati dalla blueprint nello stesso modo in cui vengono aggiornati normalmente tali record nella [!DNL Workfront] interfaccia. Inoltre, quando installi una blueprint, il modello viene memorizzato nel [!UICONTROL Modelli] area [!DNL Workfront] e il progetto originale rimane nel [!UICONTROL Blueprint] area. Non è necessario creare una copia del modello prima di iniziare a personalizzarlo in base alle proprie esigenze.

Le blueprint non rimuovono o sostituiscono elementi configurati nel tuo ambiente. Se desideri sostituire un modello esistente installando un modello che crea un nuovo modello, ti consigliamo di disattivare la versione precedente per evitare confusione tra i pianificatori che creano progetti a partire da modelli.
