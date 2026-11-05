---
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%
---
# AGENTS.md

Indicazioni sull&#39;agente per l&#39;archivio **workfront.en** (inglese Adobe Workfront)
documentazione). Questo file punta alle istruzioni canoniche in modo che qualsiasi agente —
indipendentemente dal file della convenzione che legge, segue le stesse regole.

## File di istruzioni canoniche

- **Regole a livello di repository**: [.github/copilot-instructions.md](.github/copilot-instructions.md)
— formati di ricerca di articoli candidati, di proposte preliminari alla modifica, di impegni di messaggi e PR,
e &quot;riempire i vuoti in modo intelligente&quot;.
- **Standard di scrittura** (si applica automaticamente a `help/**/*.md`):
  [.github/instructions/writing-quality.instructions.md](.github/instructions/writing-quality.instructions.md),
con dettagli completi in
  [.cursor/skills/writing-quality/reference.md](.cursor/skills/writing-quality/reference.md).
- **Note sulla versione** (si applica automaticamente a `product-announcements/product-releases/**`):
  [.github/instructions/release-notes-formatter.instructions.md](.github/instructions/release-notes-formatter.instructions.md).
- **Pulizia evidenziazione anteprima** (flusso di lavoro su richiesta):
  [.github/prompts/remove-preview-highlighting.prompt.md](.github/prompts/remove-preview-highlighting.prompt.md).

## Comportamenti non negoziabili

1. **Trovare gli articoli candidati prima di crearne di nuovi.** Quando arriva un nuovo contenuto
in, cerca `help/` e visualizza un elenco di articoli esistenti che potrebbe contenere,
quindi chiedi a chi appartiene prima di scrivere.
2. **Proporre modifiche prima di modificare qualsiasi articolo della Guida `.md`.** Mostra la proposta
Differf e attendi l’approvazione esplicita. L&#39;unica eccezione è quando dico &quot;correggi
it&quot; o &quot;don&#39;t ask, just edit&quot; (non chiedere, modifica solo) nello stesso turno. Ricerca in sola lettura e in chat
le bozze vanno sempre bene.
3. **Risolvi gli spazi in modo intelligente.** Quando l&#39;intento è chiaro, esegui il commit
una risposta alle best practice e che corrisponda ai titoli dell’articolo circostante,
terminologia e struttura invece di presentare i menu di opzione.
4. **Applica gli standard di scrittura in modo proattivo** a ogni modifica di `help/`. Non aspettare
da ricordare.

## Convenzioni Commit e PR

Per informazioni complete, vedere [.github/copilot-instructions.md](.github/copilot-instructions.md)
formato commit-message (oggetto imperativo ≤ ~50 caratteri; 📖 per le aggiunte, ✏️ per
modifiche) e struttura PR (ID Jira dal nome della filiale; `# Summary`,
`# Changes` per file, `# Context` → `## Jira`).
