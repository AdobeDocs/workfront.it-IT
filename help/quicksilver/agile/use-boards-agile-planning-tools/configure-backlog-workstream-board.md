---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Configurare il backlog in una bacheca del flusso di lavoro
description: Puoi scegliere di visualizzare una colonna di backlog su una bacheca in un flusso di lavoro e definire una query per le schede inserite nel backlog della bacheca dall’elenco delle schede del flusso di lavoro.
author: Lisa
feature: Agile
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Configurare il backlog in una bacheca del flusso di lavoro

Puoi scegliere di visualizzare una colonna di backlog su una bacheca in un flusso di lavoro e definire una query per le schede inserite nel backlog della bacheca dall’elenco delle schede del flusso di lavoro.

>[!NOTE]
>
>Se aggiungi una nuova scheda nella colonna del backlog che non corrisponde ai criteri di query, la scheda scompare dal backlog quando viene aggiornata e sarà disponibile solo nell’elenco delle schede. È possibile modificare la query in qualsiasi momento per modificare le schede visualizzate nella colonna del backlog.

La colonna backlog e la query non sono disponibili nelle bacheche autonome. Per informazioni sull’aggiunta di una colonna di acquisizione a una bacheca autonoma, consulta [Aggiungere una colonna Acquisizione a una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

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
   <td> <p>[!UICONTROL Request] o versione successiva</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Configurare il backlog in una bacheca del flusso di lavoro

{{step1-to-boards}}

1. Aprire il flusso di lavoro in cui si desidera lavorare. Per aprire un flusso di lavoro, fare clic su [!UICONTROL **Visualizza flusso di lavoro**].
1. Fare clic su una scheda del flusso di lavoro per aprirla.
1. Clic [!UICONTROL **Configura**] sulla destra della bacheca per aprire il pannello Configura.
1. Attiva [!UICONTROL **Includi una colonna backlog in questa bacheca**].

   La colonna backlog viene aggiunta a sinistra della bacheca. Rimane vuoto finché non viene applicata una query.

1. Espandi [!UICONTROL **Query backlog**].

   >[!NOTE]
   >
   >È possibile che al backlog sia già stata applicata una query predefinita che mostra tutti gli elementi di lavoro dell&#39;elenco delle schede con stato e stato non Completo.

1. Clic [!UICONTROL **Aggiungi condizione**] e fai clic sul campo &quot;vuoto&quot;.
1. Seleziona il campo in base al quale eseguire la query.

   I campi tra cui è possibile scegliere sono quelli predefiniti di una scheda.

1. Seleziona il modificatore di query.

   Le opzioni del modificatore dipendono dai campi a cui possono essere applicate. Ad esempio, il campo &quot;name&quot; non contiene &quot;maggiore di&quot; o &quot;minore di&quot; come scelte di modificatore, in quanto tali modificatori si applicano solo ai numeri.

1. Seleziona il valore.

   Il valore non è disponibile quando si utilizza &quot;exists&quot; (esiste) o &quot;not exists&quot; (non esiste) come modificatore.

   Ad esempio, se scegli &quot;Scadenza&quot; ed &quot;esiste&quot;, nel backlog vengono visualizzate le schede con date di scadenza assegnate. Qualsiasi scheda senza una data di scadenza non verrà inserita nel backlog.

1. (Facoltativo) Fai clic su [!UICONTROL **Aggiungi condizione**] per aggiungere un&#39;altra condizione alla query.

   ![Query arretrati](assets/backlog-query-wrkstrm-board.png)

1. (Facoltativo) Fai clic su [!UICONTROL **Crea gruppo**] per aggiungere un gruppo di condizioni connesse alla prima condizione con un operatore OR.
1. Clic [!UICONTROL **Salva query**].

   La query viene applicata e le schede che soddisfano i criteri vengono visualizzate nella colonna backlog.
