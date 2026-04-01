---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 1%

---
# Messaggi di commit Git

Applica sempre questa regola. Quando crei o generi un messaggio di commit Git (ad esempio nella casella di commit Controllo Source o quando richiesto nella chat dell’agente), segui questo formato.

## Oggetto (solo prima riga)

- Massimo **50 caratteri**.
- Riepilogare la modifica in **umore imperativo** (ad esempio, &quot;Aggiungi...&quot;, &quot;Correggi...&quot;, &quot;Refactoring...&quot;).

## Riga vuota

Lascia una **riga vuota** dopo l&#39;oggetto davanti al corpo.

## Corpo (descrizione dettagliata)

- Racchiudi righe a circa **72 caratteri** (inclusi il prefisso e lo spazio del punto elenco).
- Utilizza **righe punto elenco** per la spiegazione. Ogni punto elenco deve iniziare esattamente con uno dei seguenti:
   - **📖** — utilizzare quando la modifica **aggiunge** qualcosa di nuovo: nuovi file, nuove sezioni, nuove funzionalità, nuove intestazioni, nuove righe o altri contenuti di greenfield.
   - **✏️** — da utilizzare quando la modifica **modifica** il lavoro esistente: modifica righe esistenti, aggiornamenti a sezioni esistenti, refactoring del codice esistente o modifiche al contenuto corrente.

Applica **📖** o **✏️** a ogni punto elenco in modo che sia chiaro cosa è stato introdotto e cosa è stato modificato.

## Modello

Compila i segnaposto (non lasciare parentesi angolari nel messaggio finale):

```
<Summarize change(s) in around 50 characters or less>

<More detailed explanatory description of the change wrapped into about 72
characters with bullets. >
```

## Esempio

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```
