---
navigation-topic: use-lists
title: Modificare la visualizzazione di un elenco
description: In [!DNL Adobe Workfront], è possibile personalizzare la visualizzazione di un elenco. Gli altri utenti che visualizzano l’elenco non visualizzano le modifiche apportate.
feature: Get Started with Workfront
author: Lisa
exl-id: 3ef7ff03-7293-4b56-9481-e89e1a47a904
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

# Modificare la visualizzazione di un elenco

In [!DNL Adobe Workfront], è possibile personalizzare la visualizzazione di un elenco. Gli altri utenti che visualizzano l’elenco non visualizzano le modifiche apportate.

Puoi effettuare le seguenti personalizzazioni:

* Numero di elementi visualizzati
* Larghezza o ordine della colonna
* Se i raggruppamenti vengono espansi o compressi

>[!NOTE]
>
>Le modifiche apportate alla visualizzazione di cui sopra vengono ripristinate quando si esce da [!DNL Workfront] o chiudi il browser. Queste modifiche potrebbero anche essere ripristinate dopo un periodo di 8 ore.

Oltre alle personalizzazioni temporanee di cui sopra, è anche possibile modificare le colonne ordinate dall’elenco in base alle quali, in base alle quali, [!DNL Workfront] conserva anche dopo la disconnessione o la chiusura del browser. Tuttavia, se qualcuno modifica le opzioni di ordinamento nella visualizzazione di un elenco, la selezione di ordinamento precedente non viene mantenuta.

Per informazioni sulla modifica delle informazioni visualizzate nell’elenco, consulta [Elementi di reporting: filtri, visualizzazioni e raggruppamenti](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Request] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Accesso all'area in cui si trova l'elenco</p> <p>Ad esempio, per modificare la visualizzazione di un progetto, è necessario disporre dell’accesso a Progetti.</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso.<br>Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Autorizzazioni [!UICONTROL View] o successive per la visualizzazione applicata all'elenco</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Modificare la visualizzazione di un elenco

1. Vai all’elenco in [!DNL Workfront] che si desidera modificare.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   By default, groupings are collapsed.
   </MadCap:conditionalText>
   <br> </p>
   -->

1. (Facoltativo e condizionale) Se i raggruppamenti nell’elenco sono compressi e desideri visualizzare ulteriori informazioni, fai clic sul raggruppamento desiderato per espandere l’elenco e visualizzare le informazioni in esso elencate.

   Oppure

   Per espandere tutti i raggruppamenti, fare clic sulla freccia a destra della casella di controllo nell&#39;intestazione della colonna.

   ![expand_groupings__1_.png](assets/expand-groupings--1--350x227.png)

1. (Facoltativo e condizionale) Per visualizzare un numero specifico di elementi sullo schermo, fai clic sul pulsante **[!UICONTROL Visualizzazione]** menu a discesa nell&#39;angolo inferiore destro dello schermo, quindi selezionare per visualizzare **100**, **250**, **500**, **[!UICONTROL Tutto]** oppure **2000** oggetti.

   ![](assets/list-number-page-350x119.png)

   >[!TIP]
   >
   >Per impostazione predefinita, vengono visualizzati 2.000 elementi per gli elenchi aggiornati e 100 per gli elenchi legacy. Se l’elenco contiene più di 2.000 elementi, non è possibile visualizzare tutti gli elementi su una pagina.
   >
   >
   >Per ottenere le migliori prestazioni negli elenchi di grandi dimensioni in cui gli oggetti contengono campi di testo formattati, si consiglia di limitare questo numero a 250.
   >
   >
   >Per ulteriori informazioni sui 2 tipi di elenco, consulta la sezione [Differenza tra gli elenchi aggiornati e quelli legacy](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) nell&#39;articolo [Guida introduttiva agli elenchi in [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   I risultati dell’elenco vengono impaginati in modo da visualizzare il numero selezionato di elementi per pagina. Per accedere ai risultati su altre pagine, fai clic sulle frecce indietro e avanti o seleziona una pagina specifica.

1. Per ridimensionare la larghezza di una colonna, posiziona il cursore del mouse sulla linea che separa 2 colonne, quindi fai clic su per trascinarla nella larghezza desiderata.

   La colonna viene ridimensionata finché non si cancella la cache sul browser o finché non si ridimensiona nuovamente manualmente.

1. Per riordinare le colonne di un elenco, passate il puntatore del mouse su un&#39;intestazione di colonna per visualizzare lo strumento mano, quindi fate clic per trascinare la colonna nel punto in cui desiderate visualizzarla.

   La posizione della colonna viene salvata fino all’aggiornamento della pagina.\
   Per ulteriori informazioni sulla personalizzazione della larghezza e dell’ordine delle colonne di un elenco, consulta l’articolo [Modificare la larghezza e l’ordine delle colonne](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

1. Per regolare l’ordinamento di un elenco, fare clic su un’intestazione di colonna per selezionarla, quindi tenere premuto il tasto CMD (su [!DNL Mac]) o CTRL (attivato) [!DNL Windows]) sulla tastiera e seleziona fino a 2 intestazioni di colonna aggiuntive per ordinarle.

   L’elenco viene ordinato in base a ciascuna colonna selezionata nell’ordine della selezione.

   Tutte le modifiche apportate all’elenco vengono salvate immediatamente.

   >[!NOTE]
   >
   >Se si ordinano i gruppi nel [!UICONTROL Gruppi] area [!UICONTROL Configurazione], la visualizzazione gerarchica dei gruppi e dei relativi sottogruppi non viene suddivisa quando si modifica l’ordine dell’elenco, in quanto i sottogruppi restano associati ai gruppi principali. L’elenco è ordinato prima per gruppi di primo livello. Quindi, sotto ogni gruppo padre, l&#39;elenco dei sottogruppi che si trovano sullo stesso livello viene ordinato insieme.
