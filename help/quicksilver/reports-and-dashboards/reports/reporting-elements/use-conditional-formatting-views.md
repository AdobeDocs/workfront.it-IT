---
product-area: reporting
navigation-topic: reporting-elements
title: Utilizzare la formattazione condizionale nelle visualizzazioni
description: Quando condividi i rapporti con altri utenti in Adobe Workfront, considera la possibilità di personalizzare la visualizzazione dei rapporti, di semplificare la lettura di determinate informazioni o di distinguerli.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '1148'
ht-degree: 2%

---

# Utilizzare la formattazione condizionale nelle visualizzazioni

Quando condividi i rapporti con altri utenti in Adobe Workfront, considera la possibilità di personalizzare la visualizzazione dei rapporti, di semplificare la lettura di determinate informazioni o di distinguerli.

Puoi personalizzare la scheda Dettagli dei rapporti aggiungendo formattazione speciale o condizionale alla visualizzazione dei rapporti.

È necessario disporre delle autorizzazioni di gestione per il rapporto, per poter modificarlo e aggiungere una formattazione speciale alla visualizzazione.

Per ulteriori informazioni sulla creazione di rapporti, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Formattando le colonne in modo condizionato nella visualizzazione del rapporto, è possibile impostare regole che influiscono sulla modalità di visualizzazione del rapporto. Quando tali condizioni o regole vengono soddisfatte, viene applicata la formattazione speciale.

Ad esempio, se la percentuale di completamento di un&#39;attività è inferiore al 20%, è possibile evidenziare il campo visualizzando il numero percentuale in grassetto, testo rosso e un colore di sfondo giallo.

Con una visualizzazione in formato condizionale è possibile:

* Modificare l’intestazione di una colonna.
* Modifica il valore di una colonna in un testo personalizzato o in un’immagine.
* Formattare la visualizzazione di un campo modificando il tipo di font, il colore, l’allineamento o il colore dello sfondo.

Le modifiche apportate nella visualizzazione del rapporto hanno effetto solo nella scheda Dettagli del rapporto. Queste modifiche non influiscono sulle schede Riepilogo, Matrice o Grafico del rapporto.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Modificare l’accesso a Report, Dashboard e Calendari per modificare una visualizzazione in un report</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Gestire le autorizzazioni per un rapporto per creare o modificare una visualizzazione in un rapporto</p> <p>Gestire le autorizzazioni per una visualizzazione</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario creare un rapporto prima di potervi aggiungere la formattazione condizionale.

Per informazioni sulla creazione di un rapporto, vedi [Creare un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Creare una visualizzazione con formattazione condizionale

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **Rapporti**.

1. Fare clic sul nome di un rapporto in cui si desidera creare una visualizzazione con formattazione condizionale.

   Oppure

   Fai clic su **Azioni dei rapporti**, quindi fai clic su **Modifica**.

1. (Condizionale) Se hai modificato un rapporto, seleziona una colonna esistente o creane una nuova.
1. Fai clic su **Opzioni avanzate**.

1. Specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Etichetta colonna personalizzata</strong></td> 
      <td> <p>Specifica un nome per la colonna.</p> <p>Se modifichi una colonna esistente, specificando un nome in questo caso viene modificato il nome della colonna esistente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formato campo</strong></td> 
      <td>Scegli il formato in cui viene visualizzato il valore nella colonna. A seconda del campo colonna, questo consente di impostare la modalità di visualizzazione di date, numeri o valute.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostra questa colonna quando in un dashboard</strong></td> 
      <td>Selezionare questo campo se si desidera che la colonna venga visualizzata quando il rapporto è posizionato su un dashboard. La colonna viene sempre visualizzata quando si guarda il rapporto all’esterno di un dashboard.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Aggiungi una regola per questa colonna**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. In **Quando:** imposta un&#39;istruzione condizione per la colonna . Ad esempio: quando la percentuale di completamento attività è uguale a (distinzione maiuscole/minuscole) 50.
1. In **Mostra il campo in questo modo:** specifica l’aspetto del campo quando viene soddisfatta la condizione definita sopra.

   Specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Colore testo</strong></td> 
      <td> <p>Selezionare il colore in cui viene visualizzato il testo. Sono disponibili 8 colori.</p> <p>Nota: Se il campo contiene un collegamento ipertestuale, le selezioni del colore del testo non vengono applicate a questo campo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formato testo</strong></td> 
      <td>Seleziona se visualizzare il testo in grassetto o corsivo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Allineamento testo</strong></td> 
      <td>Seleziona se allineare il testo a destra, al centro o a sinistra all’interno della colonna.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Background</strong></td> 
      <td>Selezionare il colore dello sfondo del testo. Sono disponibili 8 colori.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostra icona</strong></td> 
      <td>Seleziona una delle 16 icone per visualizzare un’icona invece del valore effettivo per questa colonna.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostra testo</strong></td> 
      <td> <p>Seleziona questa opzione per visualizzare un’etichetta personalizzata per questa colonna, anziché il relativo valore effettivo. Specifica il testo da visualizzare invece del valore nel campo fornito.</p> <p>Importante: Selezione <strong>Mostra testo</strong> disabilita la modifica in linea del testo in questa colonna.<br>Inoltre, non è possibile modificare il valore di una colonna Predecessore perché contiene una logica incorporata.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Applica a tutta la riga</strong></td> 
      <td>Selezionare questa opzione per applicare le impostazioni all’intera riga anziché applicare le impostazioni solo alla colonna selezionata.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Aggiungi regola**.\
   Puoi aggiungere altre regole alla stessa colonna o ad altre colonne.

   Le regole vengono applicate nell’ordine in cui sono state create. Sono combinate ma non si sovrascrivono a vicenda, anche se una regola di colonna ha la precedenza su una regola di riga sulla stessa cella.

   Esempio 1: È innanzitutto possibile creare una regola che indica quando lo stato del progetto è Creazione, che il colore del testo è viola e grassetto. È quindi necessario creare una seconda regola che indichi che il nome dell’attività non è vuoto, che il colore del testo sia rosso e corsivo e che il colore dello sfondo sia verde. In questo esempio si verifica quanto segue:

   * Le attività il cui stato progetto è in corso di creazione vengono visualizzate in testo viola e grassetto. Se il nome dell&#39;attività non è vuoto, anche le attività hanno uno sfondo verde.
   * Le attività il cui stato del progetto è diverso da Generazione (e il nome dell&#39;attività non è vuoto) vengono visualizzate in un testo rosso e in corsivo con sfondo verde.

   Esempio 2: Crea una regola sulla data di completamento pianificata del progetto che influisce sull’intera riga, visualizzando il grigio di sfondo se il progetto viene annullato (Stato = &quot;Dead&quot;). Quindi crea una regola di colonna che diventa rossa quando la data di completamento pianificata del progetto è inferiore a quella odierna (ovvero se il progetto è in ritardo). In questo esempio, se un progetto annullato ha una data di completamento ritardata, la cella verrà visualizzata in rosso anche se le altre celle della riga sono grigie. Per correggere la formattazione:

   * Modificare la formattazione per la data di completamento pianificata ed eliminare la regola della colonna relativa allo sfondo rosso per i progetti in ritardo.
   * Aggiungi una regola di colonna con la stessa formattazione della regola di riga (sfondo grigio quando Stato progetto = &quot;Morto&quot;).
   * Aggiungi nuovamente la regola della colonna per lo sfondo rosso per i progetti in ritardo.
   * Quando salvi le regole e la visualizzazione, lo sfondo rosso non viene applicato a un progetto annullato.


1. Fai clic su **Fine**.
1. Fai clic su **Salva e chiudi**.\
   Nel rapporto, gli utenti visualizzano le modifiche al formato se le condizioni specificate sono state soddisfatte.
