---
product-area: reporting
navigation-topic: reporting-elements
title: Rimuovere filtri, visualizzazioni e raggruppamenti
description: È possibile rimuovere un filtro, una visualizzazione o un raggruppamento da elenchi e report se sono stati creati o condivisi con l'utente. Non è possibile rimuovere filtri, viste o raggruppamenti predefiniti.
author: Lisa
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: b56e6591c7da166bd1548420b562b838cc7fe0f2
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# Rimuovere filtri, visualizzazioni e raggruppamenti

<span class="preview">Nell’ambiente di anteprima, l’esperienza di filtro avanzata (precedentemente denominata &quot;beta&quot;) è ora l’impostazione predefinita. Questi filtri migliorati sono ora &quot;standard&quot; e l’esperienza del filtro precedente è &quot;legacy&quot;.</span>

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
   <td> <p>Visualizzare le autorizzazioni con accesso per condividere il filtro, la visualizzazione o il raggruppamento che si desidera rimuovere</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Rimuovere un filtro, una vista o un raggruppamento utilizzando il generatore standard

È possibile rimuovere un filtro, una vista o un raggruppamento per tutti gli elenchi di oggetti utilizzando l&#39;interfaccia standard del generatore.

### Considerazioni sulla rimozione di filtri, viste e raggruppamenti

La modalità di rimozione di un elemento di reporting dipende dal fatto che sia stato creato inizialmente o che sia stato condiviso con te.

Quando si rimuove un raggruppamento, si verificano gli scenari seguenti:

* **Se hai creato il raggruppamento e lo hai rimosso**, il raggruppamento viene rimosso dal sistema Workfront. Il raggruppamento non è più disponibile per gli utenti con cui l’hai condiviso in precedenza.
* **Se il raggruppamento è stato condiviso con te e lo rimuovi**, il raggruppamento viene rimosso solo per te. L’utente che l’ha creato originariamente e tutti gli altri utenti con cui è stato condiviso hanno ancora accesso al raggruppamento.

### Rimuovere un filtro, una vista o un raggruppamento utilizzando il generatore standard

1. Consente di passare a un elenco di oggetti o a un report.
1. (Condizionale) Da un elenco, fai clic su **Filtro**, **Visualizza**, o **Raggruppamento** , quindi posizionare il puntatore del mouse sul filtro, la visualizzazione o il raggruppamento che si desidera rimuovere, fare clic sul pulsante **Altro** icona ![](assets/more-icon.png), quindi **Rimuovi**. Il filtro, la visualizzazione o il raggruppamento vengono rimossi.
1. (Condizionale) Da un rapporto, fai clic su **Raggruppamento**, **Filtro**, o **Visualizza** menu a discesa e selezionare **Rimuovi raggruppamento**, **Rimuovi filtro**, o **Rimuovi visualizzazione**.

   Il **I Miei Raggruppamenti**, **I miei filtri,** o **Le Mie Viste** viene visualizzata.

   Tutti gli elementi di reporting per i quali disponi dei diritti di rimozione sono disponibili per la rimozione. Gli altri elementi di reporting vengono visualizzati in grigio.

1. Fai clic su **x** accanto a qualsiasi elemento di reporting che si desidera rimuovere.
1. (Condizionale) Fai clic su **Sì, elimina** se si è scelto di eliminare un filtro, una visualizzazione o un raggruppamento creato e successivamente condiviso con altri utenti. Il filtro, la visualizzazione o il raggruppamento verranno eliminati dal sistema Workfront.

   >[!TIP]
   >
   >Se si rimuove un filtro, una vista o un raggruppamento creato senza condividerlo con altri utenti, il filtro o la vista verrà rimosso dal sistema senza richiedere conferma.

1. Clic **Fine**.

## Rimuovere o eliminare un filtro tramite il generatore beta

Puoi rimuovere un filtro condiviso con te dagli elenchi di progetti, attività o problemi utilizzando l’interfaccia beta builder. L’interfaccia del generatore di versione beta non è disponibile per altri oggetti o per visualizzazioni o raggruppamenti.

Puoi anche eliminare i filtri di tua proprietà da elenchi di progetti, attività o problemi utilizzando l’interfaccia beta builder.

Impossibile rimuovere o eliminare i filtri predefiniti di sistema.

### Considerazioni sulla rimozione o eliminazione di filtri tramite il generatore beta

Quando si rimuove o si elimina un filtro, si verificano gli scenari seguenti:

* Se il filtro è stato condiviso con te e lo rimuovi, viene rimosso solo per te. L’utente che l’ha creato originariamente e tutti gli altri utenti con cui è stato condiviso hanno ancora accesso al filtro.
* Se il filtro è di tua proprietà e lo elimini, viene rimosso dal sistema di Workfront. Il filtro non è più disponibile per gli utenti con cui l’hai condiviso in precedenza.
* Se sei un amministratore di Workfront, puoi eliminare il filtro che viene eliminato definitivamente per tutti gli utenti, incluso il proprietario.

### Rimuovere un filtro con il generatore beta

1. Consente di passare a un elenco di progetti, attività o problemi.
1. Fai clic su **Filtro** icona ![Icona Filtro](assets/filter-nwepng.png) e, se necessario, abilita il generatore beta.
1. Passa il puntatore del mouse su un filtro in **Condiviso con me**, fare clic su **Altro** menu ![Icona Altro](assets/more-icon-spectrum.png), quindi fai clic su **Rimuovi**.

   ![Rimuovi filtro](assets/new-filters-more-menu-remove-filter.png)

1. Seleziona **Rimuovi** sul messaggio di conferma per rimuovere definitivamente il filtro.

### Eliminare un filtro con il generatore beta

1. Consente di passare a un elenco di progetti, attività o problemi.
1. Fai clic su **Filtro** icona ![Icona Filtro](assets/filter-nwepng.png) e, se necessario, abilita il generatore beta.
1. Passa il puntatore del mouse su un filtro per il quale disponi delle autorizzazioni di eliminazione, fai clic sul pulsante **Altro** menu ![Icona Altro](assets/more-icon-spectrum.png), quindi fai clic su **Elimina**.

   ![Elimina filtro](assets/new-filters-more-menu-options-with-delete.png)

1. (Facoltativo) Fai clic su **Annulla** nel messaggio di conferma per evitare l’eliminazione e tornare all’elenco dei filtri.
1. Clic **Elimina** sul messaggio di conferma per confermare l’eliminazione.

   Il filtro viene eliminato per te e per tutti gli utenti che disponevano delle autorizzazioni necessarie.

