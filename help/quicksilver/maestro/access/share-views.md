---
title: Condividere le visualizzazioni
description: Puoi condividere una visualizzazione con altri utenti per garantire la collaborazione quando utilizzi la pianificazione di Adobe Workfront.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live-->

# Condividere le visualizzazioni

{{maestro-important-intro}}

È possibile condividere una visualizzazione con altri utenti per garantire la collaborazione durante l&#39;utilizzo dei record nella pianificazione di Adobe Workfront.

La concessione di autorizzazioni a un&#39;area di lavoro non consente ad altri utenti di concedere autorizzazioni per le visualizzazioni nelle pagine dei tipi di record. È necessario concedere autorizzazioni alle singole visualizzazioni in una pagina di tipo record per condividerle con altri utenti.

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
<p>L’organizzazione deve essere iscritta al programma beta chiuso di pianificazione di Adobe Workfront. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
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
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td>
   <td> Nessun controllo di accesso per la pianificazione di Adobe Workfront </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td>
   <td> <p>Gestire le autorizzazioni per una visualizzazione</p>

</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p> <p>Per informazioni, consulta <a href="/help/quicksilver/maestro/access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Condivisione delle autorizzazioni per una visualizzazione

Puoi condividere le viste create o le viste per le quali disponi delle autorizzazioni di gestione.

>[!NOTE]
>
>Gli amministratori di sistema non possono visualizzare o condividere viste che non hanno creato personalmente. Possono accedere o condividere solo le visualizzazioni condivise con loro.
>
>Gli amministratori di sistema possono disporre solo delle autorizzazioni di gestione per una visualizzazione.

{{step1-to-maestro}}

1. Aprire l&#39;area di lavoro di cui si desidera condividere la visualizzazione, quindi fare clic su una scheda del tipo di record.

   Verrà aperta la pagina del tipo di record.

1. Dalla scheda Visualizza, passa il puntatore del mouse sulla visualizzazione da condividere e fai clic sul pulsante **Altro** menu ![](assets/more-menu.png) a destra del nome della visualizzazione, quindi fai clic su **Condividi**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. In **Concedi l’accesso in visualizzazione a** , inizia a digitare il nome di un utente o di un gruppo, quindi fai clic su di esso quando viene visualizzato nell’elenco.

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Seleziona uno dei seguenti livelli di autorizzazione dal menu a discesa:
   * Visualizza
   * Gestire

     Per informazioni sui livelli di autorizzazione e sulle azioni che gli utenti possono eseguire per ciascun livello, consulta [Panoramica delle autorizzazioni di condivisione nella pianificazione di Adobe Workfront](../access/sharing-permissions-overview.md).

     <!--System administrators always receive Manage permissions to views shared with them.-->

1. Clic **Copia collegamento** per copiare negli Appunti un collegamento alla visualizzazione.
1. Condividi il collegamento copiato con altri utenti. Gli utenti che ricevono il collegamento devono essere utenti attivi e accedere a Workfront per poter accedere alla pagina del tipo di record e visualizzarla nella visualizzazione selezionata.
1. Fai clic su **Salva**.

## Rimuovere le autorizzazioni per una visualizzazione

{{step1-to-maestro}}

1. Aprire l&#39;area di lavoro di cui si desidera condividere la visualizzazione, quindi fare clic su una scheda del tipo di record. Verrà aperta la pagina del tipo di record.
1. Dal menu a discesa della vista, passa il puntatore sulla vista da condividere e fai clic sul pulsante **Altro** menu ![](assets/more-menu.png) a destra del nome della visualizzazione, quindi fai clic su **Condividi**.
1. Trova l’utente o il gruppo da rimuovere, quindi fai clic su **Rimuovi** nel menu a discesa autorizzazioni a destra del nome dell’utente o del gruppo.
1. Clic **Salva**.
L&#39;utente o gli utenti che appartengono al gruppo rimosso non hanno più accesso alla visualizzazione. Non esiste alcuna notifica per gli utenti che sono stati rimossi dall’accesso alla vista.
