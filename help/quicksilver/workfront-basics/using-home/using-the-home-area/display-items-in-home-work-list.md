---
product-area: projects
navigation-topic: use-the-home-area
title: Visualizza elementi nell'[!UICONTROL Elenco lavori] nell'area Home
description: Ogni widget contiene il proprio elenco di lavoro. Negli elenchi di lavoro vengono visualizzati tutti gli elementi di lavoro assegnati all'utente. Puoi controllare gli elementi da visualizzare nell'[!UICONTROL elenco lavori] utilizzando filtri e raggruppamenti.
author: Courtney
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: 107bb601b8d4fd9376657b5cf5840cee5d086613
workflow-type: tm+mt
source-wordcount: '991'
ht-degree: 4%

---

# Visualizza elementi nell&#39;elenco lavori [!UICONTROL 1} nell&#39;area [!UICONTROL Home]]

<!-- Audited: 1/2024 -->

Ogni widget contiene il proprio elenco di lavoro. Negli elenchi di lavoro vengono visualizzati tutti gli elementi di lavoro assegnati all&#39;utente. Puoi controllare gli elementi da visualizzare nell&#39;[!UICONTROL elenco lavori] utilizzando filtri e raggruppamenti.

>[!IMPORTANT]
>
>* Per visualizzare le attività e i problemi nei widget Home, il progetto principale deve essere nello stato Corrente o in uno stato equivalente a Corrente.
>* I progetti devono anche essere nello stato Attuale o uno stato che equivale allo stato Attuale da visualizzare nella Home.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza</strong></td> 
   <td> <p>Nuovo:</p><ul><li>[!UICONTROL Contributor] solo per le approvazioni</li> <li>[!UICONTROL Standard] o versione successiva per tutti gli altri oggetti</li> <p>Oppure</p> 
  </ul><p>Corrente:</p><ul><li>[!UICONTROL Revisione] solo per le approvazioni</li> <li>[!UICONTROL Work] o versione successiva per tutti gli altri oggetti</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso</strong></td> 
   <td> <p>Accesso di [!UICONTROL View] o versione successiva a progetti, attività, problemi e documenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Autorizzazioni Contribute o superiore per le attività e i problemi su cui devi lavorare</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisiti per gli elementi di lavoro da visualizzare nell’elenco lavori

Esistono requisiti incorporati per i quali gli elementi di lavoro vengono visualizzati in determinati elenchi di lavoro dei widget. Gli elementi di lavoro devono soddisfare questi requisiti per essere visualizzati negli elenchi di lavoro dei widget seguenti.

### Widget attività personali

Le attività devono soddisfare i seguenti requisiti per essere visualizzate nel widget Le mie attività:

* Lo stato dell&#39;attività non corrisponde a Completo.
* L&#39;utente connesso deve essere assegnato all&#39;attività.
* Lo stato dell&#39;attività non è uguale a Fine.
* Lo stato del progetto a cui appartiene l&#39;attività deve essere Corrente.


### Widget problemi personali

Affinché i problemi vengano visualizzati nel widget I miei problemi, è necessario che soddisfino i seguenti requisiti:

* L&#39;utente connesso deve essere assegnato al problema.
* Lo stato del problema non corrisponde a Completo.
* Non è presente un oggetto non risolto associato al problema.
* Lo stato del problema non è uguale a Fine.
* Lo stato del progetto a cui appartiene il problema deve essere Corrente.

### Widget team personali

Per essere visualizzate nel widget Team personali, le richieste del team devono soddisfare i seguenti requisiti:

* L&#39;utente connesso appartiene al team a cui è assegnato l&#39;elemento di lavoro.
* Lo stato dell&#39;elemento di lavoro non equivale a Completato.
* All&#39;elemento di lavoro non è associato un processo di approvazione non risolto.
* L&#39;elemento di lavoro non è un&#39;attività ricorrente.
* Lo stato del progetto a cui appartiene l&#39;elemento di lavoro deve essere Corrente.

## Filtrare il lavoro

È possibile filtrare gli elementi di un widget [!UICONTROL Elenco lavori] per visualizzare solo tipi specifici di elementi. Ad esempio, puoi filtrare il mio lavoro [!UICONTROL Elenco lavori] per visualizzare solo i problemi o le richieste.

>[!NOTE]
>
>Le opzioni del filtro sono memorizzate nel browser. Se utilizzi sempre lo stesso browser sullo stesso computer (e non cancelli i dati del sito), i filtri selezionati non cambiano. Se si cambia browser o computer, i filtri tornano all&#39;opzione predefinita, che è con tutti i filtri deselezionati.

Per filtrare il lavoro:

1. Fai clic sul **[!UICONTROL menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Fai clic su **Personalizza** per aggiungere i seguenti widget:

   | Widget | Descrizione |
   |--------------|---------------------------------------------------------------------------------------------------|
   | Bacheche | Visualizza tutte le bacheche create o che sono state invitate a utilizzare |
   | Il mio lavoro | Visualizza le attività e i problemi assegnati all&#39;utente |
   | I miei progetti | Visualizza i progetti di cui sei proprietario o a cui lavori |
   | Le mie attività | Visualizza le attività assegnate a te |
   | I miei problemi | Visualizza le Issues assegnate a te |
   | Le mie richieste | Visualizza tutte le richieste inviate |
   | Le mie approvazioni | Visualizza tutte le approvazioni in sospeso, assegnate, delegate e inviate |

1. Fai clic sull&#39;icona ![](assets/filter-nwepng.png) del **filtro** nell&#39;angolo superiore destro dell&#39;elenco lavori widget.
1. Scegli un filtro **Suggested** o un filtro creato.
Per informazioni dettagliate sui filtri suggeriti, vedere [Panoramica sui filtri widget principale](/help/quicksilver/workfront-basics/using-home/using-the-home-area/widget-filter-overview-home.md).
1. (Facoltativo) Attiva **Sovrapponi filtri** per selezionare più opzioni filtro.

   ![](assets/my-task-filter-open.png)


## Raggruppare il lavoro

Puoi raggruppare il widget [!UICONTROL elenco lavori] per mantenere organizzati i tuoi elementi di lavoro.

Per raggruppare l&#39;elenco lavori:

1. Fai clic sul **[!UICONTROL menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Fai clic su **Personalizza** per aggiungere i seguenti widget:

   | Widget | Descrizione |
   |--------------|---------------------------------------------------------------------------------------------------|
   | Bacheche | Visualizza tutte le bacheche create o che sono state invitate a utilizzare |
   | Il mio lavoro | Visualizza le attività e i problemi assegnati all&#39;utente |
   | I miei progetti | Visualizza i progetti di cui sei proprietario o a cui lavori |
   | Le mie attività | Visualizza le attività assegnate a te |
   | I miei problemi | Visualizza le Issues assegnate a te |
   | Le mie richieste | Visualizza tutte le richieste inviate |
   | Le mie approvazioni | Visualizza tutte le approvazioni in sospeso, assegnate, delegate e inviate |

1. Fai clic sull&#39;icona ![](assets/group-icon.png) del **Gruppo** nell&#39;angolo superiore destro dell&#39;elenco lavori widget.
1. Scegli un raggruppamento **Consigliato** o un raggruppamento creato.
   ![](assets/grouping-expanded.png)


## Personalizzare le colonne dell’elenco lavori

È possibile scegliere quali colonne visualizzare nell&#39;elenco di lavoro widget:

1. Fai clic sul **[!UICONTROL menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Fai clic su **Personalizza** per aggiungere i seguenti widget:

   | Widget | Descrizione |
   |--------------|---------------------------------------------------------------------------------------------------|
   | Bacheche | Visualizza tutte le bacheche create o che sono state invitate a utilizzare |
   | Il mio lavoro | Visualizza le attività e i problemi assegnati all&#39;utente |
   | I miei progetti | Visualizza i progetti di cui sei proprietario o a cui lavori |
   | Le mie attività | Visualizza le attività assegnate a te |
   | I miei problemi | Visualizza le Issues assegnate a te |
   | Le mie richieste | Visualizza tutte le richieste inviate |
   | Le mie approvazioni | Visualizza tutte le approvazioni in sospeso, assegnate, delegate e inviate |

1. Fai clic sull&#39;icona ![](assets/column-icon.png) della **Colonna** nell&#39;angolo superiore destro dell&#39;elenco lavori widget.
1. Attiva o disattiva le colonne a seconda delle preferenze.
1. (Facoltativo) Fai clic sull&#39;icona **Trascina** ![](assets/drag-icon.png) per riordinare le colonne.
   ![](assets/columns-expanded.png)


## Visualizza elementi in ritardo

[!DNL Adobe Workfront] utilizza le date seguenti per determinare se le richieste di lavoro sono in ritardo:

* **Attività**: [!UICONTROL Data di completamento Pianificata]
* **Problemi**: [!UICONTROL Data di completamento Pianificata]
* **Documenti**: [!UICONTROL Data di invio]
* **Schede orario**: [!UICONTROL Data invio]
* **Approvazioni**: [!UICONTROL Data invio]
* **Approvazioni bozza**: [!UICONTROL Scadenza bozza]




