---
title: "Best practice di Adobe Workfront Planning"
description: In qualità di responsabile delle operazioni di marketing, puoi utilizzare Adobe Workfront Planning per organizzare il lavoro nel ciclo di vita di marketing per tutti i team. Di seguito sono riportate alcune best practice consigliate all'avvio di Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d1da3ee59b074dec3e161cf1e0134aba39ad90a4
workflow-type: tm+mt
source-wordcount: '1217'
ht-degree: 0%

---


# Best practice di Adobe Workfront Planning

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

In qualità di responsabile delle operazioni di marketing, puoi utilizzare Adobe Workfront Planning per organizzare il lavoro nel ciclo di vita di marketing per tutti i team.

In questo articolo vengono illustrate alcune best practice consigliate all&#39;avvio di Workfront Planning.

## Che cos&#39;è Workfront Planning?

Il modulo Workfront Planning è una delle tre funzionalità distinte ma collegate di Workfront che insieme creano un sistema di registrazione di marketing. Le tre funzionalità sono:

* **Pianificazione**: nuove funzionalità avanzate incluse in Workfront Planning.

* **Flusso di lavoro**: le funzionalità di gestione collaborativa del lavoro attualmente utilizzate in Workfront (gestione dei progetti, gestione delle risorse, ecc.)

* **Automazione e integrazione**: funzionalità complete di integrazione e automazione basate su Workfront Fusion.

Workfront Planning è altamente personalizzabile. Per ulteriori informazioni sulla terminologia e sui concetti chiave di Workfront Planning, vedere [Panoramica di Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

## Domande da porre prima di configurare Workfront Planning

Dopo aver acquisito familiarità con la terminologia e l&#39;architettura di Workfront Planning, è possibile iniziare a configurare il nuovo ambiente.

Alcune domande che potresti porti durante la configurazione di Planning sono:

* **Utilizzare le aree di lavoro per gruppi organizzativi più grandi? O dovrei incoraggiare le persone a crearne di personali?**

  Potresti scoprire che c&#39;è un buon utilizzo per entrambi. È consigliabile non disporre di troppe aree di lavoro, in quanto potrebbero diventare difficili da gestire e i flussi di lavoro potrebbero essere troppo frammentati.

  >[!TIP]
  >
  >    In una singola istanza di Workfront è possibile avere 1.000 aree di lavoro.

* **Quali tipi di record personalizzati è necessario creare in ogni area di lavoro?**

  I tipi di record sono simili ai tipi di oggetto di Workfront. Pensa ai tuoi flussi di lavoro e decidi quali tipi di record (oggetti di lavoro, oggetti persone, tassonomie, ecc.) potrebbe essere necessario per ogni flusso di lavoro.

  Per informazioni, consulta [Crea tipi di record](/help/quicksilver/planning/architecture/create-record-types.md)

* **Come posso creare i miei documenti? Esiste un elenco o un foglio di calcolo esterno che contiene già i record da aggiungere a Planning che è possibile utilizzare? I record verranno aggiunti gradualmente in base alle esigenze? Oppure verranno importate utilizzando un’integrazione Fusion o API personalizzata?**

  Per informazioni, consulta:

   * [Crea record](/help/quicksilver/planning/records/create-records.md)
   * [Moduli di Adobe Workfront Planning](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-planning-modules.md)

* **Quali campi è necessario creare per i record?**

  Per informazioni, consulta [Crea campi](/help/quicksilver/planning/fields/create-fields.md).

* **Quali tipi di oggetto di Workfront o AEM Assets sono necessari per connettersi ai tipi di record di Workfront Planning in modo da visualizzare le dipendenze e creare un flusso di lavoro senza soluzione di continuità per l&#39;organizzazione?**

  Per informazioni, consulta [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md)

* **Quali calendari e visualizzazioni di marketing avrò bisogno per raccontare la storia delle mie campagne? E a quali soggetti interessati potrei rendere disponibili questi punti di vista per una collaborazione fluida?**

  Per informazioni, consulta [Gestire le visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).


## Best practice di Workfront Planning

In questa sezione sono elencate diverse procedure consigliate e non consigliate e le linee guida sulle best practice per la configurazione di Workfront Planning.

Le linee guida sono organizzate in base all’oggetto o all’area che stai impostando.

### Aree di lavoro

#### Funzionalità e funzionalità delle aree di lavoro

* Progettazione per il volume più basso di aree di lavoro a livello di organizzazione

  Ad esempio, prova a creare un singolo Workspace per tutte le attività di marketing

* Curare periodicamente le aree di lavoro. Potresti scoprire di poter modificare un elemento esistente invece di crearne uno nuovo da zero.

* Creare un nuovo Workspace per un team con un movimento operativo completamente diverso.

  Un’area di lavoro &quot;Sviluppo prodotto&quot; deve essere distinta da un’area di lavoro &quot;Marketing&quot;

* Non creare un&#39;area di lavoro unica per ogni elemento. Considera le aree di lavoro più come un sistema di record che può avvantaggiare un’intera organizzazione e consentire a tutti di mappare i flussi di lavoro e collaborare, piuttosto che come uno spazio privato per tenere traccia delle richieste personali.

* Non creare aree di lavoro univoche per ogni team o processo di un&#39;organizzazione.

  L’organizzazione Marketing deve impegnarsi a mantenere un’unica area di lavoro per mantenere la visibilità e consentire il rollup dei dati a livello di pianificazione globale.

  Evita di creare aree di lavoro simili o duplicate per i team che seguono processi simili (ad esempio, marketing EMEA VS APAC marketing), soprattutto quando questi team possono svolgere un lavoro che si completa in una campagna strategica comune.

#### Come si utilizzano le sezioni di Workspace?

* Creare ed etichettare le sezioni per aiutare gli utenti a comprendere come organizzare il ciclo di vita operativo.

  Ad esempio, puoi creare una sezione denominata &quot;Record core&quot; in cui inserire campagne, tattiche e risultati finali.

* Raggruppare insieme i tipi di record &quot;like&quot;.

  È possibile creare una sezione denominata &quot;Geografie&quot; che contiene tipi di record quali: Area geografica, Paese e Città.

#### Come posso gestire le autorizzazioni per l’area di lavoro?

* Non limitare l&#39;accesso &quot;Gestisci&quot; a un gruppo selezionato di persone attendibili, che non elimineranno accidentalmente un tipo di record o non creeranno in altro modo tipi di record e campi non necessari.

  >[!TIP]
  >
  >Abbiamo scoperto durante il nostro programma beta che molti clienti si sentono come se concedessero l’accesso &quot;Gestisci&quot; agli amministratori dei gruppi.

* Aggiungere l&#39;area Planning al modello di layout degli utenti con una licenza Standard.

* Non consentire agli utenti con una licenza Standard di creare aree di lavoro personali. Questo offre loro uno spazio sicuro per imparare lo strumento e diventare a loro agio con esso. Ciò non confonde l’esperienza per gli altri e può migliorare la produttività personale dell’utente.

  >[!TIP]
  >
  >    Consigliagli di non condividere le aree di lavoro personali come best practice.


### Tipi di record

#### Un campo a selezione singola o multipla rispetto a un tipo di record collegato

* Creare un nuovo tipo di record se l&#39;oggetto verrà utilizzato in più altri tipi di record

  Ad esempio, una campagna può avere una connessione a più tipi di pubblico Target e una tattica può avere una connessione a un singolo tipo di pubblico Target.

* Creare un nuovo tipo di record se l&#39;oggetto deve memorizzare valori di metadati aggiuntivi che potrebbero essere utili nelle ricerche.

  Ad esempio, un tipo di record Canale come &quot;E-mail&quot; può memorizzare un elenco di risultati finali di supporto, come metadati nativi o come connessione a un tipo di record &quot;Risultati finali&quot; standalone.

* Non aggiungere un nuovo tipo di record se i dati che si stanno memorizzando devono essere inclusi in un singolo tipo di record. Utilizza invece un campo di selezione.

  Ad esempio, un tipo di record Campagna può avere un campo a selezione singola denominato Dimensione campagna che è rilevante solo quando è direttamente associato a una campagna specifica.

#### Come etichettare i tipi di record?

Creare ed etichettare tipi di record che rappresentano un singolo costrutto o nome, ad esempio &quot;Campagne&quot;

:no_entry_sign: Non creare un tipo di record meglio rappresentato come livello di visualizzazione. Ad esempio, &quot;Calendario&quot; è una scelta sbagliata per un tipo di record, perché non è il tipo di record stesso, ma una visualizzazione dei record.

### Quanti livelli di gerarchia devo creare?

Viste

...

Flusso di lavoro

...

### Gestione dei campi

Campo primario

Non utilizzare valori di campo primari univoci per semplificare la ricerca e la selezione di tali record quando si creano connessioni.

Quando si effettua una connessione, gli utenti eseguiranno la ricerca in base ai valori del campo Principale e, se non sono univoci, non sapranno quale scegliere.

Evita di utilizzare valori non univoci come campo principale, in quanto possono creare confusione per gli utenti che devono eseguire ricerche nel campo principale quando utilizzano il menu del selettore delle connessioni.



Da Chris O&#39;Neal:

Un&#39;altra area da considerare o meno sono i casi d&#39;uso che sono (o non sono) i migliori utilizzi di Planning. Ad esempio, la discussione sulla gestione delle risorse che abbiamo avuto oggi.



Note di Alina:

Esempio di articolo &quot;Best practice&quot; da ExL: https://experienceleague.adobe.com/en/docs/commerce-operations/implementation-playbook/best-practices/planning/sites-stores-store-views

Ulteriori informazioni da Field Readiness di Lauren S.: https://fieldreadiness-adobe.highspot.com/spots/5fd14ae8b7b7390523f57346