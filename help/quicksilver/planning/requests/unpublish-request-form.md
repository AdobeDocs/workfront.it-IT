---
title: Annullare la pubblicazione di un modulo di richiesta in Adobe Workfront Planning
description: Puoi annullare la pubblicazione di un modulo di richiesta se non è più necessario o pertinente. Annullando la pubblicazione, verranno rimosse le autorizzazioni di accesso al modulo per tutti gli utenti.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
source-git-commit: f171db8474df703fddbf63a673f9bfbd2ab2db27
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 3%

---

# Annullare la pubblicazione di un modulo di richiesta in Adobe Workfront Planning


<!--take Preview and Production references at Production time-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puoi annullare la pubblicazione di un modulo di richiesta se non è più necessario o pertinente. Annullando la pubblicazione, verranno rimosse le autorizzazioni di accesso al modulo per tutti gli utenti.

È inoltre possibile modificare le entità con cui si condivide un modulo di richiesta, se si desidera mantenerlo disponibile a un gruppo più piccolo di persone.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </td>

<tr>
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td>
   <td>
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p>
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td>
   <td>
   <p>Standard</p>
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
   <ul>
   <li><p>Gestisci le autorizzazioni per un'area di lavoro <span class="preview"> e tipo di record</span> </p></li>
    <li><p>Gli amministratori di sistema possono gestire le aree di lavoro che non hanno creato. </p></li>
    </ul>
   <p>Per informazioni sulle autorizzazioni di condivisione per gli oggetti di Workfront Planning, vedere  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p>  
</td>
  </tr>
 </tbody>
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

## Modificare la condivisione di un modulo di richiesta

Se si condivide una richiesta di accesso pubblica con tutti, inclusi gli utenti esterni all&#39;organizzazione, è possibile limitare l&#39;accesso a determinati utenti che visualizzano o gestiscono l&#39;area di lavoro a cui è associato il modulo.

Per modificare la condivisione di un modulo di richiesta:

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro in cui si desidera aggiungere i record.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record. Per informazioni sulla creazione di un tipo di record, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

   La pagina del tipo di record viene visualizzata nella visualizzazione a cui si è effettuato l&#39;ultimo accesso. Per impostazione predefinita, nella vista tabella viene visualizzata una pagina del tipo di record.

1. Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record nell&#39;intestazione della pagina, quindi fai clic su **Gestisci moduli di richiesta**.

   Tutte le maschere di richiesta associate al tipo di record vengono visualizzate in una vista tabella.
1. Passa il mouse sul nome di un modulo di richiesta, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome, quindi fai clic su **Condividi**.
1. Aggiornare le scelte di condivisione selezionando una delle opzioni seguenti:

   * Chiunque con accesso alla visualizzazione, o superiore, all’area di lavoro
   * Chiunque con accesso per contribuire, o superiore, all’area di lavoro
   * Chiunque abbia il collegamento

   Per ulteriori informazioni, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. (Facoltativo) Se hai modificato la condivisione del modulo di richiesta e desideri condividerlo con il nuovo gruppo di persone con un nuovo collegamento, fai clic su **Copia collegamento**.

## Annullare la pubblicazione di un modulo di richiesta per un tipo di record

Quando un modulo di richiesta diventa irrilevante e non desideri più che qualcuno vi acceda, puoi annullarne la pubblicazione.

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro in cui si desidera aggiungere i record.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record. Per informazioni sulla creazione di un tipo di record, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

   La pagina del tipo di record viene visualizzata nella visualizzazione a cui si è effettuato l&#39;ultimo accesso. Per impostazione predefinita, nella vista tabella viene visualizzata una pagina del tipo di record.

1. Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record nell&#39;intestazione della pagina, quindi fai clic su **Gestisci moduli di richiesta**.

   Tutte le maschere di richiesta associate al tipo di record vengono visualizzate in una vista tabella.
1. Passa il puntatore del mouse sul nome di un modulo di richiesta, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome, quindi fai clic su **Annulla pubblicazione**

Oppure

Fai clic sul nome del modulo di richiesta per aprirlo, quindi fai clic su **Annulla pubblicazione** nell&#39;angolo superiore destro del modulo di richiesta.

![Pulsante Annulla pubblicazione evidenziato](assets/unpublish-button-highlighted.png)

Nella parte inferiore della schermata viene visualizzata una conferma che notifica l’annullamento della pubblicazione del modulo.

Il collegamento o pulsante **Annulla pubblicazione** diventa **Pubblica**.

1. (Condizionale) Se dopo l&#39;apertura del modulo hai annullato la pubblicazione, fai clic su **Salva**.

   Gli utenti non possono più accedere al modulo di richiesta da un collegamento o dalla coda richieste nell’area Richieste di Workfront.

   Tutti i record aggiunti in precedenza utilizzando il modulo di richiesta rimangono nella pagina del tipo di record.

   Tutte le richieste precedentemente aggiunte rimangono nell&#39;area Richieste di Workfront, nella scheda Pianificazione.
