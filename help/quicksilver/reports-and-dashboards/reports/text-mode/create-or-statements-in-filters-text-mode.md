---
product-area: reporting
navigation-topic: text-mode-reporting
title: Creare istruzioni "OR" nei filtri in modalità testo
description: È possibile includere più istruzioni quando si crea un filtro in elenchi e rapporti.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Creare istruzioni &quot;OR&quot; nei filtri in modalità testo

È possibile includere più istruzioni quando si crea un filtro in elenchi e rapporti.

Per informazioni sulla creazione dei filtri, consulta i seguenti articoli:

* [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Modificare un filtro utilizzando la modalità testo](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Operatori del filtro Modalità testo

Per informazioni sugli operatori di filtri Adobe Workfront nell’interfaccia di filtro standard, vedi [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront dispone di 2 operatori filtro che collegano ogni istruzione filtro:

* **E**: Quando si unisce l’istruzione di filtro 2 dall’operatore AND, si indica che si desidera soddisfare entrambe le istruzioni di filtro contemporaneamente.

   Per impostazione predefinita, le istruzioni in un filtro sono collegate dall’operatore AND.

   Quando si crea un filtro AND nell’interfaccia in modalità testo, non è necessario utilizzare l’operatore AND. Si presume.

   **Esempio:** Per filtrare le attività con una data di completamento pianificata di oggi e una percentuale di completamento inferiore al 100%, utilizzare il seguente codice della modalità di testo:

   <pre>scheduledCompletionDate=$$OGGI</pre><pre>scheduledCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **O**: Quando si uniscono 2 istruzioni di filtro dall&#39;operatore OR, si indica che si desidera soddisfare entrambe le istruzioni.

   >[!TIP]
   >
   >Quando si modificano le istruzioni AND in istruzioni OR, il numero di elementi nel rapporto dovrebbe aumentare.

   Quando si crea un filtro OR utilizzando l’interfaccia in modalità testo, è necessario utilizzare l’operatore OR.

   **Esempio:** Per filtrare le attività per le quali la data di completamento pianificata è oggi o la percentuale di completamento è inferiore al 100%, utilizzare il seguente codice della modalità di testo:

   <pre>scheduledCompletionDate=$$OGGI</pre><pre>scheduledCompletionDate_Mod=eq</pre><pre>O:1:percentComplete=100</pre><pre>O:1:percentComplete_Mod=lt</pre>

## Sintassi della modalità testo per i filtri OR

La sintassi della modalità testo per un filtro OR deve contenere quanto segue:

* Operatore OR seguito da due punti, un numero e un altro due punti all&#39;inizio di ogni riga di filtro che fa riferimento all&#39;oggetto nell&#39;istruzione OR. Ciò include la linea che fa riferimento al campo o all&#39;attributo del filtro e la linea che fa riferimento al modificatore del filtro.

   Segui questo pattern durante la creazione di un filtro OR:

   <pre><field name in camel case>=<value></pre><pre><field name in camel case>_Mod=<modifier value></pre><pre>O:1:<field name in camel case>=<value></pre><pre>O:1:<field name in camel case>_Mod=<modifier value></pre>

   >[!TIP]
   >
   >L’operatore OR distingue tra maiuscole e minuscole ed è sempre maiuscolo.

   È possibile che in un filtro siano presenti più istruzioni OR. In questo caso, ogni istruzione OR riceve un numero, nell&#39;ordine in cui si desidera applicare le istruzioni.

   **Esempio:**  Per filtrare le attività che hanno una data di completamento pianificata di oggi o una percentuale di completamento inferiore al 100% O uno stato di nuovo, utilizzare il seguente codice della modalità di testo:

   <pre>scheduledCompletionDate=$$OGGI</pre><pre>scheduledCompletionDate_Mod=eq</pre><pre>O:1:status=NEW</pre><pre>O:1:status_Mod=in</pre><pre>O:2:percentComplete=100</pre><pre>O:2:percentComplete_Mod=lt</pre>

* Il nome dei campi o degli attributi a cui si fa riferimento in un filtro deve essere scritto in camel case. Per informazioni sul cammello, vedi [Panoramica della sintassi della modalità testo](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* Quando si fa riferimento a campi personalizzati in un filtro OR, è necessario inserire DE: tra la sintassi del modificatore OR e il nome del campo personalizzato. È necessario digitare il nome del campo personalizzato così come viene visualizzato nell’interfaccia di Workfront.

   **Esempio:** Per filtrare le attività che hanno uno stato Nuovo o una percentuale di completamento inferiore al 100% O un campo personalizzato denominato &quot;Tipo account&quot; con un valore pari a &quot;Uguale&quot;, utilizza il seguente codice della modalità di testo:

   <pre>status=NEW</pre><pre>status_Mod=in</pre><pre>O:1:percentComplete=100</pre><pre>O:1:percentComplete_Mod=lt</pre><pre>O:2:DE:Tipo di conto=Capitale</pre><pre>O:2:DE:Tipo di account_Mod=in</pre>
