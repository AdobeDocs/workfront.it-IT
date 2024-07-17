---
product-area: projects
navigation-topic: manage-issues
title: Sposta i problemi
description: Puoi spostare i problemi tra progetti e attività.
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 6c82c585376b41cff0e57b253b6a214fb00309de
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 1%

---

# Sposta i problemi

È possibile spostare i problemi tra i seguenti oggetti:

* Da un progetto a un altro
* Da un&#39;attività a un&#39;altra attività nello stesso progetto o in un altro progetto
* Da un&#39;attività al progetto o a un altro progetto
* Da un progetto a un&#39;attività nello stesso progetto o a un&#39;attività in un altro progetto

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiedi o superiore</p> <p>Rivedi o ottieni una licenza per spostare i problemi nella sezione Problemi di un progetto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica l'accesso alle Issues</p> <p>Accesso di visualizzazione o superiore ai progetti e alle attività</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni sull'accesso ai problemi nel tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concedere l'accesso ai problemi</a>. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il problema</p> <p>Autorizzazioni di Contribute per l’elemento in cui stai spostando il problema con la possibilità di aggiungere problemi.</p> <p> Per informazioni sulla concessione delle autorizzazioni per i problemi, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema </a></p> <p>Per informazioni sulla richiesta di autorizzazioni aggiuntive, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront.

## Considerazioni sullo spostamento dei problemi

Quando si spostano problemi che contengono documenti o sono associati a una coda di richieste, considera quanto segue:

* **Quando un problema è associato a una coda di richieste:** Quando si sposta un problema in un altro oggetto e il problema è associato a una coda di richieste, il problema spostato non è più associato alla coda originale da cui ha avuto origine il primo problema.
* **Quando un documento è allegato al problema:** Quando si sposta un problema in un altro oggetto a cui è associato un documento, anche il documento, le relative versioni e bozze vengono spostati nel nuovo problema. Eventuali approvazioni associate al documento non vengono spostate.
* **Quando un problema è collegato a un documento o a una cartella:** Quando si sposta un problema che include documenti o cartelle collegati a un servizio di terze parti come Google Drive, i collegamenti ai documenti vengono spostati insieme al problema.

## Sposta i problemi in un elenco

È possibile spostare uno o più problemi da un elenco di problemi o da un report di problemi.

1. Vai al progetto che contiene il problema o i problemi che desideri spostare.

   Oppure

   Passa a un report sui problemi.

1. Se hai selezionato di passare a un progetto, fai clic su **Problemi** nel pannello a sinistra.
1. Seleziona il problema o i problemi da spostare e fai clic sul **menu Altro** nella parte superiore dell&#39;elenco dei problemi, quindi fai clic su **Sposta in**.

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. Continuare con lo spostamento del problema, come descritto nella sezione [Spostare un singolo problema](#move-a-single-issue) a partire dal passaggio 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step stays accurate)
   </MadCap:conditionalText>
   -->

## Spostare un singolo problema {#move-a-single-issue}

È possibile spostare un problema durante la visualizzazione.

### Spostare un singolo problema nell’ambiente di anteprima

1. Vai al problema che desideri copiare, fai clic sul menu **Altro** ![](assets/more-icon.png)a destra del nome del problema, quindi seleziona **Sposta** in.

   ![](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   Viene visualizzata la casella **Sposta problema**.

   ![](assets/move-issue-box-nwe-350x280.png)

1. Nella sezione **Seleziona progetto di destinazione**, specifica il nome del progetto in cui desideri spostare i problemi. Il nome del progetto corrente viene visualizzato per impostazione predefinita.

   >[!TIP]
   >
   >Nell’elenco vengono visualizzati solo 100 progetti.

1. (Condizionale) Se non disponi dell&#39;accesso per spostare i problemi nel progetto, fai clic su **richiedi accesso**.
1. (Facoltativo) Se disponi dell’accesso per aggiungere problemi a una delle attività nel progetto di destinazione, continua a spostare il problema sul progetto di destinazione selezionato senza richiedere l’accesso.

   ![](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >Messaggi simili vengono visualizzati se il progetto selezionato è in attesa di approvazione, completato o inattivo, quando l’amministratore di Workfront impedisce l’aggiunta di problemi a questi progetti. Per ulteriori informazioni, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Facoltativo) Nella sezione **Opzioni**, deseleziona uno degli elementi elencati nella tabella seguente per rimuoverli dal problema spostato. Tutte le opzioni sono selezionate per impostazione predefinita.

   >[!IMPORTANT]
   >
   >Deselezionando gli elementi nell&#39;elenco Opzioni si verifica una perdita di dati. Le informazioni del problema esistente verranno rimosse e non potranno essere recuperate.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Seleziona tutto</td> 
      <td>Deseleziona questa opzione per rimuovere tutte le informazioni dal problema durante lo spostamento nella nuova posizione. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Assegnazioni</td> 
      <td>Rimuove gli utenti, le mansioni o i team assegnati al problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Avanzamento</td> 
      <td>Rimuove l'eventuale percentuale di completamento del problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Documenti</p></td> 
      <td> <p>Rimuove tutti gli elementi presenti nella scheda documenti, incluse le versioni dei documenti, i documenti collegati e le cartelle.

   <b>NOTA</b>

   Se si sceglie di non spostare i documenti con il problema, i documenti verranno eliminati e posizionati nel Cestino per 30 giorni. Un amministratore può ripristinarli e saranno ripristinati al momento dello spostamento del problema.

   Se il problema viene eliminato dopo lo spostamento, i documenti ripristinati verranno inseriti nell&#39;area Documenti della pagina utente dell&#39;amministratore che li ripristina.
   <br> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Autorizzazioni</td> 
      <td>Rimuove le entità con cui è condiviso il problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aggiornamenti</td> 
      <td>Rimuove i commenti dalla sezione Aggiornamenti del problema.</td> 
     </tr> 
    </tbody> 
   </table>


1. (Facoltativo) Nella sezione **Seleziona attività**, seleziona l&#39;attività in cui desideri spostare il problema.
1. Se hai selezionato più problemi in un elenco, fai clic su **Sposta problema** o **Sposta problemi**.

   I problemi spostati vengono aggiunti al progetto specificato.




