---
title: Modifica tipi di record
description: È possibile modificare i tipi di record dopo il salvataggio. I tipi di record sono i tipi di oggetto di Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 7f24186c8803237a6f5116293b3c6a5fd1ea90f6
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 2%

---


# Modifica tipi di record

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. È possibile modificare l&#39;aspetto dei tipi di record creati dall&#39;utente o da qualsiasi altro utente. Per informazioni sulla creazione di tipi di record di Workfront Planning, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso.

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
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p> Standard </p>
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
   <td>   <p>Gestisci le autorizzazioni per un'area di lavoro <span class="preview"> e tipo di record</span> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
   <p>Solo gli amministratori di sistema possono abilitare i tipi di record alla connessione da altre aree di lavoro</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

## Modifica tipi di record

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera modificare i tipi di record.

   Viene visualizzata la pagina dell&#39;area di lavoro e i tipi di record.
1. Esegui una delle operazioni seguenti:

   * Passa il puntatore del mouse sulla scheda di un tipo di record e fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) nell&#39;angolo superiore destro della scheda del tipo di record, quindi fai clic su **Modifica**
Oppure
   * Fai clic su una scheda del tipo di record per aprire la pagina del tipo di record, fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record, quindi fai clic su **Modifica**.

   ![Altre opzioni di menu dalla scheda del tipo di record](assets/more-menu-options-from-record-type-card.png)

1. Nella casella **Modifica tipo di record**, per impostazione predefinita viene aperta la scheda **Aspetto**.

   ![Modifica la scheda dell&#39;aspetto della casella del tipo di record ](assets/edit-record-type-box-appearance-tab.png)

   Aggiorna le seguenti informazioni nella scheda **Aspetto**:

   * Se necessario, modificare il nome del tipo di record. <!--did they add a field label for this?-->
   * **Descrizione**: modificare o aggiungere una descrizione per il tipo di record con ulteriori informazioni.
   * Modificare il colore e la forma dell&#39;icona associata al tipo di record. Effettua le seguenti operazioni:
      * Selezionare un colore per identificare il tipo di record. Colore dell&#39;icona del tipo di record.
      * Seleziona un’icona dall’elenco, oppure inizia a digitare il nome di un’icona per descrivere ciò che rappresenta, quindi selezionala quando viene visualizzata. Icona del tipo di record. Per impostazione predefinita, viene selezionata un&#39;icona di file.

1. (Condizionale) Se sei un amministratore di sistema, fai clic sulla scheda **Impostazioni avanzate** nella casella **Modifica tipo di record**. <!--the info here is duplicated in the Create record types article-->

   ![Scheda Impostazioni avanzate della casella Modifica tipo di record](assets/edit-record-type-box-advanced-settings-tab.png)

1. (Condizionale) Aggiorna le seguenti informazioni nella scheda **Impostazioni avanzate**:

   * Abilita l&#39;impostazione **Connetti da altra area di lavoro**. Se attivato, il tipo di record è accessibile e può essere connesso da altre aree di lavoro.
   * Scegliere le aree di lavoro da cui è possibile accedere al tipo di record. Scegli una delle seguenti opzioni:

      * **A livello di sistema**: gli utenti possono connettersi a questo tipo di record da tutte le aree di lavoro in cui dispongono di autorizzazioni di gestione.
      * **Aree di lavoro specifiche**: aggiungere i nomi delle aree di lavoro a cui i responsabili area di lavoro possono connettersi a questo tipo di record.

1. Fai clic su **Salva**.

   La scheda del tipo di record nell&#39;area di lavoro visualizza un&#39;icona di connettività ![Connetti da altre aree di lavoro](assets/connect-from-other-workspaces-icon.png) nell&#39;angolo superiore destro per indicare che il record è ora accessibile da altre aree di lavoro.

1. (Facoltativo) Fai clic sulla scheda del tipo di record nell’area di lavoro per aprire la pagina del tipo di record, quindi rinomina il tipo di record nell’intestazione.

1. (Facoltativo) Per modificare un altro tipo di record, dalla pagina tipo di record espandere la freccia rivolta verso il basso a destra del nome di un tipo di record, cercare un tipo di record e selezionarlo quando viene visualizzato nell&#39;elenco.

   ![Elenco a discesa del tipo di record nella pagina del tipo di record con casella di ricerca](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
