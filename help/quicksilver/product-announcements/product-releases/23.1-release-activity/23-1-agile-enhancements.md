---
title: 23.1 Miglioramenti di Agile
description: 23.1 Miglioramenti di Agile
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# 23.1 Miglioramenti di Agile

Questa pagina descrive tutti i miglioramenti Agile apportati con la versione 23.1 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione la settimana del 16 gennaio 2023.

Per un elenco di tutte le modifiche disponibili con la versione 23.1, consulta [Panoramica sulla versione 23.1](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

## Pianificazione Scrum per le schede madri Workfront

Le nuove funzioni di pianificazione Scrum nelle schede madri Adobe Workfront offrono opzioni flessibili per gestire i processi agili. Utilizzando questi strumenti, è possibile:

* Tracciare il lavoro in iterazioni o sprint
* Utilizzare Velocity per gestire gli impegni del team
* Tracciamento burndown e velocità di completamento

Le funzioni di pianificazione di Scrum saranno una &quot;procedura rapida&quot; dopo il rilascio della versione 23.1.

## Le date di scadenza sulle schede sono associate alla data di completamento pianificata sull’oggetto Workfront

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in anticipato per le schede madri Workfront.

Le date di scadenza sulle schede collegate nelle Schede Workfront ora vengono mappate alla data di completamento pianificata sull’oggetto Workfront associato. Se aggiorni la data di scadenza su una scheda, la data di completamento pianificata viene aggiornata sull’attività o sul problema. La modifica della data di completamento pianificata cambia anche la data di scadenza sulla scheda. In precedenza, la data di scadenza della scheda era un inserimento manuale e non veniva mappata ad alcuna data su un’attività o un problema.

La mappatura della data si applica anche agli elementi dell’elenco di controllo connessi che sono sincronizzati con le sottoattività.

La data di scadenza sia sulle schede collegate che su quelle ad hoc ora include anche un campo ora.

Per ulteriori informazioni, consulta [Utilizzare le schede collegate sulle bacheche](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3411952/){target=_blank}

## Le voci dell’elenco di controllo della bacheca e le sottoattività di Workfront sono ora collegate

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in anticipato per le schede madri Workfront.

Quando aggiungi una scheda collegata a una bacheca per un’attività di Workfront, tutte le sottoattività vengono importate come voci dell’elenco di controllo sulla scheda. Inoltre, quando si crea una voce dell&#39;elenco di controllo su una scheda connessa, all&#39;attività Workfront viene aggiunta un&#39;attività secondaria. Gli elementi dell’elenco di controllo sui problemi non sono collegati ad alcun oggetto Workfront.

In precedenza, le voci degli elenchi di controllo e le sottoattività non erano collegate. Se desideri includere una sottoattività nella bacheca, puoi importarla come una scheda collegata separata o aggiungere manualmente una voce dell’elenco di controllo a una scheda.

Per ulteriori informazioni, consulta [Utilizzare le schede collegate sulle bacheche](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) e [Gestire le voci dell’elenco di controllo sulle schede](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3411951/){target=_blank}

## Colonne del contatore della carta sulla bacheca

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in anticipato per le schede madri Workfront.

È disponibile una nuova impostazione di configurazione per attivare un contatore di schede per tutte le colonne di una scheda. Se si utilizza il limite WIP in una colonna, non viene aggiunto un contatore di schede separato.

Per ulteriori informazioni, consulta [Gestisci colonne bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

## Cerca e ordina nel dashboard delle bacheche

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in anticipato per le schede madri Workfront.

Ora puoi ordinare la dashboard delle bacheche per nome o data e cercare una bacheca specifica nell’elenco.

Per ulteriori informazioni, consulta [Utilizzare il dashboard delle bacheche](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md).

## Lo stato viene visualizzato sulla scheda

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in anticipato per le schede madri Workfront.

Se a una scheda di una bacheca è assegnato uno stato, questo viene ora visualizzato sulla scheda in modo da non dover aprire la scheda per visualizzarne lo stato. Questo miglioramento si applica sia alle schede ad hoc che a quelle connesse.

Per ulteriori informazioni, consulta [Utilizzare le schede collegate sulle bacheche](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) e [Aggiungere una scheda ad hoc a una bacheca](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

![stato sulla scheda](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## Le schede collegabili sono ora disponibili sulle bacheche

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in anticipato per le schede madri Workfront.

Ora puoi inviare un collegamento a una scheda specifica a un altro utente delle bacheche. La persona deve avere accesso alla visualizzazione della bacheca prima di poter aprire il collegamento.

Quando apri una scheda su una bacheca, l’URL del browser si presenta così:

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

Puoi copiare l’URL completo e inviarlo a un altro utente. Passeranno direttamente alla scheda aperta quando accederanno al collegamento.

In precedenza, i collegamenti erano disponibili per le bacheche, ma non per schede specifiche.

Per informazioni sulle schede, consulta [Aggiungere una scheda ad hoc a una bacheca](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) e [Utilizzare le schede collegate sulle bacheche](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Filtra per connessione su bacheche

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in anticipato per le schede madri Workfront.

L’elenco dei filtri su una bacheca ora include l’opzione per filtrare in base alla connessione, che mostra tutte le schede collegate per un progetto specifico. È inoltre possibile filtrare in base a schede non connesse.

Per ulteriori informazioni, consulta [Filtrare ed eseguire ricerche in una bacheca](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3412381/){target=_blank}

## Archiviare le schede da una bacheca in base a una pianificazione

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in anticipato per le schede madri Workfront.

È possibile configurare una bacheca in modo che le schede vengano archiviate, o che &quot;cadano&quot; dalla bacheca, in base a una pianificazione. Sono disponibili opzioni per impostare le schede in una particolare colonna da archiviare in un certo numero di giorni o settimane. Ad esempio, puoi definire la diminuzione in modo che le schede in una colonna Complete vengano archiviate dopo che sono state nella colonna per due settimane.

Se si desidera visualizzare di nuovo le schede dopo che cadono dalla bacheca, è possibile impostare il filtro della bacheca per visualizzare le schede archiviate.

Per ulteriori informazioni, consulta [Configurare la perdita di dati della scheda](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3412323/){target=_blank}
