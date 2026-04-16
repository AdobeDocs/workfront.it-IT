---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Definire gli attributi dei tassi
description: Gli attributi della tariffa estendono la funzionalità delle schede e delle tariffe di Adobe Workfront consentendoti di aggiungere ulteriori dimensioni alle tariffe oltre il ruolo lavorativo. Workfront può quindi selezionare automaticamente la tariffa corretta per le assegnazioni, garantendo l'accuratezza e la coerenza finanziaria tra i progetti.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d570ef6a-935f-4dd0-9c54-a480163ec9d8
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '1378'
ht-degree: 2%

---

# Definire gli attributi dei tassi

Gli attributi della tariffa estendono la funzionalità delle schede e delle tariffe di Adobe Workfront consentendoti di aggiungere ulteriori dimensioni alle tariffe oltre il ruolo lavorativo. Ciò è fondamentale per le agenzie e le aziende in cui le tariffe variano non solo in base al ruolo, ma anche in base a fattori quali agenzia, ubicazione, marchio, centro di costo o altri.
Combinando questi attributi, Workfront può selezionare automaticamente la tariffa corretta per le assegnazioni, garantendo l&#39;accuratezza e la coerenza finanziaria tra i progetti.

>[!IMPORTANT]
>
>Gli attributi della tariffa sono un’impostazione di base una tantum.

Una volta che gli attributi vengono abilitati e applicati alle schede e alle tariffe di valutazione, la loro successiva modifica potrebbe compromettere l’integrità dei dati nell’intera configurazione finanziaria.

## Panoramica degli attributi dei tassi

Gli attributi dei tassi vengono considerati una configurazione una tantum perché:

* Gli attributi diventano parte del modello di dati finanziari una volta abilitati.
* Tassi, assegnazioni, valori pianificati e valori effettivi dipendono tutti dai valori attributo scelti.
* La modifica degli attributi in un secondo momento (ridenominazione, rimozione o riordinamento) può causare:

   * Perdita di collegamento tra tassi e attributi
   * Percentuali non valide o &quot;orfane&quot;
   * Disallineamento nelle fatturazioni e nei rapporti

Per questi motivi, gli attributi devono essere progettati attentamente durante l’implementazione iniziale di Workfront e lasciati invariati in seguito.

### Oggetti utilizzati come attributi di tasso

Workfront attualmente supporta tre oggetti di sistema che possono essere utilizzati come attributi di frequenza:

* **Gruppo**: spesso rinominato come _Agenzia_ o _Business Unit_.
* **Società**: Può rappresentare _Marchio_, _Cliente_ o _Cliente_.
* **Posizione**: In genere utilizzato come _Mercato_, _Regione_ o _Ufficio_.

  La posizione è definita gerarchicamente fino a 3 livelli. (Esempio: Se definisci &quot;Posizione&quot; come Los Angeles, California e USA verranno utilizzati anche nelle corrispondenze delle tariffe.)

Ogni oggetto può essere rinominato in base alla terminologia della tua organizzazione quando imposti gli attributi.
Ad esempio:

* Etichetta &quot;Agency&quot; = riferimento a un oggetto appartenente al gruppo
* Etichetta &quot;Centro di costo&quot; = riferimento oggetto sottogruppo
* Etichetta &quot;Location&quot; = riferimento all&#39;oggetto Location

Questo consente alla configurazione di rispecchiare la struttura aziendale mantenendo l’integrità del modello dati di Workfront.

### Note sugli attributi dei tassi in Workfront

* Workfront supporta fino a 5 livelli di attributi. Il sistema segue sempre la gerarchia degli attributi, selezionando la corrispondenza più specifica disponibile.

   * 0 = tasso di base generico
   * 1 - 5 = aliquote progressivamente più specifiche

* È possibile rinominare gli attributi per riflettere la propria attività (agenzia, marchio, mercato, centro di costo, ecc.).
* La configurazione è una tantum: la modifica degli attributi in un secondo momento rischia di compromettere l&#39;integrità dei dati finanziari.
* Gli attributi ai quali non si fa riferimento in alcun punto del sistema possono essere eliminati senza problemi.

  Tuttavia, se un attributo è già in uso (a cui si fa riferimento nelle schede delle tariffe, nei profili utente, nelle risorse o nelle assegnazioni), l’eliminazione viene bloccata per proteggere l’integrità dei dati. In questi casi, se si tenta di rimuovere l’attributo, in particolare tramite una chiamata API, si verifica un errore.

* Test prima del lancio: crea una scheda del tasso pilota e verifica che i tassi corretti siano risolti nelle assegnazioni.
* Documenta la configurazione: condividi la configurazione degli attributi della tariffa con i team in modo che possano comprenderne il funzionamento.

### Dove è possibile applicare gli attributi della tariffa

Gli attributi delle tariffe sono supportati in tutte le aree in cui sono presenti tariffe in Workfront:

* Schede tariffe: consente di definire i tassi in base alla mansione e agli attributi.
* Sostituzioni a livello di progetto: applica gli attributi quando aggiorni i tassi a livello di progetto.
* Ruoli (in Configurazione): imposta le percentuali predefinite dei ruoli con gli attributi.
* Utenti (profili utente): assegna attributi nativi ai singoli utenti in modo che le loro assegnazioni vengano risolte automaticamente in base alle percentuali corrette.

<!--
BULLET POINT Staffing plan resources
BULLET POINT Non-labor resources: Attributes can also be defined on resources such as equipment or services.-->

<!--Non-labor resource categories and -->I ruoli di lavoro non supportano gli attributi del tasso direttamente a livello di oggetto. Sono collegate agli attributi della tariffa attraverso le tariffe definite su di essi.

Quando è possibile creare assegnazioni segnaposto associate ai valori di attributo corretti, le tariffe verranno compilate di conseguenza.

* Per le mansioni, quando successivamente sostituite il segnaposto con un utente reale, il sistema reimposta automaticamente gli attributi dell&#39;assegnazione a quelli definiti nel profilo dell&#39;utente. A questo punto, gli attributi non possono più essere modificati a livello di assegnazione. Ereditano gli attributi dall’utente per preservare la coerenza ed evitare il disallineamento tra gli attributi utente e le tariffe applicate.

<!-- BULLET POINT For non-labor resource categories, placeholder assignments can be used similarly: You assign the category through a placeholder that carries the required attributes. Once the actual non-labor resource is substituted, the attributes are automatically pulled from the resource's profile. Just like with users, these attributes cannot be overridden manually at the assignment level, ensuring financial data integrity and preventing accidental mismatches between resources and their designated attributes.-->

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td>Flusso di lavoro Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td><p>[!UICONTROL Standard]</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurare gli attributi della tariffa

Ogni attributo dispone di un set di opzioni configurabili, incluse le proprietà generali e i filtri.
I filtri controllano il modo in cui i valori degli attributi vengono suggeriti e convalidati durante la definizione delle tariffe. Sono essenziali per mantenere coerenti le selezioni degli attributi, indirizzare gli utenti verso opzioni valide ed evitare combinazioni non valide.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Attributi della tariffa**.
1. Fare clic sull&#39;icona di un segno più nel diagramma per aggiungere un attributo.

   >[!NOTE]
   >
   >Nel diagramma possono essere presenti fino a cinque attributi. L&#39;ordine dall&#39;alto verso il basso definisce la gerarchia di applicazione degli attributi. Fai clic sull&#39;icona **Ruota** ![Icona Ruota](assets/rotate-attribute-view-icon.png) per visualizzare il diagramma da sinistra a destra. È inoltre possibile ingrandire o ridurre e adattare il diagramma allo schermo.

1. Seleziona un attributo per aprire il pannello di configurazione a destra dello schermo.

   ![Configura attributi frequenza](assets/configure-rate-attributes.png)

1. Rinominare gli oggetti (Gruppo, Società, Sede) nei termini necessari per la propria attività (ad esempio Agenzia, Sede, Centro di costo).
1. Fai clic su **Salva** per ciascun attributo per salvare la convenzione di denominazione.

   I nomi di questi attributi verranno visualizzati su tutte le schede e le tariffe del sistema.

1. Impostate le proprietà per ciascun attributo nel pannello di configurazione:

   * **Obbligatorio**: selezionare se l&#39;attributo è un campo obbligatorio nelle tariffe.
   * **Da utilizzare nel calcolo dei ricavi**: include questo attributo nei calcoli delle tariffe di fatturazione.
   * **Da utilizzare nel calcolo dei costi**: include questo attributo nei calcoli dei tassi di costo.

     >[!NOTE]
     >
     >È necessario selezionare almeno una delle opzioni di calcolo affinché l&#39;attributo funzioni nei calcoli finanziari.

   * (Facoltativo) **Gerarchico**: consente all&#39;attributo di rispettare le relazioni padre-figlio, ad esempio Città > Stato > Paese.

     Questa proprietà è disponibile solo per l&#39;oggetto Location.

### Definire i filtri per gli attributi

Per gli attributi sono disponibili due tipi di filtri:

* I filtri suggerimenti restringono l’elenco delle opzioni disponibili in base alla logica di sistema o alle selezioni di attributi precedenti. Gli elenchi a discesa sono facili da usare e tengono conto del contesto.

  Esempio: Agenzia > Ubicazione > Centro di costo

  In questa impostazione, l&#39;attributo Centro di costo deve disporre di un filtro suggerimenti che fa riferimento sia all&#39;agenzia che all&#39;ubicazione.

  Quando si aggiunge una tariffa, se per prima cosa si seleziona Agenzia = &quot;Stella&quot;, il menu a discesa Posizione suggerirà solo le posizioni che appartengono a &quot;Stella&quot;.

  Se in seguito selezioni Posizione = Chicago sulla tariffa, il menu a discesa Centro di costo suggerirà solo i centri di costo associati a &quot;Star&quot; e Chicago.

* I filtri di relazione stabiliscono la catena di dipendenze tra gli attributi. Assicurano che il sistema comprenda il modo in cui gli attributi si relazionano tra loro e applichi dipendenze valide.

  Esempio: Agenzia > Ubicazione > Centro di costo

  In questa impostazione, l&#39;attributo Agenzia deve disporre di un filtro di relazione che lo associa a ubicazioni e centri di costo validi.

I filtri devono essere sempre configurati in entrambe le direzioni. Se l&#39;attributo A dispone di un filtro di relazione con l&#39;attributo B, l&#39;attributo B deve disporre di un filtro di suggerimento per tornare all&#39;attributo A. Ciò garantisce l’integrità dei dati e un’esperienza utente pulita.

1. Seleziona le opzioni per definire i Filtri di suggerimento e i Filtri di relazione per l’attributo nel pannello di configurazione:

   * **Tipo filtro**:

      * Un filtro **Standard** applica una condizione universale all&#39;oggetto attributo. Ad esempio, Posizione > È attivo = True (verranno visualizzate solo le posizioni attive).

        Il filtro Standard viene sempre applicato, indipendentemente dal fatto che siano selezionati altri attributi.

      * Un filtro **Attribute** collega un attributo a un altro nella catena. Ad esempio, Posizione > Riferimento = Agenzia (verranno visualizzate solo le sedi associate all&#39;Agenzia selezionata).

        Il filtro Attributo viene applicato solo se l’attributo di riferimento ha un valore. Ad esempio, se è selezionata l&#39;opzione Agenzia, vengono suggerite solo le sedi valide. Se l’Agenzia è vuota, vengono visualizzate tutte le posizioni (ma è possibile che i filtri standard applicati alla posizione ne limitino comunque il numero).

   * **Campo**: campo diretto dall&#39;oggetto attributo, ad esempio ID posizione o Flag attivo.
   * **Operatore**: queste opzioni dipendono dal tipo di campo selezionato. Gli esempi includono È uguale a, Non è uguale a, È vuoto, True/False.
   * (Solo tipo di filtro standard) **Valore**: Ad esempio, Is Active = True.
   * (Solo tipo di filtro attributi) **Riferimento**: attributo da cui dipende il filtro, ad esempio Agenzia.
   * (Solo per tipo di filtro attributi) **Campo di riferimento**: campo dell&#39;attributo di riferimento che deve corrispondere, ad esempio ID agenzia.

1. Fai clic su **Salva** per ogni attributo per salvare le proprietà e i filtri.
