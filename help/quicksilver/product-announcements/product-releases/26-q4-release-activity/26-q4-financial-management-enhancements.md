---
title: Miglioramenti alla gestione finanziaria nel quarto trimestre 2026
description: Miglioramenti alla gestione finanziaria nel quarto trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
source-git-commit: 0c08d79733bc6da0ecfd41f765ce2c624e71ad0e
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 3%
---
# Miglioramenti alla gestione finanziaria nel quarto trimestre 2026

Questa pagina descrive i miglioramenti apportati all’ambiente di anteprima con la versione del quarto trimestre 2026 di Financial Management. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili a questo punto del ciclo di rilascio del quarto trimestre 2026, consulta [Panoramica sulla versione del quarto trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

<!--

## Enhancements to billing rates on templates

>[!NOTE]
>
>Preview: October 1, 2026
>Production fast release: October 15, 2026
>Production for everyone: October 15, 2026

Multiple updates have been made to the billing rates functionality on a project template.

### For customers on all Workfront and Workflow packages

The Rates area on templates has been updated to an enhanced list.

For more information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### For customers on the Workflow Ultimate package only

Rate attributes are now available to apply to job role billing rates on the template.

For more information, see [Edit project templates](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md#add-more-items-to-a-template) and [Override Job Role Billing Rates at the project level](/help/quicksilver/manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

-->

## Miglioramenti alle tariffe di fatturazione della società

>[!NOTE]
>
>Anteprima: 3 settembre 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Sono stati apportati diversi aggiornamenti alla funzionalità delle tariffe di fatturazione della società.

### Per i clienti su tutti i pacchetti Workfront e Workflow

* Sono state aggiornate le finestre di dialogo per l’aggiunta e la modifica delle tariffe di fatturazione della società con un design più moderno che è coerente con altre aree di Workfront.
* L’impostazione &quot;Consenti tariffe di fatturazione a livello di società per sostituire le tariffe di fatturazione a livello di progetto&quot; aggiunge correttamente le sostituzioni delle tariffe quando una società viene aggiunta a un progetto e i calcoli dei ricavi pianificati utilizzano le tariffe di fatturazione a livello di società.
* Gli utenti che non hanno accesso a Modifica finanza generale e Modifica tariffe di fatturazione a livello di progetto non possono più aggiungere una società a un determinato progetto.

### Solo per i clienti nel pacchetto Workflow Ultimate

Gli attributi delle tariffe sono ora disponibili per l’applicazione alle tariffe di fatturazione a livello aziendale. Le date di validità possono essere applicate anche alle tariffe aziendali.

NOTA: i tassi a livello di società non sono stati aggiunti alla gerarchia dei tassi.

Per ulteriori informazioni, vedere [Sostituire le tariffe di fatturazione dei ruoli a livello aziendale](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md) e [Sostituire le tariffe di fatturazione a livello di progetto con le tariffe di fatturazione a livello aziendale](/help/quicksilver/manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Le gerarchie di attributi ora rimangono connesse automaticamente

>[!NOTE]
>
>Anteprima: 3 settembre 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026
>Questa funzione è disponibile solo per le organizzazioni incluse nel pacchetto Workflow Ultimate.

Quando si utilizzano gli attributi di tasso come filtri in varie aree di Workfront, ad esempio Assegnazioni avanzate, viene ora applicata una convalida aggiuntiva al filtro padre-figlio.

In precedenza, se si collegava un attributo a un padre e tale padre a un nonno, il sistema non riconosceva automaticamente l&#39;attributo originale come appartenente anche al nonno. Ora, quando si sceglie l&#39;attributo di livello più basso, ogni livello superiore viene assegnato automaticamente.

Per informazioni sugli attributi, vedere [Definire gli attributi del tasso](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).
