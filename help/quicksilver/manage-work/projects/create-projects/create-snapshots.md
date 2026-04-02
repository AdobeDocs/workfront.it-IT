---
product-area: projects
navigation-topic: create-projects
title: Creare e visualizzare le istantanee del progetto
description: Le istantanee in Adobe Workfront consentono di visualizzare le differenze tra le istantanee (acquisite in una data e in un’ora specifiche) e i dati correnti del progetto.
author: Lisa
feature: Work Management
hidefromtoc: true
hide: true
source-git-commit: 6ccb4669a973a8f855120e83de7c0d437c9495a4
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 2%

---

# Creare e visualizzare le istantanee del progetto

{{highlighted-preview-article-level}}

I project manager spesso devono confrontare i dati passati di un progetto con lo stato corrente per prendere decisioni informate e vedere come sono cambiati i loro progetti nel tempo.

Le istantanee in Adobe Workfront consentono di visualizzare queste differenze tra le istantanee (scattate in una data e in un’ora specifiche) e i dati correnti del progetto in modo rapido e preciso, consentendo di gestire i progetti in modo più efficace e di prendere decisioni migliori. I confronti tra istantanee mostrano l&#39;evoluzione del progetto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td> <p>Flusso di lavoro Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
    <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Configurazione del livello di accesso</td> 
   <td>Modifica accesso ai progetti</td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td>Quando si visualizza uno snapshot, è possibile visualizzare tutti i campi per i quali si dispone dell'autorizzazione di visualizzazione sul progetto originale </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare un’istantanea

1. Vai a un progetto.
1. Nel pannello a sinistra, fai clic su **Snapshot**.

   ![Snapshot per un progetto](assets/snapshot-list.png)

1. Fare clic su **Nuovo snapshot**.
1. Digitare un nome per lo snapshot nella finestra di dialogo **Nuovo snapshot** e fare clic su **Salva**.

   Il nome dello snapshot viene visualizzato nell&#39;elenco.

   >[!NOTE]
   >
   >Quando si crea un&#39;istantanea, questa non è immediatamente disponibile. In base ai dati in esecuzione in background, la preparazione potrebbe richiedere fino a 4 ore. Lo stato di creazione è **In sospeso** quando lo snapshot non è ancora disponibile e **Pronto** quando visualizzarlo.

## Visualizza un&#39;unica istantanea

1. Vai a un progetto e fai clic su **Snapshot** nel pannello a sinistra.
1. Fare clic sul nome di un&#39;istantanea nell&#39;elenco per aprirla. Lo stato deve essere **Pronto** prima di poterlo aprire.

   >[!TIP]
   >
   >Le breadcrumb nella parte superiore dello schermo ti collegano al progetto e ti consentono di identificare se stai visualizzando un’istantanea.

   Lo snapshot visualizza i seguenti elementi esistenti al momento della creazione dello snapshot:

   * Gerarchia di attività e sottoattività nel progetto
   * Dettagli del progetto ed eventuali moduli personalizzati allegati ai dettagli
   * Progetti associati e relativa gerarchia
   * Problemi
   * Tariffe
   * Record di fatturazione
   * Spese <!--* Bookings (on its own line of course when they get released)-->
   * Team del progetto (scheda Persone)

   È possibile personalizzare qualsiasi elenco dello snapshot filtrando, ordinando, aggiungendo e rimuovendo colonne o applicando una visualizzazione. I KPI basati sulla tempificazione sono disponibili per l&#39;aggiunta alla visualizzazione snapshot. Per ulteriori informazioni, vedere [Personalizzare gli elenchi di snapshot](#customize-snapshot-lists) in questo articolo.

## Confronto delle istantanee

1. Vai a un progetto e fai clic su **Snapshot** nel pannello a sinistra.
1. Selezionare un&#39;opzione per il confronto degli snapshot:

   * Per confrontare due o più snapshot tra loro, selezionare le caselle di controllo accanto agli snapshot nell&#39;elenco e fare clic su **Confronta** nella barra delle azioni nella parte inferiore dello schermo.
   * Per confrontare gli snapshot con il progetto corrente, selezionare le caselle di controllo accanto agli snapshot nell&#39;elenco e fare clic su **Confronta con corrente** nella barra delle azioni nella parte inferiore dello schermo.

     >[!NOTE]
     >
     >Lo stato di ogni snapshot che si desidera confrontare deve essere **Pronto**.

1. Nella schermata Confronto, espandi ogni istantanea e il progetto corrente per visualizzare la gerarchia sottostante.

   ![Schermata Confronto snapshot](assets/snapshot-comparison.png)

1. È possibile personalizzare il confronto ordinando, aggiungendo e rimuovendo colonne oppure applicando una visualizzazione. Per ulteriori informazioni, vedere [Personalizzare gli elenchi di snapshot](#customize-snapshot-lists) in questo articolo.

## Esporta snapshot

È possibile esportare l&#39;elenco di tutte le istantanee o un confronto delle istantanee in formato xlsx o csv. Tutte le colonne visualizzate sono incluse nel file esportato.

1. Fare clic sull&#39;icona **Esporta** ![Esporta icona](assets/export-icon.png) nell&#39;elenco snapshot o nel confronto snapshot.
1. Selezionare il formato per il file di esportazione.

   Il file viene salvato nel computer. È possibile che venga richiesto di scegliere la posizione.

1. (Facoltativo) Aprire l&#39;elenco esportato utilizzando l&#39;applicazione appropriata.

## Personalizzare gli elenchi di snapshot

È possibile personalizzare l&#39;elenco di tutti gli snapshot, nonché di tutti gli elenchi all&#39;interno di uno snapshot o di un confronto, filtrando, ordinando, aggiungendo e rimuovendo colonne o applicando una visualizzazione.

Per ulteriori informazioni sulle personalizzazioni degli elenchi, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### Filtrare gli elementi in un elenco

I filtri consentono di ridurre la quantità di informazioni visualizzate nell’elenco.

1. Fai clic su **Filtro** sopra l&#39;elenco.
1. Nella casella Filtro fare clic su **Aggiungi condizione**.
1. Seleziona un campo in base al quale filtrare.
1. Seleziona un modificatore di filtro, ad esempio &quot;Ha uno di&quot;, &quot;Non ha nessuno di&quot;, &quot;È prima&quot; o &quot;È dopo&quot;. Le opzioni del modificatore variano a seconda del tipo di campo in base al quale si sta filtrando.
1. Seleziona il valore o i valori del campo. A seconda del tipo di campo in base al quale si sta filtrando, è possibile che venga richiesto di selezionare l&#39;elemento da un elenco, cercarlo o utilizzare un calendario per selezionare un intervallo di date.

   ![Filtrare l&#39;elenco di snapshot](assets/filter-snapshot-list.png)

   Il filtro viene applicato automaticamente all’elenco.

1. Fare clic su **Aggiungi condizione** per aggiungere un&#39;altra condizione al filtro.

   È possibile unire più filtri tramite un connettore AND o OR.

1. Quando il filtro viene applicato, è possibile aprire nuovamente le opzioni **Filtro** per modificare le opzioni del filtro o cancellare tutti i filtri.

   Un indicatore viene visualizzato sul pulsante **Filtro** quando si applica un filtro all&#39;elenco.

   ![Indicatore filtro applicato](assets/glist-filter-applied-indicator.png)

### Ordinare in un elenco

Per ordinare le singole colonne:

1. Passa il puntatore del mouse sulla colonna, quindi fai clic sulla freccia giù e seleziona **Ordina**.

   Un&#39;icona accanto al nome di una colonna indica che l&#39;elenco è ordinato in base ai valori della colonna e alla direzione dell&#39;ordinamento.

   ![Ordina elenco snapshot](assets/sort-snapshot-list.png)

### Personalizzare le colonne di un elenco

È possibile nascondere, visualizzare e riordinare le colonne di un elenco.

1. Fai clic su **Colonne** sopra l&#39;elenco.

   ![Colonne per elenco snapshot](assets/hide-display-columns-on-snapshot.png)

1. Utilizza i pulsanti per visualizzare o nascondere le colonne nell’elenco.
1. Per riordinare le colonne, fare clic sull&#39;icona **Trascina** ![Trascina icona](assets/drag-icon.png) e spostare una colonna nella posizione desiderata. Lo spostamento delle colonne determina la modifica automatica dell&#39;elenco.

   >[!NOTE]
   >
   >Il campo principale è la prima colonna dell&#39;elenco. È fisso nella prima posizione e non è possibile modificarne la colonna. Se il numero di colonne è elevato, il campo principale viene bloccato a sinistra e quando scorri orizzontalmente lo visualizzerai sempre.
   >
   >L&#39;icona accanto al nome di un campo mostra il tipo di campo, ad esempio testo o campo data.

   Un indicatore viene visualizzato sul pulsante **Colonne** quando le colonne sono nascoste. L&#39;indicatore non viene visualizzato quando si riordinano le colonne.

   ![Indicatore per colonne nascoste](assets/glist-columns-hidden-indicator.png)

### Aggiungere e rimuovere colonne con Gestione colonne

È possibile utilizzare Gestione colonne in alcuni elenchi avanzati per aggiungere e rimuovere facilmente colonne nell&#39;elenco. È possibile aggiungere o rimuovere come colonne sia i campi di sistema che quelli personalizzati già esistenti in Workfront.

1. Fai clic sull&#39;icona **+** nell&#39;angolo superiore destro della tabella per aprire la casella **Gestione colonne**.

   ![Gestione colonne per snapshot](assets/column-manager-on-snapshot-no-kpi-tab.png)

1. Cerca un campo oggetto esistente nella colonna **Available**, quindi fai clic su **+** a destra del nome del campo per aggiungerlo alla colonna **Selected**.
1. Fare clic su **-** a destra di un campo nella colonna **Selected** per rimuoverlo dall&#39;elenco.
1. Fai clic su **Salva**.

   L’elenco aggiorna le colonne in base alle scelte effettuate.

### Applicare una visualizzazione a un elenco

Per applicare o creare una vista:

1. Fai clic sul menu a discesa **Viste** e seleziona una vista esistente da applicare all&#39;elenco

   O

   Fai clic su **Nuova visualizzazione** per crearne una.

   ![Menu Visualizzazioni in uno snapshot](assets/views-on-snapshot-list.png)

1. (Condizionale) Per aggiungere una nuova visualizzazione, immettere un nome per la visualizzazione, quindi fare clic su **Crea**.
1. (Facoltativo) Nascondi, mostra o ridisponi le colonne. Per ulteriori informazioni, vedere [Personalizzare le colonne in un elenco](#customize-columns-in-a-list).
1. (Facoltativo) Filtra l’elenco. Per ulteriori informazioni, vedere [Filtrare gli elementi in un elenco](#filter-items-in-a-list).

Le modifiche alle viste vengono salvate automaticamente. Alla successiva applicazione di questa visualizzazione, le impostazioni delle colonne e dei filtri rimangono invariate. Per ulteriori informazioni sulle visualizzazioni, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

