---
title: Personalizzare la Home utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Puoi utilizzare un modello di layout per configurare ciò che gli utenti visualizzano all’apertura della pagina Home in Adobe Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: 1e69d715f343bfef1e5aee658a1dff12abfc61a0
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 1%

---

# Personalizzare la Home utilizzando un modello di layout

È possibile utilizzare un modello di layout per configurare gli elementi visualizzati dagli utenti la prima volta che aprono Home.

Puoi configurare:

* Quali widget vengono visualizzati nell’area di lavoro per impostazione predefinita
* Quale sfondo è selezionato
* Impostazioni specifiche dei widget, inclusi i filtri e i gruppi disponibili per i widget Progetti personali, Attività personali e Problemi personali, nonché i relativi valori predefiniti

>[!IMPORTANT]
>
>Gli utenti finali possono modificare lo sfondo e riordinare i widget sulla pagina dopo l’applicazione del modello di layout. Non sono in grado di rimuovere i widget inclusi da un amministratore Workfront.
> 
>Gli amministratori possono aggiungere nuovi widget per gli utenti. Tuttavia, se un utente finale ha già personalizzato l’ordine dei widget o la selezione di sfondo, tali personalizzazioni specifiche non vengono modificate.

Per informazioni sulla Home, vedere [Introduzione alla Home](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

Per informazioni sulla creazione di modelli di layout, vedere [Creare e gestire modelli di layout](../use-layout-templates/create-and-manage-layout-templates.md).

Per informazioni sui modelli di layout per i gruppi, vedere [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Dopo aver configurato un modello di layout, è necessario assegnarlo agli utenti affinché le modifiche apportate siano visibili agli altri utenti. Per informazioni sull&#39;assegnazione di un modello di layout agli utenti, vedere [Assegnare gli utenti a un modello di layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td><p>Nuovo: Standard</p>
  <p> Corrente: Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.
Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizza la Home utilizzando un modello di layout

Per personalizzare la Home tramite un modello di layout:

1. Iniziare a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Fai clic sulla freccia giù ![](assets/dropdown-arrow.png) in **Personalizza gli elementi visualizzati dagli utenti**, quindi fai clic su **Home Workspace**.

1. Nelle schede a destra, fare clic su una delle opzioni seguenti:

   * **Progettazione e layout**: selezionare per scegliere e disporre i widget e lo sfondo
   * **Impostazioni widget**: selezionare questa opzione per gestire le impostazioni per i singoli widget, ad esempio i filtri e i gruppi disponibili.

   Nella tabella seguente sono riportati i dettagli di ogni scheda:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Progettazione e layout</td> 
      <td>
      <p>Selezionate i widget da visualizzare nelle aree di lavoro degli utenti, la loro posizione e scegliete uno sfondo.</p> 
      <p>Gli utenti non possono rimuovere i widget selezionati, ma possono spostarli e ridimensionarli liberamente. Possono anche aggiungere altri widget.</p>
      <p>Questa scheda funziona essenzialmente come un’anteprima dell’area di lavoro Home effettiva che gli utenti con questo modello di layout sperimenteranno.</p> 
      <p> Effettua una delle seguenti operazioni: </p>
      <ul><li>Personalizzare questa scheda in base ai passaggi descritti in <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Aggiungere, modificare o rimuovere widget nella Home</a>. </li>
      <li>Selezionate i widget e disponete l'area di lavoro come desiderate che appaia per gli utenti.</li>
      <li>Per modificare lo sfondo, seguire i passaggi descritti in <b>Personalizzazione in background</b> in <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref">Introduzione alla Home</a>.</li></p>
      <p>

   >[!NOTE]
   >
   >Solo lo spostamento o il ridimensionamento dei widget nel modello di layout non attiverà le home page degli utenti per aggiornare il layout. Tuttavia, l’aggiunta o la rimozione di un widget attiverà un aggiornamento delle pagine degli utenti.

   </p>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Impostazioni widget</td> 
      <td>
      <p>Modificare le impostazioni per i singoli widget.</p> 
      <p>

   >[!NOTE]
   >
   >Queste opzioni non si estendono al pannello Riepilogo. È necessario configurare tale area nella scheda Riepilogo del modello di layout.

   </p>
      <p> Selezionate uno dei seguenti widget dall'elenco a sinistra:</p>
      <ul>
        <li>I miei progetti</li>
        <li>Le mie attività</li>
        <li>I miei problemi</li>
      </ul>
      <p>Dopo aver selezionato il widget da modificare, seleziona i <b>Filtri</b>, <b>Colonne</b> e <b>Gruppi</b> che desideri rendere disponibili per la Home a destra.</p>
      <p> È possibile:</p>
      <ul>
      <li><p>Seleziona e ordina i Filtri, le Colonne o i Gruppi disponibili per gli utenti selezionando la casella accanto alle opzioni nell’elenco. Le opzioni non selezionate non vengono visualizzate per gli utenti.</p></li>
      <li> <p>Trascina le opzioni nell’elenco per impostare un ordine.</p></li>
      <p>

   >[!IMPORTANT]
   >
   >* Le opzioni Filtro, Colonne e Gruppo sono collegate alle opzioni di personalizzazione elenco nel modello di layout. Le modifiche apportate qui verranno applicate anche a queste impostazioni.
   >* Gli utenti devono disporre almeno dell&#39;accesso Crea alle visualizzazioni per consentire la corretta applicazione della configurazione della colonna Amministratore alle proprie home page.

   </p>
      <li><p>Impostare un filtro o un gruppo predefinito per il widget passando il mouse su un'opzione e facendo clic su <b>Imposta come predefinito</b>. Il valore predefinito corrente visualizza un contrassegno blu <b>Predefinito</b> a destra.</p></li>
      <li><p>Aggiungere un filtro, una colonna o un gruppo esistente all'elenco delle opzioni disponibili facendo clic sul pulsante del segno più nella parte inferiore di ogni elenco per aggiungere un'opzione all'elenco. Solo i filtri, i campi (per le colonne) o i gruppi esistenti possono essere aggiunti in questo modo.</p></li>
      </ul>
      <p>

   >[!NOTE]
   >
   >Se impostate un filtro o un raggruppamento predefinito per un widget specifico utilizzando un modello di layout, potrebbe non avere effetto immediato a causa delle preferenze utente esistenti. Per applicare immediatamente il nuovo filtro o raggruppamento, è possibile che tu o l’utente debba reimpostare le preferenze utente aggiungendo &quot;/resetUser&quot; alla fine dell’URL.

   </p>
      </td> 
      </tr>
      </tbody> 
      </table>

1. Continuate a personalizzare il modello di layout.

   Oppure

   Se hai completato la personalizzazione, fai clic su **Salva** nell&#39;angolo in basso a sinistra.

   >[!IMPORTANT]
   >
   >Gli utenti devono aggiornare la home page per visualizzare le personalizzazioni dal modello di layout.
