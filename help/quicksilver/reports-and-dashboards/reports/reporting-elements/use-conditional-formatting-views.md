---
product-area: reporting
navigation-topic: reporting-elements
title: Utilizzare la formattazione condizionale nelle visualizzazioni
description: Quando condividi i tuoi rapporti con altri utenti in Adobe Workfront, prendi in considerazione la possibilità di personalizzare la visualizzazione dei rapporti per semplificare la lettura di determinate informazioni o distinguerti facilmente.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1220'
ht-degree: 3%

---

# Utilizzare la formattazione condizionale nelle visualizzazioni

<!--Audited: 01/2024-->

Quando condividi i tuoi rapporti con altri utenti in Adobe Workfront, prendi in considerazione la possibilità di personalizzare la visualizzazione dei rapporti per semplificare la lettura di determinate informazioni o distinguerti facilmente.

È possibile personalizzare la scheda Dettagli dei rapporti aggiungendo formattazione speciale o condizionale alla visualizzazione dei rapporti.

Per ulteriori informazioni sulla creazione di rapporti, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Formattando le colonne in modo condizionale nella visualizzazione del rapporto, è possibile impostare regole che influiscono sulla modalità di visualizzazione del rapporto. Quando tali condizioni o regole vengono soddisfatte, viene applicata la formattazione speciale.

Se ad esempio la percentuale di completamento di un&#39;attività è inferiore al 20%, è possibile evidenziare il campo visualizzando il numero in grassetto, in rosso e con un colore di sfondo giallo.

Con una vista con formattazione condizionale è possibile:

* Modifica l’intestazione di una colonna.
* Modificate il valore di una colonna in testo personalizzato o immagine.
* Formattare la visualizzazione di un campo modificando il tipo di carattere, il colore, l&#39;allineamento o il colore dello sfondo.

Le modifiche apportate nella visualizzazione del report hanno effetto solo nella scheda Dettagli del report. Queste modifiche non influiscono sulle schede Riepilogo, Matrice o Grafico del rapporto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Nuovo:</p> 
   <ul><li>Standard per le visualizzazioni di report</li>
  <li> Collaboratore o versione successiva per le visualizzazioni elenco</li></ul>

<p>Corrente:</p>
   <ul>
    <li> Pianificare le visualizzazioni dei rapporti </li>
    <li> Richiedi o superiore per le visualizzazioni elenco </li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare una visualizzazione in un rapporto</p> <p><b>NOTA</b></p> <p>Se non disponi dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Gestire le autorizzazioni per un report per creare o modificare una visualizzazione in un report</p> <p>Gestire le autorizzazioni per una visualizzazione</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

+++

## Prerequisiti

È necessario creare un report prima di aggiungere la formattazione condizionale alla relativa visualizzazione.

Per informazioni sulla creazione di un rapporto, consulta [Creare un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Creare una vista con formattazione condizionale

{{step1-to-reports}}

1. Fare clic sul nome di un report in cui si desidera creare una visualizzazione con formattazione condizionale

   Oppure

   Clic **Nuovo rapporto**, quindi selezionare un tipo di oggetto per creare un nuovo report.

1. (Condizionale) Se modifichi un rapporto esistente, fai clic su **Azioni report**, quindi fai clic su **Modifica**.

1. In **Colonne (visualizzazione)** , fare clic per selezionare una colonna esistente o fare clic su **Aggiungi colonna** per creare una colonna.
1. In **Mostra in questa colonna** nell’angolo in alto a sinistra del report builder, seleziona il campo da visualizzare nella nuova colonna.
1. Clic **Opzioni avanzate**.

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

1. In **Quando:** , impostare un&#39;istruzione di condizione per la colonna.

   Ad esempio: &quot;quando la percentuale di completamento dell&#39;attività è uguale a (distinzione maiuscole/minuscole) 50&quot;.
1. In **Mostra il campo in questo modo:** specifica l’aspetto di questo campo quando viene soddisfatta la condizione definita sopra.

   Specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Colore testo</strong></td> 
      <td> <p>Selezionare il colore di visualizzazione del testo. Sono disponibili 8 colori.</p> <p><b>NOTA</b></p> <p> Se il campo contiene un collegamento ipertestuale, le selezioni del colore del testo non vengono applicate al campo.</p> </td> 
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
      <td>Selezionare il colore dello sfondo per il testo. Sono disponibili 8 colori.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostra icona</strong></td> 
      <td>Se desideri visualizzare un’icona invece del valore effettivo di questa colonna, selezionala da una delle 16 icone.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostra testo</strong></td> 
      <td> <p>Selezionare questa opzione per visualizzare un'etichetta personalizzata per la colonna anziché il valore effettivo. Specifica il testo da visualizzare al posto del valore nel campo fornito.</p> <p><b>IMPORTANTE</b></p> <p>Selezione <strong>Mostra testo</strong> disabilita la possibilità di modificare in linea il testo in questa colonna.<br>Inoltre, non puoi modificare il valore di una colonna Predecessore perché contiene una logica incorporata.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Applica a tutta la riga</strong></td> 
      <td>Selezionare questa opzione per applicare le impostazioni all'intera riga anziché alla sola colonna selezionata.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Aggiungi regola**.\
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

1. Clic **Fine**.
1. Fai clic su **Salva e Chiudi**.\
   Nel report, gli utenti visualizzano le modifiche al formato se sono state soddisfatte le condizioni specificate.
