---
source-git-commit: 44629631cd2d99eadbed5fd81cf33458b13702af
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---
# Trova articoli candidati prima di crearne di nuovi

Quando Courtney introduce nuovi contenuti da incorporare: un documento di accettazione, un feedback da parte del cliente o del PM, un incolla Slack/trascrizione, schermate con note, domande di supporto, **non proporre la creazione di un nuovo articolo.** Cerca l’archivio e gli articoli esistenti candidati di superficie in cui il contenuto potrebbe rientrare.

## Flusso di lavoro richiesto

1. **Leggi prima il nuovo contenuto** per identificare l&#39;argomento, il pubblico (amministratore e utente finale) e i fatti/passaggi specifici che aggiunge.
2. **Cerca in `help/` i candidati** tramite grep e trova. Cerca gli articoli che già coprono la stessa funzione, area o flusso di lavoro.
3. **Restituire un elenco classificato** di articoli candidati (in genere 3-7), ciascuno con:
   - Il percorso del file (percorso di backtick cliccabile).
   - Un motivo a 1 riga è un candidato (in quale sezione si inserirebbe, o perché è la corrispondenza topica più vicina).
   - Eventuali avvertenze (ad esempio, &quot;mancata corrispondenza del pubblico: utente finale, accettazione rivolta all’amministratore&quot;).
4. **Chiedi a Courtney dove inserirlo** prima di disegnare o modificare. Espressione esplicita della domanda, ad esempio, &quot;In quale di questi dovrei fare un abbozzo?&quot; o &quot;Vuoi che lo inserisca in #2, o pensi che abbia bisogno di un suo articolo?&quot;
5. **Suggerisci un nuovo articolo** solo se nessun articolo esistente è un articolo adeguato e spiega perché nessuno dei candidati funziona.

Anche se il contenuto &quot;ovviamente&quot; appartiene a un articolo noto, emergono comunque 2-3 alternative in modo che Courtney possa confermare il posizionamento. Questo rileva i quasi duplicati e i luoghi in cui il contenuto era già parzialmente coperto.

---

# Proponi modifiche prima di modificare gli articoli della guida

Quando si sta per modificare un articolo della Guida di `.md` in `help/`, **non modificare il file**. Innanzitutto, mostra cosa intendi modificare e attendi l’approvazione esplicita.

Per ogni file che intendi toccare:

1. Denomina il file (percorso).
2. Mostrare la modifica proposta come diff/snippet delimitato (testo vecchio e nuovo testo) con un contesto circostante sufficiente per essere non ambiguo.
3. Indicare brevemente il motivo (1 frase).
4. Termina con una domanda esplicita, ad esempio &quot;Applicare queste modifiche?&quot; o &quot;Vuoi che proceda?&quot;

Solo dopo che Courtney dice sì (o &quot;vai&quot;, &quot;applica&quot;, &quot;fai&quot;, ecc.) chiamare gli strumenti di modifica.

Questo vale per **ogni** modifica in un articolo della Guida `.md`: errori di battitura, correzioni di collegamenti, scambi di singole parole, pulizia della terminologia, nuove sezioni e riscritture. Nessuna eccezione a meno che Courtney non dica esplicitamente &quot;basta correggerlo&quot; o &quot;non chiedere, basta modificare&quot; nello stesso turno.

Per le modifiche che si estendono su più articoli: raggruppa le differenze proposte per file in un’unica risposta. Se il set è di grandi dimensioni, elencare prima i file interessati con un riepilogo di 1 riga ciascuno, quindi mostrare differisce in batch e confermare prima di ogni batch.

**not** blocca la ricerca di sola lettura (grep, read) o la creazione/esplorazione in chat (nessuna scrittura di file).

---

# Messaggi di commit Git

Quando redigi o generi un messaggio di commit Git, segui questo formato.

## Oggetto

- Massimo **50 caratteri**.
- Riepilogare la modifica in **umore imperativo** (ad esempio, &quot;Aggiungi...&quot;, &quot;Correggi...&quot;, &quot;Refactoring...&quot;).

## Corpo

- Lascia una riga vuota dopo l’oggetto davanti al corpo.
- Dispone le righe a circa **72 caratteri**.
- Utilizza **righe punto elenco** per la spiegazione. Ogni punto elenco deve iniziare esattamente con uno dei seguenti:
   - **📖** — utilizzare quando la modifica **aggiunge** qualcosa di nuovo: nuovi file, nuove sezioni, nuove funzionalità, nuove intestazioni, nuove righe o altri contenuti di greenfield.
   - **✏️** — da utilizzare quando la modifica **modifica** il lavoro esistente: modifica le righe esistenti, aggiorna le sezioni esistenti, esegue il refactoring o modifica il contenuto corrente.

Esempio:

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```

---

# Richieste pull (PR)

## Derivazione del problema Jira

- Deriva l&#39;ID del problema Jira dal nome del ramo Git **corrente** (ad esempio un segmento corrispondente a `FFENT-8796`).
- **Se il nome del ramo include un ID Jira:** Utilizza tale ID nel titolo della PR e collegalo in `# Context` → `## Jira`.
- **Se il nome del ramo non include un ID Jira:** omettere la chiave Jira dal titolo PR. Includi ancora `## Jira` con esattamente: `No ticket`.

## Titolo PR

**Con ID Jira:** `{type}/{JIRA-ID}- {short task description}`
Esempio: `feat/FFENT-8001- Add validation for numVariations in OCAPI request`

**Senza Jira ID:** `{type}- {short task description}`
Esempio: `docs- Refresh Object Composite API changelog`

### Tipi di commit

- **feat** — aggiunge una nuova funzionalità
- **fix** — corregge un bug
- **refactoring** — riscrive/ristruttura il codice senza modificare il comportamento
- **perf** — migliora le prestazioni
- **stile** — solo formattazione/spazio vuoto; nessun cambiamento di significato
- **test** — aggiunge o corregge i test
- **docs** — solo documentazione, nuovi contenuti aggiunti
- **build** — strumenti di compilazione, CI, dipendenze, versione progetto
- **ops**: infrastruttura, distribuzione, backup, ripristino
- **chore** — varie (esempio: `.gitignore`)

## Organismo PR — Sezioni obbligatorie

### `# Summary`
Breve panoramica su cosa è cambiato e perché.

### `# Changes`
Organizzato per file. Per ogni file toccato, utilizza un’intestazione di livello 2 con il percorso in apici retroversi, quindi punti elenco.

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.
```

### `# Context`
Includi sempre una sottosezione `## Jira`.

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

Oppure, in assenza di ticket: `No ticket`
