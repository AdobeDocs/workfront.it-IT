---
title: Esempi di campo di ricerca esterna in un modulo personalizzato
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Un campo di ricerca esterna in un modulo personalizzato chiama un’API esterna e restituisce i valori come opzioni in un campo a discesa. Questo articolo fornisce esempi sull’utilizzo del campo Ricerca esterna per richiamare la stessa istanza di Workfront o un’API pubblica.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: a082f010dbd78235aaad41a80d87d772ca77ff89
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# Esempi di campo di ricerca esterna in un modulo personalizzato

Un campo di ricerca esterna in un modulo personalizzato chiama un’API esterna e restituisce i valori come opzioni in un campo a discesa. Gli utenti che utilizzano l’oggetto a cui è associato il modulo personalizzato possono selezionare una o più di queste opzioni dal menu a discesa.

Questo articolo fornisce esempi sull’utilizzo del campo Ricerca esterna per richiamare la stessa istanza di Workfront o un’API pubblica. È inoltre possibile utilizzare la funzione di ricerca esterna per comunicare con un sistema esterno come Jira, Salesforce o ServiceNow.

Per ulteriori informazioni sull’aggiunta di un campo di ricerca esterna a un modulo personalizzato e ulteriori definizioni dei componenti di ricerca esterna, vedi [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Impostare un campo di ricerca esterna per la stessa istanza di Workfront

Puoi utilizzare la funzione di ricerca esterna per inserire nel modulo personalizzato i dati dell’istanza di Workfront.

Questo esempio mostra come chiamare l’API Workfront e inserire i dati dal campo &quot;Status Query&quot; esistente nel campo di ricerca esterna.

1. Apri il modulo personalizzato.
1. Sul lato sinistro dello schermo, trovare **Ricerca esterna** e trascinarlo in una sezione dell’area di lavoro.
1. Inserisci il **Etichetta** e **Nome** per il campo.
1. Seleziona la **Formato** per il campo.
1. Immetti la chiamata URL API in **URL API di base** campo.

   * È possibile aggiungere $$HOST per fare riferimento alla stessa istanza.
   * È possibile aggiungere $$QUERY per filtrare i risultati in base all&#39;esecuzione di query in un campo diverso.

   **Esempio**
   `$$HOST/attask/api/v15.0/project/search?status={DE:StatusQuery}&$$QUERY`

1. Rivedi **Dipendenze** per i campi a cui fa riferimento il campo di ricerca nell’API.

   Un campo dipendenza può essere un qualsiasi campo personalizzato o nativo esistente nella pagina dei dettagli dell&#39;oggetto.

   In questo esempio, la proprietà `{DE:StatusQuery}` verrà sostituito con il valore del campo personalizzato StatusQuery.

1. Seleziona la **Metodo HTTP**.

   Questo sarà per lo più **Ottenere**.

1. Inserisci il **Percorso JSON** per ottenere i risultati dalla chiamata API.

   **Esempio**
   `$.data[*].name`

   >[!NOTE]
   >
   >**Intestazione** non sono necessarie informazioni per una chiamata alla stessa istanza di Workfront.

1. Clic **Applica**.

   ![Configurazione della chiamata API a Workfront in formato personalizzato](assets/external-lookup-to-workfront.png)

   Quando il modulo personalizzato viene aggiunto a un oggetto Workfront (in questo esempio, un progetto), ha un aspetto simile al seguente.

   ![Modulo personalizzato con campo di ricerca esterno](assets/external-lookup-project-status-example1.png)

   ![Opzioni di ricerca esterna basate sullo stato](assets/external-lookup-project-status-example2.png)

## Configurare un campo di ricerca esterno per un’API pubblica

Puoi utilizzare la funzione di ricerca esterna per richiamare un’API pubblica esterna e recuperare dati.

Questo esempio mostra come chiamare un’API di paesi (come <https://api.first.org/data/v1/countries>) in modo da non dover codificare tutti i nomi dei paesi nelle opzioni a discesa.

1. Apri il modulo personalizzato.
1. Sul lato sinistro dello schermo, trovare **Ricerca esterna** e trascinarlo in una sezione dell’area di lavoro.
1. Inserisci il **Etichetta** e **Nome** per il campo.
1. Seleziona la **Formato** per il campo.
1. Immetti la chiamata URL API in **URL API di base** campo.

   * È possibile aggiungere $$QUERY per implementare il filtro delle query per gli utenti finali.

   **Esempi**
Elenca tutti i paesi: <https://api.first.org/data/v1/countries>

   Consente all’utente di cercare qualsiasi paese nel campo a discesa: <https://api.first.org/data/v1/countries?q=$$QUERY>

   Consente all&#39;utente di cercare un paese in un&#39;area: <https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

   * Le aree disponibili sono definite in un campo personalizzato separato in Workfront.
   * Quando l’utente seleziona un’area nel modulo, il campo Ricerca esterna mostra solo i paesi di tale area (quale paese si trova in quale area è definita nell’API). L’utente può anche cercare un paese nell’area selezionata.

1. Rivedi **Dipendenze** per i campi a cui fa riferimento il campo di ricerca nell’API.

   Un campo dipendenza può essere un qualsiasi campo personalizzato o nativo esistente nella pagina dei dettagli dell&#39;oggetto.

   In questo esempio, la proprietà `{DE:Region}` verrà sostituito con il valore del campo personalizzato Regione.

1. Seleziona la **Metodo HTTP**.

   Questo sarà per lo più **Ottenere**.

1. Inserisci il **Percorso JSON** per ottenere i risultati dalla chiamata API.

   Questa opzione consente di estrarre i dati dal JSON restituito dall’URL API. Serve come modo per selezionare quali valori dall’interno del JSON appariranno nelle opzioni a discesa.

   **Esempio**
   `$.data[*].country`

1. (Facoltativo) Fai clic su **Aggiungi intestazione** e digita o incolla la coppia chiave-valore richiesta per l’autenticazione con l’API.

   >[!NOTE]
   >
   >I campi Intestazione non rappresentano un luogo sicuro in cui archiviare le credenziali. È necessario prestare attenzione a ciò che si immette e si salva.

1. (Facoltativo) Seleziona **Elenco a discesa a selezione multipla** per consentire all’utente di selezionare più di un valore nel menu a discesa.

1. Clic **Applica**.

   ![Configurazione della chiamata API all&#39;API pubblica in un modulo personalizzato](assets/external-lookup-to-api-for-countries.png)

   Quando il modulo personalizzato viene aggiunto a un oggetto Workfront (in questo esempio, un progetto), ha un aspetto simile al seguente.

   ![Modulo personalizzato con campo di ricerca esterno](assets/external-lookup-countries-example1.png)

   ![Opzioni di ricerca esterna per un paese in base all’area geografica](assets/external-lookup-countries-example2.png)

