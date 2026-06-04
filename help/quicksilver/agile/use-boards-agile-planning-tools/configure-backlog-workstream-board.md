---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Configurare il backlog in una bacheca Workstream
description: Puoi scegliere di visualizzare una colonna di backlog su una bacheca in un flusso di lavoro e definire una query per le schede inserite nel backlog della bacheca dall’elenco delle schede del flusso di lavoro.
author: Courtney
feature: Agile
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/ECCX25ZQGtYXBdo8Xkds3OjtFUjoWGXIr9lOOiwwCe8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 480
ht-degree: 10%

---

# Configurare il backlog in una bacheca del flusso di lavoro

>[!IMPORTANT]
>
>I flussi di lavoro sono disponibili solo per un gruppo specifico di clienti.

Puoi scegliere di visualizzare una colonna di backlog su una bacheca in un flusso di lavoro e definire una query per le schede inserite nel backlog della bacheca dall’elenco delle schede del flusso di lavoro.

>[!NOTE]
>
>Se aggiungi una nuova scheda nella colonna del backlog che non corrisponde ai criteri di query, la scheda scompare dal backlog quando viene aggiornata e sarà disponibile solo nell’elenco delle schede. È possibile modificare la query in qualsiasi momento per modificare le schede visualizzate nella colonna del backlog.

La colonna backlog e la query non sono disponibili nelle bacheche autonome. Per informazioni sull&#39;aggiunta di una colonna di acquisizione a una bacheca autonoma, vedere [Aggiungere una colonna di acquisizione a una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o successiva</p> 
   <p>Richiedente o successiva</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurare il backlog in una bacheca del flusso di lavoro

{{step1-to-boards}}

1. Aprire il flusso di lavoro in cui si desidera lavorare. Per aprire un flusso di lavoro, fare clic su [!UICONTROL **Visualizza flusso di lavoro**].
1. Fare clic su una scheda del flusso di lavoro per aprirla.
1. Fai clic su [!UICONTROL **Configura**] a destra della bacheca per aprire il pannello Configura.
1. Attiva [!UICONTROL **Includi colonna backlog in questa bacheca**].

   La colonna backlog viene aggiunta a sinistra della bacheca. Rimane vuoto finché non viene applicata una query.

1. Espandere [!UICONTROL **Query backlog**].

   >[!NOTE]
   >
   >È possibile che al backlog sia già stata applicata una query predefinita che mostra tutti gli elementi di lavoro dell&#39;elenco delle schede con stato e stato non Completo.

1. Fai clic su [!UICONTROL **Aggiungi condizione**] e poi sul campo &quot;vuoto&quot;.
1. Seleziona il campo in base al quale eseguire la query.

   I campi tra cui è possibile scegliere sono quelli predefiniti di una scheda.

1. Seleziona il modificatore di query.

   Le opzioni del modificatore dipendono dai campi a cui possono essere applicate. Ad esempio, il campo &quot;name&quot; non contiene &quot;maggiore di&quot; o &quot;minore di&quot; come scelte di modificatore, in quanto tali modificatori si applicano solo ai numeri.

1. Seleziona il valore.

   Il valore non è disponibile quando si utilizza &quot;exists&quot; (esiste) o &quot;not exists&quot; (non esiste) come modificatore.

   Ad esempio, se scegli &quot;Scadenza&quot; ed &quot;esiste&quot;, nel backlog vengono visualizzate le schede con date di scadenza assegnate. Qualsiasi scheda senza una data di scadenza non verrà inserita nel backlog.

1. (Facoltativo) Fai clic su [!UICONTROL **Aggiungi condizione**] per aggiungere un&#39;altra condizione alla query.

   ![Query backlog](assets/backlog-query-wrkstrm-board.png)

1. (Facoltativo) Fai clic su [!UICONTROL **Crea gruppo**] per aggiungere un gruppo di condizioni connesse alla prima condizione con un operatore OR.
1. Fai clic su [!UICONTROL **Salva query**].

   La query viene applicata e le schede che soddisfano i criteri vengono visualizzate nella colonna backlog.
