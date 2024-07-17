---
product-area: reporting
navigation-topic: reporting-elements
title: Rimuovere filtri, visualizzazioni e raggruppamenti
description: È possibile rimuovere un filtro, una visualizzazione o un raggruppamento da elenchi e report se sono stati creati o condivisi con l'utente. Non è possibile rimuovere filtri, viste o raggruppamenti predefiniti.
author: Nolan
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 1%

---

# Rimuovere filtri, visualizzazioni e raggruppamenti

È possibile rimuovere un filtro, una visualizzazione o un raggruppamento da elenchi e report se sono stati creati o condivisi con l&#39;utente. Non è possibile rimuovere filtri, viste o raggruppamenti predefiniti.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>Accesso di visualizzazione o superiore a filtri, visualizzazioni, raggruppamenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Visualizzare le autorizzazioni con accesso per condividere il filtro, la visualizzazione o il raggruppamento che si desidera rimuovere</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Rimuovere o eliminare un filtro mediante il generatore standard

Puoi rimuovere un filtro condiviso con te dagli elenchi di progetti, attività o problemi utilizzando l’interfaccia standard di generazione. L&#39;interfaccia standard del generatore non è disponibile per altri oggetti o per viste o raggruppamenti.

Utilizzando l’interfaccia standard di generazione, puoi anche eliminare i filtri di tua proprietà da elenchi di progetti, attività o problemi.

Impossibile rimuovere o eliminare i filtri predefiniti di sistema.

### Considerazioni sulla rimozione o eliminazione di filtri tramite il generatore standard

Quando rimuovi o elimini un filtro con il generatore standard esistono gli scenari seguenti:

* Se il filtro è stato condiviso con te e lo rimuovi, viene rimosso solo per te. L’utente che l’ha creato originariamente e tutti gli altri utenti con cui è stato condiviso hanno ancora accesso al filtro.
* Se il filtro è di tua proprietà e lo elimini, viene rimosso dal sistema di Workfront. Il filtro non è più disponibile per gli utenti con cui l’hai condiviso in precedenza.
* Se sei un amministratore di Workfront, puoi eliminare il filtro che viene eliminato definitivamente per tutti gli utenti, incluso il proprietario.

### Rimuovere un filtro tramite il generatore standard

1. Consente di accedere a un elenco di progetti, attività, problemi, portafogli, programmi, utenti, modelli o gruppi.
1. Fai clic sull&#39;icona **Filtro** ![Icona Filtro](assets/filter-nwepng.png).
1. Passa il puntatore del mouse su un filtro in **Condiviso con me**, fai clic sul menu **Altro** ![Altro](assets/more-icon-spectrum.png), quindi fai clic su **Rimuovi**.

   ![Rimuovi filtro](assets/new-filters-more-menu-remove-filter.png)

1. Selezionare **Rimuovi** nel messaggio di conferma per rimuovere definitivamente il filtro.

### Eliminare un filtro con il generatore standard

1. Consente di accedere a un elenco di progetti, attività, problemi, portafogli, programmi, utenti, modelli o gruppi.
1. Fai clic sull&#39;icona **Filtro** ![Icona Filtro](assets/filter-nwepng.png).
1. Passa il puntatore del mouse su un filtro per cui disponi delle autorizzazioni di eliminazione, fai clic sul menu **Altro** ![Altro](assets/more-icon-spectrum.png), quindi fai clic su **Elimina**.

   ![Elimina filtro](assets/new-filters-more-menu-options-with-delete.png)

1. (Facoltativo) Fai clic su **Annulla** nel messaggio di conferma per evitare l&#39;eliminazione e tornare all&#39;elenco dei filtri.
1. Fai clic su **Elimina** nel messaggio di conferma per confermare l&#39;eliminazione.

   Il filtro viene eliminato per te e per tutti gli utenti che disponevano delle autorizzazioni necessarie.

## Rimuovere un filtro, una visualizzazione o un raggruppamento mediante il generatore di versioni precedenti

È possibile rimuovere un filtro, una vista o un raggruppamento per tutti gli elenchi di oggetti utilizzando l’interfaccia del generatore di versioni precedenti.

### Considerazioni sulla rimozione di filtri, viste e raggruppamenti tramite il generatore legacy

La modalità di rimozione di un elemento di reporting dipende dal fatto che sia stato creato inizialmente o che sia stato condiviso con te.

Quando si rimuove un filtro, una visualizzazione o un raggruppamento, si verificano gli scenari seguenti:

* **Se l&#39;elemento è stato creato e rimosso**, l&#39;elemento verrà rimosso dal sistema Workfront. Non è più disponibile per gli utenti con cui l’hai condiviso in precedenza.
* **Se l&#39;elemento è stato condiviso con te e lo rimuovi**, l&#39;elemento verrà rimosso solo per te. L’utente che l’ha creato originariamente e tutti gli altri utenti con cui è stato condiviso hanno ancora accesso a esso.

### Rimuovere un filtro, una visualizzazione o un raggruppamento mediante il generatore di versioni precedenti

1. Consente di passare a un elenco di oggetti o a un report.
1. (Condizionale) Da un elenco, fai clic sull&#39;icona **Filtro**, **Visualizzazione** o **Raggruppamento**, quindi passa il puntatore del mouse sul filtro, sulla visualizzazione o sul raggruppamento che desideri rimuovere, fai clic sull&#39;icona **Altro** ![](assets/more-icon.png), quindi su **Rimuovi**. Il filtro, la visualizzazione o il raggruppamento vengono rimossi.
1. (Condizionale) Da un report, fare clic sul menu a discesa **Raggruppamento**, **Filtro** o **Visualizza** e selezionare **Rimuovi raggruppamento**, **Rimuovi filtro** o **Rimuovi visualizzazione**.

   Viene visualizzata la finestra di dialogo **I miei raggruppamenti**, **I miei filtri,** o **Le mie visualizzazioni**.

   Tutti gli elementi di reporting per i quali disponi dei diritti di rimozione sono disponibili per la rimozione. Gli altri elementi di reporting vengono visualizzati in grigio.

1. Fai clic sull&#39;icona **x** accanto a qualsiasi elemento di reporting che desideri rimuovere.
1. (Condizionale) Fai clic su **Sì, eliminalo** se hai selezionato di eliminare un filtro, una visualizzazione o un raggruppamento che hai creato e successivamente condiviso con altri utenti. Il filtro, la visualizzazione o il raggruppamento verranno eliminati dal sistema Workfront.

   >[!TIP]
   >
   >Se si rimuove un filtro, una vista o un raggruppamento creato senza condividerlo con altri utenti, il filtro o la vista verrà rimosso dal sistema senza richiedere conferma.

1. Fai clic su **Fine**.

