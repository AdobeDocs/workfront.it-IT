---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---
# Richieste pull (PR)

Quando redigi o rivedi un titolo o una descrizione di richiesta di pull (ad esempio in GitHub/GitLab o quando viene richiesto nella chat dell’agente), segui queste convenzioni.

## Derivazione del problema Jira

- **Source of true:** deriva l&#39;ID del problema Jira dal **nome del ramo Git corrente** (ad esempio un segmento corrispondente al modello di chiave del progetto, ad esempio `FFENT-8796`).
- **Se il nome del ramo include un ID Jira:** Utilizza tale ID nel titolo PR (vedi sotto) e collegalo in `# Context` → `## Jira`.
- **Se il nome della filiale non include un ID Jira:** Considera la PR come non associata a un ticket. **Ometti** la chiave Jira dal titolo PR (non inventare un ticket). Includi ancora `# Context` → `## Jira`, con il contenuto esatto: `No ticket` (nessun collegamento).

## Titolo PR

**Quando il nome del ramo include un ID problema Jira**, includi **entrambi**:

1. **ID problema Jira** (esempio: `FFENT-8001`).
2. Il tipo **commit** (vedi elenco di seguito), che utilizza questo modello:

`{type}/{JIRA-ID}- {short task description}`

Esempio:

`feat/FFENT-8001- Add validation for numVariations in OCAPI request`

Utilizza una descrizione concisa in stile imperativo dopo l’ID. Corrispondenza con il pattern di spaziatura mostrato: testo, barra, tasto Jira con trattino finale, spazio, quindi descrizione.

**Se il nome del ramo non include un ID di problema Jira**, ometti il ticket dal titolo e utilizza:

`{type}- {short task description}`

Esempio:

`docs- Refresh Object Composite API changelog`

### Tipi di commit accettabili (utilizzare esattamente queste etichette prima di `/`)

- **feat** — aggiunge una nuova funzionalità. Quando viene aggiunto un nuovo elemento del sommario o il file JIRA è connesso a un altro Jira con etichetta `feat`.
- **fix** — corregge un bug
- **refactoring** — riscrive/ristruttura il codice senza modificare il comportamento
- **perf** — migliora le prestazioni (refactoring speciale)
- **stile** — solo formattazione/spazio vuoto; nessun cambiamento di significato. Solo modifiche
- **test** — aggiunge o corregge i test
- **documenti** — Nuovo contenuto aggiunto. solo documentazione
- **build**: strumenti di compilazione, CI, dipendenze, versione del progetto e così via.
- **ops**: infrastruttura, distribuzione, backup, ripristino e così via.
- **chore** — varie (esempio: `.gitignore`)

## Organismo PR — Sezioni obbligatorie

Utilizza **esattamente le sezioni principali** (intestazioni Markdown):

### 1. `# Summary`

Breve panoramica di **cosa** è cambiato e **perché** (intento tecnico o commerciale).

### 2. `# Changes`

Organizza per **file**. Per ogni file toccato, utilizza un’intestazione di livello 2 con il percorso in apici retroversi, quindi punti elenco che descrivono le modifiche.

Formato:

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

## `another/file.ts`
* Another bullet for that file.
```

### 3. `# Context`

Includi sempre una sottosezione **Jira** in `# Context`.

**Quando il nome del ramo include un ID Jira:** Utilizza un collegamento cliccabile per il problema (deriva la chiave dal nome del ramo).

Formato:

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

Sostituisci la chiave e l’URL con il ticket effettivo. Se vengono applicati più biglietti, elencarli ciascuno sulla propria riga nella stessa sottosezione.

**Se il nome del ramo non include un ID Jira:** Mantieni `## Jira` e utilizza esattamente:

```markdown
# Context

## Jira
No ticket
```

## Esempio (descrizione PR completa)

```markdown
# Summary
Adds minimum and maximum constraints for numVariations in the Object Composite API v4 OpenAPI spec.

# Changes

## `static/object-composite-v4.json`
* numVariations in OCAPIRequest now includes minimum: 1 and maximum: 3 to align with the allowed range (number of variations to generate).

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

## Esempio (descrizione PR completa, ramo senza ID Jira)

**Titolo:** `docs- Refresh Object Composite API changelog`

```markdown
# Summary
Refreshes the changelog for the Object Composite API.

# Changes

## `CHANGELOG.md`
* Documents the latest OCAPI v4 constraint updates.

# Context

## Jira
No ticket
```
