---
title: Modifica campi
description: Ad Adobe, Maestro può modificare le impostazioni dei campi già creati.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: c264c0c96b818934a7c25ed54c7666d2d6c95e54
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!---
title: Edit foelds
description: In Adobe Maestro, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->


# Modifica campi

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono a Adobe Maestro, una nuova offerta di Adobe Workfront.
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti. Per utilizzare le funzionalità Maestro, devi essere un cliente Workfront.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

È possibile modificare le impostazioni dei campi già creati.

Per informazioni sulla creazione di campi Adobe Maestro, consulta [Crea campi](../fields/create-fields.md).

Questo articolo descrive come modificare le impostazioni per i campi Maestro. Per informazioni sulla modifica dei valori dei campi per i record Maestro, vedere [Modifica record](/help/quicksilver/maestro/records/edit-records.md).

## Considerazioni sulla modifica delle informazioni sui campi

* Se disponi delle autorizzazioni di gestione per l’area di lavoro a cui appartengono i campi, puoi modificare i campi creati o quelli creati da altri utenti.
* È possibile modificare un campo nella tabella del tipo di record.
* Non è possibile modificare un campo nella pagina Dettagli di un record o nella visualizzazione timeline.
* Non è possibile modificare il tipo di campo dopo il salvataggio del campo.
* Non è possibile deselezionare l&#39;impostazione Consenti numeri negativi precedentemente selezionata per un campo Numerico, Percentuale o Valuta se sono già presenti valori negativi memorizzati nei record a cui è associato.
<!--this is not true yet; one piece of it is true and I added it as the bullet above: 
* You cannot edit the options, or the special format of the following fields, after they are saved:

    * Allow negative numbers option from a Number, Percentage, or Currency field. 
    * The Options of a Single-select or a Multi-select field.
-->

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Prodotto</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>La tua organizzazione deve essere iscritta al programma beta chiuso Adobe Maestro. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>piano Adobe Workfront</p></td>
   <td>
<p>Qualsiasi</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td>
   <td>
   <p>Qualsiasi</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td>
   <td> <p>Non ci sono controlli di accesso per Maestro</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestire le autorizzazioni per un’area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L’amministratore del Workfront o del gruppo deve aggiungere l’area Maestro nel modello di layout. Per informazioni, consulta <a href="../access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Modifica campi

1. Fai clic su **Menu principale** icona ![](assets/main-menu-workfront.png) nell&#39;angolo superiore destro di Workfront oppure **Menu principale** icona ![](assets/main-menu-shell.png)  nell’angolo superiore sinistro, se disponibile, fai clic su **Maestro** ![](assets/maestro-icon.png).

   Per impostazione predefinita, viene aperta l’ultima area di lavoro a cui si è effettuato l’accesso.

1. (Facoltativo) Espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente e selezionare il workspace per il quale si desidera eliminare i tipi di record.

   Verrà aperto il workspace e verranno visualizzati i tipi di record e le tassonomie ad esso associati.
1. Fare clic sulla scheda relativa al tipo di record o alla tassonomia di cui si desidera modificare i campi.

   Verrà aperta la pagina del tipo di record.
1. (Condizionale) Seleziona un **Vista tabella** dal **Visualizza** nell&#39;angolo superiore destro della pagina del tipo di record.
1. Passa il puntatore del mouse sull&#39;intestazione di colonna di un campo che desideri modificare, quindi fai clic sulla freccia rivolta verso il basso dopo il nome del campo, quindi fai clic su **Modifica campo**

   Oppure

   Fare doppio clic sull&#39;intestazione di colonna per il campo.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Aggiorna le informazioni sul campo e fai clic su **Salva**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >Non è possibile aggiornare il tipo di campo dopo il salvataggio del campo.


1. (Condizionale) Per i campi record collegati, fai clic su **Modifica campi di ricerca** e aggiungere o rimuovere qualsiasi campo dal tipo di record collegato.

   Per ulteriori informazioni, consulta [Connetti tipi di record](../architecture/connect-record-types.md).
