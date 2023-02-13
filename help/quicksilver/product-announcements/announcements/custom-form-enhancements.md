---
title: Miglioramenti al modulo personalizzato
description: Nella versione 22.2 sono stati apportati i seguenti miglioramenti significativi alla gestione dei moduli personalizzati.
author: Luke
exl-id: 81568eab-8a65-4767-b8ab-fb9353a90bb6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Miglioramenti al modulo personalizzato

Nella versione 22.2 sono stati apportati i seguenti miglioramenti significativi alla gestione dei moduli personalizzati.

## Aggiungi widget risorse

È possibile incorporare l’immagine nei moduli personalizzati. Ciò consente di comunicare con gli utenti di moduli personalizzati in modo più interattivo e visivo. Ulteriori tipi di widget saranno presto disponibili.

![](assets/image-in-custom-form.png)

Quando un modulo personalizzato contenente un widget è associato a un oggetto, gli utenti che lavorano con esso possono visualizzarlo nelle seguenti aree:

* Area Dettagli dell’oggetto (ad esempio, per un progetto, l’area Dettagli progetto) &#x200B;

   ![](assets/see-image-details-page.png)

* La casella Modifica per l’oggetto, se presenta il nuovo aspetto dell’esperienza Adobe Workfront (ad esempio, le caselle Modifica progetto e Modifica attività) &#x200B;

   ![](assets/image-see-in-edit.png)

Attualmente, gli utenti non possono visualizzare il widget nelle seguenti aree: &#x200B;

* Elenchi e rapporti
* Home e Riepilogo
* La casella Modifica per l’oggetto, se non presenta il nuovo aspetto dell’esperienza Adobe Workfront (ad esempio, la casella Modifica spesa)
* &#x200B; l’app mobile Workfront

Per ulteriori informazioni sull’aggiunta di widget ai moduli personalizzati, vedere [Aggiungere o modificare un’immagine o un altro widget di risorse in un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Associare un modulo personalizzato a più tipi di oggetti

È possibile associare più tipi di oggetto a un nuovo modulo personalizzato:

![](assets/new-custom-form-object-types.png)

O qualsiasi modulo personalizzato esistente:

![](assets/add-object-type-existing-form.png)

Ciò consente di creare un singolo modulo personalizzato da utilizzare per progetti, attività, problemi e qualsiasi altro tipo di oggetto supportato per i moduli personalizzati.

Questa funzione è particolarmente utile quando si converte un problema o un&#39;attività perché è possibile trasferire un modulo personalizzato e i relativi dati all&#39;oggetto convertito. Non è più necessario creare e mantenere copie esatte dello stesso modulo personalizzato per vari tipi di oggetti. Aggiungere manualmente il modulo personalizzato al progetto.

>[!INFO]
>
>**Esempio:**
>
>Un utente invia una richiesta IT interna (problema) e fornisce dettagli su ciò che è necessario in un modulo personalizzato allegato.
>
>Il problema viene convertito in un progetto per gli utenti che ci lavoreranno.
>
>Poiché il modulo personalizzato contenente i dettagli del mittente è associato sia al tipo di oggetto Problema che al tipo di oggetto Progetto, il modulo personalizzato e tutti i dettagli vengono trasferiti al progetto durante la conversione.

>[!NOTE]
>
>Quando la conversione viene eseguita, il modulo personalizzato deve essere già associato al tipo di oggetto in cui si sta eseguendo la conversione.

Per istruzioni su come aggiungere un widget di risorse a un modulo personalizzato, consulta [Aggiungere o modificare un’immagine o un altro widget di risorse in un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

Quando si crea o si modifica un modulo personalizzato con più oggetti, tenere presente quanto segue:

* [Opzioni di autorizzazione per le interruzioni di sezione](#permission-options-for-section-breaks)
* [Compatibilità del campo personalizzato calcolata](#calculated-custom-field-compatibility)
* [Attenzione all’eliminazione di un tipo di oggetto da un modulo personalizzato](#caution-about-deleting-an-object-type-from-a-custom-form)

### Opzioni di autorizzazione per le interruzioni di sezione

Il set di opzioni di autorizzazione per le interruzioni di sezione disponibile per i tipi di oggetto Issue, Task, Project e User dispone di un&#39;opzione di autorizzazione in più rispetto al set di opzioni di autorizzazione per tutti gli altri tipi di oggetto: Modifica limitata.

![](assets/section-break-permissions-limited-edit.png)

Il set di autorizzazioni di interruzione di sezione disponibile per tutti gli altri tipi di oggetti (Portfolio, Documento, Programma, Spese, Società, Iterazione, Record fatturazione e Gruppo) non include Modifica limitata:

![](assets/section-break-permissions-no-limited-edit.png)

In un modulo personalizzato associato a tipi di oggetti di entrambi i gruppi, il sistema utilizza un set comune di autorizzazioni di interruzione di sezione che funzionano per tutti i tipi di oggetto. In particolare, invece di utilizzare l’opzione di autorizzazione Modifica limitata, questo set comune sostituisce l’opzione di autorizzazione Modifica per l’opzione di autorizzazione Modifica limitata. L’opzione Modifica è compatibile con tutti i tipi di oggetto.

Quando si associa un tipo di oggetto che utilizza opzioni di autorizzazione diverse rispetto agli altri tipi di oggetto già presenti in un modulo personalizzato, per il modulo viene visualizzato un messaggio che consente di passare al set comune di opzioni di autorizzazione. Questa modifica verrà applicata a tutti i campi, anche se non si trovano sotto un’interruzione di sezione.

Per ulteriori informazioni, consulta [Aggiungere un’interruzione di sezione a un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).

### Compatibilità del campo personalizzato calcolata

In un modulo personalizzato con più oggetti, se un campo calcolato fa riferimento a campi disponibili per l&#39;uso con tutti i tipi di oggetto associati al modulo (ad esempio {name}, {description} e {entryDate}, disponibili per più tipi di oggetto), i dati vengono calcolati correttamente, indipendentemente dall&#39;oggetto a cui sono associati.

Ad esempio, se si dispone di un modulo con più oggetti per progetti e problemi e si aggiunge un campo calcolato contenente l&#39;espressione {name}, il campo visualizza il nome del progetto quando si aggiunge il modulo a un progetto e il nome dell&#39;attività di aggiunta del modulo a un&#39;attività.

Tuttavia, se un campo calcolato nel modulo fa riferimento a un campo non compatibile con tutti i tipi di oggetto del modulo, viene visualizzato un messaggio di avviso per avvisare l’utente di apportare modifiche.

>[!INFO]
>
>**Esempio:** In un modulo personalizzato associato al tipo di oggetto Task, è possibile creare un campo personalizzato calcolato che faccia riferimento al campo predefinito Assegnato a: Nome in modo che possa mostrare il nome dell’assegnatario principale incaricato ogni volta che il modulo è associato a un’attività:
>
>
```
>Assigned To: Name{assignedTo}.{name}
>```
>
>Successivamente, aggiungere il tipo di oggetto Progetto al modulo personalizzato. Un messaggio di avviso indica che il tipo di oggetto Progetto non è compatibile con il campo personalizzato calcolato. Questo perché il campo Assegnato a non è disponibile per i progetti.

In questo caso, è possibile effettuare una delle seguenti operazioni:

* Rimuovere dal modulo personalizzato uno dei due elementi incompatibili, ovvero il tipo di oggetto o il campo a cui si fa riferimento.
* Mantieni entrambi gli elementi e utilizza la variabile del filtro caratteri jolly `$$OBJCODE` come condizione in un&#39;espressione IF per creare due versioni diverse del campo In Charge . Questo consente al campo di funzionare correttamente, indipendentemente dal tipo di oggetto a cui è associato il modulo.

   Utilizzando l’esempio precedente, anche se non è presente alcun oggetto predefinito Assegnato a: Campo Nome per i progetti, è disponibile un campo Proprietario integrato (che viene compilato automaticamente con il nome della persona che ha creato il progetto, a meno che non venga modificato manualmente da un utente). Quindi, nel campo personalizzato In Charge, puoi utilizzare `$$OBJCODE` come mostrato di seguito, fare riferimento al campo Proprietario quando il modulo personalizzato è associato a un progetto e al campo Assegnato a: Campo Nome quando il modulo è associato a un’attività:

   ```
   IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})
   ```

>[!NOTE]
>
>  Se si aggiunge un tipo di oggetto davanti al nome di un campo, questo fa riferimento all&#39;oggetto principale dell&#39;oggetto, pertanto non è possibile utilizzare `{project}.{name}` con un progetto, ma è possibile utilizzarlo con un’attività.

Per istruzioni sull’aggiunta di un campo personalizzato calcolato a un modulo personalizzato, vedere [Aggiungere dati calcolati a un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Per ulteriori informazioni su variabili come `$$OBJCODE`, vedi [Variabili filtro caratteri jolly](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

### Attenzione all’eliminazione di un tipo di oggetto da un modulo personalizzato

È possibile eliminare un tipo di oggetto in un modulo personalizzato in qualsiasi momento, ma questa operazione deve essere eseguita con cautela. Se il modulo personalizzato è già stato allegato a oggetti del tipo che si desidera eliminare e vi sono stati aggiunti dei dati, tali dati verranno eliminati definitivamente al momento dell’eliminazione del tipo di oggetto sul modulo.

Inoltre, non esiste un sistema di notifica per avvisare gli utenti che utilizzano il modulo personalizzato eliminato.

Per ulteriori informazioni, consulta [Eliminare un campo o un widget personalizzato dal sistema](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
