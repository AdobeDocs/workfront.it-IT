---
user-type: administrator
product-area: system-administration;user-management
keywords: gestisci, sottogruppo, modifica
navigation-topic: create-and-manage-subgroups
title: Gestire un sottogruppo
description: In qualità di amministratore di gruppo di un sottogruppo, è possibile creare, spostare, visualizzare, modificare, copiare, rinominare, esportare ed eliminare il sottogruppo. È inoltre possibile rendere un sottogruppo un gruppo di livello principale rimuovendolo dal gruppo principale.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 1%

---

# Gestire un sottogruppo

In qualità di amministratore di gruppo di un sottogruppo, è possibile creare, spostare, visualizzare, modificare, copiare, rinominare, esportare ed eliminare il sottogruppo.

È inoltre possibile rendere un sottogruppo un gruppo di livello principale rimuovendolo dal gruppo principale.

Se ci sono gruppi al di sopra del gruppo, i loro amministratori possono fare queste cose anche per il tuo gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

Per ulteriori informazioni sui sottogruppi, consulta [Panoramica sui sottogruppi](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>È necessario essere un amministratore del gruppo o un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Creare, spostare, visualizzare, modificare, copiare, rinominare, esportare o eliminare un sottogruppo

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

   Nell’elenco visualizzato, puoi vedere i gruppi gestiti e tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Fare clic sul nome del gruppo che contiene il sottogruppo su cui si desidera lavorare.

   Oppure

   Se stai spostando uno o più sottogruppi, fai clic sul nome del gruppo di destinazione (specificherai i sottogruppi da spostare in un passaggio successivo).

1. Nel menu a sinistra, fai clic su **Sottogruppi**.

1. Effettua una delle seguenti operazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Creare un nuovo sottogruppo</td> 
      <td> <p>Se si desidera creare il nuovo sottogruppo un livello inferiore dal gruppo visualizzato, fare clic su <strong>Aggiungi sottogruppo</strong>.</p> <p>Oppure, se si desidera creare il nuovo sottogruppo sotto un altro sottogruppo nell’elenco, selezionare il sottogruppo, quindi fare clic su <strong>Aggiungi s</strong><strong>sottogruppo</strong>.</p> <p>Per informazioni sulle opzioni utilizzabili per configurare il sottogruppo, consulta la tabella in <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">Creare un sottogruppo</a>.</p> <p>Una gerarchia di gruppi non può superare i 15 livelli, ma un singolo livello può avere un numero illimitato di gruppi paralleli.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spostare un sottogruppo </td> 
      <td> <p>È possibile spostare i sottogruppi esistenti sotto un altro gruppo amministrato.</p> <p>Una gerarchia di gruppi non può superare i 15 livelli, ma un singolo livello può avere un numero illimitato di gruppi paralleli.</p> 
       <ol> 
        <li value="1"> <p>(Facoltativo) Seleziona un sottogruppo per renderlo il gruppo di destinazione.</p> <p>Se salti questo passaggio, il gruppo selezionato al passaggio 3 è il gruppo di destinazione.</p> </li> 
        <li value="2">Fai clic su <strong>Aggiungi sottogruppo</strong> &gt; <strong>Gruppo esistente</strong>.</li> 
        <li value="3"> <p>In <strong>Gruppo esistente</strong> nella casella visualizzata, inizia a digitare il nome di un sottogruppo da spostare.</p> <p>I risultati visualizzati non contengono gruppi al di sopra del gruppo di destinazione.</p> <p>Per selezionare il gruppo di destra, posiziona il cursore sopra di esso e fai clic sull’icona delle informazioni <img src="assets/info-icon.png"> viene visualizzato accanto a esso. Viene visualizzata una descrizione comandi che elenca le informazioni sul gruppo, ad esempio la gerarchia dei gruppi al di sopra di esso e i relativi amministratori.</p> </li> 
        <li value="4"> <p>Fare clic sul nome del sottogruppo che si desidera spostare quando viene visualizzato nell’elenco.</p> </li> 
        <li value="5"> <p>Ripeti i passaggi c-d per tutti gli altri sottogruppi da spostare al gruppo di destinazione</p> </li> 
        <li value="6">Fai clic su <strong>Salva</strong>.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modificare un sottogruppo</td> 
      <td> <p>Seleziona il sottogruppo da modificare, quindi fai clic sull’icona Modifica <img src="assets/edit-icon.png">.</p> <p>Per informazioni sulle opzioni utilizzabili per configurare il sottogruppo, consulta la tabella in <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Creare un gruppo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Esportare uno o più sottogruppi</td> 
      <td> 
       <ol> 
        <li value="1">Selezionare il sottogruppo o i sottogruppi da esportare.</li> 
        <li value="2">Fai clic sull’icona Esporta <img src="assets/export.png">, quindi selezionare il formato di file desiderato.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copiare un sottogruppo per creare un nuovo gruppo principale</td> 
      <td> <p>(Disponibile solo per gli amministratori di Workfront). Quando copi un sottogruppo, questo diventa un gruppo principale. Tutti i membri e i sottogruppi del gruppo vengono copiati con esso. I membri dei gruppi conservano tutte le assegnazioni che avevano nel gruppo originale.</p> <p>Per ulteriori informazioni sulla copia di un sottogruppo, consulta <a href="#about-copying-a-subgroup" class="MCXref xref">Informazioni sulla copia di un sottogruppo</a> in questo articolo.</p> 
       <ol> 
        <li value="1">Seleziona un sottogruppo, quindi fai clic sull’icona Copia <img src="assets/copy-icon.png"> per creare un nuovo gruppo di primo livello basato sul gruppo selezionato.</li> 
        <li value="2"> <p>Configura le impostazioni del nuovo gruppo.</p> <p>Per informazioni su queste impostazioni, consulta la tabella nella sezione . <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Creare un gruppo di primo livello copiando un gruppo o un sottogruppo esistente</a> nell'articolo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Creare un gruppo di primo livello copiando un gruppo o un sottogruppo esistente</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminare un sottogruppo</td> 
      <td> <p><b>IMPORTANTE</b>: Quando si elimina un gruppo o un sottogruppo, è necessario mantenere gli utenti, gli elementi di lavoro ed eventuali sottogruppi attualmente assegnati. Per assicurarti che siano mantenuti, un prompt richiede di riassegnare gli oggetti del gruppo a un gruppo diverso nel passaggio seguente.</p> 
       <ol> 
        <li value="1">Seleziona il sottogruppo, quindi fai clic sull’icona Elimina <img src="assets/delete.png">.</li> 
        <li value="2">In <strong>Elimina gruppo</strong> viene visualizzata la casella che inizia a digitare e quindi selezionare il nome del gruppo in cui si desidera spostare i membri, gli elementi di lavoro e i sottogruppi del gruppo che si sta eliminando.</li> 
        <li value="3">Fai clic su <strong>Eliminali</strong>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>Quando gestisci un gruppo che contiene sottogruppi, è utile essere in grado di identificare e filtrare i dati relativi all’intero gruppo e a tutti i relativi sottogruppi. A tale scopo, utilizza il campo ID principale in un rapporto o in un elenco.
>
>Ad esempio, immagina di gestire un grande reparto Marketing e di volere un elenco di tutti i progetti su cui sta lavorando l&#39;intero reparto.
>
>In Workfront, questo reparto marketing è rappresentato da un gruppo chiamato Marketing, con 3 sottogruppi chiamati Field Marketing, Product Marketing e Digital Marketing. Per elencare i progetti che appartengono all&#39;intero reparto Marketing (tutti e 4 i gruppi), puoi creare un filtro per l&#39;area Progetti con la seguente regola filtro:
>
>
```
>Group: Top Parent ID > Equal > Marketing
>```
>
>È inoltre possibile utilizzare il campo Nome padre principale per identificare i dati associati a un gruppo di livello principale, ma solo in Visualizzazioni, non in Filtri o Raggruppamenti.

## Rimuovere un sottogruppo dal gruppo padre e renderlo un gruppo di livello principale

È possibile rendere un sottogruppo un gruppo di livello principale rimuovendolo dal gruppo principale.

>[!TIP]
>
>Quando disattivi un gruppo con sottogruppi, anche questi diventano inattivi. Se si desidera che uno di essi sia attivo, è possibile utilizzare queste istruzioni per rimuoverlo dal gruppo padre, quindi riattivarlo.
>
>Per istruzioni sulla disattivazione e la riattivazione dei gruppi, consulta le sezioni [Visualizzare e gestire i dettagli di un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) e [Visualizzare e gestire i dettagli di un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) nell&#39;articolo [Visualizzare e gestire i dettagli di un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Selezionare il gruppo padre del gruppo che si desidera creare come gruppo di livello principale, quindi fare clic sull&#39;icona Modifica ![](assets/edit-icon.png).
1. In **Modifica gruppo** casella visualizzata, sotto **Membri del gruppo e amministratori del gruppo**, inizia a digitare il nome del sottogruppo che desideri creare un gruppo di livello principale, quindi fai clic sulla X a destra del nome corrispondente quando viene visualizzata.
1. Fai clic su **Salva**.

## Visualizzare e gestire i membri del sottogruppo di un gruppo

Quando visualizzi la pagina principale di un gruppo che gestisci, puoi visualizzare e gestire tutti gli utenti dei sottogruppi del gruppo. Per istruzioni, consulta [Visualizzare e gestire i membri dei sottogruppi](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Informazioni sulla copia di un sottogruppo {#about-copying-a-subgroup}

Quando copi un sottogruppo, tieni presente quanto segue.

* Se un sottogruppo copiato ha i propri sottogruppi, questi vengono inclusi nella copia e i relativi nomi vengono formattati come segue:

   ```
   Original subgroup name (Copy)
   ```

* Anche qualsiasi sottogruppo appartenente a un gruppo pubblico è pubblico, in modo che qualsiasi utente con accesso per l’utente con accesso per la modifica, all’interno o all’esterno del gruppo, possa aggiungere utenti al sottogruppo.
