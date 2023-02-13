---
product-area: reporting
navigation-topic: reporting-elements
title: Rimuovere filtri, visualizzazioni e raggruppamenti
description: Puoi rimuovere un filtro, una visualizzazione o un raggruppamento da elenchi e rapporti se li hai creati o sono stati condivisi con te. Non è possibile rimuovere filtri, viste o raggruppamenti predefiniti.
author: Lisa
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: a3e4eb500570f86c689ef3bef654d659b9c465a2
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# Rimuovere filtri, visualizzazioni e raggruppamenti

Puoi rimuovere un filtro, una visualizzazione o un raggruppamento da elenchi e rapporti se li hai creati o sono stati condivisi con te. Non è possibile rimuovere filtri, viste o raggruppamenti predefiniti.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Richiesta o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Visualizza o un accesso superiore a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Visualizza le autorizzazioni con accesso per condividere con il filtro, la visualizzazione o il raggruppamento che si desidera rimuovere</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Rimuovere un filtro, una visualizzazione o un raggruppamento utilizzando il generatore standard

È possibile rimuovere un filtro, una vista o un raggruppamento per tutti gli elenchi di oggetti utilizzando l’interfaccia standard di generazione.

### Considerazioni sulla rimozione di filtri, visualizzazioni e raggruppamenti

La modalità di rimozione di un elemento di reporting dipende dal fatto che sia stato creato inizialmente o che sia stato condiviso con te.

Quando rimuovi un raggruppamento esistono i seguenti scenari:

* **Se hai creato il raggruppamento e lo rimuovi**, il raggruppamento viene rimosso dal sistema Workfront. Il raggruppamento non è più disponibile per gli utenti con cui lo hai condiviso in precedenza.
* **Se il raggruppamento è stato condiviso con te e lo rimuovi**, il raggruppamento viene rimosso solo per voi. L’utente che lo ha creato originariamente e tutti gli altri utenti con cui è stato condiviso hanno ancora accesso al raggruppamento.

### Rimuovere un filtro, una visualizzazione o un raggruppamento utilizzando il generatore standard

1. Passare a un elenco di oggetti o a un report.
1. (Condizionale) Da un elenco, fai clic sul pulsante **Filtro**, **Visualizza** oppure **Raggruppamento** quindi fai clic sul pulsante **Altro** icona ![](assets/more-icon.png), quindi **Rimuovi**. Il filtro, la visualizzazione o il raggruppamento vengono rimossi.
1. (Condizionale) Da un rapporto, fai clic sul pulsante **Raggruppamento**, **Filtro** oppure **Visualizza** menu a discesa e seleziona **Rimuovi raggruppamento**, **Rimuovi filtro** oppure **Rimuovi vista**.

   La **Gruppi personali**, **I miei filtri,** o **Visualizzazioni personali** viene visualizzata la finestra di dialogo.

   Sono disponibili per la rimozione tutti gli elementi di reporting per i quali si dispone dei diritti di rimozione. Gli altri elementi di reporting vengono visualizzati in grigio.

1. Fai clic sul pulsante **x** accanto a qualsiasi elemento di reporting che desideri rimuovere.
1. (Condizionale) Fai clic su **Sì, eliminalo** se hai selezionato di eliminare un filtro, una visualizzazione o un raggruppamento creato e successivamente condiviso con altri. Questo elimina il filtro, la visualizzazione o il raggruppamento dal sistema Workfront.

   >[!TIP]
   >
   >La rimozione di un filtro, una visualizzazione o un raggruppamento creato senza condividerlo con altri utenti lo rimuove dal sistema senza richiedere una conferma.

1. Fai clic su **Fine**.

## Rimuovere o eliminare un filtro utilizzando il generatore beta

Puoi rimuovere un filtro condiviso con te dagli elenchi di progetti, attività o problemi utilizzando l’interfaccia del generatore di versioni beta. L’interfaccia del generatore beta non è disponibile per altri oggetti o per viste o raggruppamenti.

È inoltre possibile eliminare i filtri di proprietà da elenchi di progetti, attività o problemi utilizzando l’interfaccia del generatore di versioni beta.

I filtri predefiniti del sistema non possono essere rimossi o eliminati.

### Considerazioni sulla rimozione o l’eliminazione di filtri con il generatore di versioni beta

Quando rimuovi o elimini un filtro esistono i seguenti scenari:

* Se il filtro è stato condiviso con te e lo rimuovi, il filtro viene rimosso solo per te. L’utente che l’ha creato originariamente e tutti gli altri utenti con cui è stato condiviso hanno ancora accesso al filtro.
* Se possiedi il filtro e lo elimini, il filtro viene rimosso dal sistema Workfront. Il filtro non è più disponibile per gli utenti con cui lo hai condiviso in precedenza.
* Se sei un amministratore di Workfront, puoi eliminare il filtro e questo viene eliminato definitivamente per tutti gli utenti, incluso il proprietario.

### Rimuovere un filtro utilizzando il generatore beta

1. Passare a un elenco di progetti, attività o problemi.
1. Fai clic sul pulsante **Filtro** icona ![Icona Filtro](assets/filter-nwepng.png) e, se necessario, abilita il generatore beta.
1. Passa il puntatore del mouse su un filtro in **Condiviso con me**, fai clic su **Altro** menu ![Icona Altro](assets/more-icon-spectrum.png), quindi fai clic su **Rimuovi**.

   ![Rimuovi filtro](assets/new-filters-more-menu-remove-filter.png)

1. Seleziona **Rimuovi** nel messaggio di conferma per rimuovere definitivamente il filtro.

### Eliminare un filtro utilizzando il generatore di versioni beta

1. Passare a un elenco di progetti, attività o problemi.
1. Fai clic sul pulsante **Filtro** icona ![Icona Filtro](assets/filter-nwepng.png) e, se necessario, abilita il generatore beta.
1. Passa il puntatore del mouse su un filtro che si dispone delle autorizzazioni necessarie per eliminare, fai clic sul pulsante **Altro** menu ![Icona Altro](assets/more-icon-spectrum.png), quindi fai clic su **Elimina**.

   ![Elimina filtro](assets/new-filters-more-menu-options-with-delete.png)

1. (Facoltativo) Fai clic su **Annulla** nel messaggio di conferma per evitare l’eliminazione e tornare all’elenco dei filtri.
1. Fai clic su **Elimina** nel messaggio di conferma per confermare l’eliminazione.

   Il filtro viene eliminato per te e per tutti gli utenti che disponevano delle autorizzazioni necessarie.

