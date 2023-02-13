---
product-area: projects
navigation-topic: manage-issues
title: Sposta i problemi
description: È possibile spostare i problemi tra progetti e attività.
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 6c82c585376b41cff0e57b253b6a214fb00309de
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 1%

---

# Sposta i problemi

È possibile spostare i problemi tra i seguenti oggetti:

* Da un progetto a un altro progetto
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
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> <p>Rivedi o una licenza superiore per spostare i problemi nella sezione Problemi di un progetto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai problemi</p> <p>Visualizza o consente un accesso più elevato a progetti e attività</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni sull'accesso ai problemi relativi al livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concedere l’accesso ai problemi</a>. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni al problema</p> <p>Autorizzazioni di Contribute per l'elemento in cui si sta spostando il problema con la possibilità di aggiungere problemi.</p> <p> Per informazioni sulla concessione delle autorizzazioni per i problemi, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema </a></p> <p>Per informazioni sulla richiesta di autorizzazioni aggiuntive, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Considerazioni sullo spostamento dei problemi

Quando si spostano problemi che contengono documenti o sono associati a una coda di richiesta, considera quanto segue:

* **Quando un problema è associato a una coda di richieste:** Quando si sposta un problema in un altro oggetto e il problema è associato a una coda di richiesta, il problema spostato non è più associato alla coda originale da cui è nato il primo problema.
* **Quando un documento è allegato al problema:** Quando si sposta un problema in un altro oggetto e al problema è allegato un documento, il documento, le sue versioni e prove passano al nuovo problema. Le approvazioni associate al documento non vengono spostate.
* **Quando un problema è collegato a un documento o a una cartella:** Quando si sposta un problema che include documenti o cartelle collegati a un servizio di terze parti come Google Drive, i collegamenti ai documenti si spostano con il problema.

## Spostare i problemi in un elenco

È possibile spostare uno o più problemi da un elenco di problemi o da un report di problemi.

1. Passa al progetto contenente il problema o i problemi da spostare.

   Oppure

   Passa a un rapporto del problema.

1. Se hai selezionato di passare a un progetto, fai clic su **Problemi** nel pannello a sinistra.
1. Seleziona il problema o i problemi da spostare e fai clic sul pulsante **Menu Altro** in alto nell&#39;elenco dei problemi, quindi fai clic su **Sposta a**.

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. Continua a spostare il problema, come descritto nella sezione . [Spostare un singolo problema](#move-a-single-issue) a partire dal passaggio 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step stays accurate)
   </MadCap:conditionalText>
   -->

## Spostare un singolo problema {#move-a-single-issue}

È possibile spostare un problema quando lo si visualizza.

### Spostare un singolo problema nell&#39;ambiente Preview

1. Passa a un problema da copiare e fai clic sul pulsante **Altro** menu ![](assets/more-icon.png)a destra del nome del problema, quindi seleziona **Sposta** a.

   ![](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   La **Problema di spostamento** viene visualizzata la casella .

   ![](assets/move-issue-box-nwe-350x280.png)

1. In **Seleziona progetto di destinazione** Specifica il nome del progetto in cui desideri spostare i problemi. Per impostazione predefinita viene visualizzato il nome del progetto corrente.

   >[!TIP]
   >
   >Nell’elenco vengono visualizzati solo 100 progetti.

1. (Condizionale) Fai clic su **richiesta di accesso** se non hai accesso per spostare i problemi nel progetto.
1. (Condizionale) Continua a spostare il problema sul progetto di destinazione selezionato senza richiedere l’accesso se hai accesso per aggiungere problemi a una delle attività del progetto di destinazione.

   ![](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >Messaggi simili vengono visualizzati se il progetto selezionato è in attesa di approvazione, completato o disattivato, quando l’amministratore di Workfront impedisce l’aggiunta di problemi a tali progetti. Per ulteriori informazioni, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Facoltativo) In **Opzioni** deseleziona uno degli elementi elencati nella tabella seguente per rimuoverli dal problema spostato. Tutte le opzioni sono selezionate per impostazione predefinita.

   >[!IMPORTANT]
   >
   >Deselezionando gli elementi nell&#39;elenco Opzioni si verifica una perdita di dati. Le informazioni del problema esistente verranno rimosse e non possono essere recuperate.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Seleziona tutto</td> 
      <td>Deseleziona questa opzione per rimuovere tutte le informazioni dal problema quando lo si sposta nella nuova posizione. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Assegnazioni</td> 
      <td>Rimuove utenti, ruoli o team assegnati al problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Avanzamento</td> 
      <td>Rimuove l’eventuale percentuale di completamento del problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Documenti</p></td> 
      <td> <p>Rimuove tutti gli elementi presenti nella scheda documenti, incluse le versioni del documento, i documenti collegati e le cartelle.

   <b>NOTA</b>

   Se si sceglie di non spostare i documenti con il problema, i documenti verranno eliminati e inseriti nel Cestino per 30 giorni. Un amministratore può ripristinarli e ripristinarli sul problema spostato.

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


1. (Facoltativo) In **Seleziona attività** selezionare l&#39;attività in cui si desidera spostare il problema.
1. Fai clic su **Sposta problema** o **Problemi di spostamento**, se hai selezionato più problemi in un elenco.

   I problemi spostati vengono aggiunti al progetto specificato.




