---
title: Rivedere le formule dei campi calcolati con l’Assistente IA
content-type: reference
description: È possibile utilizzare l’Assistente AI per risolvere gli errori nelle espressioni personalizzate non valide nei campi calcolati.
author: Becky
feature: Get Started with Workfront
exl-id: 5f144a6f-5c2a-42fc-a961-ab9066432d93
source-git-commit: bec1318d83938964697d76b83062ef11745802e3
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Generare o rivedere formule di campi calcolati con Assistente IA

È possibile utilizzare l’Assistente IA per generare formule in base a un prompt fornito. Puoi anche risolvere gli errori nelle espressioni personalizzate non valide nei campi calcolati.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td><p>Nuovo: Prime o Ultimate</p>
       <p>oppure</p>
       <p>Corrente: non disponibile</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>oppure</p>
       <p>Corrente: non disponibile</p></td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisiti

* L’amministratore di Workfront deve aver abilitato l’Assistente AI per la tua organizzazione.

  Per ulteriori informazioni, vedere [Prerequisiti per l&#39;Assistente IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant) nell&#39;articolo Panoramica dell&#39;Assistente IA.
* L&#39;amministratore di Workfront deve aver abilitato l&#39;Assistente AI per il proprio livello di accesso.

  Per ulteriori informazioni, vedere [Attivare o disattivare l&#39;Assistente AI](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

<!--## Generate a calculated field expression-->

## Modificare un&#39;espressione di campo calcolato

Quando crei il campo calcolato nel generatore di moduli personalizzati, viene visualizzato un messaggio di errore sotto il campo se la formula non è valida.

![Errore espressione non valida](assets/invalid-expression.png)

L’Assistente IA può aiutarti a rivedere la formula in un’espressione di campo calcolato valida.

Per modificare un&#39;espressione di campo calcolato non valida:

1. Fai clic sull&#39;icona **Assistente AI** ![Icona Assistente AI](assets/ai-assistant-icon.png) nell&#39;angolo superiore destro dello schermo.
1. nell’area del prompt, nella parte inferiore del pannello dell’Assistente AI, inserisci un prompt come:
   `Rewrite this formula to remove the invalid expression error`
1. Copia l’espressione non valida dal generatore di moduli personalizzati e incollala nell’area dei prompt.
1. Premere **Invio**.

   La generazione della formula rivista può richiedere alcuni minuti, a seconda delle dimensioni o della complessità della formula.
1. Visualizza la formula rivista nel pannello Assistente IA.
1. (Facoltativo) Copia la formula rivista dal pannello Assistente IA e incollala nel campo calcolato nel generatore di moduli personalizzati.

>[!NOTE]
>
>È consigliabile verificare che il campo calcolato recuperi il risultato previsto.

Per ulteriori informazioni sui campi calcolati in Workfront, vedere [Aggiungere campi calcolati a un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

