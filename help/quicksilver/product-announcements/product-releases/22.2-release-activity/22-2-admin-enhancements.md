---
title: 22.2 Miglioramenti per gli amministratori
description: 22.2 Miglioramenti per gli amministratori
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 55fb0b85-937d-4903-8a64-6f627dd4291f
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 0%

---

# 22.2 Miglioramenti per gli amministratori

Questa pagina descrive tutti i miglioramenti per gli amministratori apportati con la versione 22.2 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la settimana del 4 aprile 2022. Per un elenco di tutte le modifiche disponibili con la versione 22.2, consulta [Panoramica sulla versione 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Configurare un modulo personalizzato per l&#39;utilizzo con più tipi di oggetto

Ora è possibile configurare un modulo personalizzato nuovo o esistente in modo che funzioni con più tipi di oggetto, rendendo il modulo molto più utile. Gli utenti potranno allegare e compilare il modulo su oggetti di tutti i tipi per i quali lo si configura.

In precedenza era possibile configurare un modulo personalizzato in modo che funzionasse con un solo tipo di oggetto.

Questa funzionalità funziona con tutti i moduli personalizzati creati in precedenza nel sistema Workfront. Ad esempio, se si dispone già di un modulo personalizzato creato per il tipo di oggetto Attività, è ora possibile configurare il modulo in modo che funzioni anche con altri tipi di oggetto, ad esempio Progetto e Problema.

Per ulteriori informazioni, consulta la sezione [Inizia a creare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start) nell’articolo [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

>[!NOTE]
>
>* Al momento del rilascio iniziale dell’anteprima di questa funzionalità, è stata temporaneamente disabilitata la possibilità di copiare un modulo personalizzato con più oggetti. Questa abilità è stata abilitata il 24 marzo. Per informazioni sulla copia di un modulo personalizzato, consulta [Copiare un modulo personalizzato per crearne uno nuovo](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).
>* In un campo personalizzato calcolato, alcuni campi a cui si fa riferimento potrebbero non essere compatibili con i tipi di oggetto configurati per il modulo. La nostra soluzione è un carattere jolly che consentirà al calcolo di generare valori diversi, a seconda dell’oggetto a cui è associato il modulo. Abbiamo aggiunto il wild card il 24 marzo. Per informazioni su come utilizzarlo, consulta la sezione [Campi personalizzati calcolati nei moduli personalizzati con più oggetti](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat) nell’articolo [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
>* Per le interruzioni di sezione nei moduli personalizzati, è stato creato un set di autorizzazioni comuni di visualizzazione e modifica per tutti i tipi di oggetto che è possibile configurare per un modulo. In uno scenario, una di queste autorizzazioni, Modifica limitata, potrebbe causare errori in un modulo. Questo problema è stato risolto il 24 marzo. Per ulteriori informazioni sulle interruzioni di sezione, vedere [Aggiungere un’interruzione di sezione a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).
>

## Il catalogo blueprint è disponibile per tutti gli utenti e gli amministratori possono consentire le richieste

Tutti gli utenti di Adobe Workfront ora possono sfogliare il catalogo dei blueprint disponibili. Per ulteriori informazioni, consulta [Sfoglia il catalogo dei blueprint e richiedi l’installazione dei blueprint](../../../administration-and-setup/blueprints/browse-catalog.md).

Inoltre, l’amministratore di sistema può consentire agli utenti di richiedere l’installazione dei blueprint. L’assegnazione di una coda di richieste per archiviare le richieste consente agli utenti di effettuare richieste dal catalogo blueprint. Per ulteriori informazioni, consulta [Configurare l’accesso ai blueprint](../../../administration-and-setup/blueprints/configure-access-to-blueprints.md).

## Aggiungere un’immagine a un modulo personalizzato

In un modulo personalizzato creato o modificato, è ora possibile aggiungere un’immagine e includere una descrizione comando informativa o istruttiva che gli utenti possono leggere quando passano il puntatore del mouse su di essa.

Potrebbe essere utile, ad esempio, per mostrare il marchio di un nuovo prodotto o per fornire informazioni visive di cui gli utenti hanno bisogno durante la compilazione del modulo.

In precedenza, i moduli personalizzati erano completamente basati su testo.

>[!NOTE]
>
>Nelle nuove aree di esperienza di Adobe Workfront che non sono ancora state modernizzate, ad esempio la casella visualizzata quando si modificano elementi in blocco, le immagini dei moduli personalizzati non vengono visualizzate. Verranno visualizzate man mano che continuiamo ad aggiornare tali aree.

Per ulteriori informazioni, consulta [Aggiungere o modificare un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Nuove configurazioni del livello di accesso predefinito

Per soddisfare al meglio le esigenze della maggior parte degli amministratori che creano nuovi livelli di accesso, abbiamo modificato la configurazione predefinita per le opzioni &quot;Ottimizza impostazioni&quot; elencate di seguito. Questi vengono visualizzati quando si fa clic sull’icona a forma di ingranaggio ![](assets/gear-icon-in-access-levels.png) su un pulsante Modifica.

Tutte queste modifiche disabilitano un&#39;opzione precedentemente abilitata per impostazione predefinita. Se non soddisfa le esigenze della tua organizzazione, puoi abilitarle quando imposti un nuovo livello di accesso o in qualsiasi momento successivo.

>[!IMPORTANT]
>
>Questa modifica di configurazione predefinita influisce solo sui livelli di accesso creati da ora in poi, non su quelli creati in precedenza.

* In un nuovo livello di accesso con un tipo di licenza Pianificazione:

   * La funzione Condividi a livello di sistema è ora disabilitata per progetti, attività, problemi, portfolio, programmi, report, filtri, documenti e modelli.
   * Per i rapporti è disabilitata anche la funzione Visualizza rapporti incorporati e Condividi pubblicamente.
   * Condividi documenti pubblicamente è disabilitato anche per i documenti.

* In un nuovo livello di accesso con un tipo di licenza Lavoro:

   * Condividi a livello di sistema è ora disabilitato per filtri e documenti.
   * Condividi documenti pubblicamente è disabilitato anche per i documenti.

* In un nuovo livello di accesso con un tipo di licenza Richiesta o Revisione:

   * La condivisione a livello di sistema è ora disabilitata per i filtri.

## Disattivare un gruppo

Man mano che le organizzazioni interne cambiano, potrebbe essere necessario interrompere l’utilizzo di determinati gruppi in Workfront e crearne di nuovi. Per facilitare questa fase, è stata aggiunta la possibilità di disattivare un gruppo senza perdere i dati storici. Per gli utenti normali che non hanno bisogno di visualizzarli, i gruppi inattivi vengono cancellati dai campi di completamento del tipo di gruppo.

Puoi comunque trovare e configurare opzioni, preferenze e associazioni di oggetti per i gruppi inattivi che gestisci. La disattivazione di un gruppo non comporta alcuna modifica per gli oggetti a cui è associato.

In precedenza, non era possibile disattivare un gruppo.

Per ulteriori informazioni, consulta [Disattivare o riattivare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Miglioramenti alla cronologia di installazione dei blueprint

Quando installi una blueprint, un messaggio ora visualizza gli oggetti specifici (come ruoli, team o gruppi) installati correttamente con la blueprint ed eventuali oggetti che non sono stati installati. È inoltre possibile visualizzare l&#39;elenco degli oggetti installati nella pagina Dettagli blueprint facendo clic su Visualizza dettagli accanto a una specifica installazione nella tabella della cronologia di installazione.

Per ulteriori informazioni, consulta [Installare una blueprint](../../../administration-and-setup/blueprints/blueprints-install.md).

![](assets/blueprints-installation-history-350x95.png)

## Ora viene visualizzato un avviso durante l’installazione di una blueprint di sola anteprima in Produzione

Alcuni blueprint sono disponibili per l’installazione nell’ambiente di anteprima solo a scopo di test.

Se accedi a contenuti di sola anteprima nell’ambiente di produzione, Sandbox 1 o Sandbox 2, il pulsante di installazione non è attivo e potresti visualizzare un messaggio di avviso.

Per ulteriori informazioni, consulta [Installare una blueprint](../../../administration-and-setup/blueprints/blueprints-install.md).
