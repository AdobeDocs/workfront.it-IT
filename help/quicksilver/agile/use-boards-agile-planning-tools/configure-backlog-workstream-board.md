---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Configurare il backlog su una scheda del flusso di lavoro
description: Potete scegliere di visualizzare una colonna backlog su una bacheca in un flusso di lavoro e definire una query per le schede che vengono estratte nel backlog della bacheca dall'elenco delle schede del flusso di lavoro.
author: Lisa
source-git-commit: b58831d50c2be421c666515808091aa4863bb471
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Configurare il backlog su una scheda del flusso di lavoro

Potete scegliere di visualizzare una colonna backlog su una bacheca in un flusso di lavoro e definire una query per le schede che vengono estratte nel backlog della bacheca dall&#39;elenco delle schede del flusso di lavoro. Queste opzioni non sono disponibili su schede indipendenti. Per informazioni sull&#39;aggiunta di una colonna di aspirazione a una bacheca indipendente, consulta [Aggiungere una colonna di assunzione a una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Request] o superiore</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Configurare il backlog su una scheda del flusso di lavoro

{{step1-to-boards}}

1. Aprire il flusso di lavoro in cui si desidera lavorare. Per aprire un flusso di lavoro, fai clic su [!UICONTROL **Visualizza flusso di lavoro**].
1. Fate clic su una bacheca nel flusso di lavoro per aprirla.
1. Fai clic su [!UICONTROL **Configura**] sulla destra della bacheca per aprire il pannello Configura .
1. Attiva [!UICONTROL **Includi una colonna backlog in questa bacheca**].

   La colonna backlog viene aggiunta a sinistra della bacheca. Rimane vuoto finché non viene applicata una query.

1. Espandi [!UICONTROL **Query backlog**].
1. Fai clic su [!UICONTROL **Aggiungi condizione**] e fai clic nel campo &quot;vuoto&quot;.
1. Selezionare il campo per cui eseguire la query.

   I campi predefiniti disponibili in una scheda sono quelli predefiniti.

1. Selezionare il modificatore di query.

   Le opzioni sono: è uguale a, non è uguale a, esiste e non esiste.

   Esempio: Se scegli Data di scadenza ed esiste, il backlog visualizza le schede con le date di scadenza assegnate. Qualsiasi scheda senza una data di scadenza non verrà inserita nel backlog.

1. Seleziona il valore.

   Il valore è disponibile solo se è uguale o meno a come modificatore.

1. (Facoltativo) Fai clic su [!UICONTROL **Aggiungi condizione**] per aggiungere un’altra condizione alla query.

   ![Query arretrati](assets/backlog-query-wrkstrm-board.png)

1. (Facoltativo) Fai clic su [!UICONTROL **Crea gruppo**] aggiungere un gruppo di condizioni connesse alla prima condizione con un operatore OR.
1. Fai clic su [!UICONTROL **Salva query**].

   La query viene applicata e le schede che soddisfano i criteri vengono visualizzate nella colonna backlog.
