---
product-area: home
navigation-topic: use-the-home-area
title: Gestisci il tuo lavoro con il widget Il mio lavoro
description: Il widget Il mio lavoro mostra tutte le attività, i problemi e le richieste assegnati in un'unica posizione. In questa finestra è possibile filtrare e organizzare il lavoro, registrare il tempo, apportare aggiornamenti e contrassegnare gli elementi di lavoro come completati.
author: Courtney
feature: Get Started with Workfront
exl-id: e110f0f6-4ecb-419b-a368-c3f802de5920
source-git-commit: fddb927f2c9639b4c26d590bbea7dba684ed2b6c
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 4%

---

# Gestisci il tuo lavoro con il widget Il mio lavoro

Il widget Il mio lavoro mostra tutte le attività, i problemi e le richieste assegnati in un&#39;unica posizione. In questa finestra è possibile filtrare e organizzare il lavoro, registrare il tempo, apportare aggiornamenti e contrassegnare gli elementi di lavoro come completati.

>[!IMPORTANT]
>
>Per visualizzare le attività e i problemi nel widget Il mio lavoro, il progetto principale deve trovarsi nello stato Corrente o in uno stato equivalente a Corrente.

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
   <td> <p>Corrente: Contribute</p>
   <p>Oppure</p> 
   <p>Nuovo:[!UICONTROL Light] o versione successiva<p> 
  </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso</strong></td> 
   <td> <p>Accesso di [!UICONTROL View] o versione successiva a progetti, attività, problemi e documenti</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Autorizzazioni per contribuire o superiore alle attività e ai problemi su cui devi lavorare</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Trovare il lavoro con i filtri

Puoi perfezionare i filtri Il mio lavoro per concentrarti su elementi specifici nell’elenco del lavoro:

![Filtro Il mio lavoro](assets/filter-my-work-widget.png)

### Dettagli filtro

<table>
  <tbody>
    <tr>
      <td>Lavori</td>
      <td>Visualizza gli elementi su cui si sta lavorando</td>
    </tr>
    <tr>
      <td>È il momento di iniziare?</td>
      <td>Visualizza gli elementi con 
      <ul>
      <li>Nessun predecessore o vincolo di attività incompleto</li>
      <p>e</p>
      <li>La data di inizio pianificata è nel passato o è prevista entro due settimane</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>Non pronto</td>
      <td>Visualizza gli elementi con
       <ul>
      <li>Predecessori incompleti o vincoli di attività che impediscono la lavorazione dell'elemento</li>
      <p>oppure</p>
      <li>La data di inizio pianificata nel futuro è tra più di due settimane</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>Richiesto il</td>
      <td>Visualizza i problemi per i quali non hai iniziato a lavorare</td>
    </tr>
    <tr>
      <td>Delegata da me</td>
      <td>Visualizza gli elementi delegati ad altri utenti</td>
    </tr>
    <tr>
      <td>Delegata a me</td>
      <td>Visualizza gli elementi che gli utenti ti hanno delegato</td>
    </tr>
    <tr>
      <td>Completato</td>
      <td>Visualizza il lavoro completato nelle ultime due settimane. Questa opzione di filtro non include le approvazioni.</td>
    </tr>
  </tbody>
</table>

>[!TIP]
>
>Se stai cercando opzioni di filtro più specifiche, puoi utilizzare i widget Attività personale o Problema personale. Per ulteriori informazioni sui filtri Attività personali e Problemi personali, vedere [Panoramica sui filtri dei widget principali](/help/quicksilver/workfront-basics/using-home/using-the-home-area/widget-filter-overview-home.md).

## Organizzare il lavoro

È possibile utilizzare le funzioni di ordinamento e raggruppamento del widget Il mio lavoro per organizzare il lavoro in modo appropriato.

### Ordina

È possibile ordinare l&#39;elenco di lavoro in base a

* Data di scadenza
Gli elementi scaduti visualizzano un&#39;icona di avviso accanto alla data. Workfront utilizza la Data di completamento pianificata per determinare se le attività e i problemi sono scaduti.
* Nome
* Percentuale completato
* Stato

>[!TIP]
>
>Per creare un elenco che visualizzi tutti gli elementi scaduti nella parte superiore del widget Il mio lavoro, ordinarli per data di scadenza e non applicare un raggruppamento.


![Ordina nel widget Il mio lavoro](assets/sort-my-work-widget.png)

### Gruppo

È possibile raggruppare l’elenco lavori per

* Progetto
* Stato
* Data di scadenza
La data di scadenza è determinata dalla data di completamento pianificata.

>[!NOTE]
>
>Quando si applica un raggruppamento, la selezione nel menu Ordina determina l&#39;ordine all&#39;interno del raggruppamento.


![Raggruppamento nel widget Il mio lavoro](assets/group-my-work-widget.png)

## Aggiornare le informazioni sull&#39;elemento di lavoro nel Riepilogo

Puoi aprire il pannello Riepilogo per aggiornare rapidamente le informazioni in un’attività o in un problema. Nel Riepilogo, puoi

* Aggiornare la percentuale di completamento
* Aggiungi un aggiornamento
* Passare all&#39;area Documento per caricare un documento
* Visualizzare i dettagli degli elementi di lavoro e aggiornare i campi personalizzati
Gli amministratori di Workfront possono personalizzare i campi da visualizzare nel Riepilogo nel modello di layout. Per ulteriori informazioni, vedere [Personalizzare il pannello Riepilogo utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).
* Modificare lo stato dell&#39;elemento di lavoro
* Visualizza le sottoattività
* Registra ore
* Visualizza i processi di approvazione allegati

Per aprire il Riepilogo, passa il puntatore sull&#39;elemento di lavoro, quindi fai clic sull&#39;icona **Riepilogo** ![Icona Riepilogo](assets/open-summary-new-home.png).

Per ulteriori informazioni sull&#39;utilizzo del pannello Riepilogo, vedere [Panoramica di riepilogo](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md).

## Utilizzare le azioni rapide per aggiornare gli elementi di lavoro

È possibile utilizzare il menu Azioni rapide per

* Registra ore
* Aggiungi un aggiornamento
* Aggiornare un modulo personalizzato
* Carica un file

Per individuare il menu Azioni rapide, passa il puntatore sull&#39;elemento di lavoro. L&#39;elenco delle azioni rapide viene visualizzato accanto al pulsante **Lavoraci** o **Fine**.

![Menu Azioni rapide](assets/quick-actions-new-home.png)


## Visualizzare approvazioni e richieste del team

Le approvazioni e le richieste del team non vengono visualizzate nel widget Il mio lavoro. Se lavori regolarmente con approvazioni e richieste del team, ti consigliamo di aggiungere i seguenti widget alla nuova home page:

* La mia approvazione
* Tutte le approvazioni
* Richieste team

Per informazioni sull&#39;aggiunta di widget alla nuova home page, vedere [Aggiungere, modificare o rimuovere widget nella home](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md).
