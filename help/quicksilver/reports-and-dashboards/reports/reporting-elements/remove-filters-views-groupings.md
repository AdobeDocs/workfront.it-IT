---
product-area: reporting
navigation-topic: reporting-elements
title: Rimuovere filtri, visualizzazioni e raggruppamenti
description: È possibile rimuovere un filtro, una visualizzazione o un raggruppamento da elenchi e report se sono stati creati o condivisi con l'utente. Non è possibile rimuovere filtri, viste o raggruppamenti predefiniti.
author: Nolan
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 1%

---

# Rimuovere filtri, visualizzazioni e raggruppamenti

<!-- Audited: 11/2024 -->

È possibile rimuovere un filtro, una visualizzazione o un raggruppamento da elenchi e report se sono stati creati o condivisi con l&#39;utente. Non è possibile rimuovere filtri, viste o raggruppamenti predefiniti.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</strong></td> 
   <td> 
    <p>Collaboratore o versione successiva</p>
    <p>Richiedi o superiore</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
    <td> <p>Visualizzare le autorizzazioni con accesso per condividere il filtro, la visualizzazione o il raggruppamento che si desidera rimuovere</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
1. (Condizionale) Da un elenco, fai clic sull&#39;icona **Filtro**, **Visualizzazione** o **Raggruppamento**, quindi passa il puntatore del mouse sul filtro, sulla visualizzazione o sul raggruppamento che desideri rimuovere, fai clic sull&#39;icona **Altro** ![Icona Altro](assets/more-icon.png), quindi **Rimuovi**. Il filtro, la visualizzazione o il raggruppamento vengono rimossi.
1. (Condizionale) Da un report, fare clic sul menu a discesa **Raggruppamento**, **Filtro** o **Visualizza** e selezionare **Rimuovi raggruppamento**, **Rimuovi filtro** o **Rimuovi visualizzazione**.

   Viene visualizzata la finestra di dialogo **I miei raggruppamenti**, **I miei filtri,** o **Le mie visualizzazioni**.

   Tutti gli elementi di reporting per i quali disponi dei diritti di rimozione sono disponibili per la rimozione. Gli altri elementi di reporting vengono visualizzati in grigio.

1. Fai clic sull&#39;icona **x** accanto a qualsiasi elemento di reporting che desideri rimuovere.
1. (Condizionale) Fai clic su **Sì, eliminalo** se hai selezionato di eliminare un filtro, una visualizzazione o un raggruppamento che hai creato e successivamente condiviso con altri utenti. Il filtro, la visualizzazione o il raggruppamento verranno eliminati dal sistema Workfront.

   >[!TIP]
   >
   >Se si rimuove un filtro, una vista o un raggruppamento creato senza condividerlo con altri utenti, il filtro o la vista verrà rimosso dal sistema senza richiedere conferma.

1. Fai clic su **Fine**.

