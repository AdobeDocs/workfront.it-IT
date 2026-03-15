---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Panoramica sui progetti
description: I blueprint sono set di oggetti Workfront che trattano casi d'uso comuni in Workfront. Puoi scaricare e installare un modello, quindi configurare gli oggetti per il tuo caso d'uso specifico.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 1%

---

# Panoramica delle blueprint

<!--Audited: 01/2024-->

I blueprint sono set di oggetti Workfront che trattano casi d&#39;uso comuni in Workfront. Puoi scaricare e installare un modello, quindi configurare gli oggetti per il tuo caso d&#39;uso specifico.

![Pagina principale blueprint](assets/blueprints-main-page-catalog.png)

>[!INFO]
>
>Esempi:
>
>* **Configurazione organizzazione risorse umane**
>
>   Questo progetto contiene la configurazione delle strutture organizzative da espandere a un reparto di Risorse umane.
>
>* **Aggiungi nuovo elenco di controllo IT dipendente**
>
>   This blueprint contains a template to organize new employee onboarding activities. Using this template allows IT teams to operate efficiently, leading to a positive new employee experience and faster track to productivity.
>
>* **Inherited Instance Basics | Checklist**
>
>    Questo blueprint contiene un modello di progetto (o elenco di controllo) che puoi esaminare con un breve elenco di domande, risorse e collegamenti per comprendere chiaramente come è stata configurata la tua istanza di Workfront. Utilizzalo quando hai ereditato di recente un’istanza Workfront e hai bisogno di istruzioni su dove iniziare.
>
>Per esaminare i blueprint correnti, vedi [Elenco dei blueprint disponibili](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).


I blueprint forniscono elementi di base per aiutarti a creare un sistema di gestione del lavoro che cresce con te. System administrators can browse the blueprints catalog and install ready-to-use project templates, dashboards, and organizational structures. Other users can browse the catalog and request installation of a blueprint. For more information, see [Browse the blueprints catalog and request installation of blueprints](../../administration-and-setup/blueprints/browse-catalog.md).

Each blueprint is targeted to a department and specific maturity level to help you implement proven best practices in your system faster. The maturity levels detailed below are indicated in the blueprint catalog card and details.

* **[!UICONTROL Managed]:** Managed project templates help support the adoption of a new business process before activities and deliverables are fully accepted as a standard procedure. They contain tasks to ensure each step of the new process is being followed.

* **[!UICONTROL Integrated]:** Integrated project templates assume that business functions are supported through a standard operating procedure. I collaboratori del processo conoscono i passaggi e le attività che devono completare per seguire il processo. I modelli di progetto per supportare questo processo contengono un numero inferiore di attività per tenere traccia solo delle attività cardine e di altri risultati finali fondamentali necessari per la creazione di rapporti.

## Trovare il progetto giusto

Puoi sfogliare i progetti per caso d’uso, livello di maturità, stato di installazione e testo con i filtri sul lato destro del catalogo. Una volta individuato il progetto che ti interessa, puoi visualizzare i dettagli nella pagina dei dettagli.

### Tipi di blueprint

The blueprint type shows what&#39;s included in the blueprint. Il tipo è elencato nella parte inferiore della scheda blueprint nel catalogo. Si noti che un progetto può avere più di un tipo.

Sono disponibili i seguenti tipi di blueprint:

* **Modelli di progetto**: include oggetti standard associati a un modello di progetto (attività, problemi, ruoli e team) e alcune preferenze relative a tali oggetti. Per ulteriori informazioni, vedere [Configurare un progetto](../../administration-and-setup/blueprints/configure-template-package.md).
* **Strutture organizzative**: include oggetti associati alla struttura di un&#39;organizzazione (società, gruppi, ruoli e team). Per ulteriori informazioni, vedere [Configurare un progetto](../../administration-and-setup/blueprints/configure-template-package.md).
* **Dashboards**: Includes one or more dashboards for a specific use case, such as implementation services.
<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

To review the current blueprints, see [List of available blueprints](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).

### Visualizza dettagli

Ogni blueprint contiene una pagina Dettagli. Da questa pagina è possibile effettuare le seguenti operazioni:

* Visualizzare un riepilogo del contenuto del flusso di lavoro
* Read a brief summary of the blueprint
* View installation history (click **[!UICONTROL See Details]** to see the full list of objects installed with the blueprint)
* See role, team, company, and group descriptions
* See a visual example of the specific blueprint, such as a project template (you can preview the full image in the browser or download it)

![[!UICONTROL Blueprint Details] page](assets/blueprint-details-page-2022.png)

## Installare una blueprint

Un amministratore Workfront può installare un progetto direttamente in qualsiasi ambiente (di produzione, anteprima o sandbox). Per ulteriori informazioni, vedere [Installare un progetto](../../administration-and-setup/blueprints/blueprints-install.md) o [Configurare un progetto](../../administration-and-setup/blueprints/configure-template-package.md).

Dopo l’installazione, potresti non essere sicuro delle migliori azioni successive da intraprendere. Per informazioni, vedere [Azioni da eseguire dopo l&#39;installazione di un progetto](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

## Note aggiuntive su progetti e modelli

Blueprints do not replace the project templates functionality in [!DNL Adobe Workfront]. Blueprints are a way for you to create new templates faster to organize more of your work in [!DNL Workfront].

You cannot copy or edit a blueprint. However, once you have installed the solution from a blueprint, you can modify the project template, job roles, or teams that are created from the blueprint the same way you normally update those records in the [!DNL Workfront] interface. Also, when you install a blueprint, the template is stored in the [!UICONTROL Templates] area of [!DNL Workfront] and the original blueprint stays in the [!UICONTROL Blueprints] area. Non è necessario creare una copia del modello prima di iniziare a personalizzarlo in base alle proprie esigenze.

I blueprint non rimuovono o sostituiscono nulla di configurato nell&#39;ambiente. Se desideri sostituire un modello esistente installando una blueprint che crea un nuovo modello, ti consigliamo di disattivare la versione precedente per evitare confusione tra i responsabili della pianificazione che creano progetti a partire da modelli.
