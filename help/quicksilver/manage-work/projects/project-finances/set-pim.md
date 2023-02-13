---
product-area: projects
navigation-topic: financials
title: Impostare il metodo Performance Index (PIM)
description: Il metodo PIM (Performance Index Method) per il progetto controlla il metodo utilizzato da Adobe Workfront per calcolare le metriche delle prestazioni del progetto, ad esempio l’indice delle prestazioni dei costi (CPI), l’indice delle prestazioni della pianificazione dei costi (CSI), l’indice delle prestazioni della pianificazione (SPI) e la stima al completamento (EAC).
author: Alina
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 1%

---

# Impostare il metodo Performance Index (PIM)

Il metodo PIM (Performance Index Method) per il progetto controlla il metodo utilizzato da Adobe Workfront per calcolare le metriche delle prestazioni del progetto, ad esempio l’indice delle prestazioni dei costi (CPI), l’indice delle prestazioni della pianificazione dei costi (CSI), l’indice delle prestazioni della pianificazione (SPI) e la stima al completamento (EAC).

Workfront calcola questi valori utilizzando quanto segue:

* Ore
* Costo

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
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l’accesso a progetti e dati finanziari</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il progetto con autorizzazioni per Manage Finance</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Considerazioni su PIM in Workfront

* L’amministratore di Workfront o un amministratore di gruppo imposta l’impostazione predefinita per specificare se il metodo di indice delle prestazioni (PIM) deve essere basato su ore o su costi. I calcoli per le metriche delle prestazioni cambiano in base a come viene impostata questa impostazione predefinita. Per ulteriori informazioni su come modificare il valore predefinito per il calcolo del PIM, vedere [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* I project manager possono inoltre modificare l&#39;impostazione per il PIM, a livello di progetto, per i singoli progetti nella sottoscheda Finanza del progetto. Per modificare la sottoscheda Finanza del progetto, è necessario disporre delle autorizzazioni Gestisci per il progetto.

## Impostare il metodo di indice delle prestazioni (PIM) per un progetto

1. Passa a un progetto di cui sei il proprietario.

   >[!IMPORTANT]
   >
   >Per eseguire i passaggi seguenti, è necessario disporre delle autorizzazioni di gestione per il progetto. È inoltre consigliabile che solo il proprietario del progetto apporti modifiche all&#39;area Finanza del progetto.

1. Fai clic su **Dettagli progetto** nel pannello a sinistra, quindi vai alla **Finanza** area.
1. Fai doppio clic sul valore nel **Metodo indice prestazioni** per modificarlo.
1. Seleziona tra le seguenti opzioni nel **Metodo indice prestazioni** campo:

   | Basato su Ore | Workfront utilizza le ore pianificate per calcolare l’IPC e l’EAC del progetto e l’EAC del progetto viene visualizzato come numero, in ore. |
   |---|---|
   | Basato su Costo | Workfront utilizza il costo del lavoro pianificato per calcolare l’IPC e l’EAC del progetto, e l’EAC viene visualizzato come valore di valuta. Quando si seleziona questa opzione, assicurarsi che le assegnatarie dell&#39;attività (ruoli o utenti) siano associate alle tariffe di costo. |

   {style=&quot;table-layout:auto&quot;}

1. Fai clic su **Salva** **Modifiche**.
