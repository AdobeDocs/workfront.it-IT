---
title: Personalizzare la nuova Home utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: È possibile utilizzare un modello di layout per configurare ciò che gli utenti visualizzano quando aprono una nuova Home.
author: Nolan
feature: System Setup and Administration
role: Admin
source-git-commit: ac70fc3564273ef7865de2ae4ca704bb7f61af70
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 1%

---

# Personalizzare la nuova Home utilizzando un modello di layout

È possibile utilizzare un modello di layout per configurare ciò che gli utenti visualizzano quando aprono una nuova Home.

Puoi configurare:

* Quali widget vengono visualizzati nell’area di lavoro per impostazione predefinita e il relativo layout nella pagina
* Quale sfondo è selezionato
* Impostazioni specifiche dei widget, inclusi i filtri e i gruppi disponibili per i widget Progetti personali, Attività personali e Problemi personali, nonché i relativi valori predefiniti

>[!IMPORTANT]
>
>Le scelte del modello di layout amministratore descritte in questa pagina hanno la precedenza sulle scelte di personalizzazione dei singoli utenti.
>
>Quando si salvano le modifiche apportate a un modello di layout, la nuova home page degli utenti di tale modello viene modificata in modo da corrispondere al modello di layout e le selezioni di widget esistenti vengono spostate nella parte inferiore della pagina. I widget selezionati dall’amministratore possono essere riposizionati e ridimensionati da un utente, ma non possono essere rimossi.

Per informazioni sulla nuova Home, consulta [Introduzione alla nuova home](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

Per informazioni sulla creazione di modelli di layout, vedere [Creare e gestire modelli di layout](../use-layout-templates/create-and-manage-layout-templates.md).

Per informazioni sui modelli di layout per i gruppi, vedere [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Dopo aver configurato un modello di layout, è necessario assegnarlo agli utenti affinché le modifiche apportate siano visibili agli altri utenti. Per informazioni sull&#39;assegnazione di un modello di layout agli utenti, vedere [Assegnare utenti a un modello di layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisiti di accesso

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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.
Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizzare la nuova Home utilizzando un modello di layout

1. Iniziare a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Fare clic sulla freccia giù ![](assets/dropdown-arrow.png) in **Personalizzare gli elementi visualizzati dagli utenti**, quindi fai clic su **Area di lavoro Home**.

1. Nelle schede visualizzate a destra, fare clic su **Progettazione e layout** per scegliere e disporre i widget e lo sfondo, oppure **Impostazioni widget** per gestire le impostazioni per i singoli widget, ad esempio i filtri e i gruppi disponibili.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Progettazione e layout</td> 
      <td>
      <p>Selezionate i widget che saranno presenti nelle aree di lavoro degli utenti, la loro posizione e scegliete uno sfondo. Gli utenti non possono rimuovere i widget selezionati, ma possono spostarli e ridimensionarli liberamente e aggiungere altri widget.</p>
      <p>Questa scheda funziona essenzialmente come una nuova piccola area di lavoro Home; in quanto tale, può essere personalizzata in base ai passaggi descritti in <a href="/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Aggiungere, modificare o rimuovere widget nella nuova Home</a>. Selezionate i widget e disponete l'area di lavoro come desiderate che appaia per gli utenti.</p>
      <p>Per modificare lo sfondo, segui i passaggi descritti in <b>Personalizzazione dello sfondo</b> in <a href="/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md" class="MCXref xref">Introduzione alla nuova home</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Impostazioni widget</td> 
      <td>
      <p>Modificare le impostazioni per i singoli widget. Attualmente sono supportati solo tre widget:</p>
      <ul>
        <li>I miei progetti</li>
        <li>Le mie attività</li>
        <li>I miei problemi</li>
      </ul>
      <p>Dopo aver selezionato il widget da modificare, le opzioni disponibili vengono visualizzate a destra. Attualmente, queste opzioni sono <b>Filtri</b> e <b>Gruppi</b>. È possibile:</p>
      <ul>
        <li><b>Seleziona i Filtri o Gruppi che saranno disponibili per gli utenti:</b><p>Seleziona la casella accanto a tutte le opzioni nell’elenco che desideri possano essere utilizzate dagli utenti. Le opzioni non selezionate non vengono visualizzate per gli utenti.</li></p>
        <li><b>Impostate un filtro o un gruppo predefinito per il widget:</b><p>Passa il puntatore del mouse su un’opzione e viene visualizzato un pulsante che consente di impostare tale opzione come predefinita per gli utenti. Il valore predefinito corrente presenta un contrassegno predefinito blu a destra.</li></p>
        <li><b>Aggiungi un filtro o un gruppo esistente all’elenco delle opzioni disponibili:</b><p>Fare clic sul pulsante con il segno più nella parte inferiore di ogni elenco per aggiungere un'opzione all'elenco. Solo i filtri o i gruppi esistenti possono essere aggiunti in questo modo.</li></p>
      </ul>
      </td> 
     </tr>
    </tbody> 
   </table>

1. Continuate a personalizzare il modello di layout.

   Oppure

   Se hai finito di personalizzare, fai clic su **Salva** nell’angolo in basso a sinistra.
