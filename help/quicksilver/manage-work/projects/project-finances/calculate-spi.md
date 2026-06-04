---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcolare l’Indice prestazioni pianificazione (SPI)
description: L'indice delle prestazioni della pianificazione (SPI) descrive il rapporto tra la pianificazione pianificata e la pianificazione effettiva.
author: Lisa
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
TQID: https://experienceleague.adobe.com/WfZDTGfYIcngo8a3MQAh-Z7jnKm4nnBppV8hYSweygo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 398
ht-degree: 18%

---

# Calcolare l’Indice prestazioni pianificazione (SPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

L&#39;indice delle prestazioni della pianificazione (SPI) descrive il rapporto tra la pianificazione pianificata e la pianificazione effettiva. Adobe Workfront calcola l’indice SPI ai livelli di progetto e di attività. Questa metrica viene tracciata dai project manager e le attività o i progetti sono attualmente in anticipo o in ritardo rispetto alla pianificazione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td>
   <p>Chiaro o superiore</p>
   <p>Revisione o successiva</p></td>  
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Accesso ai progetti e ai dati finanziari</td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td>Visualizza o autorizzazioni superiori per il progetto con autorizzazioni per Visualizza contabilità generale</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Panoramica di Schedule Performance Index (SPI)

* [Descrizione del valore SPI](#what-the-spi-value-shows)
* [Calcolo SPI in Workfront](#how-workfront-calculates-spi)

### Cosa mostra il valore SPI {#what-the-spi-value-shows}

I project manager sono consapevoli del fatto che un valore SPI pari a 1 indica che il progetto è pianificato o pianificato.  I valori maggiori di 1 indicano che un progetto è in anticipo rispetto alla programmazione e i valori minori di 1 indicano che un progetto è in ritardo.  Più lontano da 1, maggiore è la deviazione dal piano.

| **Valore SPI** | **Indicazione di &quot;On Schedule&quot;** |
|---|---|
| 1 | Al piano o nei tempi previsti |
| > 1 (maggiore di 1) | In anticipo rispetto al programma |
| &lt; 1 (meno di 1) | In ritardo sulla pianificazione |

{style="table-layout:auto"}

### Calcolo SPI in Workfront  {#how-workfront-calculates-spi}

Workfront calcola SPI con la formula seguente:

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;Se le ore pianificate sono pianificate fino alla data = 0, SPI = 1*.

Le ore pianificate dalla pianificazione alla data vengono calcolate al minuto in cui vengono eseguiti i calcoli. Mostra il numero di ore pianificate fino alla data corrente. Può essere ricalcolato automaticamente quando si modificano i dati finanziari per garantire la precisione. Nessun campo in Workfront che indica questo valore.

Ad esempio, se si dispone di un progetto con 1 attività e l&#39;attività ha 10 ore pianificate e una Durata di 10 giorni, la Pianificazione ore pianificate fino alla data del 5° giorno sarà 5.

## Individuare SPI in un progetto o in un&#39;attività

1. Passare al progetto o all&#39;attività in cui si desidera visualizzare SPI.
1. A seconda che si desideri visualizzare SPI in un progetto o in un&#39;attività, effettuare una delle seguenti operazioni:

   1. Fai clic su **Dettagli progetto** nel pannello a sinistra, quindi visualizza l&#39;area **Finanza**.

   1. Fai clic su **Dettagli attività** nel pannello a sinistra, quindi visualizza l&#39;area **Finanza**.

      ![SPI nel progetto](assets/spi-on-project-nwe.png)

1. Trova il campo **CPI/ SPI/ CSI**.
