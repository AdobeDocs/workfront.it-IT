---
description: Standard di scrittura tecnica Workfront per gli articoli della guida. Applica la Guida di stile alla documentazione di Workfront e i principi DQTI (Developing Quality Technical Information).
applyTo: "help/**/*.md"
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 1%
---

# Qualità di scrittura

Applicare questi standard durante la modifica, la revisione o la scrittura di un articolo della Guida.
Preservare l&#39;intento dell&#39;autore e l&#39;accuratezza tecnica. Per il completamento
punteggiatura, terminologia, maiuscole e riferimento alla procedura, da leggere
[.cursor/skills/writing-quality/reference.md](../../.cursor/skills/writing-quality/reference.md).

**non** applica queste regole alle note sulla versione in
`help/quicksilver/product-announcements/product-releases/` — utilizza
invece, istruzioni release-notes-formatter.

## Voce e punto di vista

- Usa **seconda persona** (&quot;Puoi...&quot;) quando si rivolge al lettore.
- Usa le contrazioni per un tono di conversazione (non, non può, è, sono).
- Utilizzare &quot;Consigliamo&quot; per le best practice, non &quot;È consigliato&quot; o &quot;Dovresti&quot;.
- Quando scrivi per un gruppo di utenti, fai riferimento ad altri ruoli in terza persona.
- Non usare mai pronomi di genere — ristrutturate la frase o usate &quot;loro&quot;.
- Nessuna barra per le scelte — usa &quot;o&quot; (&quot;lui o lei&quot; non &quot;lui/lei&quot;).

## Chiarezza (DQTI)

- Un&#39;idea per frase; mantieni le frasi sotto ~25 parole dove possibile.
- Lead con l’azione o il risultato, non con il contesto di sfondo.
- Utilizza la parola più semplice (&quot;utilizzare&quot; non &quot;utilizzare&quot;, &quot;avviare&quot; non &quot;avviare&quot;).
- Evita le nominalizzazioni (&quot;crea&quot; e non &quot;creazione di&quot;).
- Utilizza un linguaggio specifico e concreto: evita termini vaghi (&quot;diversi&quot;, &quot;diversi&quot;).
- Evita doppi negativi.

## Concretezza e orientamento dei compiti (DQTI)

- Utilizza esempi specifici con valori realistici; denomina elementi e campi dell’interfaccia utente esatti.
- Concentrati su ciò che l&#39;utente può *fare*, non su ciò che il sistema *è*.
- Eseguire procedure con verbi imperativi (&quot;Creare un&#39;attività&quot;, &quot;Configurare le notifiche&quot;).
- Fornisci un contesto sufficiente per agire, ma non più.
- Includi un collegamento alla Guida dettagliata (&quot;Per ulteriori informazioni, vedi [articolo].&quot;).

## Uso delle maiuscole

- **Titoli**: maiuscole/minuscole della frase sempre (&quot;Crea un&#39;attività&quot;, non &quot;Crea un&#39;attività&quot;).
- **Termini di Workfront**: usare l&#39;iniziale maiuscola solo quando si fa riferimento direttamente a un elemento dell&#39;interfaccia utente.
  - Diretto: &quot;Completare il campo Data di completamento pianificata&quot;.
  - Indiretto: &quot;Ogni attività deve avere una data di completamento pianificata.&quot;
  - Suggerimento: se riesci a mettere &quot;il&quot; o &quot;a&quot; davanti al termine, di solito è in minuscolo.
- **Pulsanti**: segui le maiuscole nell&#39;interfaccia utente; i pulsanti maiuscoli diventano lettere maiuscole.
- **Ruoli**: &quot;Amministratore di sistema&quot; per il ruolo nell&#39;interfaccia utente; &quot;Workfront
administrator&quot; per la persona.

## Intestazioni

- Comando imperativo in caso di frase, basato su attività (&quot;Configura livelli di accesso&quot;).
- Gli articoli Panoramica terminano con &quot;Panoramica&quot; (&quot;Panoramica dei progetti&quot;).
- Suddividi sezioni lunghe in più intestazioni con obiettivi secondari chiari.

## Riferimenti incrociati e collegamenti

| Situazione | Formato |
|-----------|--------|
| Collega dopo aver fornito le informazioni | &quot;Per ulteriori informazioni, vedere [Nome articolo].&quot; |
| Collegamento senza informazioni precedenti | &quot;Per informazioni, vedere [Nome articolo].&quot; |
| Collegamento a una sezione in un altro articolo | &quot;Per ulteriori informazioni, vedere [Nome sezione] in [Nome articolo].&quot; |
| Collegamento a una sezione nello stesso articolo | &quot;Per ulteriori informazioni, vedere [Nome sezione] in questo articolo.&quot; |

- In un paragrafo: in linea. In un passaggio della procedura: su una nuova riga dopo il passaggio.
- Più collegamenti: utilizza un elenco puntato.
- Utilizzare &quot;angolo superiore destro&quot; / &quot;angolo superiore sinistro&quot; per le posizioni dello schermo.

## Grassetto e corsivo

- **Bold** azioni selezionabili ed elementi dell&#39;interfaccia utente **solo nei passaggi della procedura**.
- Non applicare il grassetto agli elementi dell&#39;interfaccia utente, ai nomi delle finestre di dialogo, alle pagine, alle icone o ai menu
nomi al di fuori dei passaggi della procedura.
- Utilizza *corsivo* per il testo che l&#39;utente deve digitare (&quot;Digitare *my.workfront.com*...&quot;).
- Non usate mai il corsivo per enfasi — ristrutturate la frase invece.

## Note, suggerimenti e avvisi

Usare con moderazione: l&#39;uso eccessivo li rende invisibili.

- Massimo una nota/suggerimento/avviso per sezione; non sovrapporle mai.
- Combinare le note correlate in una nota con un elenco puntato.
- Non utilizzare le note per annunciare nuove funzionalità. Rielaborare il testo dell&#39;articolo.

| Tipo | Scopo |
|------|---------|
| `>[!NOTE]` | Informazioni che non rientrano nel paragrafo; controllo delle versioni/compatibilità |
| `>[!TIP]` | Suggerimenti utili per semplificare la vita dell&#39;utente |
| `>[!IMPORTANT]` | Informazioni essenziali per la fase o la procedura |
| `>[!WARNING]` | Avvisa l&#39;utente in caso di potenziale perdita di dati |

## Procedure

- Utilizza le intestazioni di comando imperative; le introduzioni solo se necessario.
- Formato di introduzione preferito: frase infinita + due punti (&quot;Per creare un
password:&quot;).
- Le procedure in un unico passaggio utilizzano ancora un elenco numerato.
- Utilizzare &quot;type&quot; o &quot;select&quot;, evitando parole vaghe come &quot;set&quot; o &quot;specified&quot;.
- Passaggi condizionali: &quot;(condizionale) Se sei membro di più team,
seleziona...&quot;. Passaggi facoltativi: &quot;(Facoltativo) Per aggiungere un’emoji, fai clic su...&quot;.
- Descrivere la risposta del sistema prima o immediatamente dopo.
- Più metodi: documenta prima il modo più semplice, quindi utilizza &quot;Or&quot;.
- Navigazione menu/scheda: &quot;Fai clic su **E-mail** > **Notifiche**&quot; (grassetto i nomi, non
le parentesi; spazi intorno alle parentesi). Non utilizzare parentesi per il menu principale
navigazione - utilizzare lo snippet del menu principale.

## Riferimento rapido punteggiatura

| Regola | Esempio |
|------|---------|
| Oxford virgola sempre | &quot;movente, mezzi e opportunità&quot; |
| Virgola prima di &quot;then&quot; nelle procedure | &quot;Fare clic su Configurazione, quindi su Interfaccia.&quot; |
| Virgola dopo anno in una data a metà frase | Il 2 gennaio 2016, numero di... |
| Nessuna virgola con solo mese-anno | &quot;Gennaio 2016&quot; |
| Due punti prima di un elenco, lettere minuscole dopo | &quot;Selezionare una delle opzioni seguenti: opzione A&quot; |
| Nessun due punti dopo i titoli della procedura | &quot;Creare un’attività&quot; |
| Trattini lungo | Ristrutturare la pena se possibile |
| Periodi nelle estensioni file | &quot;Carica un file .pdf&quot; |

## Organizzazione (DQTI)

- Struttura logica con divulgazione progressiva (panoramica → dettagli → riferimento).
- Un argomento per sezione; utilizza gli elenchi per più di 3 elementi paralleli.
- Mantieni le voci di elenco e le relative consegne grammaticalmente parallele.
- Utilizzare le tabelle per confronti strutturati o descrizioni di campi.
- Evita i paragrafi a muro di testo, suddividendoli in blocchi digeribili.

## Elenco di controllo per la convalida

- [ ] seconda persona in tutto, contrazioni utilizzate.
- [ ] Tutte le intestazioni sono in maiuscolo.
- [ ] termini Workfront maiuscoli correttamente (riferimento diretto o indiretto).
- [ ] Grassetto solo per le azioni selezionabili nei passaggi della procedura.
- [ ] I riferimenti incrociati utilizzano il formato standard.
- [ ] note/suggerimenti/avvisi non sovrapposti, massimo uno per sezione.
- [ ] virgola Oxford utilizzata in modo coerente.
- [ ] Le procedure utilizzano verbi specifici (tipo, selezione, clic).
- [ ] Passaggi condizionali/facoltativi etichettati correttamente.
- [ ] Nessun pronome con genere.
- [ ] Le frasi sono chiare, concrete e orientate alle attività; la struttura parallela è valida.
