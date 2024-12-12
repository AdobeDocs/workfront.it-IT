---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcola indice prestazioni Schedule (SPI)
description: L'indice delle prestazioni della pianificazione (SPI) descrive il rapporto tra la pianificazione pianificata e la pianificazione effettiva.
author: Lisa
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Calcola indice prestazioni Schedule (SPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

L&#39;indice delle prestazioni della pianificazione (SPI) descrive il rapporto tra la pianificazione pianificata e la pianificazione effettiva. Adobe Workfront calcola l’SPI a livello di progetto e di attività. I project manager esaminano questa metrica per verificare se le attività o i progetti sono in fase di verifica in anticipo o in ritardo rispetto alla programmazione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Nuovo: Chiaro o superiore</p>
   <p>oppure</p>
   <p>Corrente: revisione o versione successiva</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Accesso ai progetti e ai dati finanziari</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Visualizza o autorizzazioni superiori per il progetto con autorizzazioni Visualizza contabilità</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Panoramica di Schedule Performance Index (SPI)

* [Descrizione del valore SPI](#what-the-spi-value-shows)
* [Calcolo SPI in Workfront](#how-workfront-calculates-spi)

### Cosa mostra il valore SPI {#what-the-spi-value-shows}

I project manager sono consapevoli del fatto che un valore SPI pari a 1 indica che il progetto è pianificato o pianificato.  I valori maggiori di 1 indicano che un progetto è in anticipo rispetto alla programmazione e i valori minori di 1 indicano che un progetto è in ritardo.  Più lontano da 1, maggiore è la deviazione dal piano.

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

Le ore pianificate dalla pianificazione alla data vengono calcolate al minuto in cui vengono eseguiti i calcoli. Mostra il numero di ore pianificate fino alla data corrente. Può essere ricalcolato automaticamente quando si modificano i dati finanziari per garantire la precisione. Nessun campo in Workfront che indica questo valore.

Ad esempio, se si dispone di un progetto con 1 attività e l&#39;attività ha 10 ore pianificate e una Durata di 10 giorni, la Pianificazione ore pianificate fino alla data del 5° giorno sarà 5. 

## Individuare SPI in un progetto o in un&#39;attività

1. Passare al progetto o all&#39;attività in cui si desidera visualizzare SPI.
1. A seconda che si desideri visualizzare SPI in un progetto o in un&#39;attività, effettuare una delle seguenti operazioni:

   1. Fai clic su **Dettagli progetto** nel pannello a sinistra, quindi visualizza l&#39;area **Finanza**.

   1. Fai clic su **Dettagli attività** nel pannello a sinistra, quindi visualizza l&#39;area **Finanza**.

      ![](assets/spi-on-project-nwe.png)

1. Trova il campo **CPI/ SPI/ CSI**.
