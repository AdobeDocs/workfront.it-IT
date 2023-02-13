---
product-area: projects
navigation-topic: manage-projects
title: Richiedi tempo per l’approvazione di un progetto
description: Richiedi tempo per l’approvazione di un progetto
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Richiedi tempo per l’approvazione di un progetto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN A TOOLTIP IN THE EDIT PROJECT MODAL) </p>
-->

Puoi configurare il progetto in modo che le ore registrate rispetto al progetto vengano approvate dal proprietario del progetto. Una volta configurate in questo modo, le ore devono essere approvate dal proprietario del progetto prima di poter essere utilizzate in un record di fatturazione.\
Per ulteriori informazioni sui record di fatturazione, consulta l’articolo [Creazione di record di fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>L&#39;abilitazione di questa opzione non rimuove la capacità di un approvatore della scheda attività di approvare il tempo sulla scheda attività. Se il proprietario del progetto non approva o rifiuta il tempo, un approvatore della scheda attività può comunque approvare l&#39;ora in una scheda attività.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Pianificare l'approvazione del progetto per richiedere tempo</p>
   <p>Rivedi o versione successiva per approvare le ore di accesso a un progetto</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Progetti o versioni successive</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza autorizzazioni per il progetto o versioni successive</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Accesso aggiuntivo</td> 
   <td> <p>Per approvare il tempo di un progetto, è necessario soddisfare almeno una delle seguenti condizioni:</p> 
    <ul> 
     <li>Sei il proprietario del progetto con l’accesso e le autorizzazioni specificate sopra. In questo caso, puoi effettuare le seguenti operazioni se esiste una delle condizioni seguenti: 
      <ul>
       <li>Se disponi delle autorizzazioni di gestione per il progetto, puoi approvare o rifiutare le ore di accesso al progetto da parte di qualsiasi altro utente.</li>
       <li> Se disponete dell'accesso a Contribute o View per il progetto, potrete approvare o rifiutare solo le ore registrate dall'utente o da qualsiasi altro utente che effettua il reporting.<br></li>
      </ul></li> 
     <li>Hai una licenza Plan con accesso amministrativo a Timesheets &amp; Hours. In questo caso:
      <ul>
       <li>Puoi approvare o rifiutare qualsiasi ora relativa ai progetti per i quali disponi almeno delle autorizzazioni di visualizzazione. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Richiedi tempo per l’approvazione di un progetto

Per richiedere l&#39;approvazione del project manager per ore sul progetto:

1. Passa al progetto in cui desideri richiedere l’approvazione per ore.
1. Fai clic sul pulsante **Altro** icona ![](assets/more-icon.png) a destra del nome del progetto, quindi fai clic su **Modifica**.\
   Viene visualizzata la finestra di dialogo Modifica progetto.

1. In **Impostazioni progetto** sezione , seleziona **Richiedi tempo per l&#39;approvazione del progetto**.
1. Fai clic su **Salva**.\
   Ora, quando l&#39;ora viene registrata e approvata, queste ore vengono bloccate e non possono essere modificate dall&#39;utente che le ha inserite nel progetto o nella scheda attività. Solo un amministratore Workfront può regolare l&#39;ora registrata.

## Approvare e rifiutare il tempo di un progetto

In qualità di project manager, puoi approvare o rifiutare le ore registrate per attività, problemi o progetti.

L&#39;approvazione delle ore a livello di progetto non ha alcun impatto sulla scheda attività di nessuno degli utenti che hanno registrato le ore. Ad esempio, le ore nel progetto possono essere approvate dal project manager, ma la scheda attività deve ancora essere approvata dal responsabile dell&#39;utente o dall&#39;approvatore della scheda attività. 

Se si imposta un progetto per richiedere l’approvazione nelle ore registrate, il project manager deve approvare le ore affinché siano disponibili per essere incluse in un record di fatturazione per il progetto. Per ulteriori informazioni sulla creazione di record di fatturazione, consulta l’articolo [Creazione di record di fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md).

Per approvare o rifiutare le ore in un progetto:

1. Vai al progetto.
1. Fai clic sul pulsante **Ore** nel pannello a sinistra. Questo potrebbe essere situato sotto **Mostra altro** area.

1. Le ore registrate per problemi, attività e visualizzazione del progetto e devono avere lo stato **Inviato**.\
   Fai clic sulla casella a sinistra delle voci dell’ora per selezionare le ore da approvare.

1. Fai clic su **Approva**.\
   Lo stato delle ore cambia in **Approvato**.\
   Se in seguito si rifiutano le ore approvate, lo stato delle ore cambia in **Non approvato**.\
   Quando si includono le ore approvate in un record di fatturazione, lo stato delle ore cambia in **Fatturato e approvato**. Impossibile eliminare le ore aggiunte a un record di fatturazione. Per ulteriori informazioni sulla creazione di record di fatturazione, consulta l’articolo [Creazione di record di fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md)

1. (Facoltativo) Fai clic su **Rifiuta** per rifiutare le voci temporali nel progetto.\
   Lo stato delle ore cambia in **Rifiutato**.
