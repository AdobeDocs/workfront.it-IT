---
title: Abilitare o disabilitare l’Assistente IA
content-type: reference
description: Puoi controllare quali livelli di accesso nell’organizzazione hanno accesso all’Assistente AI.
author: Becky
feature: Get Started with Workfront
exl-id: eec9f484-e29b-4256-b9ef-b45eb2e78eac
source-git-commit: e8e10f02f77f6c1df9f0af380eb16cc6bbc3b5d1
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 14%

---

# Abilitare o disabilitare l’Assistente IA

In qualità di amministratore di Workfront, puoi controllare quali utenti dell’organizzazione dispongono di Assistente AI abilitato. Questo viene gestito tramite i livelli di accesso.

Prima di poter abilitare l’Assistente AI per un livello di accesso, devi abilitarlo per la tua organizzazione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td><p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Attivare o disattivare l&#39;Assistente AI per l&#39;organizzazione

Per abilitare l&#39;Assistente IA per la tua organizzazione:

{{step-1-to-setup}}

1. Seleziona **Sistema** nel menu di navigazione a sinistra, quindi seleziona **Preferenze**.
1. Scorri verso il basso fino alla sezione **Preferenze IA**.
1. Attiva/disattiva **Attiva IA**.

>[!IMPORTANT]
>
>Prima di poter utilizzare l’Assistente AI, devi disporre di un accordo Gen AI firmato su file con Adobe.
>Per ulteriori informazioni sul Contratto di intelligenza artificiale di generazione, consulta [Firmare il Contratto di intelligenza artificiale di Adobe di generazione](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) nell&#39;articolo Assistente di intelligenza artificiale di Workfront.

## Attivare o disattivare l&#39;Assistente AI per un livello di accesso

Per abilitare l&#39;Assistente AI per un determinato livello di accesso:

{{step-1-to-setup}}

1. Seleziona **Livelli di accesso** nel menu di navigazione a sinistra.
1. Seleziona il livello di accesso desiderato, quindi fai clic sull&#39;icona **Modifica** ![Modifica](assets/edit-icon.png) sopra l&#39;elenco.
1. Nell&#39;area **Imposta restrizioni aggiuntive...** della casella **Modifica livello di accesso**, deselezionare la casella di controllo **Disattiva l&#39;Assistente di Workfront AI**.
1. Fai clic su **Salva**.
1. Ripeti i passaggi 3-5 per ogni livello di accesso per il quale desideri abilitare l’Assistente AI.



>[!NOTE]
>
>* L’Assistente IA è disabilitato per impostazione predefinita per i non amministratori.
>* Se un non amministratore interagisce con l’icona Assistente IA in Workfront, viene visualizzato il contratto per l’Assistente IA in cui si richiede al non amministratore di accettare i termini e le condizioni. Se accetta l’accordo, può utilizzare l’Assistente IA anche se è disabilitato nel modello di layout.

