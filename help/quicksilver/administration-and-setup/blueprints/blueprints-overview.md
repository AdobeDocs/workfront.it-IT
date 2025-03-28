---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Panoramica dei blueprint
description: I blueprint sono set di oggetti Workfront che trattano casi d’uso comuni in Workfront. Puoi scaricare e installare una blueprint, quindi configurare gli oggetti per il tuo caso d’uso specifico.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Panoramica dei blueprint

<!--Audited: 01/2024-->

I blueprint sono set di oggetti Workfront che trattano casi d’uso comuni in Workfront. Puoi scaricare e installare una blueprint, quindi configurare gli oggetti per il tuo caso d’uso specifico.

![Pagina principale blueprint](assets/blueprints-main-page-catalog.png)

>[!INFO]
>
>Esempi:
>
>* **Configurazione organizzazione risorse umane**
>
>   Questo blueprint contiene la configurazione delle strutture organizzative da espandere a un reparto Risorse umane.
>
>* **Aggiungi nuovo elenco di controllo IT dipendente**
>
>   Questo blueprint contiene un modello per organizzare nuove attività di onboarding dei dipendenti. L&#39;utilizzo di questo modello consente ai team IT di operare in modo efficiente, garantendo un&#39;esperienza positiva per i nuovi dipendenti e una maggiore produttività.
>
>* **Nozioni di base sull&#39;istanza ereditata | Elenco di controllo**
>
>    Questo blueprint contiene un modello di progetto (o elenco di controllo) che puoi esaminare con un breve elenco di domande, risorse e collegamenti per comprendere chiaramente come è stata configurata la tua istanza di Workfront. Utilizzalo quando hai ereditato di recente un’istanza Workfront e hai bisogno di istruzioni su dove iniziare.
>
>Per esaminare i blueprint correnti, vedi [Elenco dei blueprint disponibili](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).


I blueprint forniscono elementi di base per aiutarti a creare un sistema di gestione del lavoro che cresce con te. Gli amministratori di sistema possono sfogliare il catalogo dei blueprint e installare modelli di progetto, dashboard e strutture organizzative pronti all’uso. Altri utenti possono sfogliare il catalogo e richiedere l’installazione di una blueprint. Per ulteriori informazioni, consulta [Sfogliare il catalogo blueprint e richiedere l&#39;installazione dei blueprint](../../administration-and-setup/blueprints/browse-catalog.md).

Ogni blueprint è destinato a un reparto e a un livello di maturità specifico per aiutarti a implementare più rapidamente best practice comprovate nel tuo sistema. I livelli di maturità dettagliati di seguito sono indicati nella scheda del catalogo blueprint e nei relativi dettagli.

* **[!UICONTROL Gestiti]:** I modelli di progetto gestiti consentono di supportare l&#39;adozione di un nuovo processo aziendale prima che le attività e i risultati finali vengano accettati completamente come procedura standard. Contengono attività per garantire il rispetto di ogni fase del nuovo processo.

* **[!UICONTROL Integrato]:** I modelli di progetto integrati presuppongono che le funzioni aziendali siano supportate tramite una procedura operativa standard. I collaboratori del processo conoscono i passaggi e le attività da completare per seguire il processo. I modelli di progetto per supportare questo processo contengono un numero inferiore di attività per tenere traccia solo delle attività cardine e di altri risultati finali chiave necessari a scopo di reporting.

## Trova la blueprint giusta

Puoi sfogliare i blueprint per caso d’uso, livello di maturità, stato di installazione e digitare con i filtri sul lato destro del catalogo. Dopo aver trovato una blueprint che ti interessa, puoi visualizzare i dettagli nella pagina dei dettagli.

### Tipi di blueprint

Il tipo di blueprint mostra ciò che è incluso nella blueprint. Il tipo è elencato nella parte inferiore della scheda blueprint nel catalogo. Tieni presente che una blueprint può avere più di un tipo.

Sono disponibili i seguenti tipi di blueprint:

* **Modelli di progetto**: include oggetti standard associati a un modello di progetto (attività, problemi, ruoli e team) e alcune preferenze correlate a tali oggetti. Per ulteriori informazioni, vedere [Configurare una blueprint](../../administration-and-setup/blueprints/configure-template-package.md).
* **Strutture organizzative**: include gli oggetti associati alla struttura di un&#39;organizzazione (società, gruppi, ruoli e team). Per ulteriori informazioni, vedere [Configurare una blueprint](../../administration-and-setup/blueprints/configure-template-package.md).
* **Dashboard**: include uno o più dashboard per un caso d&#39;uso specifico, ad esempio i servizi di implementazione.
<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

Per esaminare i blueprint correnti, vedi [Elenco dei blueprint disponibili](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).

### Visualizza dettagli

Ogni blueprint contiene una pagina Dettagli. Da questa pagina è possibile effettuare le seguenti operazioni:

* Visualizzare un riepilogo del contenuto del flusso di lavoro
* Leggi un breve riepilogo della blueprint
* Visualizza cronologia di installazione (fare clic su **[!UICONTROL Visualizza dettagli]** per visualizzare l&#39;elenco completo degli oggetti installati con la blueprint)
* Consulta le descrizioni di ruoli, team, società e gruppi
* Vedi un esempio visivo della blueprint specifica, ad esempio un modello di progetto (puoi visualizzare l’anteprima dell’immagine completa nel browser o scaricarla)

![[!UICONTROL Dettagli blueprint] pagina](assets/blueprint-details-page-2022.png)

## Installare una blueprint

Un amministratore Workfront può installare una blueprint direttamente in qualsiasi ambiente (ambiente di produzione, di anteprima o sandbox). Per ulteriori informazioni, consulta [Installare una blueprint](../../administration-and-setup/blueprints/blueprints-install.md) o [Configurare una blueprint](../../administration-and-setup/blueprints/configure-template-package.md).

Dopo l&#39;installazione, è possibile che non si sia sicuri delle migliori azioni da eseguire in futuro. Per informazioni, vedere [Azioni da eseguire dopo l&#39;installazione di una blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

## Note aggiuntive su blueprint e modelli

I blueprint non sostituiscono la funzionalità dei modelli di progetto in [!DNL Adobe Workfront]. I blueprint consentono di creare nuovi modelli più rapidamente per organizzare più lavoro in [!DNL Workfront].

Non puoi copiare o modificare una blueprint. Tuttavia, dopo aver installato la soluzione da una blueprint, è possibile modificare il modello di progetto, le mansioni o i team creati dalla blueprint nello stesso modo in cui si aggiornano normalmente tali record nell&#39;interfaccia [!DNL Workfront]. Inoltre, quando installi una blueprint, il modello viene archiviato nell&#39;area [!UICONTROL Modelli] di [!DNL Workfront] e la blueprint originale rimane nell&#39;area [!UICONTROL Blueprint]. Non è necessario creare una copia del modello prima di iniziare a personalizzarlo in base alle proprie esigenze.

I blueprint non rimuovono o sostituiscono nulla di configurato nell&#39;ambiente. Se desideri sostituire un modello esistente installando una blueprint che crea un nuovo modello, ti consigliamo di disattivare la versione precedente per evitare confusione tra i responsabili della pianificazione che creano progetti a partire da modelli.
