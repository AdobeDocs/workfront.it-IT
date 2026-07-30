---
name: release-notes-formatter
description: Formatta e convalida le note sulla versione di Workfront per coerenza, struttura corretta e collegamento corretto. Da utilizzare solo per i file delle note sulla versione nelle directory delle versioni di prodotto o quando l’utente cita note sulla versione, versioni di prodotto o versioni trimestrali. Non applicare ad articoli tutorial o alla documentazione generale.
source-git-commit: fa39320af72acf6d2ceaf201480baf78a07ae76e
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 2%

---


# Note sulla versione Formatter

Formatta e convalida le note sulla versione di Adobe Workfront nella directory `help/quicksilver/product-announcements/product-releases/`.

## Tipi di pagina

Identifica il tipo di pagina dal percorso e dal contenuto del file:

| Tipo di pagina | Pattern file | Modello |
|-----------|-------------|----------|
| **Panoramica** | `{YY}-q{N}-release-overview.md` | Vedi .claude/commands/_release-notes-formatter-reference.md#overview-page-template |
| **Area di prodotto** | `{YY}-q{N}-{area}.md` | Vedi .claude/commands/_release-notes-formatter-reference.md#product-area-page-template |
| **Pianificazione** | `planning-release-activity-{YY}-q{N}.md` | Simile all&#39;area di prodotto |
| **Aspetto** | `look-and-feel-updates-{YY}-q{N}.md` | Vedi .claude/commands/_release-notes-formatter-reference.md#look-and-feel-page-template |

## Passaggio 0: Determinare il trimestre (eseguire questa operazione prima di qualsiasi altra operazione)

>[!IMPORTANT]
>
>Non assegnare mai una funzione a un trimestre documento utilizzando la matematica del trimestre calendario nella data di anteprima o produzione. Il doc-trimestre si basa sulla **versione mensile** in cui viene spedita la funzionalità, in base al raggruppamento interno del calendario delle versioni di Workfront, che è offset dal trimestre del calendario. Vedere la tabella del [Calendario delle versioni di 2026](#2026-release-calendar) vicino alla fine del file. Ad esempio, una funzione con data di produzione del 13 agosto 2026 appartiene al trimestre `26-q4`, non a `26-q3`, perché la versione mensile di agosto è mappata su `26-q4`.
>
>La tabella &quot;Mappatura trimestre&quot; più in basso (Modulo scritto / Mesi) serve per scrivere i nomi dei trimestri nei titoli (ad esempio, &quot;Terzo trimestre&quot; per Q3) — è **non** sufficiente da solo per decidere in quali file del trimestre una funzione appartiene. Eseguire sempre il controllo incrociato con la tabella Calendario rilascio prima di creare o modificare qualsiasi file.
>
>Se la data di produzione di una funzione non viene visualizzata nella tabella del calendario di rilascio (ad esempio, è oltre l’intervallo di date della tabella), chiedi all’utente un calendario aggiornato anziché indovinare.

## Flusso di lavoro di formattazione

### Passaggio 1: Convalida materiale

Campi obbligatori per tutte le pagine delle note sulla versione:

```yaml
---
title: <descriptive title>
description: <matches or summarizes the title>
author: <author name>
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: <existing UUID — never generate or change>
---
```

Regole:
- `feature` deve essere esattamente `Product Announcements`
- `recommendations` deve essere esattamente `noDisplay, noCatalog`
- Non inventare mai un `exl-id`. Includere solo se ne esiste già uno
- Non aggiungere `draft: Probably` a pagine reali (solo modelli)

### Passaggio 2: Convalida struttura per tipo di pagina

#### Pagine area prodotto

1. **H1**: `{Written Quarter} {Area} enhancements`
   - Esempio: `# Second Quarter 2026 Administrator enhancements`
   - Il trimestre deve essere compilato: &quot;Primo trimestre&quot;, &quot;Secondo trimestre&quot;, &quot;Terzo trimestre&quot;, &quot;Quarto trimestre&quot;

2. **Paragrafo introduttivo**: descrive l&#39;area e i collegamenti alla panoramica
   - Deve essere collegato al file di panoramica **del trimestre corretto**
   - Bug comune: collegamento al trimestre precedente (ad esempio, `26-q1` anziché `26-q2`)

3. **H2 per funzionalità**: titolo funzionalità come intestazione
   - **Prima le nuove funzioni**: la nota sulla versione più recente deve apparire come primo H2 dopo il paragrafo dell&#39;introduzione
   - Le feature meno recenti seguono in ordine cronologico inverso

4. **Blocco callout data** dopo ogni H2:

```markdown
>[!NOTE]
>
>Preview: {Month Day, Year}
>Production fast release: {Month Day, Year}
>Production for everyone: {Month Day, Year}
```

&#x200B;5. **Corpo**: descrizione funzione, quindi collegamento alla documentazione

#### Pagine Panoramica

1. **H1**: `{Written Quarter} release overview`

2. **Paragrafo introduttivo** con mese di rilascio pianificato

3. **`>[!IMPORTANT]`blocco** con tabella di pianificazione della versione

4. **H2`Adobe Workfront enhancements`** con elenco puntato di collegamenti di ancoraggio:

```markdown
* [Administrator enhancements](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
```

&#x200B;5. **H3 per area di prodotto** con tabella delle funzionalità di HTML (vedere .claude/commands/_release-notes-formatter-reference.md#overview-feature-table)
   - All&#39;interno di ogni tabella, **prima le funzionalità più recenti**. La riga più recente viene visualizzata nella parte superiore della tabella (dopo la riga di intestazione)

&#x200B;6. **Sezioni finali** (H2): note sulla versione per altre aree, aggiornamenti del visualizzatore per la verifica del desktop, annunci, versione API, aggiornamenti di manutenzione, aggiornamenti di formazione

### Passaggio 3: Convalidare i collegamenti

- **Collegamento alla panoramica nelle pagine dell&#39;area di prodotto**: deve puntare allo stesso trimestre
  - Corretto: `26-q2-release-activity/26-q2-release-overview.md`
  - Sbagliato: `26-q1-release-activity/26-q1-release-overview.md`
- **Collegamenti di ancoraggio nella panoramica**: devono corrispondere agli ID H3 (lettere minuscole, trattini)
- **Collegamenti alle funzionalità nelle tabelle di panoramica**: deve utilizzare `class="MCXref xref" xrefformat="{para}"`
- **Collegamenti alla documentazione della Guida**: deve iniziare con `/help/quicksilver/`

### Passaggio 4: Convalidare le date

- Formato: `{Month} {Day}, {Year}` (esempio: &quot;12 marzo 2026&quot;)
- Usa `TBD` per date sconosciute
- Le date nel blocco della pagina dell&#39;area di prodotto `>[!NOTE]` devono corrispondere alla riga della tabella di panoramica corrispondente
- Le date di anteprima devono precedere le date di produzione

### Passaggio 5: Correzioni comuni

Applica queste correzioni durante la formattazione:

| Problema | Correggi |
|-------|-----|
| Trimestre collegamento panoramica errato | Aggiorna per corrispondere al trimestre del file |
| Blocco date `>[!NOTE]` mancante | Aggiungi blocco dopo l&#39;intestazione della funzionalità H2 |
| Formato data non coerente | Standardizza su `Month Day, Year` |
| Riga vuota mancante prima di `>[!NOTE]` | Aggiungi riga vuota |
| Spazi aggiuntivi nelle linee del callout | Ritaglia spazio vuoto finale |
| HTML nelle pagine dell’area prodotti | Mantieni come markdown (HTML è solo per tabelle di panoramica) |
| Manca `exl-id` | Escludilo — non generarne uno |

### Passaggio 6: aggiornare il sommario

Ogni volta che crei una pagina delle note sulla versione di **new** (panoramica o area prodotti), aggiungila a `help/quicksilver/TOC.md` con la stessa modifica. Una pagina non inclusa nel sommario non verrà visualizzata nella navigazione pubblicata, anche se i collegamenti presenti nella tabella panoramica vi fanno riferimento.

Dove aggiungerlo:

- Il sommario include una sezione al trimestre sotto un&#39;intestazione come `* 2026 Q3 Release {#release-26-q3}`. Se il titolo del trimestre non esiste ancora (prima pagina di un nuovo trimestre), aggiungilo sopra il trimestre precedente in modo che sia in alto il trimestre più recente.
- Sotto l’intestazione del trimestre, elenca le pagine nell’ordine seguente:
  1. **Panoramica** (`Third Quarter 2026 release overview`).
  2. **Pagine dell&#39;area di prodotto** in ordine alfabetico per nome area (amministratore, documenti, operazioni dell&#39;organizzazione, progetti, reporting, richiesta).
  3. **Altri miglioramenti** sono stati apportati per ultimi (sempre dopo le aree alfabetiche dei prodotti).

Ogni voce del sommario è un collegamento di markdown che utilizza il titolo della pagina e il percorso assoluto dell’archivio:

```markdown
      * [Third Quarter 2026 Documents enhancements](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-documents.md)
```

Abbina il rientro (sei spazi) alle voci circostanti. Utilizzare la pagina H1 come testo di collegamento, ad esempio `Documents enhancements`, `Requesting enhancements` (non `Requests`), in modo che le etichette del sommario corrispondano ai trimestri precedenti.

Errori comuni da evitare:

- Creazione di una pagina dell&#39;area di prodotto senza aggiungerla al sommario.
- Collegamento alla panoramica di un trimestre diverso dalla nuova pagina dell’area di prodotto (passaggio 3).
- Inserire le pagine di un nuovo trimestre sotto l&#39;intestazione del trimestre precedente.

### Passaggio 7: aggiornare la home page

Quando crei una **nuova pagina di panoramica del trimestre** (ovvero, questa è la prima pagina di un nuovo trimestre, non solo una nuova pagina di area di prodotto aggiunta a un trimestre esistente), aggiorna `help/quicksilver/home.md` con la stessa modifica:

- Nella sezione `>[!TAB Latest release]`, sostituisci il collegamento della panoramica della versione con il collegamento della panoramica del nuovo trimestre.
- Anche in questa sezione, aggiornare il collegamento dell&#39;attività di rilascio di Adobe Workfront Planning in modo che punti al file di pianificazione del nuovo trimestre (`planning-release-activity-{YY}-q{N}.md`), se esistente.
- Nella scheda `>[!TAB {YYYY} releases]` per l&#39;anno corrente, aggiungi il collegamento di panoramica del nuovo trimestre nella parte superiore dell&#39;elenco, sopra la voce del trimestre precedente.

Non toccare `home.md` quando si aggiunge solo una pagina dell&#39;area di prodotto a un trimestre in cui è già elencata una pagina di panoramica.

Errori comuni da evitare:

- Creazione della pagina di panoramica di un nuovo trimestre senza aggiornamento della scheda &quot;Ultima versione&quot; di `home.md` (continuerà a puntare al trimestre precedente).
- Dimenticando di aggiungere anche il nuovo trimestre all’elenco di schede dell’anno corrente.

## Convenzioni di denominazione dei file

| Tipo | Pattern | Esempio |
|------|---------|---------|
| Panoramica | `{YY}-q{N}-release-overview.md` | `26-q2-release-overview.md` |
| Area di prodotto | `{YY}-q{N}-{area-slug}.md` | `26-q2-admin-and-setup.md` |
| Directory | `{YY}-q{N}-release-activity/` | `26-q2-release-activity/` |

Campioni area standard: `admin-and-setup`, `documents`, `projects`, `reports`, `requests`, `other`

## Mappatura trimestre

>[!NOTE]
>
>Questa tabella serve per scrivere i nomi dei trimestri (ad esempio, in un H1 o in un titolo). Non determina i file del trimestre a cui appartiene una funzionalità. A tale scopo, utilizza la tabella [Calendario di rilascio 2026](#2026-release-calendar) riportata di seguito, poiché il trimestre doc viene scostato dal trimestre del calendario.

| Trimestre | Modulo scritto | Months |
|---------|-------------|--------|
| Q1 | Primo Trimestre | Gen-Mar |
| Q2 | Secondo trimestre | Apr-Giu |
| Q3 | Terzo trimestre | lug-set |
| Q4 | Quarto trimestre | Ott-Dic |

**Importante: il trimestre del documento utilizzato nei nomi dei file (`26-q3`, `26-q4`, ecc.) è scostato di un mese da questo mapping del calendario.** Segue invece il raggruppamento interno del calendario di rilascio di Workfront, dove ogni trimestre doc = i due rilasci mensili precedenti + il mese di rilascio trimestrale. Ad esempio, il trimestre del documento `26-q3` copre i rilasci mensili di maggio/giugno/luglio 2026 (rilascio trimestrale `2026.07`) e il trimestre del documento `26-q4` copre i rilasci mensili di agosto/settembre/ottobre 2026 (rilascio trimestrale `2026.10`). Controlla sempre il calendario di rilascio riportato di seguito (o richiedine uno aggiornato) prima di considerare il trimestre di un file in base alla tabella dei trimestri del calendario riportata sopra.

## Calendario delle versioni 2026

Source: &quot;2026 Monthly Release Calendar&quot; (wiki di Adobe corp, spazio AWF — `wiki.corp.adobe.com`, chiave dello spazio AWF, titolo &quot;2026 Monthly Release Calendar&quot;). WebFetch non può raggiungere questa pagina (richiede l’SSO di Adobe); chiedi all’utente di incollare un PDF/tabella aggiornato quando sono necessarie date diverse da quelle acquisite qui.

| Mese di rilascio | Anteprima finale | Production | Rilascio mensile | Rilascio trimestrale | Trimestre doc |
|---|---|---|---|---|---|
| Novembre 2025 | 30 ottobre 2025 | 13 novembre 2025 | 2025.11 | 2026.01 | 26-q1 |
| Dic 2025 | 27 novembre 2025 | 11 dicembre 2025 | 2025.12 | 2026.01 | 26-q1 |
| Gennaio 2026 | 23 dicembre 2025 | 15 gennaio 2026 | 2026.01 | 2026.01 | 26-q1 |
| Febbraio 2026 | 29 gennaio 2026 | 12 febbraio 2026 | 2026.02 | 2026.04 | 26-q2 |
| Mar 2026 | 26 febbraio 2026 | 12 marzo 2026 | 2026.03 | 2026.04 | 26-q2 |
| Apr 2026 | 2 aprile 2026 | 16 aprile 2026 | 2026.04 | 2026.04 | 26-q2 |
| Maggio 2026 | 30 aprile 2026 | 14 maggio 2026 | 2026.05 | 2026.07 | 26-q3 |
| Giu 2026 | 28 maggio 2026 | 11 giugno 2026 | 2026.06 | 2026.07 | 26-q3 |
| Lug 2026 | 7 luglio 2026 | 16 luglio 2026 | 2026.07 | 2026.07 | 26-q3 |
| Ago 2026 | 30 luglio 2026 | 13 agosto 2026 | 2026.08 | 2026.10 | 26-q4 |
| Set 2026 | 3 settembre 2026 | 17 settembre 2026 | 2026.09 | 2026.10 | 26-q4 |
| Ott 2026 | 1 ottobre 2026 | 15 ottobre 2026 | 2026.10 | 2026.10 | 26-q4 |
| Novembre 2026 | 29 ottobre 2026 | 12 novembre 2026 | 2026.11 | 2027.01 | 27-q1 |
| Dic 2026 | 26 novembre 2026 | 10 dicembre 2026 | 2026.12 | 2027.01 | 27-q1 |
| Gennaio 2027 | 5 gennaio 2027 | 14 gennaio 2027 | 2027.01 | 2027.01 | 27-q1 |

Note sull&#39;utilizzo di questa tabella:

- **Anteprima finale** è l&#39;ultima data in cui le funzionalità possono essere visualizzate nell&#39;anteprima per la versione mensile specifica. Utilizzarla per l&#39;elenco puntato &quot;data dell&#39;ultima visualizzazione delle funzionalità nell&#39;ambiente di anteprima&quot; della pagina della panoramica (solo per il mese di fine trimestre).
- **Produzione** è la data ufficiale di produzione per tutti per quella versione mensile.
- Per il mese di fine trimestre (quello corrispondente alla colonna Rilascio trimestrale), la tabella di pianificazione della pagina della panoramica elenca la versione di quel mese **due volte**: una volta nella colonna &quot;Rilascio mensile&quot; data **un giorno prima** della data di produzione (data di rilascio rapido) e una volta nella colonna &quot;Rilascio trimestrale&quot; data della data di produzione effettiva. I mesi non finali di un trimestre utilizzano la stessa data di produzione sia nell’elenco mensile che nei riferimenti &quot;a rilascio rapido&quot;, senza necessità di adeguamento.
- Questa tabella va fino a gennaio 2027. Se sono necessarie date successive, chiedi all’utente di fornirgli un calendario aggiornato anziché indovinarlo.

Il rilascio della produzione trimestrale solitamente arriva il giovedì della seconda settimana completa dell’ultimo mese del trimestre.

## Elenco di controllo convalida

Durante la revisione di un file delle note sulla versione, verificare:

- [ ] Frontmatter ha tutti i campi obbligatori con valori corretti
- [ ] H1 corrisponde al formato del tipo di pagina
- [ Il collegamento Panoramica di ] punta al trimestre corretto
- [ ] Ogni funzione ha un blocco di data `>[!NOTE]` (pagine dell&#39;area prodotti)
- [ ] Formato data coerente (`Month Day, Year`)
- [ ] righe della tabella delle funzionalità nella panoramica corrispondono al contenuto della pagina dell&#39;area di prodotto
- [ ] Nessun collegamento interno interrotto
- [ ] I collegamenti di ancoraggio nella panoramica corrispondono agli ID sezione H3
- [ Le funzionalità di ] sono ordinate in ordine di novità (sia nelle pagine dell&#39;area di prodotto che nelle tabelle di panoramica)
- [ ] Le nuove pagine delle note sulla versione sono elencate in `help/quicksilver/TOC.md` nel trimestre corretto, con la prima panoramica e le aree di prodotto in ordine alfabetico (Altre ultime)
- [ ] Se è stata creata la pagina della panoramica di un nuovo trimestre, `help/quicksilver/home.md` la scheda &quot;Ultima versione&quot; e la scheda dell&#39;anno corrente vi puntano

## Risorse aggiuntive

- Per esempi e modelli completi di HTML, consultate .claude/commands/_release-notes-formatter-reference.md
