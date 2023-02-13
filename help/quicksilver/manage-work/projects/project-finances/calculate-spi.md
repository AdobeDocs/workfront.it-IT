---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcola indice delle prestazioni della pianificazione (SPI)
description: L'indice delle prestazioni della pianificazione (SPI) descrive il rapporto tra la pianificazione pianificata e la pianificazione effettiva.
author: Alina
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# Calcola indice delle prestazioni della pianificazione (SPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

L&#39;indice delle prestazioni della pianificazione (SPI) descrive il rapporto tra la pianificazione pianificata e la pianificazione effettiva. Adobe Workfront calcola SPI a livello di progetto e di attività. I project manager esaminano questa metrica per identificare se le attività o i progetti vengono attualmente monitorati in anticipo o in ritardo.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a progetti e dati finanziari</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per il progetto con autorizzazioni per visualizzare Finanza</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Panoramica di Schedule Performance Index (SPI)

* [Mostra il valore SPI](#what-the-spi-value-shows)
* [Come Workfront calcola SPI](#how-workfront-calculates-spi)

### Mostra il valore SPI {#what-the-spi-value-shows}

I responsabili del progetto comprendono che un valore SPI pari a 1 indica che il progetto è in programma o in programma.  Valori superiori a 1 indicano che un progetto è in anticipo rispetto alla pianificazione e valori inferiori a 1 indicano che un progetto è in ritardo.  Più lontano da 1, maggiore deviazione dal piano.

| **Valore SPI** | **Indicazione di &quot;On Schedule&quot;** |
|---|---|
| 1 | In programma o in programma |
| > 1 (maggiore di 1) | Prima del programma |
| &lt; 1 (inferiore a 1) | In ritardo |

{style=&quot;table-layout:auto&quot;}

### Come Workfront calcola SPI  {#how-workfront-calculates-spi}

Workfront calcola SPI con la seguente formula:

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;Se Orari pianificati pianificati = 0, SPI = 1*.

La pianificazione degli orari da programmare a data viene calcolata al minuto in cui si eseguono i calcoli. Mostra il numero di ore pianificate pianificate fino alla data corrente. Può essere ricalcolato automaticamente quando si modificano i dati finanziari in modo che siano accurati. Nessun campo in Workfront che indica questo valore.

Ad esempio, se si dispone di un progetto con 1 attività e l&#39;attività ha 10 ore pianificate e una durata di 10 giorni, l&#39;orario pianificato per la data del 5° giorno è 5. 

## Individuare SPI in un progetto o un&#39;attività

1. Passare al progetto o all&#39;attività in cui si desidera visualizzare SPI.
1. A seconda che si desideri visualizzare SPI su un progetto o un&#39;attività, effettuare una delle seguenti operazioni:

   1. Fai clic su **Dettagli progetto** nel pannello a sinistra, quindi visualizza la **Finanza** area.

   1. Fai clic su **Dettagli attività** nel pannello a sinistra, quindi visualizza la **Finanza** area.

      ![](assets/spi-on-project-nwe.png)

1. Trova il **CPI/ SPI/ CSI** campo .
