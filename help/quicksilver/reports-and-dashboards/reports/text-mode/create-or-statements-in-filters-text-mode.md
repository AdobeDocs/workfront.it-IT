---
product-area: reporting
navigation-topic: text-mode-reporting
title: Creare istruzioni "OR" nei filtri in modalità testo
description: È possibile includere più istruzioni quando si crea un filtro in elenchi e report.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: af4a82ad11b57c7a7457d5d7ee74ee18494a1dc0
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Creare istruzioni &quot;OR&quot; nei filtri in modalità testo

È possibile includere più istruzioni quando si crea un filtro in elenchi e report.

Per informazioni sulla creazione di filtri, consulta i seguenti articoli:

* [Panoramica filtri](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Modificare un filtro utilizzando la modalità testo](/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Operatori filtro modalità testo

Per informazioni sugli operatori dei filtri Adobe Workfront nell&#39;interfaccia dei filtri standard, vedere [Panoramica sui filtri](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront dispone di 2 operatori di filtro che collegano ogni istruzione di filtro:

* **AND**: quando si unisce a 2 l&#39;istruzione di filtro dell&#39;operatore AND, si indica che si desidera che entrambe le istruzioni di filtro vengano soddisfatte contemporaneamente.

  Per impostazione predefinita, le istruzioni in un filtro sono unite dall&#39;operatore AND.

  Quando si crea un filtro AND nell&#39;interfaccia in modalità testo, non è necessario utilizzare l&#39;operatore AND. Si presume.

  **Esempio:** Per filtrare le attività con una data di completamento pianificata di oggi e una percentuale di completamento inferiore al 100%, utilizzare il codice in modalità testo seguente:

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq 
  percentComplete=100 percent
  Complete_Mod=lt
  ```

* **OR**: quando si uniscono due istruzioni di filtro dell&#39;operatore OR, si indica che si desidera soddisfare una delle due istruzioni.

  >[!TIP]
  >
  >Quando si modificano i rendiconti AND in rendiconti OR, il numero di elementi nel rapporto dovrebbe aumentare.

  Quando si crea un filtro OR utilizzando l’interfaccia della modalità testo, è necessario utilizzare l’operatore OR.

  **Esempio:** Per filtrare le attività con una data di completamento pianificata di oggi o una percentuale di completamento inferiore al 100%, utilizzare il codice in modalità testo seguente:

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq
  OR:1:percentComplete=100
  OR:1:percentComplete_Mod=lt
  ```

## Sintassi in modalità testo per i filtri OR

La sintassi della modalità testo per un filtro OR deve contenere i seguenti elementi:

* Operatore OR seguito da due punti, un numero e un altro due punti all&#39;inizio di ogni riga di filtro che fa riferimento all&#39;oggetto nell&#39;istruzione OR. Ciò include la riga che fa riferimento al campo o all’attributo del filtro e la riga che fa riferimento al modificatore del filtro.

  Segui questo pattern durante la creazione di un filtro OR:

  ```
  <field name in camel case>=<value>
  <field name in camel case>_Mod=<modifier value>
  OR:1:<field name in camel case>=<value>
  OR:1:<field name in camel case>_Mod=<modifier value>
  ```

  >[!TIP]
  >
  >L’operatore OR distingue tra maiuscole e minuscole e utilizza sempre lettere maiuscole.

  In un filtro possono essere presenti più istruzioni OR. In questo caso, a ogni istruzione OR viene assegnato un numero, nell&#39;ordine in cui si desidera applicare le istruzioni.

  **Esempio:** Per filtrare le attività con data di completamento pianificata di oggi o con percentuale di completamento inferiore al 100% OPPURE con stato Nuovo, utilizzare il codice della modalità testo seguente:

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq
  OR:1:status=NEW
  OR:1:status_Mod=in
  OR:2:percentComplete=100
  OR:2:percentComplete_Mod=lt
  ```

* Il nome dei campi o gli attributi a cui si fa riferimento in un filtro devono essere scritti in Camel Case. Per informazioni sull&#39;uso di Camel Case, vedere [Panoramica sulla sintassi della modalità testo](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* Quando si fa riferimento a campi personalizzati in un filtro OR, è necessario inserire DE: tra la sintassi del modificatore OR e il nome del campo personalizzato. È necessario digitare il nome del campo personalizzato così come viene visualizzato nell&#39;interfaccia di Workfront.

  **Esempio:** Per filtrare le attività con uno stato Nuovo o una percentuale di completamento inferiore al 100% OPPURE un campo personalizzato denominato &quot;Tipo account&quot; con un valore &quot;Uguale a&quot;, utilizzare il codice della modalità testo seguente:

  ```
  status=NEW
  status_Mod=in
  OR:1:percentComplete=100
  OR:1:percentComplete_Mod=lt
  OR:2:DE:Account Type=Capital
  OR:2:DE:Account Type_Mod=in
  ```
