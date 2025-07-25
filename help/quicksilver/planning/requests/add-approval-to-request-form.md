---
title: Aggiungere un’approvazione a un modulo di richiesta in Adobe Workfront Planning
description: È possibile aggiungere un processo di approvazione a un modulo di richiesta di Adobe Workfront Planning, per avviare un'approvazione per ogni richiesta sottomessa, prima di creare un record.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: 83b3bd73fd30b5fba931e64783dee67485d98fe9
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 1%

---

# Aggiungere un’approvazione a un modulo di richiesta in Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

È possibile aggiungere un processo di approvazione a un modulo di richiesta di Adobe Workfront Planning, per avviare un&#39;approvazione per ogni richiesta sottomessa, prima di creare un record.

Questo articolo descrive come un manager dell&#39;area di lavoro può aggiungere un&#39;approvazione a un modulo di richiesta associato a un tipo di record.

Per informazioni sulla creazione di un modulo di richiesta in Workfront Planning, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Per informazioni sull&#39;invio di una richiesta a un tipo di record per la creazione di un record, vedere [Inviare richieste di Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md).

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

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
<p>Per poter accedere a Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p>
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
   <li><p>Gestire le autorizzazioni per un’area di lavoro e un tipo di record</p></li>
    <li><p>Gli amministratori di sistema possono gestire le aree di lavoro che non hanno creato. </p></li>
    </ul>
   <p>Per informazioni sulle autorizzazioni di condivisione per gli oggetti di Workfront Planning, vedere  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning</a> 
  </td>
  </tr>

</tbody>
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sull’aggiunta di approvazioni a un modulo di richiesta

* È possibile aggiungere uno o più approvatori a un modulo di richiesta. È possibile aggiungere solo utenti come approvatori.
* <span class="preview">È possibile visualizzare le informazioni sull&#39;approvazione in un record creato inviando un modulo di richiesta nei campi Approvato da e Data approvata. Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).</span>
* Quando si aggiungono più approvatori a un modulo di richiesta, tutti gli approvatori devono accettare la richiesta prima di creare un record in Workfront Planning.
* Se tutti gli approvatori approvano la richiesta, viene creato un record per il tipo di record associato al modulo di richiesta.
* Se almeno un approvatore rifiuta la richiesta e tutti gli altri la approvano, viene creata una richiesta per l&#39;area Richieste di Workfront, ma non viene creato alcun record per il tipo di record associato al modulo di richiesta.
* L’aggiunta di approvazioni a un modulo di richiesta è facoltativa. Workfront Planning crea immediatamente un record quando viene sottomessa una richiesta, se il modulo di richiesta non è associato a un&#39;approvazione.

## Aggiungere un’approvazione a un modulo di richiesta

1. Iniziare a creare un modulo di richiesta per un tipo di record, come descritto in [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Fare clic su **Configurazione**.

   Viene visualizzata l&#39;area **Configurazione**.

   ![Scheda Configurazione](assets/configuration-tab.png)
1. Nel campo **Approvatori**, fai clic sull&#39;icona a discesa e seleziona uno o più utenti <span class="preview">o team</span> nell&#39;elenco

   Oppure

   Inizia a digitare il nome di un utente <span class="preview">o team</span> che desideri impostare come approvatore, quindi selezionalo quando viene visualizzato nell&#39;elenco.

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* Puoi aggiungere uno o più approvatori a un modulo di richiesta.
   >
   >* Se si aggiungono più approvatori, tutti gli approvatori devono approvare la richiesta prima che Workfront Planning crei un record.
   >
   >* Se almeno un approvatore rifiuta la richiesta, la richiesta viene rifiutata e il record non viene creato. La richiesta rimane nella scheda Pianificazione della sezione Inviata nell&#39;area Richieste di Workfront.
   >
   >* Tutti gli approvatori devono prendere una decisione prima che una richiesta venga approvata o rifiutata.
   >
   >* <span class="preview">Se un team è impostato come approvatore, è necessaria una sola decisione del team.</span>


1. (Facoltativo) Fai clic su **Pubblica** se non hai mai condiviso il modulo di richiesta in precedenza

   Oppure

   Fai clic su **Condividi** per condividere il modulo, quindi su **Copia collegamento**.
1. (Facoltativo) Dopo che un utente utilizza il collegamento condiviso e invia una richiesta, Workfront Planning invia una notifica in-app di approvazione e un messaggio e-mail agli approvatori.

   >[!NOTE]
   >
   >   Per consentire agli utenti di ricevere notifiche e-mail e in-app, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.


   Per informazioni sull&#39;approvazione delle richieste, vedere [Approvare una richiesta](/help/quicksilver/planning/requests/approve-request.md).
