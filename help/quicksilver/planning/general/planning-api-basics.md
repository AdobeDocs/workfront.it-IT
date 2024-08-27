---
title: Nozioni di base sulle API di Adobe Workfront Planning
description: L’obiettivo per l’API di pianificazione di Adobe Workfront è semplificare la creazione di integrazioni con Planning introducendo un’architettura REST-ful che funziona tramite HTTP. Questo documento presuppone che tu abbia familiarità con le risposte REST e JSON e descrive l’approccio adottato dall’API di Planning.
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: 20e8d45264f9441d9576c7d4d5521e4f6053a7f3
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 1%

---


# Nozioni di base sulle API di Adobe Workfront Planning

{{planning-important-intro}}

L’obiettivo per l’API di pianificazione di Adobe Workfront è semplificare la creazione di integrazioni con Planning introducendo un’architettura REST-ful che funziona tramite HTTP. Questo documento presuppone che tu abbia familiarità con le risposte REST e JSON e descrive l’approccio adottato dall’API di Planning.

La familiarità con lo schema di Workfront Planning consente di comprendere le relazioni tra i database che possono essere utilizzate per estrarre i dati da Workfront Planning a scopo di integrazione.

Puoi richiamare l’API di pianificazione da un campo di ricerca Esterna in un modulo personalizzato Workfront.

Per ulteriori informazioni sui campi di ricerca esterna, vedere [Esempi di campi di ricerca esterna in un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

## URL API di Workfront Planning

<!--For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

### Operazioni

Gli oggetti vengono manipolati inviando una richiesta HTTP al relativo URI univoco. L&#39;operazione da eseguire è specificata dal metodo HTTP.

I metodi HTTP standard corrispondono alle operazioni seguenti:

* **GET** - Recupera un oggetto per ID, cerca tutti gli oggetti tramite una query
* **POST** - Inserisce un nuovo oggetto
* **PUT** - Modifica un oggetto esistente
* **DELETE** - Elimina un oggetto

Per ulteriori dettagli ed esempi di ciascuna operazione, vedere la [documentazione per gli sviluppatori API di Workfront Planning](https://developer.adobe.com/wf-planning/).

### Tipi di campi e modificatori di ricerca utilizzati con tali campi

È possibile utilizzare modificatori e filtri con i campi per controllare quali dati verranno restituiti nei risultati.

<!--For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

#### Utilizzo dei modificatori di ricerca

Workfront Planning supporta i seguenti modificatori di ricerca:

<table>
    <tr>
        <td><b>Modificatore</b></td>
        <td><b>Esempio</b></td>
        <td><b>Descrizione</b></td>
        <td><b>Valori possibili</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Restituisce record il cui valore di campo contiene il filtro  </td>
        <td>"Lancio di nuovi prodotti"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Restituisce record in cui il valore del campo non contiene il filtro  </td>
        <td>"Nuovo lancio"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Restituisce record il cui valore di campo corrisponde esattamente al filtro  </td>
        <td>"Lancio di nuovi prodotti"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Restituisce record il cui valore di campo non corrisponde esattamente al filtro  </td>
        <td>"Lancio di nuovi prodotti"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Restituisce record il cui valore di campo non è vuoto  </td>
        <td><ul><li>“” </li><li>nulle </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Restituisce record il cui valore di campo non è vuoto  </td>
        <td>"Lancio di nuovi prodotti"  </td>
    </tr>
    <tr>
        <td>$GREATERThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Restituisce record il cui valore di campo è maggiore del filtro  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$majorThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Restituisce record il cui valore di campo è maggiore o uguale al filtro  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Restituisce record il cui valore di campo è minore del filtro  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Restituisce record il cui valore di campo è minore o uguale al filtro </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Restituisce record il cui valore di campo è dopo il filtro  </td>
        <td>"2024-05-15T20:00:00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Restituisce record il cui valore di campo è precedente al filtro </td>
        <td>"2024-05-12T20:00:00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Restituisce record il cui valore di campo è compreso tra il filtro  </td>
        <td><ul><li>"2024-05-12T20:00:00.000Z" </li><li>"2024-05-14T20:00:00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Restituisce record il cui valore di campo non è compreso tra il filtro  </td>
        <td><ul><li>"2024-05-09T20:00:00.000Z"  </li><li>"2024-05-17T20:00:00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Restituisce record il cui valore di campo corrisponde a uno qualsiasi dei filtri  </td>
        <td><ul><li>"active" </li><li>"completato" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Restituisce record il cui valore di campo non è incluso nel filtro </td>
        <td><ul><li>"completato"  </li><li>"fisso"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Restituisce record il cui valore di campo include uno dei filtri  </td>
        <td><ul><li>["attivo", "fisso"]  </li><li>["fisso", "completato", "finito"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Restituisce record il cui valore di campo include tutto il filtro  </td>
        <td><ul><li>["attivo", "completato"]   </li><li>["attivo", "completato", "finito"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Restituisce record il cui valore di campo non contiene alcun filtro </td>
        <td>["fisso", "completato"]  </td>
    </tr>
    <tr>
        <td>$isExexact </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Restituisce record il cui valore di campo è esattamente il filtro  </td>
        <td>["attivo", "completato"]  </td>
    </tr>
</table>

#### Tipi di campo

Di seguito è riportato l’elenco dei tipi di campo supportati e i modificatori di ricerca che è possibile utilizzare con ciascuno di questi tipi di campo

| Tipo di campo | Modificatori di ricerca supportati |
|---|---|
| text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| testo lungo | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| numero | $is, $isNot, $majorThan, $majorThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| percentuale | $is, $isNot, $majorThan, $majorThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| valuta | $is, $isNot, $majorThan, $majorThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| data | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| selezione singola | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| selezione multipla | $hasAnyOf, $hasAllOf, $isExexact, $hasNoneOf, $isEmpty, $isNotEmpty |
| booleano | $is |
| utente | $hasAnyOf, $hasAllOf, $isExexact, $hasNoneOf, $isEmpty, $isNotEmpty |
| formula | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| creato da | $is, $isNot, $isAnyOf, $isNoneOf |
| creato a | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| aggiornato da | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| update-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| riferimento | $hasAnyOf, $hasAllOf, $isExexact, $hasNoneOf, $isEmpty, $isNotEmpty |
| ricerca | Dipende dal campo collegato |

### Utilizzo delle istruzioni &quot;And&quot; e &quot;Or&quot;

Nella chiamata API è possibile avere filtri basati su diversi criteri combinati da istruzioni $and&quot; e &quot;$or&quot;

```
{
  "recordTypeId": "recordTypeId",
  "offset": "integer",
  "limit": "integer",
  "filters": [
    {
      "$or": [
        {
          "launch_date": {
            "$isBetween": [
              "2024-03-31T20:00:00.000Z",
              "2024-04-01T20:00:00.000Z"
            ]
          }
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-03-31T20:00:00.000Z",
                  "2024-04-01T20:00:00.000Z"
                ]
              }
            },
            {
              "status": "active"
            }
          ]
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-04-15T00:00:00.000Z",
                  "2024-04-16T00:00:00.000Z"
                ]
              }
            },
            {
              "status": "planned"
            }
          ]
        }
      ]
    }
  ]
}
```

### Utilizzo del parametro della richiesta fields

Puoi utilizzare il parametro di richiesta fields per specificare un elenco separato da virgole di campi specifici da restituire. Questi nomi di campo fanno distinzione tra maiuscole e minuscole.

Ad esempio, la richiesta

`/v1/records/search?attributes=data,createdBy`

```
{
    "records": [
        {
            "id": "Rc6527ecb35df57c441d92ba00",
            "createdBy": "61a9cc0500002f9fdaa7a6f824f557e1",
            "createdAt": null,
            "updatedBy": null,
            "updatedAt": null,
            "customerId": null,
            "imsOrgId": null,
            "recordTypeId": null,
            "data": {
                "F666c0b58b6fee61a2ea6ea81": [
                    {
                        "externalId": null,
                        "id": "Rc665728ff95730b58bc757b13",
                        "value": null
                    },
....
```

restituisce una risposta simile alla seguente:


```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Ordinamento dei risultati della query nell’API

Puoi ordinare i risultati in base a qualsiasi campo se aggiungi quanto segue alla chiamata API:


`/v1/records/search`

Corpo della richiesta:

```
{
    "recordTypeId": "Rt6527ecb25df57c441d92b9fa",
    "filters": [],
    "sorting": [
        {
            "fieldId": "F6527ecb25df57c441d92b9fc",
            "direction": "asc"
        },
        {
            "fieldId": "F658afcbd4a0273c67c346fd5",
            "direction": "desc"
        }
    ],
    "limit": 500,
    "offset": 0,
    "rowOrderViewId": "V6527ecb75df57c441d92ba03",
    "groupingFieldIds": []
}
```

### Limiti delle query e risposte impaginate

Per impostazione predefinita, le richieste API di Planning restituiscono 500 risultati, a partire dall’inizio dell’elenco. Per ignorare il limite predefinito per il numero di risultati, è possibile utilizzare il parametro `limit` nelle richieste e impostarlo su un numero diverso, fino a 2.000 risultati.

È consigliabile considerare l&#39;utilizzo di risposte impaginate per set di dati di grandi dimensioni aggiungendo il parametro `offset` alle richieste. Le risposte impaginate consentono di specificare la posizione del primo risultato che deve essere restituito.

Ad esempio, se si desidera restituire i risultati 2001-4000, è possibile utilizzare la seguente richiesta. In questo esempio vengono restituiti 2000 record con stato attivo, a partire dal risultato 2001:

`POST /v1/records/search `



Corpo della richiesta:

```
{ 
    "recordTypeId": "recordTypeId", 
    "offset": "2001", 
    "limit": "2000", 
    "filters": [ 
        { "status": "active" } 
    ] 
} 
```

Per assicurarti che i risultati siano impaginati correttamente, utilizza un parametro di ordinamento. Questo consente di restituire i risultati nello stesso ordine, in modo che l’impaginazione non si ripeta né salti i risultati.

Per ulteriori informazioni sull&#39;ordinamento, vedere [Ordinamento dei risultati della query nell&#39;API](#sorting-query-results-in-the-api) in questo articolo.
