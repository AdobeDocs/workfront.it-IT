---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Stati personalizzati in un gruppo spostato o eliminato
description: Questo articolo spiega cosa accade agli stati personalizzati di gruppo quando si sposta o si elimina un gruppo.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# Stati personalizzati in un gruppo spostato o eliminato

Questo articolo spiega cosa accade agli stati personalizzati di gruppo quando si sposta o si elimina un gruppo.

## Stati personalizzati in un gruppo spostato

Considera gli scenari seguenti che descrivono cosa accade agli stati personalizzati di gruppo quando si sposta un gruppo in una nuova posizione all’interno di un altro gruppo.

Per informazioni sullo spostamento di un gruppo, vedere [Spostare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Quando si sposta un gruppo in un altro gruppo </td> 
   <td> <p>Tutti gli stati del gruppo spostato rimangono con esso. Non vengono aggiunti agli stati del nuovo gruppo principale del gruppo.</p> <p>Tuttavia, il gruppo spostato eredita gli eventuali stati bloccati nel gruppo o nei gruppi che sono ora più elevati nella gerarchia. D'ora in poi, se un amministratore blocca uno stato più in alto nella gerarchia, il gruppo spostato eredita tale stato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quando uno stato in entrambi i gruppi ha la stessa chiave ma attributi diversi</td> 
   <td> <p>Si supponga che due diversi sottogruppi ereditino lo stesso stato sbloccato da un gruppo padre. Gli amministratori dei 2 gruppi personalizzano quindi lo stato dei loro gruppi in modi diversi.</p> <p>Successivamente, uno dei due gruppi viene spostato sotto l'altro. Ora entrambi hanno uno stato con la stessa chiave, ma ha attributi diversi nei due gruppi.</p> <p>In questo caso, si verifica una delle seguenti situazioni:</p> 
    <ul> 
     <li>Se lo stato nel nuovo gruppo padre è sbloccato, lo stato nel gruppo spostato mantiene i relativi attributi, senza essere influenzato dallo spostamento.</li> 
     <li>Se lo stato nel nuovo gruppo padre è bloccato, gli attributi dello stato nel gruppo padre sostituiscono quelli del gruppo spostato.</li> 
    </ul> <p>Per informazioni sulle chiavi di stato, vedere <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Creare o modificare uno stato</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Quando uno stato di un gruppo spostato viene ereditato dal gruppo padre precedente </td> 
   <td> <p>Tutti gli stati personalizzati ereditati dal gruppo padre precedente vengono forniti con il gruppo spostato e ne diventano gli stati personalizzati. Non sono più connessi al gruppo padre precedente.</p> 
    <ul> 
     <li>Se il gruppo padre precedente modifica uno stato personalizzato bloccato dopo lo spostamento, le modifiche non influiscono sullo stato del sottogruppo spostato.</li> 
     <li>Se il gruppo padre precedente blocca uno stato personalizzato sbloccato durante lo spostamento del gruppo, lo stato del sottogruppo spostato non viene bloccato.</li> 
     <li>Il gruppo spostato può ora sbloccare gli stati bloccati quando li ha ereditati dal gruppo padre precedente.</li> 
    </ul> 
     <p><b>ESEMPIO:</b><p> 
     <p>Olivia, l’amministratore del gruppo Marketing, crea due stati per il gruppo. Nominò una First Review, con la chiave ABC, e la chiuse. Dà un nome all'altra Revisione Finale, con la chiave XYZ, e non la blocca.</p> 
     <p>Crea anche un sottogruppo all’interno del gruppo Marketing denominato Product Marketing. Al momento della creazione, eredita automaticamente sia la prima revisione che la revisione finale dal gruppo Marketing.</p> 
     <p>Successivamente, Olivia sposta il sottogruppo Product Marketing sotto il gruppo Product. Sia la prima revisione che la revisione finale vengono effettuate con il gruppo Product Marketing nella nuova posizione all'interno del gruppo Prodotti.</p> 
     <p>Anche se la prima revisione è stata bloccata prima dello spostamento, l’amministratore del gruppo marketing prodotti può modificarla ora perché non si tratta più di uno stato ereditato controllato dal gruppo principale da cui proviene.</p> 
     <p>La revisione finale è sbloccata e modificabile come sempre.</p> 
     <p>Per il gruppo Marketing, Olivia cambia i colori di First Review e Final Review e li rinomina First Review-Edited e Final Review-Edited. Blocca anche Final Review-Edited. Nel frattempo, nel gruppo Marketing prodotto, i colori e i nomi degli stati Prima revisione e Revisione finale non cambiano.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Stati personalizzati in un gruppo eliminato

Quando si elimina un gruppo o un sottogruppo, le informazioni associate, inclusi gli stati personalizzati, vengono riassegnate a un altro gruppo o sottogruppo. Gli stati del gruppo eliminato vengono aggiunti a quelli del gruppo di destinazione.

Se uno degli stati del gruppo eliminato era utilizzato anche dal gruppo di destinazione (lo stato in entrambi i gruppi ha la stessa chiave) e il gruppo di destinazione ha personalizzato lo stato in modi diversi, le impostazioni della versione del gruppo di destinazione sostituiscono le impostazioni della versione del gruppo spostato.

>[!INFO]
>
>**ESEMPIO:**
>
>L&#39;amministratore gruppo del Gruppo A rinomina uno stato sbloccato a livello di sistema per il gruppo. Anche l&#39;amministratore di gruppo di un Gruppo B rinomina tale stato per il proprio gruppo. Anche se lo stato ha nomi diversi nei due gruppi, ha la stessa chiave.
>
>Successivamente, il Gruppo A viene eliminato e tutte le sue informazioni vengono riassegnate al Gruppo B.
>
>* Il nome della versione del gruppo B dello stato sostituisce il nome della versione del gruppo A.
>* Se lo stato è stato applicato a un oggetto da un utente del gruppo A prima che tale gruppo fosse eliminato, il nome dello stato dell&#39;oggetto viene aggiornato in base al nome dello stato utilizzato dal gruppo B.
>
>Per informazioni sulla chiave di uno stato, vedere la tabella in questo articolo in [Creare o modificare uno stato personalizzato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [Creare o modificare uno stato per un gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create).
>
>Per informazioni sull&#39;eliminazione di un gruppo, vedere [Eliminare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).
