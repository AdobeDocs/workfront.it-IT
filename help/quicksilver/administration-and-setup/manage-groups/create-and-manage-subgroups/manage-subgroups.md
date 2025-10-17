---
user-type: administrator
product-area: system-administration;user-management
keywords: gestisci,sottogruppo,modifica
navigation-topic: create-and-manage-subgroups
title: Gestire un sottogruppo
description: In qualità di amministratore di gruppo di un sottogruppo, puoi creare, spostare, visualizzare, modificare, copiare, rinominare, esportare ed eliminare il sottogruppo. È inoltre possibile rendere un sottogruppo un gruppo di primo livello rimuovendolo dal relativo gruppo padre.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1386'
ht-degree: 0%

---

# Gestire un sottogruppo

In qualità di amministratore di gruppo di un sottogruppo, puoi creare, spostare, visualizzare, modificare, copiare, rinominare, esportare ed eliminare il sottogruppo.

È inoltre possibile rendere un sottogruppo un gruppo di primo livello rimuovendolo dal relativo gruppo padre.

Se ci sono gruppi al di sopra del gruppo, gli amministratori possono eseguire queste operazioni anche per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

Per ulteriori informazioni sui sottogruppi, vedere [Panoramica sui sottogruppi](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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
>È inoltre possibile utilizzare il campo Nome padre principale per identificare i dati associati a un gruppo di livello principale, ma solo nelle visualizzazioni, non nei filtri o nei raggruppamenti.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr>
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Devi essere un amministratore di gruppo del gruppo o un amministratore di sistema.</td>
  </tr>
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare un sottogruppo

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![Gruppi](assets/groups-icon.png).

   Nell’elenco visualizzato puoi visualizzare i gruppi che gestisci, insieme a tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Fare clic sul nome del gruppo in cui si desidera aggiungere un sottogruppo.
1. Nel menu a sinistra, fai clic su **Sottogruppi**.
1. Per creare un nuovo sottogruppo a un livello inferiore rispetto al gruppo visualizzato, fare clic su **Aggiungi sottogruppo**.

   Oppure, se si desidera creare il nuovo sottogruppo sotto un altro sottogruppo nell&#39;elenco, selezionare tale sottogruppo, quindi fare clic su **Aggiungi sottogruppo**.

   Per informazioni sulle opzioni utilizzabili per configurare il sottogruppo, vedere [Creare un sottogruppo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

   Una gerarchia di gruppi non può superare i 15 livelli, ma un singolo livello può avere un numero illimitato di gruppi paralleli.

## Spostare un sottogruppo

È possibile spostare i sottogruppi esistenti sotto un altro gruppo amministrato.

Una gerarchia di gruppi non può superare i 15 livelli, ma un singolo livello può avere un numero illimitato di gruppi paralleli.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![Gruppi](assets/groups-icon.png).

   Nell’elenco visualizzato puoi visualizzare i gruppi che gestisci, insieme a tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Fare clic sul nome del gruppo di destinazione, per specificare quali sottogruppi si desidera spostare in un passaggio successivo.
1. Nel menu a sinistra, fai clic su **Sottogruppi**.
1. (Facoltativo) Seleziona un sottogruppo per impostarlo come gruppo di destinazione.

   Se salti questo passaggio, il gruppo selezionato nel passaggio 3 è il gruppo di destinazione.

1. Fare clic su **Aggiungi sottogruppo > Gruppo esistente**.
1. Nella casella **Gruppo esistente** visualizzata, iniziare a digitare il nome di un sottogruppo che si desidera spostare.

   I risultati visualizzati non contengono gruppi sopra il gruppo di destinazione.

   Per assicurarsi di selezionare il gruppo corretto, passare il puntatore del mouse su di esso e fare clic sull&#39;icona delle informazioni ![icona delle informazioni](assets/info-icon.png) visualizzata accanto ad esso. In questo modo viene visualizzata una descrizione del gruppo contenente informazioni sul gruppo stesso, ad esempio la gerarchia dei gruppi al di sopra del gruppo e i relativi amministratori.

1. Selezionare il nome del sottogruppo che si desidera spostare quando lo si individua nell&#39;elenco.
1. Ripetere i passaggi 7-8 per tutti gli altri sottogruppi che si desidera spostare nel gruppo di destinazione.
1. Fai clic su **Salva**.

## Modificare un sottogruppo

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![Gruppi](assets/groups-icon.png).

   Nell’elenco visualizzato puoi visualizzare i gruppi che gestisci, insieme a tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Fare clic sul nome del gruppo che contiene il sottogruppo da modificare.
1. Nel menu a sinistra, fai clic su **Sottogruppi**.
1. Seleziona il sottogruppo da modificare, quindi fai clic sull&#39;icona **Modifica** ![Modifica](assets/edit-icon.png).

   Per informazioni sulle opzioni utilizzabili per configurare il sottogruppo, vedere [Creare un sottogruppo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Copiare un sottogruppo

>[!NOTE]
>
>Solo un amministratore di sistema può copiare un sottogruppo.

Quando copiate un sottogruppo, questo diventa un gruppo padre. Tutti i membri e i sottogruppi del gruppo vengono copiati con esso. I membri del gruppo mantengono tutte le assegnazioni che avevano nel gruppo originale.

Quando copiate un sottogruppo, tenete presente quanto segue:

* Se un sottogruppo copiato dispone di sottogruppi propri, questi vengono inclusi nella copia e i relativi nomi vengono formattati come segue:

  `Original subgroup name (Copy)`

* Qualsiasi sottogruppo che appartiene a un gruppo pubblico è anch’esso pubblico, pertanto qualsiasi utente con accesso alla modifica degli utenti, interni o esterni al gruppo, può aggiungere utenti al sottogruppo.

Per copiare un sottogruppo:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![Gruppi](assets/groups-icon.png).

   Nell’elenco visualizzato puoi visualizzare i gruppi che gestisci, insieme a tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Fare clic sul nome del gruppo che contiene il sottogruppo da copiare.
1. Nel menu a sinistra, fai clic su **Sottogruppi**.
1. Seleziona un sottogruppo, quindi fai clic sull&#39;icona **Copia** ![Copia icona](assets/copy-icon.png) per creare un nuovo gruppo di primo livello basato sul gruppo selezionato.
1. Configura le impostazioni del nuovo gruppo.

   Per informazioni su queste impostazioni, vedere [Creare un gruppo di primo livello copiando un gruppo o un sottogruppo esistente](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) nell&#39;articolo [Creare un gruppo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

1. Fare clic su **Crea gruppo**.

## Esportare un sottogruppo

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![Gruppi](assets/groups-icon.png).

   Nell’elenco visualizzato puoi visualizzare i gruppi che gestisci, insieme a tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Fare clic sul nome del gruppo che contiene il sottogruppo da esportare.
1. Nel menu a sinistra, fai clic su **Sottogruppi**.
1. Selezionare il sottogruppo o i sottogruppi da esportare.
1. Fai clic sull&#39;icona **Esporta** ![Icona Esporta](assets/export.png), quindi seleziona il formato di file desiderato.

## Rimuovere un sottogruppo dal relativo gruppo padre e impostarlo come gruppo di livello principale

È possibile rendere un sottogruppo un gruppo di primo livello rimuovendolo dal relativo gruppo padre.

>[!TIP]
>
>Quando disattivi un gruppo con sottogruppi al di sotto di esso, anche questi sottogruppi diventano inattivi. Se desideri che uno dei due sia attivo, puoi utilizzare queste istruzioni per rimuoverlo dal gruppo principale e riattivarlo.
>>Per istruzioni sulla disattivazione e la riattivazione dei gruppi, vedere [Disattivare o riattivare un gruppo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![Gruppi](assets/groups-icon.png).
1. Seleziona il gruppo principale del sottogruppo che desideri creare come gruppo principale, quindi fai clic sull&#39;icona **Modifica** ![Modifica icona](assets/edit-icon.png).
1. Nella casella **Modifica gruppo** visualizzata, inizia a digitare il nome del sottogruppo che desideri creare come gruppo di primo livello nel campo **Cerca** (in **Membri gruppo e amministratori gruppo**), quindi fai clic sulla X a destra del nome quando viene visualizzata.
1. Fai clic su **Salva**.

## Eliminare un sottogruppo

>[!IMPORTANT]
>
>Quando si elimina un gruppo o un sottogruppo, è necessario mantenere gli utenti, gli elementi di lavoro ed eventuali sottogruppi attualmente assegnati. Per assicurarsi che vengano mantenuti, un prompt richiede di riassegnare gli oggetti del gruppo a un gruppo diverso.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![Gruppi](assets/groups-icon.png).

   Nell’elenco visualizzato puoi visualizzare i gruppi che gestisci, insieme a tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Fare clic sul nome del gruppo che contiene il sottogruppo che si desidera eliminare.
1. Nel menu a sinistra, fai clic su **Sottogruppi**.
1. Seleziona il sottogruppo, quindi fai clic sull&#39;icona **Elimina** ![Elimina](assets/delete.png).

   Nella casella **Elimina gruppo** visualizzata, iniziare a digitare e quindi selezionare il nome del gruppo in cui si desidera spostare i membri, gli elementi di lavoro e i sottogruppi del gruppo che si sta eliminando.

1. Fare clic su **Elimina**.

## Visualizzare e gestire i membri del sottogruppo di un gruppo

Quando visualizzi la pagina principale di un gruppo che amministri, puoi visualizzare e gestire tutti gli utenti dei sottogruppi del gruppo. Per istruzioni, vedere [Visualizzare e gestire i membri del sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

