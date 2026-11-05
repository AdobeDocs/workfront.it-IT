---
description: Regole di formattazione e convalida per le note sulla versione di Adobe Workfront (panoramica, area di prodotto, pagine di pianificazione e look-and-feel).
applyTo: "help/quicksilver/product-announcements/product-releases/**/*.md"
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%
---

# Formattatore note sulla versione

Questi file sono **note sulla versione**, non articoli di istruzioni. **non** applica
standard generali di qualità della scrittura. Prima di modificare, leggi l’origine completa di
Verità, che include i modelli e il calendario di rilascio:

- [.cursor/skills/release-notes-formatter/SKILL.md](../../.cursor/skills/release-notes-formatter/SKILL.md)
- [.cursor/skills/release-notes-formatter/reference.md](../../.cursor/skills/release-notes-formatter/reference.md)

## Regola critica: determinare prima il trimestre del documento

> [!IMPORTANT]
> Non assegnare mai una funzione a un trimestre documento utilizzando la matematica del trimestre calendario sulla relativa
> Data di anteprima o produzione. Il doc-trimestre è basato su quale **rilascio mensile**
> la funzione viene fornita in, in base al raggruppamento interno del calendario delle versioni di Workfront, che
> viene scostato dal trimestre del calendario. Ad esempio, una funzione con una Production
> la data del 13 agosto 2026 appartiene al trimestre documento `26-q4`, non `26-q3`. Sempre
> controlla la tabella del calendario della versione 2026 nel file di riferimento prima di
> creazione o modifica di file. Se la data di produzione non rientra nella tabella,
> chiedere un calendario aggiornato anziché indovinare.

## Regole strutturali fondamentali

- **Frontmatter**: `feature` deve essere esattamente `Product Announcements`;
  `recommendations` deve essere esattamente `noDisplay, noCatalog`. Non inventare mai un
  `exl-id` — includerlo solo se ne esiste già uno.
- **Prima le nuove funzionalità**: la nota sulla versione più recente è la prima H2 dopo
l&#39;introduzione (pagine dell&#39;area prodotti) e la riga superiore di ogni tabella delle funzioni (panoramica
pagine).
- **Collegamento panoramica**: le pagine dell&#39;area di prodotto devono essere collegate a **del proprio trimestre**
file di panoramica — un bug comune è il collegamento al trimestre precedente.
- **Callout data**: ogni funzionalità H2 è seguita da un blocco `>[!NOTE]` con
Anteprima / Produzione versione rapida / Produzione per tutte le date, corrispondente al
riga tabella panoramica. Formattare le date come `Month Day, Year`; utilizzare `TBD` se sconosciuto.
- **Nomi di trimestre scritti** in H1: &quot;Primo trimestre&quot;, &quot;Secondo trimestre&quot;, &quot;Terzo
Quarter&quot;, &quot;Fourth Quarter&quot;.

## Aggiornamenti complementari richiesti per l’aggiunta di pagine

- **Nuova pagina (qualsiasi)**: aggiungerla a `help/quicksilver/TOC.md` con la stessa modifica
(per prima cosa, visualizza le pagine dell’area prodotto in ordine alfabetico, e per ultima gli altri miglioramenti).
- **Pagina panoramica del nuovo trimestre**: aggiorna anche `help/quicksilver/home.md` —
aggiorna i collegamenti della scheda &quot;Ultima versione&quot; e dell’attività di pianificazione, quindi aggiungi
il nuovo trimestre alla scheda versioni dell’anno corrente.

Consultate i file SKILL.md e reference.md sopra per i modelli completi,
le convenzioni di denominazione dei file, i formati dei collegamenti e il calendario completo della versione.
