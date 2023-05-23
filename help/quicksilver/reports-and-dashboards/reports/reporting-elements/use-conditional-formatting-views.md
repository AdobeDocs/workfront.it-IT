---
product-area: reporting
navigation-topic: reporting-elements
title: Utilizzare la formattazione condizionale nelle visualizzazioni
description: Quando condividi i tuoi rapporti con altri utenti in Adobe Workfront, prendi in considerazione la possibilità di personalizzare la visualizzazione dei rapporti per semplificare la lettura di determinate informazioni o distinguerti facilmente.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '1150'
ht-degree: 2%

---

# Utilizzare la formattazione condizionale nelle visualizzazioni

Quando condividi i tuoi rapporti con altri utenti in Adobe Workfront, prendi in considerazione la possibilità di personalizzare la visualizzazione dei rapporti per semplificare la lettura di determinate informazioni o distinguerti facilmente.

È possibile personalizzare la scheda Dettagli dei rapporti aggiungendo formattazione speciale o condizionale alla visualizzazione dei rapporti.

È necessario disporre delle autorizzazioni di gestione per il report, per poterlo modificare e aggiungere una formattazione speciale alla visualizzazione.

Per ulteriori informazioni sulla creazione di rapporti, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Formattando le colonne in modo condizionale nella visualizzazione del report, è possibile impostare regole che influiscono sulla modalità di visualizzazione del report. Quando tali condizioni o regole vengono soddisfatte, viene applicata la formattazione speciale.

Se ad esempio la percentuale di completamento di un&#39;attività è inferiore al 20%, è possibile evidenziare il campo visualizzando il numero in grassetto, in rosso e con un colore di sfondo giallo.

Con una vista con formattazione condizionale è possibile:

* Modifica l’intestazione di una colonna.
* Modificate il valore di una colonna in testo personalizzato o immagine.
* Formattare la visualizzazione di un campo modificando il tipo di carattere, il colore, l&#39;allineamento o il colore dello sfondo.

Le modifiche apportate nella visualizzazione del report hanno effetto solo nella scheda Dettagli del report. Queste modifiche non influiscono sulle schede Riepilogo, Matrice o Grafico del rapporto.

## Requisiti di accesso

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
   <td> <p>Richiedi o superiore </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare una visualizzazione in un rapporto</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Gestire le autorizzazioni per un report per creare o modificare una visualizzazione in un report</p> <p>Gestire le autorizzazioni per una visualizzazione</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario creare un report prima di aggiungere la formattazione condizionale.

Per informazioni sulla creazione di un rapporto, consulta [Creare un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Creare una vista con formattazione condizionale

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Workfront, quindi fai clic su **Rapporti**.

1. Fare clic sul nome di un report in cui si desidera creare una visualizzazione con formattazione condizionale.

   Oppure

   Clic **Azioni report**, quindi fai clic su **Modifica**.

1. (Condizionale) Se hai modificato un rapporto, seleziona una colonna esistente o creane una nuova.
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
      <td>Scegli il formato in cui viene visualizzato il valore nella colonna. A seconda del campo colonna, questo consente di impostare la visualizzazione di date, numeri o valuta.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostra questa colonna quando in un dashboard</strong></td> 
      <td>Seleziona questo campo se desideri che la colonna venga visualizzata quando il rapporto viene inserito in un dashboard. La colonna viene sempre visualizzata quando si esamina il rapporto all’esterno di un dashboard.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Aggiungi una regola per questa colonna**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. In **Quando:** , impostare un&#39;istruzione di condizione per la colonna. Ad esempio: quando la percentuale di completamento dell&#39;attività è uguale a (distinzione maiuscole/minuscole) 50.
1. In **Mostra il campo in questo modo:** specifica l’aspetto di questo campo quando viene soddisfatta la condizione definita sopra.

   Specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Colore testo</strong></td> 
      <td> <p>Selezionare il colore di visualizzazione del testo. Sono disponibili 8 colori.</p> <p>Nota: se il campo contiene un collegamento ipertestuale, le selezioni del colore del testo non vengono applicate al campo.</p> </td> 
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
      <td role="rowheader"><strong>Sfondo</strong></td> 
      <td>Selezionare il colore dello sfondo per il testo. Sono disponibili 8 colori.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostra icona</strong></td> 
      <td>Se desideri visualizzare un’icona invece del valore effettivo di questa colonna, selezionala da una delle 16 icone.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostra testo</strong></td> 
      <td> <p>Selezionare questa opzione per visualizzare un'etichetta personalizzata per la colonna anziché il valore effettivo. Specifica il testo da visualizzare al posto del valore nel campo fornito.</p> <p>Importante: selezione <strong>Mostra testo</strong> disabilita la possibilità di modificare in linea il testo in questa colonna.<br>Inoltre, non puoi modificare il valore di una colonna Predecessore perché contiene una logica incorporata.</p> </td> 
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

   Esempio 1: puoi innanzitutto creare una regola in cui, quando viene creato lo stato del progetto, il colore del testo è viola e grassetto. Viene quindi creata una seconda regola che indica se il campo Nome attività non è vuoto, se il colore del testo è rosso e corsivo e se il colore di sfondo è verde. In questo esempio si verifica quanto segue:

   * Le attività di cui viene generato lo stato del progetto vengono visualizzate in viola e grassetto. Se il nome dell&#39;attività non è vuoto, le attività hanno anche uno sfondo verde.
   * Le attività il cui Stato progetto è diverso da Creazione (e il cui Nome attività non è vuoto) vengono visualizzate in un testo rosso e in corsivo con uno sfondo verde.

   Esempio 2: creare una regola sulla data di completamento pianificata del progetto che influisca sull’intera riga, diventando grigio se il progetto viene annullato (Stato = &quot;Inattivo&quot;). Quindi crea una regola di colonna che attivi lo sfondo in rosso quando la Data di completamento pianificata del progetto è inferiore a oggi (ovvero il progetto è in ritardo). In questo esempio, se un progetto annullato presenta una data di completamento in ritardo, tale cella verrà visualizzata in rosso anche se le altre celle nella riga sono grigie. Per correggere questa formattazione:

   * Modifica la formattazione per Data di completamento pianificata ed elimina la regola di colonna per lo sfondo rosso sui progetti in ritardo.
   * Aggiungi una regola di colonna con la stessa formattazione della regola di riga (sfondo grigio quando Stato progetto = &quot;Inattivo&quot;).
   * Aggiungi nuovamente la regola di colonna per lo sfondo rosso nei progetti in ritardo.
   * Quando salvi le regole e la visualizzazione, lo sfondo rosso non viene applicato a un progetto annullato.


1. Clic **Fine**.
1. Clic **Salva e chiudi**.\
   Nel report, gli utenti visualizzano le modifiche al formato se sono state soddisfatte le condizioni specificate.
