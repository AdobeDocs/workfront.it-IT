---
title: Inviare richieste di Adobe Workfront Planning
description: Dopo che un utente ha condiviso un collegamento a un modulo di richiesta da una pagina di tipo di record in Adobe Workfront Planning, è possibile aggiungere una richiesta per la creazione di record per il tipo di record associato al modulo di richiesta.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 1%

---

# Inviare richieste di Adobe Workfront Planning per creare record

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->

{{planning-important-intro}}

Dopo che un utente ha condiviso un collegamento a un modulo di richiesta da una pagina di tipo di record in Adobe Workfront Planning, è possibile aggiungere una richiesta per la creazione di record per il tipo di record associato al modulo di richiesta.

Gli utenti Workfront e gli utenti esterni possono inviare richieste ai tipi di record Planning e creare record. <!--double check on the external users-->

Questo articolo descrive come inviare una richiesta per aggiungere nuovi record a un tipo di record.

Per informazioni su come un manager area di lavoro può creare un modulo di richiesta e associarlo a un tipo di record, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per accedere a Workfront Planning, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Prodotti</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td>
   <td>
<p>Uno dei seguenti piani di Workfront:</p>
<ul><li>Seleziona</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p>
   </td>
<tr>
   <td role="rowheader"><p>Piano di pianificazione Adobe Workfront*</p></td>
   <td>
<p>Qualsiasi </p>  
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </td>
<tr>
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td>
   <td>
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p>
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata di Adobe per Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td>
   <td>
   <p>Licenza Esterna, Collaboratore, Light o Standard</p>
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td>
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td>
   <td>
   <p>Visualizza o autorizzazioni superiori per un’area di lavoro, se sei un utente di Workfront</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>Per accedere all'area Planning in Workfront, è necessario disporre di un modello di layout che includa l'area Planning nel menu principale. </p>
   <p> Tuttavia, per inviare richieste a Workfront Planning non è necessario accedere all'area Planning. </p>  
</td>
  </tr>
 </tbody>
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di inviare una richiesta a un modulo di richiesta Workfront Planning, è necessario disporre dei seguenti elementi:

* In Workfront Planning devono esistere gli elementi seguenti:

   * Un’area di lavoro
   * Tipo di record associato a un modulo di richiesta. Per informazioni, vedere [Creare un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* Il modulo di richiesta deve essere condiviso con un collegamento in modo da potervi accedere. Esistono i seguenti scenari:

   * Se disponi di un account Workfront, il collegamento è stato condiviso solo con persone interne e puoi accedere all’area di lavoro. Gli utenti esterni a Workfront non possono accedere a un collegamento condiviso internamente.
   * Se non disponi di un account Workfront, il collegamento è stato condiviso con persone esterne. Gli utenti di Workfront possono anche accedere a un collegamento condiviso con persone esterne.

* Il collegamento al modulo non deve essere scaduto.

## Considerazioni sull&#39;invio di richieste a Workfront Planning

* Non è possibile accedere ai moduli di richiesta per le richieste di Workfront Planning senza un collegamento specifico ai moduli.
* Una richiesta inviata a Workfront Planning non può essere modificata.
* Ogni richiesta inviata crea un record per il tipo di record associato al modulo utilizzato.
* I record creati con l’invio di moduli di richiesta non possono essere differenziati dai record aggiunti tramite qualsiasi altro metodo. Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).

## Inviare una richiesta a Workfront Planning

1. Passare al collegamento condiviso con l&#39;utente da un tipo di record di Workfront Planning.

1. Aggiorna i campi disponibili nel modulo. I campi con un asterisco sono obbligatori.

   >[!TIP]
   >
   >   Se il campo **Oggetto** di Workfront è disponibile, potrebbe non essere visibile in Workfront Planning. È consigliabile aggiornare il maggior numero possibile di campi nella richiesta per rendere identificabile il nuovo record quando viene aggiunto al tipo di record.

1. Fai clic su **Invia**.

   Il modulo viene inviato e viene aggiunto un nuovo record al tipo di record associato al modulo.





