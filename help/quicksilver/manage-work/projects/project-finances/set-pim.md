---
product-area: projects
navigation-topic: financials
title: Impostare il metodo PIM (Performance Index Method)
description: Il metodo PIM (Performance Index Method) per il progetto controlla il metodo utilizzato da Adobe Workfront per calcolare le metriche delle prestazioni del progetto, quali l'indice delle prestazioni dei costi (CPI, Cost Performance Index), l'indice delle prestazioni del programma (CSI, Cost Schedule Performance Index), l'indice delle prestazioni del programma (SPI, Schedule Performance Index) e la stima al completamento (EAC, Estimate At Completion).
author: Alina
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 1%

---

# Impostare il metodo PIM (Performance Index Method)

Il metodo PIM (Performance Index Method) per il progetto controlla il metodo utilizzato da Adobe Workfront per calcolare le metriche delle prestazioni del progetto, quali l&#39;indice delle prestazioni dei costi (CPI, Cost Performance Index), l&#39;indice delle prestazioni del programma (CSI, Cost Schedule Performance Index), l&#39;indice delle prestazioni del programma (SPI, Schedule Performance Index) e la stima al completamento (EAC, Estimate At Completion).

Workfront calcola questi valori utilizzando i seguenti elementi:

* Ore
* Costo

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti e dati finanziari</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il progetto con le autorizzazioni per Gestire le finanze</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

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
