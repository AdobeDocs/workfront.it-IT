---
title: Miglioramenti dei moduli personalizzati
description: I seguenti miglioramenti significativi sono stati apportati alla gestione dei moduli personalizzati nella versione 22.2.
author: Luke
feature: Product Announcements, Custom Forms
exl-id: 81568eab-8a65-4767-b8ab-fb9353a90bb6
source-git-commit: d8e3c2da7f8fcd062e1bf2bb5de43a6238f5eadd
workflow-type: tm+mt
source-wordcount: '1186'
ht-degree: 0%

---

# Miglioramenti dei moduli personalizzati

I seguenti miglioramenti significativi sono stati apportati alla gestione dei moduli personalizzati nella versione 22.2.

## Aggiungi widget risorse

Puoi incorporare l’immagine nei moduli personalizzati. Questo consente di comunicare con gli utenti dei moduli personalizzati in modo più interattivo e visivo. Ulteriori tipi di widget saranno presto disponibili.

![](assets/image-in-custom-form.png)

Quando a un oggetto viene allegato un modulo personalizzato contenente un widget, gli utenti che utilizzano l&#39;oggetto possono visualizzarlo nelle seguenti aree:

* L’area Dettagli dell’oggetto (ad esempio, per un progetto, l’area Dettagli progetto )&#x200B;

  ![](assets/see-image-details-page.png)

* La casella Modifica dell’oggetto, se presenta il nuovo aspetto dell’esperienza Adobe Workfront (ad esempio le caselle Modifica progetto e Modifica attività)&#x200B;

  ![](assets/image-see-in-edit.png)

Attualmente, gli utenti non possono visualizzare il widget nelle seguenti aree:&#x200B;

* Elenchi e rapporti
* Home e Riepilogo
* La casella Modifica dell’oggetto, se non ha il nuovo aspetto dell’esperienza Adobe Workfront (ad esempio, la casella Modifica spesa)
* &#x200B;L’app mobile di Workfront

Per ulteriori informazioni sull’aggiunta di widget ai moduli personalizzati, consulta [Aggiungere o modificare un’immagine o un altro widget di risorse in un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Associare un modulo personalizzato a più tipi di oggetto

È possibile associare più tipi di oggetto a qualsiasi nuovo modulo personalizzato:

![](assets/new-custom-form-object-types.png)

Oppure qualsiasi modulo personalizzato esistente:

![](assets/add-object-type-existing-form.png)

Questo consente di creare un singolo modulo personalizzato da utilizzare su progetti, attività, problemi e qualsiasi altro tipo di oggetto supportato per i moduli personalizzati.

Questa funzione è particolarmente utile quando si converte un problema o un&#39;attività, in quanto è possibile trasferire un modulo personalizzato e i relativi dati all&#39;oggetto convertito. Non è più necessario creare e gestire copie esatte dello stesso modulo personalizzato per vari tipi di oggetti, ma aggiungere manualmente il modulo personalizzato al progetto.

>[!INFO]
>
>**Esempio:**
>
>Qualcuno invia una richiesta IT interna (problema) e fornisce dettagli su ciò che è necessario in un modulo personalizzato allegato.
>
>Converti il problema in un progetto per gli utenti che ci lavoreranno.
>
>Poiché il modulo personalizzato contenente i dettagli dell’autore dell’invio è associato sia al tipo di oggetto Problema che al tipo di oggetto Progetto, il modulo personalizzato e tutti i dettagli vengono trasferiti al progetto durante la conversione.

>[!NOTE]
>
>Quando si verifica la conversione, il modulo personalizzato deve essere già associato al tipo di oggetto in cui si desidera eseguire la conversione.

Per istruzioni sull’aggiunta di un widget di risorse a un modulo personalizzato, consulta [Aggiungere o modificare un’immagine o un altro widget di risorse in un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

Quando crei o modifichi un modulo personalizzato con più oggetti, considera quanto segue:

* [Opzioni di autorizzazione per le interruzioni di sezione](#permission-options-for-section-breaks)
* [Compatibilità del campo personalizzato calcolato](#calculated-custom-field-compatibility)
* [Attenzione sull&#39;eliminazione di un tipo di oggetto da un modulo personalizzato](#caution-about-deleting-an-object-type-from-a-custom-form)

### Opzioni di autorizzazione per le interruzioni di sezione

Il set di opzioni di autorizzazione per l&#39;interruzione di sezione disponibili per i tipi di oggetto Problema, Attività, Progetto e Utente dispone di un&#39;opzione di autorizzazione in più rispetto al set di opzioni di autorizzazione per tutti gli altri tipi di oggetto: Modifica limitata.

![](assets/section-break-permissions-limited-edit.png)

Il set di autorizzazioni di interruzione di sezione disponibile per tutti gli altri tipi di oggetto (Portfolio, Documento, Programma, Spesa, Società, Iterazione, Record fatturazione e Gruppo) non include la Modifica limitata:

![](assets/section-break-permissions-no-limited-edit.png)

In un modulo personalizzato associato a tipi di oggetto di entrambi questi gruppi, il sistema utilizza un set comune di autorizzazioni di interruzione di sezione che funzionano per tutti i tipi di oggetto. In particolare, anziché utilizzare l&#39;opzione di autorizzazione Modifica limitata, questo set comune sostituisce l&#39;opzione di autorizzazione Modifica con l&#39;opzione di autorizzazione Modifica limitata. L&#39;opzione Modifica è compatibile con tutti i tipi di oggetto.

Quando si associa un tipo di oggetto che utilizza opzioni di autorizzazione diverse rispetto agli altri tipi di oggetto già presenti in un modulo personalizzato, viene visualizzato un messaggio che consente di passare all&#39;insieme comune di opzioni di autorizzazione che verranno utilizzate per il modulo. Questa modifica verrà applicata a tutti i campi, anche se non sono inclusi in un’interruzione di sezione.

Per ulteriori informazioni, consulta [Aggiungere un’interruzione di sezione a un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).

### Compatibilità del campo personalizzato calcolato

In un modulo personalizzato con più oggetti, se un campo calcolato fa riferimento a campi disponibili per l&#39;utilizzo con tutti i tipi di oggetto associati al modulo, ad esempio {name}, {description}, e {entryDate}, disponibili per più tipi di oggetto), i dati vengono calcolati correttamente, indipendentemente dall&#39;oggetto a cui vengono associati.

Ad esempio, se disponi di un modulo con più oggetti per progetti e problemi e aggiungi un campo calcolato contenente {name} espressione, il campo visualizza il nome del progetto quando si aggiunge il modulo a un progetto e il nome dell&#39;attività dell&#39;utente che aggiunge il modulo a un&#39;attività.

Tuttavia, se un campo calcolato nel modulo fa riferimento a un campo non compatibile con tutti i tipi di oggetto del modulo, un messaggio avvisa l&#39;utente di apportare modifiche.

>[!INFO]
>
>**Esempio:** In un modulo personalizzato associato al tipo di oggetto Task, viene creato un campo personalizzato calcolato che fa riferimento al campo predefinito Assegnato a: Nome in modo che possa visualizzare il nome dell&#39;assegnatario principale responsabile ogni volta che il modulo viene allegato a un&#39;attività:
>
>```
>Assigned To: Name{assignedTo}.{name}
>```
>
>Successivamente, si aggiunge il tipo di oggetto Project al modulo personalizzato. Un messaggio di avviso indica che il tipo di oggetto Project non è compatibile con il campo personalizzato calcolato. Il campo Assegnato a non è disponibile per i progetti.

In questo caso, puoi effettuare una delle seguenti operazioni:

* Rimuovere uno dei due elementi incompatibili dal modulo personalizzato, ovvero il tipo di oggetto o il campo a cui si fa riferimento.
* Mantieni entrambi gli elementi e utilizza la variabile di filtro con caratteri jolly `$$OBJCODE` come condizione in un&#39;espressione IF per creare due versioni diverse del campo In carica. Questo consente al campo di funzionare correttamente, indipendentemente dal tipo di oggetto a cui è associato il modulo.

  Nell’esempio precedente, anche se per i progetti non è presente il campo Assegnato a: Nome, è disponibile il campo Proprietario predefinito (che viene compilato automaticamente con il nome della persona che ha creato il progetto, a meno che questa impostazione non venga modificata manualmente). Quindi, nel campo personalizzato In carica, puoi utilizzare `$$OBJCODE` come mostrato di seguito per fare riferimento al campo Proprietario quando il modulo personalizzato è allegato a un progetto e al campo Assegnato a: Nome quando il modulo è allegato a un’attività:

  ```
  IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})
  ```

>[!NOTE]
>
>  Se si aggiunge un tipo di oggetto davanti al nome di un campo, tale tipo fa riferimento all&#39;oggetto padre dell&#39;oggetto, pertanto non è possibile utilizzare `{project}.{name}` con un progetto, ma puoi utilizzarlo con un’attività.

Per istruzioni sull’aggiunta di un campo personalizzato calcolato a un modulo personalizzato, consulta [Aggiungere dati calcolati a un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Per ulteriori informazioni su variabili come `$$OBJCODE`, vedi [Panoramica delle variabili filtro con caratteri jolly](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

### Attenzione sull&#39;eliminazione di un tipo di oggetto da un modulo personalizzato

È possibile eliminare un tipo di oggetto in un modulo personalizzato in qualsiasi momento, ma questo deve essere fatto con cautela. Se gli utenti hanno già allegato il modulo personalizzato a oggetti del tipo che si desidera eliminare e vi hanno aggiunto dati, tali dati verranno eliminati definitivamente quando si elimina tale tipo di oggetto nel modulo.

Inoltre, non esiste un sistema di notifica per avvisare gli utenti che utilizzano il modulo personalizzato che il modulo è stato eliminato.

Per ulteriori informazioni, consulta [Eliminare un campo personalizzato o un widget dal sistema](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
