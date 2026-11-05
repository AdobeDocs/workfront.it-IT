---
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 1%
---
# Istruzioni copilota per workfront.en

Questo archivio contiene la documentazione inglese di Adobe Workfront. Le regole
di seguito si applicano a ogni richiesta in questa area di lavoro. Standard specifici per argomento disponibili in
`.github/instructions/*.instructions.md` e carica automaticamente quando modifichi
file corrispondenti.

## Trova articoli candidati prima di crearne di nuovi

Quando arriva un nuovo contenuto: un documento di accettazione, un feedback del cliente o del PM, un
Incolla Slack/trascrizione, schermate con note o domande di supporto — **no
proporre prima la creazione di un nuovo articolo.** Cerca l’archivio e il candidato della superficie
articoli esistenti in cui il contenuto potrebbe rientrare.

Flusso di lavoro richiesto:

1. **Leggi prima il nuovo contenuto** per identificare argomento, pubblico (amministratore vs. fine
utente) e i fatti o i passaggi specifici che aggiunge.
2. **Cerca in `help/` i candidati** tramite grep e ricerca file. Cerca
articoli che già coprono la stessa funzione, area o flusso di lavoro.
3. **Restituire un elenco classificato** di articoli candidati (in genere 3-7), ciascuno con:
   - Il percorso del file (come collegamento cliccabile).
   - Un motivo su una sola riga: è un candidato (in quale sezione si inserirebbe o perché
     è la corrispondenza più vicina).
   - Eventuali avvertenze (ad esempio, &quot;mancata corrispondenza del pubblico — questo è l’utente finale, l’accettazione è
     admin-facing&quot;).
4. **Chiedi dove inserirlo** prima di disegnare o modificare. Formulare la domanda
esplicitamente, per esempio: &quot;In quale di questi dovrei abbozzare?&quot; o &quot;Voglio che io
inseriscilo in #2, o pensi che abbia bisogno di un proprio articolo?&quot;
5. **Suggerisci un nuovo articolo** solo se nessun articolo esistente può essere considerato appropriato e
spiegare perché nessuno dei candidati lavora.

Anche se il contenuto &quot;ovviamente&quot; appartiene a un articolo noto, comunque superficie 2-3
alternative, in modo che il posizionamento possa essere confermato. Questo cattura i dati quasi duplicati e
luoghi in cui il contenuto era già parzialmente coperto.

## Proponi modifiche prima di modificare gli articoli della guida

Quando si sta per modificare un articolo della Guida di `.md` in `help/`, **non modificare il file
ancora.** Innanzitutto, mostra cosa intendi modificare e attendi l’approvazione esplicita.

Per ogni file che intendi toccare:

1. Denomina il file (percorso).
2. Mostra la modifica proposta come diff/snippet delimitato — testo precedente e nuovo —
con un contesto circostante sufficiente per essere inequivocabile.
3. Riportare brevemente il motivo (una frase).
4. Termina con una domanda esplicita, ad esempio &quot;Applicare queste modifiche?&quot; o &quot;Voglio che io
procedere?&quot;

Solo dopo approvazione esplicita (&quot;sì&quot;, &quot;vai&quot;, &quot;applica&quot;, &quot;fai&quot;, ecc.) dovresti
chiamare gli strumenti di modifica.

Questo vale per **ogni** modifica in un articolo `.md` della guida — errori di battitura, correzioni di collegamenti,
scambi di singole parole, pulizia della terminologia, nuove sezioni e riscritture. No
eccezioni a meno che l’utente non dica esplicitamente &quot;correggilo&quot; o &quot;non chiedere, solo
nello stesso turno.

Per le modifiche che si estendono su più articoli, raggruppa le differenze proposte per file in
una risposta. Se il set è di grandi dimensioni, elencare innanzitutto i file interessati con un riepilogo a una riga
ciascuno, quindi mostra differisce in batch e conferma prima di ogni batch.

**not** blocca la ricerca di sola lettura (grep, read) o la creazione di bozze/esplorazione
in chat (nessuna scrittura di file).

## Riempire gli spazi in modo intelligente

Quando l’intento è chiaro dal contesto, conferma la risposta della best practice anziché
presentazione dei menu di opzione. Applicare gli standard di scrittura (vedere
`.github/instructions/writing-quality.instructions.md`) in modo proattivo — non attendere
per essere ricordati di seguirli. Abbina il nuovo testo a quello dell&#39;articolo circostante
titoli, terminologia e struttura. Chiedi solo quando un&#39;autentica ambiguità
modificare il risultato.

## Messaggi di commit Git

### Oggetto

- Massimo **50 caratteri**.
- Riepilogare la modifica in **umore imperativo** (&quot;Aggiungi...&quot;, &quot;Correggi...&quot;, &quot;Refactoring...&quot;).

### Corpo

- Lascia una riga vuota dopo l’oggetto davanti al corpo.
- Dispone le righe a circa **72 caratteri**.
- Utilizza **righe punto elenco** per la spiegazione. Ogni punto elenco deve iniziare esattamente con
uno dei seguenti:
  - **📖** — quando la modifica **aggiunge** qualcosa di nuovo: nuovi file, nuove sezioni, nuovi
    caratteristiche, nuove intestazioni, righe nuove o altro contenuto di campi verdi.
  - **✏️** — quando la modifica **modifica** il lavoro esistente: modifica le righe esistenti,
    aggiornamenti a sezioni esistenti, refactoring o modifiche al contenuto corrente.

Esempio:

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```

## Richieste di pull

### Derivazione del problema Jira

- Deriva l&#39;ID del problema Jira dal nome del ramo Git **corrente** (ad esempio un
segmento corrispondente a `FFENT-8796`).
- **Se il nome della filiale include un ID Jira:** usa tale ID nel titolo e nel collegamento PR
tra `# Context` → `## Jira`.
- **Se il nome del ramo non include un ID Jira:** omettere la chiave Jira dal PR
titolo. Includi ancora `## Jira` con esattamente `No ticket`.

### Titolo PR

- **Con ID Jira:** `{type}/{JIRA-ID}- {short task description}`
  - Esempio: `feat/FFENT-8001- Add validation for numVariations in OCAPI request`
- **Senza Jira ID:** `{type}- {short task description}`
  - Esempio: `docs- Refresh Object Composite API changelog`

Tipi di commit: **feat** (nuova funzionalità), **fix** (correzione bug), **refactoring** (ristrutturazione)
senza modifica del comportamento), **perf** (prestazioni), **style** (solo formattazione),
**test** (test), **docs** (solo documentazione, nuovo contenuto), **build** (build/CI/
dipendenze), **ops** (infrastruttura/distribuzione), **chore** (varie).

### Organismo PR — Sezioni obbligatorie

- `# Summary` — breve panoramica delle modifiche e del motivo.
- `# Changes` - organizzato per file. Per ogni file toccato, utilizza un’intestazione di livello 2
con il percorso in apici retroversi, quindi punti elenco.
- `# Context` — includi sempre una sottosezione `## Jira` con il problema collegato, oppure
  `No ticket`.

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```
