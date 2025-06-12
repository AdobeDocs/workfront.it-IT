---
title: Ripristina record eliminati
description: È possibile recuperare i record eliminati dall'area Eliminati di recente in Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 1%

---

# Ripristina record eliminati

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

È possibile recuperare i record eliminati dall&#39;area Eliminati di recente in Adobe Workfront Planning.

Per informazioni sull&#39;eliminazione dei record, vedere [Elimina record](/help/quicksilver/planning/records/delete-records.md).

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

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
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p> Standard</p>
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
   <td>   <p>Autorizzazioni Contribute o superiori per un'area di lavoro <span class="preview"> e un tipo di record</span> </a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello layout</p></td> 
   <td> <p>Nell'ambiente di produzione, tutti gli utenti, inclusi gli amministratori di sistema, devono essere assegnati a un modello di layout che includa Planning.</p>
<p><span class="preview">Nell'ambiente di anteprima, per impostazione predefinita, Planning è abilitato per utenti standard e amministratori di sistema.</span></p></td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considerazioni sul recupero dei record eliminati

* I record vengono memorizzati nel contenitore Eliminato di recente per 30 giorni. Dopo 30 giorni, i record vengono eliminati definitivamente da Workfront Planning.
* Se i record eliminati sono collegati ad altri record, i record collegati non vengono eliminati, ma vengono eliminate anche le informazioni del record eliminato. Il ripristino dei record eliminati ripristina le informazioni dai record connessi.
* È possibile ripristinare i record in blocco.
* Quando i record vengono eliminati, le seguenti informazioni vengono memorizzate nel contenitore Eliminato di recente:
   * **Nome**: queste sono le informazioni contenute nel campo Principale del record. Per ulteriori informazioni sui campi primari dei record, vedere [Panoramica sui campi primari](/help/quicksilver/planning/fields/primary-field-overview.md).
   * **Data di eliminazione**: l&#39;ora e la data in cui il record è stato eliminato.
   * **Ora in eliminata di recente**: ora dall&#39;eliminazione del record. I record eliminati più di 30 giorni prima della data corrente non vengono visualizzati nel contenitore Eliminati di recente.
   * **Eliminato da**: nome dell&#39;utente che ha eliminato il record.

## Ripristina record eliminati

1. Passare alla pagina del tipo di record in cui sono stati eliminati i record.
1. Fai clic sull&#39;icona **Annulla** ![Icona Annulla](assets/undo-icon.png) nell&#39;angolo superiore destro di qualsiasi visualizzazione pagina di tipo record, quindi fai clic su **Eliminato di recente**.

   Viene visualizzata la casella **Eliminato di recente**.

   ![Casella eliminata di recente](assets/recently-deleted-box.png)

1. Seleziona i record da eliminare, quindi fai clic su **Ripristina** > **Ripristina**. È possibile selezionare più record.

   Se il ripristino è stato eseguito correttamente, nella parte inferiore della schermata viene visualizzata una notifica di operazione riuscita.
1. Passare alla vista tabella ed esaminare i record ripristinati.
