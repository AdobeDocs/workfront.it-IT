---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Stati personalizzati in un gruppo spostato o eliminato
description: Questo articolo spiega cosa accade agli stati personalizzati del gruppo quando si sposta o si elimina un gruppo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Stati personalizzati in un gruppo spostato o eliminato

Questo articolo spiega cosa accade agli stati personalizzati del gruppo quando si sposta o si elimina un gruppo.

## Stati personalizzati in un gruppo spostato

Considera i seguenti scenari che descrivono cosa accade agli stati personalizzati del gruppo quando si sposta un gruppo in una nuova posizione in un altro gruppo.

Per informazioni sullo spostamento di un gruppo, consulta [Spostare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Quando si sposta un gruppo sotto un altro gruppo </td> 
   <td> <p>Tutti gli stati del gruppo spostato rimangono con esso. Non vengono aggiunti agli stati del nuovo gruppo padre del gruppo.</p> <p>Tuttavia, il gruppo spostato eredita tutti gli stati bloccati nel gruppo o nei gruppi che sono ora più alti nella sua gerarchia. E, da ora in poi, se un amministratore blocca uno stato più in alto nella gerarchia, il gruppo spostato eredita tale stato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quando uno stato in entrambi i gruppi ha la stessa chiave ma attributi diversi</td> 
   <td> <p>Supponiamo che due sottogruppi diversi ereditino lo stesso stato sbloccato da un gruppo padre. Gli amministratori del gruppo dei 2 gruppi personalizzano quindi lo stato per i loro gruppi in modi diversi.</p> <p>Successivamente, uno dei due gruppi viene spostato sotto l'altro. Ora entrambi hanno uno stato con la stessa chiave, ma ha attributi diversi nei due gruppi.</p> <p>In questo caso, una delle seguenti affermazioni è vera:</p> 
    <ul> 
     <li>Se lo stato nel nuovo gruppo padre viene sbloccato, lo stato nel gruppo spostato mantiene i relativi attributi, senza che lo spostamento ne pregiudichi.</li> 
     <li>Se lo stato nel nuovo gruppo padre è bloccato, gli attributi dello stato nel gruppo padre sovrascrivono quelli dello stato nel gruppo spostato.</li> 
    </ul> <p>Per informazioni sulle chiavi di stato, vedi <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Creare o modificare uno stato</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Quando un gruppo spostato ha stati ereditati dal gruppo padre precedente </td> 
   <td> <p>Tutti gli stati personalizzati ereditati dal gruppo padre precedente vengono associati al gruppo spostato e diventano i relativi stati personalizzati. Non sono più collegati al gruppo padre precedente.</p> 
    <ul> 
     <li>Se dopo lo spostamento il gruppo padre precedente modifica uno stato personalizzato bloccato, le modifiche non influiscono sullo stato del sottogruppo spostato.</li> 
     <li>Se il gruppo padre precedente blocca uno stato personalizzato sbloccato quando il gruppo è stato spostato, lo stato del sottogruppo spostato non è bloccato.</li> 
     <li>Il gruppo spostato può ora sbloccare gli stati bloccati quando li ha ereditati dal gruppo padre precedente.</li> 
    </ul> 
     <p><b>ESEMPIO:</b><p> 
     <p>Olivia, l'amministratore del gruppo per il gruppo Marketing, crea due stati per il gruppo. Lei dà un nome a First Review, con la chiave ABC, e lo blocca. Chiama l'altra Recensione Finale, con la chiave XYZ, e non la blocca.</p> 
     <p>Crea anche un sottogruppo sotto il gruppo Marketing denominato Product Marketing. Al momento della creazione, eredita automaticamente sia First Review che Final Review dal gruppo Marketing.</p> 
     <p>Successivamente, Olivia sposta il sottogruppo Product Marketing nel gruppo Product (Prodotto). Sia First Review che Final Review vanno con il gruppo di marketing del prodotto nella sua nuova posizione sotto il gruppo di prodotti.</p> 
     <p>Anche se la prima revisione è stata bloccata prima dello spostamento, l'amministratore del gruppo di marketing prodotto può modificarla ora perché non è più uno stato ereditato controllato dal gruppo padre da cui proviene.</p> 
     <p>Final Review è sbloccato e modificabile come sempre.</p> 
     <p>Per il gruppo Marketing, Olivia cambia i colori di First Review e Final Review e li rinomina First Review-Edited e Final Review-Edited. Blocca anche Final Review-Edited. Nel frattempo, nel gruppo Product Marketing, i colori e i nomi degli stati First Review e Final Review non cambiano.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Stati personalizzati in un gruppo eliminato

Quando si elimina un gruppo o un sottogruppo, le informazioni ad esso associate, compresi i relativi stati personalizzati, vengono riassegnate a un altro gruppo o sottogruppo. Gli stati del gruppo eliminato vengono aggiunti a quelli del gruppo di destinazione.

Se uno degli stati del gruppo eliminato è stato utilizzato anche dal gruppo di destinazione (lo stato in entrambi i gruppi ha la stessa chiave) e il gruppo di destinazione ha personalizzato lo stato in modi diversi, le impostazioni della versione del gruppo di destinazione sovrascrivono le impostazioni della versione del gruppo spostato.

>[!INFO]
>
>**ESEMPIO:**
>
>L&#39;amministratore del gruppo A rinomina uno stato sbloccato a livello di sistema per il gruppo. Anche l’amministratore del gruppo di un gruppo B rinomina tale stato per il gruppo. Anche se lo stato ha nomi diversi nei due gruppi, ha la stessa chiave.
>
>Successivamente, il gruppo A viene eliminato e tutte le relative informazioni vengono riassegnate al gruppo B.
>
>* Il nome della versione del gruppo B dello stato sostituisce il nome della versione del gruppo A.
>* Se lo stato è stato applicato a un oggetto da un utente del gruppo A prima dell&#39;eliminazione del gruppo, il nome dello stato dell&#39;oggetto corrisponde al nome dello stato utilizzato dal gruppo B.
>
>Per informazioni sulla chiave per uno stato, vedi la tabella in questo articolo in [Creare o modificare uno stato personalizzato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [Creare o modificare uno stato per un gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create).
>
>Per informazioni sull&#39;eliminazione di un gruppo, vedere [Eliminare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).
