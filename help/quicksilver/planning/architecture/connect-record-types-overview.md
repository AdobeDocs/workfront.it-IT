---
title: Panoramica sui tipi di record collegati
description: Un modo per indicare la correlazione tra i singoli tipi di record consiste nel collegarli. Inoltre, è possibile collegare i tipi di record di Adobe Workfront Planning con i tipi di oggetto di altre applicazioni per migliorare l'esperienza degli utenti e mantenere lo stato attivo in un'unica applicazione.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1c04c68b-7a7f-46ae-b750-2b1f79855de4
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '2020'
ht-degree: 1%

---


<!--keep the 30 limit verbiage in yellow til Jan 2026-->

# Panoramica sui tipi di record collegati

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedi [Abilitare o disabilitare le versioni rapide per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

È possibile indicare che i singoli tipi di record sono correlati tra loro o a oggetti di altre applicazioni collegandoli.

Questo articolo offre una panoramica delle connessioni dei tipi di record e descrive i tipi di connessioni che è possibile stabilire tra tipi di record e tipi di oggetto.

Per informazioni sulla connessione dei tipi di record, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).

## Considerazioni sulla connessione dei tipi di record

In Workfront Planning sono disponibili due passaggi per le connessioni:

1. Stabilire una connessione tra due tipi di record o un tipo di record e un tipo di oggetto da un&#39;altra applicazione.

   Per informazioni su come connettere i tipi di record, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Collegare un singolo record di un tipo a record di un altro tipo dopo aver connesso i due tipi di record. Per informazioni sulla connessione dei record, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

Considerare le seguenti informazioni sulla connessione dei tipi di record:

* <span class="preview">In Workfront Planning è possibile avere fino a 30 campi connessi per un tipo di record.</span>

* È possibile connettere le seguenti entità in Adobe Workfront Planning:

   * Due tipi di record.

     Per impostazione predefinita, è possibile connettere due tipi di record dallo stesso workspace. È inoltre possibile impostare tipi di record per la connessione con tipi di record di altre aree di lavoro. Per informazioni, vedere [Modifica tipi di record](/help/quicksilver/planning/architecture/edit-record-types.md).
   * Tipo di record e tipo di oggetto di un&#39;altra applicazione.

* È possibile connettere i tipi di record di Workfront Planning ai tipi di oggetto seguenti delle applicazioni seguenti:

   * Adobe Workfront:

      * Progetti
      * Portfolio
      * Programmi
      * Aziende
      * Gruppi

   * Adobe Experience Manager Assets:

      * Immagini
      * Cartelle

   * Adobe GenStudio for Performance Marketing

      * Brand

     >[!IMPORTANT]
     >
     >Per connettersi con i marchi Adobe Experience Manager Assets e GenStudio, è necessario disporre dei seguenti elementi:
     >* Una licenza Adobe Experience Manager Assets
     >* Una licenza Adobe GenStudio for Performance Marketing
     >* Per collegare i record di Workfront Planning ad Adobe Experience Manager Assets, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Business Platform o Adobe Admin Console.
     >Per informazioni su Adobe Admin Console, consulta le [Domande frequenti su Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Dopo aver creato i record per i tipi di record, è possibile collegarli tra loro tramite il campo record connesso.

  Per informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

* Dopo aver collegato un tipo di record a un altro tipo di record o a un tipo di oggetto di un&#39;altra applicazione, si verificano i seguenti scenari:

   * **Quando si connettono due tipi di record di Planning**: viene creato un campo record collegato nel tipo di record da cui si sta effettuando la connessione. Un campo record collegato simile viene creato nel tipo di record a cui ci si connette solo quando si abilita l&#39;impostazione Crea campo corrispondente nel tipo di record collegato nella scheda Nuova connessione.

     Ad esempio, se colleghi il tipo di record &quot;Campagna&quot; al tipo di record &quot;Prodotto&quot;, nel tipo di record Campagna viene creato un campo record collegato (campo connessione) denominato &quot;Prodotto collegato&quot;. Nel tipo di record Prodotto viene creato automaticamente un tipo di record collegato denominato &quot;Campaign&quot;.

     Esistono, ad esempio, i seguenti scenari:

      * Quando si abilita l&#39;impostazione Crea campo corrispondente nel tipo di record collegato e si collega il tipo di record &quot;Campagna&quot; al tipo di record &quot;Prodotto&quot;, nel tipo di record Campagna viene creato un campo di record collegato (campo di connessione) denominato &quot;Prodotto collegato&quot;. Nel tipo di record Prodotto viene creato automaticamente un tipo di record collegato denominato &quot;Campaign&quot;.
      * Quando si disattiva l&#39;impostazione Crea campo corrispondente nel tipo di record collegato e si collega il tipo di record &quot;Campagna&quot; al tipo di record &quot;Prodotto&quot;, nel tipo di record Campagna viene creato un campo di record collegato (campo di connessione) denominato &quot;Prodotto collegato&quot;. Nel tipo di record Prodotto non viene creato un tipo di record collegato denominato automaticamente &quot;Campaign&quot;.

     Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).

   * **Quando si connette un tipo di record con un tipo di oggetto di un&#39;altra applicazione**:

      * Nel tipo di record da cui si sta effettuando la connessione viene creato un campo record collegato. Nessun campo record collegato viene creato automaticamente sul tipo di oggetto dell&#39;altra applicazione.
      * I campi dei record di Planning non sono accessibili dagli oggetti di Workfront.
      * I record di Planning sono visibili dalla sezione Planning dell&#39;oggetto Workfront. Per informazioni, vedere [Gestire le connessioni record dagli oggetti Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
      * È possibile creare un campo personalizzato della connessione Planning e allegarlo al modulo personalizzato di un oggetto Workfront. Per informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
      * I campi del record di pianificazione sono accessibili dalle risorse di Experience Manager quando l’amministratore Workfront configura la mappatura dei metadati tramite l’integrazione tra Workfront e Adobe Experience Manager Assets. Per ulteriori informazioni, consulta [Configurare la mappatura dei metadati delle risorse tra Adobe Workfront e Experience Manager Assets](https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).
      * I campi dei record di pianificazione non sono accessibili dai marchi in GenStudio for Performance Marketing.

   * **Quando si aggiungono campi di ricerca dal record o dall&#39;oggetto a cui ci si connette**: oltre a creare un campo record collegato, è anche possibile connettersi ai campi del record o del tipo di oggetto connesso denominati campi di ricerca. Un campo di ricerca collegato con le informazioni del record a cui ci si connette viene visualizzato nel record da cui ci si connette.

     È possibile collegare campi di altri tipi di record o oggetti di un&#39;altra applicazione al tipo di record di Workfront Planning.

     I campi collegati sono di sola lettura e visualizzano automaticamente le informazioni dei record connessi.

     È possibile fare riferimento a campi di ricerca di altri tipi di record o oggetti in formule, filtri o raggruppamenti.

     Ad esempio, se si collega il tipo di record &quot;Campagna&quot; a un progetto Workfront e si seleziona di inserire il campo Data di completamento pianificata del progetto nel record Pianificazione di Workfront, per la campagna viene automaticamente creato un campo collegato denominato Data di completamento pianificata (da progetto). Impossibile modificare manualmente il campo collegato. Nel campo Data di completamento pianificata (da progetto) viene visualizzata la Data di completamento pianificata dei progetti collegati.

     >[!IMPORTANT]
     >
     >Tutti gli utenti con autorizzazioni View (Visualizzazione) o superiori all&#39;area di lavoro possono visualizzare le informazioni nei campi di ricerca, indipendentemente dalle autorizzazioni o dal livello di accesso nell&#39;applicazione dei tipi di oggetto collegati o dalle autorizzazioni in altre aree di lavoro.

     I campi record collegati sono preceduti dall&#39;icona di relazione ![Icona campo relazione](assets/relationship-field-icon.png).

     I campi collegati sono preceduti da un’icona che identifica il tipo di campo. Ad esempio, i campi collegati (o di ricerca) sono preceduti da icone che indicano che un campo è un numero, un paragrafo o una data.

     >[!TIP]
     >
     >Le informazioni relative al campo data degli oggetti di Workfront vengono visualizzate nel formato 24 ore in Workfront Planning, indipendentemente da come vengono visualizzate in Workfront.
     >
     >Se, ad esempio, la Data inizio pianificata di un progetto viene visualizzata come 3:00 PM in Workfront, verrà visualizzata come 15:00 in Workfront Planning in un campo di ricerca importato.
     <!--* <span class="preview">You must connect record types to be able to create hierarchies in Workfront Planning. When record type connections don't exist, they are automatically created when you create a hierarchy. For information, see [Create workspace hierarchies](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).</span>-->


## Tipi di connessione

Dopo aver stabilito una connessione tra due tipi di record o tra un record e un tipo di oggetto da un&#39;altra applicazione, è possibile aggiungere record nei campi dei record connessi.

>[!WARNING]
>
>Le opzioni descritte in questa sezione non sono disponibili quando si collegano i seguenti elementi:
>
>* Due record da aree di lavoro diverse
>
>* Un tipo di record e risorse Experience Manager
>
>* Un tipo di record e un marchio Adobe GenStudio

È possibile scegliere se collegare un record a più record alla volta oppure un record alla volta tra di loro.

Di seguito sono riportati i tipi di connessione che è possibile scegliere per la connessione dei tipi di record:

* Quando l&#39;impostazione **Crea campo corrispondente nel tipo di record collegato** è disabilitata, è possibile scegliere tra:

   * [Selezione multipla](#multi-select-connection-type)
   * [Selezione singola](#single-select-connection-type)

* Quando l&#39;impostazione **Crea campo corrispondente nel tipo di record collegato** è abilitata, è possibile scegliere tra:

   * [Da molti a molti](#many-to-many-connection-type)
   * [Da uno a molti](#one-to-many-connection-type)
   * [Da molti a uno](#many-to-one-connection-type)
   * [Uno a uno](#many-to-one-connection-type)

### Tipo di connessione a selezione multipla

![Tipo di connessione a selezione multipla](assets/multi-select-connection-picker.png)

Quando si crea una connessione a selezione multipla tra tipi di record, è possibile selezionare più record connessi nel campo connessione dal tipo di record originale.

Ad esempio, se crei una connessione a selezione multipla tra campagne e progetti, puoi selezionare più progetti per una campagna. Per il tipo di oggetto Progetto non viene creato un tipo di record connesso di Campaign.

Dopo aver selezionato questo tipo di connessione, non è possibile modificarlo dopo averlo salvato in uno dei seguenti tipi:

* Selezione singola
* Da uno a molti
* Da molti a uno
* Da uno a uno

### Tipo di connessione a selezione singola

![Tipo di connessione a selezione singola](assets/single-select-connection-picker.png)

Quando si crea una connessione a selezione singola tra tipi di record, è possibile selezionare un record nel campo connessione dal tipo di record originale.

Ad esempio, se crei una connessione a selezione singola tra campagne e aziende, puoi selezionare una società per una campagna. Per il tipo di oggetto Company non viene creato un tipo di record connesso di Campaign.

Dopo aver selezionato questo tipo di connessione, non è possibile modificarlo dopo averlo salvato in uno dei seguenti modi:

* Da uno a molti
* Da uno a uno

</div>


<!--
* [Many to many](#many-to-many-connection-type)
* [One to many](#one-to-many-connection-type)
* [Many to one](#many-to-one-connection-type)
* [One to one](#many-to-one-connection-type)
-->

### Tipo di connessione da molti-a-molti

![Selezione connessioni molti a molti](assets/many-to-many-connection-picker.png)

Quando si crea una connessione molti-a-molti tra tipi di record, è possibile selezionare più record nel campo connessione da entrambi i tipi di record.

Ad esempio, se crei una connessione da molti-a-molti tra campagne e progetti, puoi selezionare più progetti per ogni campagna e più campagne per ogni progetto.

Un esempio reale di relazione molti-a-molti è la relazione tra film e attori. Ogni film può avere più attori e ogni attore può giocare in più film.

Quando si seleziona questo tipo di connessione, non è possibile modificarlo dopo averlo salvato.

### Tipo di connessione uno-a-molti

![Selezione connessione uno a molti](assets/one-to-many-connection-picker.png)


Quando si crea una connessione uno-a-molti tra tipi di record, è possibile selezionare più record nel campo connessione del tipo di record corrente, ma il campo connessione corrispondente nel tipo di record a cui ci si connette consente di selezionare un solo record. Il campo record connesso creato automaticamente nel secondo tipo di record viene impostato automaticamente su un tipo di relazione molti-a-uno.

Ad esempio, se crei una connessione uno-a-molti tra campagne e progetti, puoi selezionare più progetti per ogni campagna, ma ogni progetto può essere connesso a una sola campagna.

Un esempio reale di un tipo di relazione uno-a-molti è la relazione tra librerie e libri: una libreria ha molti libri nel suo inventario; ma un libro particolare può essere in una sola libreria in un dato momento.

Quando si seleziona questo tipo di connessione, è possibile modificarlo in un secondo momento solo in un tipo di connessione molti-a-molti.

### Tipo di connessione molti-a-uno

![Selezione connessione molti a uno](assets/many-to-one-connection-picker.png)


Quando si crea una connessione molti-a-uno tra tipi di record, è possibile collegare ogni record del tipo di record corrente con un solo record del tipo di record connesso. Il campo record connesso creato automaticamente nel secondo tipo di record viene impostato automaticamente su un tipo di relazione uno-a-molti.

Ad esempio, se colleghi le campagne ai progetti e scegli questo tipo di connessione, puoi aggiungere un solo progetto a una campagna. Tuttavia, puoi aggiungere più campagne a un progetto.

Un esempio reale di relazione molti-a-uno è la relazione tra molti film e un attore: un attore può essere in molti film, ma ogni film può avere un attore specifico una sola volta nel suo cast.

Quando si seleziona questo tipo di connessione, è possibile modificarlo in un secondo momento solo in un tipo di connessione molti-a-molti.

### Tipo di connessione uno-a-uno

![Selezione connessione uno a uno](assets/one-to-one-connection-picker.png)

Quando si crea una connessione uno-a-uno tra tipi di record, in entrambi i tipi di record è possibile connettere ogni record a un solo record dell&#39;altro tipo.

Ad esempio, se colleghi le campagne ai progetti e scegli questo tipo di connessione, puoi collegare una campagna a un progetto. Un progetto può essere connesso a una sola campagna.

Un esempio reale di relazione uno-a-uno è quello esistente tra una persona e l&#39;identificatore univoco del suo paese (come un numero di previdenza sociale, un ID passaporto, un ID di identificazione locale): ogni persona ha un solo identificatore univoco per un paese e ogni identificatore univoco può essere collegato a una sola persona.

Quando selezioni questo tipo di connessione, puoi successivamente modificarlo in qualsiasi altro tipo di connessione.
