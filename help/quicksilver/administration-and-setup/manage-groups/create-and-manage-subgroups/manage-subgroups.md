---
user-type: administrator
product-area: system-administration;user-management
keywords: gestisci,sottogruppo,modifica
navigation-topic: create-and-manage-subgroups
title: Gestire un sottogruppo
description: In qualità di amministratore di gruppo di un sottogruppo, puoi creare, spostare, visualizzare, modificare, copiare, rinominare, esportare ed eliminare il sottogruppo. È inoltre possibile rendere un sottogruppo un gruppo di primo livello rimuovendolo dal relativo gruppo padre.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1251'
ht-degree: 1%

---

# Gestire un sottogruppo

In qualità di amministratore di gruppo di un sottogruppo, puoi creare, spostare, visualizzare, modificare, copiare, rinominare, esportare ed eliminare il sottogruppo.

È inoltre possibile rendere un sottogruppo un gruppo di primo livello rimuovendolo dal relativo gruppo padre.

Se ci sono gruppi al di sopra del gruppo, gli amministratori possono eseguire queste operazioni anche per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

Per ulteriori informazioni sui sottogruppi, vedere [Panoramica sui sottogruppi](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>Oppure</p>
       <p>Corrente: Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Devi essere un amministratore di gruppo del gruppo o un amministratore di sistema.</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare, spostare, visualizzare, modificare, copiare, rinominare, esportare o eliminare un sottogruppo

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![Gruppi](assets/groups-icon.png).

   Nell’elenco visualizzato puoi visualizzare i gruppi che gestisci, insieme a tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Fare clic sul nome del gruppo che contiene il sottogruppo su cui si desidera lavorare.

   Oppure

   Se si spostano uno o più sottogruppi, fare clic sul nome del gruppo di destinazione (in un passaggio successivo verranno specificati i sottogruppi da spostare).

1. Nel menu a sinistra, fai clic su **Sottogruppi**.

1. Effettua una delle seguenti operazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Crea un nuovo sottogruppo</td> 
      <td> <p>Se si desidera creare il nuovo sottogruppo di un livello inferiore rispetto al gruppo visualizzato, fare clic su <strong>Aggiungi sottogruppo</strong>.</p> <p>Oppure, se desideri creare il nuovo sottogruppo sotto un altro sottogruppo nell'elenco, seleziona quel sottogruppo, quindi fai clic su <strong>Aggiungi s</strong><strong>sottogruppo</strong>.</p> <p>Per informazioni sulle opzioni utilizzabili per configurare il sottogruppo, vedere la tabella in <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">Creare un sottogruppo</a>.</p> <p>Una gerarchia di gruppi non può superare i 15 livelli, ma un singolo livello può avere un numero illimitato di gruppi paralleli.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spostare un sottogruppo </td> 
      <td> <p>È possibile spostare i sottogruppi esistenti sotto un altro gruppo amministrato.</p> <p>Una gerarchia di gruppi non può superare i 15 livelli, ma un singolo livello può avere un numero illimitato di gruppi paralleli.</p> 
       <ol> 
        <li value="1"> <p>(Facoltativo) Seleziona un sottogruppo per impostarlo come gruppo di destinazione.</p> <p>Se salti questo passaggio, il gruppo selezionato nel passaggio 3 è il gruppo di destinazione.</p> </li> 
        <li value="2">Fare clic su <strong>Aggiungi sottogruppo</strong> &gt; <strong>Gruppo esistente</strong>.</li> 
        <li value="3"> <p>Nella casella <strong>Gruppo esistente</strong> visualizzata, iniziare a digitare il nome di un sottogruppo che si desidera spostare.</p> <p>I risultati visualizzati non contengono gruppi sopra il gruppo di destinazione.</p> <p>Per assicurarsi di selezionare il gruppo corretto, passare il puntatore del mouse su di esso e fare clic sull'icona delle informazioni <img src="assets/info-icon.png"> visualizzata accanto ad esso. In questo modo viene visualizzata una descrizione del gruppo contenente informazioni sul gruppo stesso, ad esempio la gerarchia dei gruppi al di sopra del gruppo e i relativi amministratori.</p> </li> 
        <li value="4"> <p>Fare clic sul nome del sottogruppo che si desidera spostare quando viene visualizzato nell'elenco.</p> </li> 
        <li value="5"> <p>Ripeti i passaggi c-d per tutti gli altri sottogruppi che desideri spostare nel gruppo di destinazione</p> </li> 
        <li value="6">Fai clic su <strong>Salva</strong>.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modificare un sottogruppo</td> 
      <td> <p>Selezionare il sottogruppo da modificare, quindi fare clic sull'icona Modifica <img src="assets/edit-icon.png">.</p> <p>Per informazioni sulle opzioni utilizzabili per configurare il sottogruppo, vedere la tabella in <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Creare un gruppo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Esporta uno o più sottogruppi</td> 
      <td> 
       <ol> 
        <li value="1">Selezionare il sottogruppo o i sottogruppi da esportare.</li> 
        <li value="2">Fare clic sull'icona Esporta <img src="assets/export.png">, quindi selezionare il formato di file desiderato.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copiare un sottogruppo per creare un nuovo gruppo di primo livello</td> 
      <td> <p>Disponibile solo per gli amministratori di Workfront. Quando copiate un sottogruppo, questo diventa un gruppo padre. Tutti i membri e i sottogruppi del gruppo vengono copiati con esso. I membri dei gruppi conservano tutte le assegnazioni che avevano nel gruppo originale.</p> <p>Per ulteriori informazioni sulla copia di un sottogruppo, vedere <a href="#about-copying-a-subgroup" class="MCXref xref">Informazioni sulla copia di un sottogruppo</a> in questo articolo.</p> 
       <ol> 
        <li value="1">Selezionare un sottogruppo, quindi fare clic sull'icona Copia <img src="assets/copy-icon.png"> per creare un nuovo gruppo di primo livello basato sul gruppo selezionato.</li> 
        <li value="2"> <p>Configura le impostazioni del nuovo gruppo.</p> <p>Per informazioni su queste impostazioni, vedere la tabella nella sezione <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Creare un gruppo di primo livello copiando un gruppo o un sottogruppo esistente</a> nell'articolo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Creare un gruppo di primo livello copiando un gruppo o un sottogruppo esistente</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminare un sottogruppo</td> 
      <td> <p><b>IMPORTANTE</b>: quando si elimina un gruppo o un sottogruppo, è necessario mantenere gli utenti, gli elementi di lavoro ed eventuali sottogruppi attualmente assegnati. Per assicurarsi che vengano mantenuti, un prompt richiede di riassegnare gli oggetti del gruppo a un gruppo diverso nel passaggio seguente.</p> 
       <ol> 
        <li value="1">Selezionare il sottogruppo, quindi fare clic sull'icona Elimina <img src="assets/delete.png">.</li> 
        <li value="2">Nella casella <strong>Elimina gruppo</strong> visualizzata, iniziare a digitare e quindi selezionare il nome del gruppo in cui si desidera spostare i membri, gli elementi di lavoro e i sottogruppi del gruppo che si sta eliminando.</li> 
        <li value="3">Fai clic su <strong>Elimina</strong>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>Quando gestisci un gruppo che contiene sottogruppi, è utile essere in grado di identificare e filtrare i dati relativi all’intero gruppo e a tutti i suoi sottogruppi. A tale scopo, utilizza il campo ID padre principale in un report o in un elenco.
>
>Si supponga, ad esempio, di gestire un reparto di marketing di grandi dimensioni e di volere un elenco di tutti i progetti su cui sta lavorando l&#39;intero reparto.
>
>In Workfront, questo reparto marketing è rappresentato da un gruppo denominato Marketing, con 3 sottogruppi denominati Marketing sul campo, Marketing sul prodotto e Marketing digitale. Per elencare i progetti che appartengono all’intero reparto Marketing (tutti e 4 i gruppi), puoi creare un filtro per l’area Progetti con la seguente regola di filtro:
>
>`Group: Top Parent ID > Equal > Marketing`
>
>È inoltre possibile utilizzare il campo Nome padre principale per identificare i dati associati a un gruppo di livello principale, ma solo nelle Visualizzazioni, non in Filtri o Raggruppamenti.

## Rimuovere un sottogruppo dal relativo gruppo padre e impostarlo come gruppo di livello principale

È possibile rendere un sottogruppo un gruppo di primo livello rimuovendolo dal relativo gruppo padre.

>[!TIP]
>
>Quando disattivi un gruppo con sottogruppi al di sotto di esso, anche questi sottogruppi diventano inattivi. Se desideri che uno dei due sia attivo, puoi utilizzare queste istruzioni per rimuoverlo dal gruppo principale e riattivarlo.
>
>Per istruzioni sulla disattivazione e la riattivazione dei gruppi, vedere le sezioni [Visualizzare e gestire i dettagli di un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) e [Visualizzare e gestire i dettagli di un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) nell&#39;articolo [Visualizzare e gestire i dettagli di un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![Gruppi](assets/groups-icon.png).

1. Seleziona il gruppo principale del gruppo che desideri creare, quindi fai clic sull&#39;icona Modifica ![icona Modifica](assets/edit-icon.png).
1. Nella casella **Modifica gruppo** visualizzata, in **Membri gruppo e amministratori gruppo**, inizia a digitare il nome del sottogruppo che si desidera creare come gruppo principale, quindi fai clic sulla X a destra del nome quando viene visualizzato.
1. Fai clic su **Salva**.

## Visualizzare e gestire i membri del sottogruppo di un gruppo

Quando visualizzi la pagina principale di un gruppo che amministri, puoi visualizzare e gestire tutti gli utenti dei sottogruppi del gruppo. Per istruzioni, vedere [Visualizzare e gestire i membri del sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Informazioni sulla copia di un sottogruppo {#about-copying-a-subgroup}

Quando copiate un sottogruppo, tenete presente quanto segue.

* Se un sottogruppo copiato dispone di sottogruppi propri, questi vengono inclusi nella copia e i relativi nomi vengono formattati come segue:

  `Original subgroup name (Copy)`

* Qualsiasi sottogruppo che appartiene a un gruppo pubblico è anch’esso pubblico, pertanto qualsiasi utente con accesso di modifica utente, interno o esterno al gruppo, può aggiungere utenti al sottogruppo.
