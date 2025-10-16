---
product-area: reporting
navigation-topic: reporting-elements
title: Utilizzare la formattazione condizionale nelle visualizzazioni
description: Quando condividi i tuoi rapporti con altri utenti in Adobe Workfront, prendi in considerazione la possibilità di personalizzare la visualizzazione dei rapporti per semplificare la lettura di determinate informazioni o distinguerti facilmente.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 3%

---

# Utilizzare la formattazione condizionale nelle visualizzazioni

<!-- Audited: 11/2024 -->

Quando condividi i tuoi rapporti con altri utenti in Adobe Workfront, prendi in considerazione la possibilità di personalizzare la visualizzazione dei rapporti per semplificare la lettura di determinate informazioni o distinguerti facilmente.

È possibile personalizzare la scheda Dettagli dei rapporti aggiungendo formattazione speciale o condizionale alla visualizzazione dei rapporti.

Per ulteriori informazioni sulla creazione di report, vedere l&#39;articolo [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Formattando le colonne in modo condizionale nella visualizzazione del rapporto, è possibile impostare regole che influiscono sulla modalità di visualizzazione del rapporto. Quando tali condizioni o regole vengono soddisfatte, viene applicata la formattazione speciale.

Se ad esempio la percentuale di completamento di un&#39;attività è inferiore al 20%, è possibile evidenziare il campo visualizzando il numero in grassetto, in rosso e con un colore di sfondo giallo.

Con una vista con formattazione condizionale è possibile:

* Modifica l’intestazione di una colonna.
* Modificate il valore di una colonna in testo personalizzato o immagine.
* Formattare la visualizzazione di un campo modificando il tipo di carattere, il colore, l&#39;allineamento o il colore dello sfondo.

Le modifiche apportate nella visualizzazione del report hanno effetto solo nella scheda Dettagli del report. Queste modifiche non influiscono sulle schede Riepilogo, Matrice o Grafico del rapporto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</strong></td> 
   <td> 
    <p>Standard o piano per le visualizzazioni dei rapporti</p>
    <p>Collaboratori o richieste di visualizzazioni elenco</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare una visualizzazione in un rapporto</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
    <td> <p>Gestire le autorizzazioni per un report per creare o modificare una visualizzazione in un report</p> <p>Gestire le autorizzazioni per una visualizzazione</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

È necessario creare un report prima di aggiungere la formattazione condizionale alla relativa visualizzazione.

Per informazioni sulla creazione di un report, vedere [Creare un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Creare una vista con formattazione condizionale

{{step1-to-reports}}

1. Fare clic sul nome di un report in cui si desidera creare una visualizzazione con formattazione condizionale

   Oppure

   Fai clic su **Nuovo report**, quindi seleziona un tipo di oggetto per generare un nuovo report.

1. (Condizionale) Se modifichi un rapporto esistente, fai clic su **Azioni rapporto**, quindi su **Modifica**.

1. Nella scheda **Colonne (Visualizzazione)**, fare clic per selezionare una colonna esistente oppure fare clic su **Aggiungi colonna** per creare una colonna.
1. Nel campo **Mostra in questa colonna** nell&#39;angolo superiore sinistro del Report Builder, selezionare il campo che si desidera visualizzare nella nuova colonna.
1. Fare clic su **Opzioni avanzate**.

1. Specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Etichetta colonna personalizzata</strong></td> 
      <td> <p>Specificare un nome per la colonna.</p> <p>Se si sta modificando una colonna esistente, specificando un nome si modifica anche il nome della colonna esistente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formato campo</strong></td> 
      <td>Scegli il formato in cui viene visualizzato il valore nella colonna. A seconda del campo colonna, questo consente di impostare la visualizzazione di date, numeri o valuta. Questa opzione non è visualizzata in tutte le colonne.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostra questa colonna quando in un dashboard</strong></td> 
      <td>Seleziona questo campo se desideri che la colonna venga visualizzata quando il rapporto viene inserito in un dashboard. La colonna viene sempre visualizzata quando si esamina il rapporto all’esterno di un dashboard.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Aggiungi una regola per la colonna**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. Nella sezione **When:**, impostare un&#39;istruzione di condizione per la colonna.

   Ad esempio: &quot;quando la percentuale di completamento dell&#39;attività è uguale a (distinzione maiuscole/minuscole) 50&quot;.
1. Nella sezione **Mostra il campo come:** specificare l&#39;aspetto del campo quando viene soddisfatta la condizione definita sopra.

   Specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Colore testo</strong></td> 
      <td> <p>Selezionare il colore in cui il testo viene visualizzato utilizzando il selettore colore.</p> <p><b>NOTA</b></p> <p> Se il campo contiene un collegamento ipertestuale, le selezioni del colore del testo non vengono applicate al campo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formato testo</strong></td> 
      <td>Seleziona se visualizzare il testo in grassetto o corsivo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Allineamento testo</strong></td> 
      <td>Selezionare se allineare il testo a destra, al centro o a sinistra all'interno della colonna.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Informazioni di base</strong></td> 
      <td>Selezionare il colore dello sfondo per il testo utilizzando il selettore colore.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostra icona</strong></td> 
      <td>Se desideri visualizzare un’icona invece del valore effettivo di questa colonna, selezionala da una delle 16 icone.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostra testo</strong></td> 
      <td> <p>Selezionare questa opzione per visualizzare un'etichetta personalizzata per la colonna anziché il valore effettivo. Specifica il testo da visualizzare al posto del valore nel campo fornito.</p> <p><b>IMPORTANTE</b></p> <p>Se si seleziona <strong>Mostra testo</strong>, non sarà possibile modificare il testo in linea in questa colonna.<br>Inoltre, non è possibile modificare il valore di una colonna Predecessore perché contiene una logica incorporata.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Applica a tutta la riga</strong></td> 
      <td>Selezionare questa opzione per applicare le impostazioni all'intera riga anziché alla sola colonna selezionata.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Aggiungi regola**.\
   Puoi aggiungere altre regole alla stessa colonna o ad altre colonne.

   Le regole vengono applicate nell&#39;ordine in cui sono state create. Sono combinate ma non si sovrascrivono a vicenda, anche se una regola di colonna ha la precedenza su una regola di riga sulla stessa cella.

   **ESEMPIO 1**

   Innanzitutto, puoi creare una regola in cui si specifichi che quando un progetto è nello Stato di creazione, il colore del testo è viola e grassetto. Viene quindi creata una seconda regola che indica che quando il nome di un&#39;attività non è vuoto, il colore del testo è rosso e corsivo e il colore di sfondo è verde. In questo esempio si verifica quanto segue:

   * Le attività di cui viene generato lo stato del progetto vengono visualizzate in viola e grassetto. Se il nome dell&#39;attività non è vuoto, le attività hanno anche uno sfondo verde.
   * Le attività il cui Stato progetto è diverso da Creazione (e il cui Nome attività non è vuoto) vengono visualizzate in un testo rosso e in corsivo con uno sfondo verde.

   **ESEMPIO 2**

   Creare nella colonna Data di completamento pianificata del progetto una regola che influisca sull&#39;intera riga, rendendo grigio lo sfondo se il progetto viene annullato, ad esempio quando lo stato del progetto è Inattivo. Quindi crea una regola di colonna che attivi lo sfondo in rosso quando la Data di completamento pianificata del progetto è inferiore a oggi (ovvero il progetto è in ritardo). In questo esempio, se un progetto annullato presenta una data di completamento in ritardo, tale cella verrà visualizzata in rosso anche se le altre celle nella riga sono grigie. Per correggere questa formattazione:

   * Modifica la formattazione per Data di completamento pianificata ed elimina la regola di colonna per lo sfondo rosso sui progetti in ritardo.
   * Aggiungi una regola di colonna con la stessa formattazione della regola di riga (sfondo grigio quando Stato progetto = Inattivo).
   * Aggiungi nuovamente la regola di colonna per lo sfondo rosso nei progetti in ritardo.
   * Quando salvi le regole e la visualizzazione, lo sfondo rosso non viene applicato a un progetto annullato.

1. Fai clic su **Salva**.
1. Fai clic su **Salva e Chiudi**.\
   Nel report, gli utenti visualizzano le modifiche al formato se sono state soddisfatte le condizioni specificate.
