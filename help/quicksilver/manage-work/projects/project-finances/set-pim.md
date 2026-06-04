---
product-area: projects
navigation-topic: financials
title: Impostare il Metodo indice prestazioni (PIM)
description: Il metodo PIM (Performance Index Method) per il progetto controlla il metodo utilizzato da Adobe Workfront per calcolare le metriche delle prestazioni del progetto, quali l'indice delle prestazioni dei costi (CPI, Cost Performance Index), l'indice delle prestazioni del programma (CSI, Cost Schedule Performance Index), l'indice delle prestazioni del programma (SPI, Schedule Performance Index) e la stima al completamento (EAC, Estimate At Completion).
author: Lisa
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
TQID: https://experienceleague.adobe.com/g4FYe8k1psS9xuL6Z40teAyJ-SV4UD6ThnWvnvl8au4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 418
ht-degree: 12%

---

# Impostare il Metodo indice prestazioni (PIM)

Il metodo PIM (Performance Index Method) per il progetto controlla il metodo utilizzato da Adobe Workfront per calcolare le metriche delle prestazioni del progetto, quali l&#39;indice delle prestazioni dei costi (CPI, Cost Performance Index), l&#39;indice delle prestazioni del programma (CSI, Cost Schedule Performance Index), l&#39;indice delle prestazioni del programma (SPI, Schedule Performance Index) e la stima al completamento (EAC, Estimate At Completion).

Workfront calcola questi valori utilizzando i seguenti elementi:

* Ore
* Costo

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi </td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Modifica accesso a progetti e dati finanziari</td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td>Gestisci le autorizzazioni per il progetto con le autorizzazioni per Modifica contabilità generale</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sulla gestione delle informazioni personali in Workfront

* L&#39;amministratore di Workfront o un amministratore di gruppo imposta l&#39;impostazione predefinita per determinare se il metodo di indicizzazione delle prestazioni (PIM, Performance Index Method) deve essere basato su ore o su costi. I calcoli per le metriche delle prestazioni variano a seconda di come viene impostato questo valore predefinito. Per ulteriori informazioni su come modificare l&#39;impostazione predefinita per il calcolo del PIM, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* I project manager possono inoltre modificare l&#39;impostazione per il PIM a livello di progetto per singoli progetti nella scheda secondaria Finanza del progetto. Per modificare la scheda secondaria Finanza del progetto, è necessario disporre delle autorizzazioni Gestione del progetto.

## Impostare il metodo PIM (Performance Index Method) per un progetto

1. Vai a un progetto di cui sei il proprietario.

   >[!IMPORTANT]
   >
   >Per eseguire i passaggi seguenti, è necessario disporre delle autorizzazioni di gestione per il progetto. È inoltre consigliabile che solo il proprietario del progetto apporti modifiche all&#39;area Finanza del progetto.

1. Fai clic su **Dettagli progetto** nel pannello a sinistra, quindi vai all&#39;area **Finanza**.
1. Fare doppio clic sul valore nel campo **Metodo indice prestazioni** per modificarlo.
1. Selezionare una delle opzioni seguenti nel campo **Metodo indice prestazioni**:

   | Basato su Ore | Workfront utilizza le ore pianificate per calcolare l’IPC e l’CES del progetto, e l’CES del progetto viene visualizzato come un numero, in ore. |
   |---|---|
   | Basato su Costo | Workfront utilizza il Costo manodopera pianificata per calcolare l&#39;IPC e l&#39;CES del progetto e l&#39;CES viene visualizzato come valore di valuta. Quando si seleziona questa opzione, verificare che gli assegnatari delle attività (mansioni o utenti) siano associati a tassi di costo. |

   {style="table-layout:auto"}

1. Fai clic su **Salva** **Modifiche**.
