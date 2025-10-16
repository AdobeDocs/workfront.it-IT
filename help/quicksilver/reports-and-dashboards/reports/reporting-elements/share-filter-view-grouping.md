---
product-area: reporting
navigation-topic: reporting-elements
title: Condividere un filtro, una visualizzazione o un raggruppamento
description: Puoi condividere filtri, viste e raggruppamenti a cui hai accesso per visualizzarli con altri utenti.
author: Nolan
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 2%

---

# Condividere un filtro, una visualizzazione o un raggruppamento

<!-- Audited: 11/2024 -->

<!--(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)
(NOTE: This is linked from the TOC article in WF Basics > permissions section)-->

L’amministratore di Adobe Workfront consente agli utenti di visualizzare o modificare gli oggetti quando assegnano i livelli di accesso. Per ulteriori informazioni sulla concessione dell&#39;accesso agli oggetti, vedere [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Oltre al livello di accesso concesso agli utenti, è possibile concedere loro anche le autorizzazioni per visualizzare o modificare oggetti specifici creati o di cui si dispone dell&#39;accesso alla condivisione. Per ulteriori informazioni sui livelli di accesso e sulle autorizzazioni, vedere [Funzionamento dei livelli di accesso e delle autorizzazioni](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Puoi condividere filtri, viste e raggruppamenti a cui hai accesso per visualizzarli con altri utenti.

Quando un filtro, una visualizzazione o un raggruppamento è condiviso con l&#39;utente, è possibile applicarlo agli elenchi. A seconda dell’accesso concesso all’utente, potrebbe essere possibile modificarlo e condividerlo con altri utenti.

Per informazioni su come creare un filtro, una visualizzazione o un raggruppamento, vedere gli articoli seguenti:

* [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

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
   <td> <p>Accesso di visualizzazione o superiore a filtri, visualizzazioni, raggruppamenti</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
    <td> <p>Autorizzazioni di visualizzazione o di livello superiore con accesso alla condivisione di una visualizzazione, un filtro o un raggruppamento</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Condividere un filtro, una visualizzazione o un raggruppamento

<!--(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)-->

La condivisione di filtri negli elenchi di selezione varia a seconda dell’interfaccia utilizzata per condividere il filtro da: standard o legacy. Per informazioni sui tipi di interfacce per la creazione di filtri, vedere [Creare o modificare filtri in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

Puoi condividere viste e raggruppamenti solo nell’interfaccia legacy.

### Condivisione di filtri tramite l’interfaccia standard di generazione

Nell’interfaccia standard puoi condividere un filtro da elenchi di progetti, attività, problemi, portfolio, programmi, utenti, modelli o gruppi. L’interfaccia standard del generatore di filtri non è disponibile per altri oggetti o per viste o raggruppamenti.

Condividi un filtro tramite l’interfaccia standard di generazione:

1. Consente di passare a un elenco di progetti, attività o problemi.
1. Fai clic sull&#39;icona **Filtro** ![Icona Filtro](assets/filter-nwepng.png).

   ![Generatore di filtri standard](assets/new-filters-all-filter-types.png)

1. Rivedi i seguenti elenchi di filtri:

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Preferiti</strong></td>
   <td>Filtri contrassegnati come preferiti. Quando si preferisce un filtro, la posizione originale viene visualizzata sotto il nome del filtro e viene nascosta dall'elenco originale a meno che non venga rimosso come preferito.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Salvato</strong></td>
   <td>Filtri creati e salvati personalmente. Per impostazione predefinita, in questo elenco vengono visualizzati i filtri salvati in ordine di quelli salvati più di recente, ma i nomi dei filtri possono essere trascinati per riordinare manualmente l’elenco.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Impostazioni predefinite di sistema</strong></td>
   <td>Filtri predefiniti di Workfront e filtri aggiunti dall’amministratore Workfront all’elenco dei filtri, a livello di sistema o nel modello di layout.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Condivisi con me</strong></td>
   <td>Filtri creati e condivisi da altri utenti con te o condivisi a livello di sistema.</td>
   </tr>
   </tbody>
   </table>

1. Passa il puntatore del mouse su un filtro a cui hai accesso per visualizzare e condividere almeno, quindi fai clic sul menu **Altro** ![Altro](assets/more-icon-spectrum.png), quindi fai clic su **Condividi**.

   ![Altre opzioni di menu](assets/new-filters-more-menu-options-with-delete.png)

   Viene visualizzata la casella Condivisione filtro.

1. Inizia a digitare i nomi di utenti, team, ruoli, gruppi o aziende con cui vuoi condividere nel campo **Concedi l&#39;accesso a**.

   ![Casella di condivisione filtro](assets/new-filters-share-filter.png)

1. (Facoltativo) Fai clic sulla freccia rivolta a destra accanto al nome di un&#39;entità per modificarne le autorizzazioni per il filtro, quindi abilita l&#39;opzione **Visualizza** o **Gestisci**. **Visualizza** è l&#39;impostazione predefinita.

   ![Autorizzazioni di condivisione](assets/new-filters-sharing-permissions.png)

1. (Facoltativo) Abilita o disabilita le autorizzazioni aggiuntive per un’entità effettuando una delle seguenti operazioni:

   1. Fai clic su **Visualizza** e disabilita l&#39;opzione **Condividi**. Questa opzione è abilitata per impostazione predefinita.
   1. Fai clic su **Gestisci** e disabilita l&#39;opzione **Condividi** o **Elimina**. Sono attivati per impostazione predefinita.

      >[!NOTE]
      >
      >Se abiliti l’accesso Gestisci con l’opzione Elimina, questi utenti potranno eliminare il filtro da tutti gli utenti, anche se non sono i proprietari del filtro.

   >[!TIP]
   >
   >Gli utenti non possono ricevere un’autorizzazione superiore al loro livello di accesso. Se non hanno accesso a Modifica filtri nel loro livello di accesso, non possono ricevere le autorizzazioni per gestire un filtro. Workfront disabilita l’opzione Gestisci per questi utenti e l’opzione è disabilitata.

1. Fai clic su **Condividi**. Il filtro viene condiviso con le entità specificate.

   >[!TIP]
   >
   >La condivisione con i gruppi consente di assegnare le autorizzazioni per il filtro ai membri del gruppo e di tutti i sottogruppi.

   I filtri condivisi vengono visualizzati nella sezione **Condivisi con me** del pannello dei filtri per tali entità.

   ![Filtri condivisi con me](assets/new-filters-shared-with-me.png)

### Condividere filtri, visualizzazioni e raggruppamenti utilizzando l’interfaccia legacy

La condivisione di filtri, viste e raggruppamenti nell’interfaccia legacy è identica.

1. Consente di passare a un elenco di oggetti o a un report.
1. (Condizionale) Da un elenco, fai clic sull&#39;icona **Filtro**, **Visualizzazione** o **Raggruppamento**, quindi passa il puntatore del mouse sul filtro, sulla visualizzazione o sul raggruppamento che desideri condividere e fai clic sull&#39;icona **Altro** ![Icona Altro](assets/more-icon.png), quindi **Condividi**.

   Da un report, fare clic sul menu a discesa **Filtro**, **Visualizza** o **Raggruppamento**, quindi selezionare il filtro, la visualizzazione o il raggruppamento che si desidera condividere.

1. (Condizionale) Se condividi da un report, fai clic nuovamente sul menu a discesa **Filtro**, **Visualizza** o **Raggruppamento**, quindi fai clic su **Condividi filtro**, **Condividi visualizzazione** o **Condividi raggruppamento**.\
   Viene visualizzata la finestra di dialogo **Accesso filtro**, **Accesso visualizzazione** o **Accesso raggruppamento**.

   ![Condividi filtro](assets/share-filter-people-box-nwe-350x458.png)

1. Completa una delle seguenti operazioni, a seconda di chi desideri condividere con:

   **Per condividere con singoli utenti, team, ruoli, gruppi o società:** Nel campo specificato iniziare a digitare il nome dell&#39;utente, del team, della mansione, del gruppo o della società con cui si desidera condividere il nome, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.\
   Ripeti questa procedura per condividere l’accesso con più utenti, team, ruoli, gruppi o aziende.

   >[!TIP]
   >
   >La condivisione con i gruppi consente di assegnare le autorizzazioni per il filtro, la visualizzazione o il raggruppamento ai membri del gruppo e di tutti i sottogruppi.

   **Per condividere con tutti gli utenti del sistema:** Fai clic sull&#39;icona **Impostazioni**, quindi fai clic su **Rendi visibile a livello di sistema**.\
   Per rendere disponibile questa opzione, l&#39;amministratore deve selezionare l&#39;opzione Condividi a livello di sistema. Per ulteriori informazioni, vedere gli articoli [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) e [Condividere report, dashboard e calendari](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Condizionale) Se condividi con singoli utenti, team, ruoli, gruppi o società, fai clic sul menu a discesa per definire il livello di accesso che desideri concedere.

   Puoi scegliere una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Visualizzare</strong></td> 
      <td> <p>Selezionare questa opzione per consentire ai destinatari della condivisione di utilizzare solo il filtro, la visualizzazione o il raggruppamento condivisi. Quando questa opzione è selezionata, i destinatari non possono apportare modifiche all’elemento condiviso.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gestire</strong></td> 
      <td> <p>Selezionare questa opzione per consentire ai destinatari della condivisione di utilizzare e modificare il filtro, la visualizzazione o il raggruppamento condivisi.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condividi</strong></td> 
      <td> <p>Fai clic su <strong>Impostazioni avanzate</strong>, quindi seleziona o cancella l'opzione <strong>Condividi</strong>, a seconda che si desideri che i destinatari possano condividere con altri.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

   Gli utenti con cui hai condiviso il filtro, la visualizzazione o il raggruppamento possono accedervi facendo clic sull&#39;icona o sul menu a discesa **Filtro**, **Visualizzazione** o **Raggruppamento** e scorrendo verso il basso fino alla sezione **Condiviso con me**.


