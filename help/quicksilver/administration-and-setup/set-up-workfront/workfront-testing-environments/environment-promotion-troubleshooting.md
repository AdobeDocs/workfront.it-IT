---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Risoluzione dei problemi di promozione dell’ambiente
description: Risolvere i problemi comuni relativi alla promozione dell’ambiente.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 830dd573-d954-4ba2-a1d3-d1645b3fbac8
TQID: https://experienceleague.adobe.com/N6spdHNxoRMwUjQY6HrHPm11d7kZaYHMbDGAkeqbyvY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 330
ht-degree: 1%

---

# Risoluzione dei problemi di promozione dell’ambiente

Questo articolo descrive come risolvere i problemi relativi alla promozione dell’ambiente.

## Problema: il pacchetto di promozione dell’ambiente è in fase di stallo o non riesce

Se il pacchetto di promozione dell’ambiente è in fase di stallo o non riesce, prova quanto segue:

* Se l&#39;installazione di un pacchetto si interrompe dopo 10-15 minuti o se si verifica un errore, riassemblare il pacchetto esistente o crearne uno nuovo.

* Se l&#39;installazione di un pacchetto non riesce, è possibile che si sia verificato un problema con uno o più oggetti. Controlla i messaggi di errore, che identificano l’oggetto e possono aiutare a identificare il problema. Dopo aver risolto il problema con l&#39;oggetto, riassemblare il pacchetto e ritentare l&#39;installazione.

* Se si verificano ancora problemi con un&#39;installazione, provare a replicarla in un ambiente di destinazione diverso. Mantenere il più vicino possibile all&#39;installazione originale, inclusi gli oggetti e le azioni di installazione selezionati.

* È consigliabile controllare sempre il contenuto del pacchetto dopo che è stato assemblato per verificare che contenga gli oggetti previsti.


## Problema: impossibile promuovere il modulo personalizzato

Ciò può verificarsi perché il modulo personalizzato include un campo calcolato. Se un campo calcolato fa riferimento a un campo a cui non si fa riferimento in un modulo personalizzato, un pacchetto che include questo modulo non viene promosso e l’utente potrebbe visualizzare il seguente messaggio:

&quot;I campi seguenti non sono validi: Espressione personalizzata non valida Espressione non valida: Espressione personalizzata non valida.&quot;

Questo problema può verificarsi quando si fa riferimento a un campo esistente non associato ad alcun modulo personalizzato nell’ambiente di destinazione o con un campo appena creato.

Per risolvere il problema, eseguire una delle operazioni seguenti:

* Crea un pacchetto con un modulo personalizzato di tipo progetto che include il campo di riferimento. Dopo aver promosso il pacchetto nell’ambiente di destinazione, promuovi il pacchetto originariamente previsto contenente il campo calcolato.
* Crea manualmente il campo a cui si fa riferimento nell’ambiente di destinazione e associalo a un modulo personalizzato di tipo progetto. Al termine dell’operazione, il campo verrà riconosciuto e potrai promuovere il pacchetto senza riscontrare l’errore.
