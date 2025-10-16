---
navigation-topic: get-started-with-workfront
title: Gestire il lavoro nel calendario Priorità
description: Tieni traccia del tuo lavoro con un calendario chiaro e visivo.
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: d24ad7d1-3a88-479e-beaf-69f8264c9a6b
source-git-commit: 0940e4c89de6cd3518cd98a1e06dc726f434846b
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 4%

---

# Gestire il lavoro nel calendario Priorità

Monitora facilmente il tuo lavoro con un calendario chiaro e visivo. Con il calendario Priorità è possibile:

* Utilizzare i filtri per trovare il lavoro
* Applicare campi personalizzati come stato e livello di attivazione per identificare il lavoro ad alta priorità
* Applicazione dei colori per un&#39;organizzazione rapida

>[!IMPORTANT]
>
>I progetti devono essere nello stato Attuale o in uno stato che sia uguale a Attuale per poter visualizzare i progetti e le relative attività e Issues figlio.


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Revisore o versione successiva</p>
   <p>Chiaro o superiore</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o modifica per l'oggetto su cui si trova l'aggiornamento</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di visualizzazione all'oggetto</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizza il tuo lavoro nel calendario

In Priorità vengono visualizzati gli elementi di lavoro assegnati all&#39;utente. Non è possibile visualizzare gli elementi di lavoro assegnati al team nel calendario Priorità.

{{step1-to-priorities}}

1. Fai clic sull&#39;icona **Calendario** nella parte superiore dell&#39;elenco lavori.
   ![icona calendario](assets/calendar-tab.png)
1. Selezionare uno o più filtri per limitare gli elementi di lavoro.

   +++Espandi per visualizzare informazioni dettagliate sui filtri disponibili
   <table>
    <tbody>
    <tr>
    <th>Filtro</th>
    <th>Descrizione</th>
    </tr>
        <tr>
        <td>Ci sto lavorando</td>
        <td>Visualizza gli elementi su cui si sta lavorando.</td>
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
        <li>La data di inizio pianificata è nel futuro più di due settimane.</li>
        </ul>
        </td>
        </tr>
        <tr>
        <td>Richiesto il</td>
        <td>Visualizza i problemi per i quali non hai iniziato a lavorare.</td>
        </tr>
        <td>Terminato</td>
        <td>Visualizza il lavoro completato nelle ultime due settimane. Questa opzione di filtro non include le approvazioni.</td>
        </tr>
        <tr>
        <td>Progetto</td>
        <td>Visualizza i progetti che contengono le attività o i problemi che ti sono stati assegnati.</td>
        </tr>
        <tr>
        <td>Data di scadenza</td>
        <td>Visualizza il lavoro per data di completamento pianificata.</td>
        </tr>
        <tr>
        <td>Stato</td>
        <td>Visualizza le attività o i problemi in stato Nuovo, In corso e Completato.</td>
        </tr>
        <tr>
        <td>Il mio focus</td>
        <td>Visualizza le attività o i problemi in cui sono stati assegnati livelli di attivazione. I livelli di attivazione vengono assegnati e gestiti dal singolo utente.</td>
        </tr>
    </tbody>
    </table>

   +++

1. Fare clic sulla barra degli elementi di lavoro nel calendario per aprire il riepilogo laterale. Il riepilogo laterale consente di:

   * Visualizzare e modificare i dettagli del progetto e dell&#39;elemento di lavoro
   * Creare e visualizzare commenti
   * Visualizzare e caricare i documenti
   * Creare una bozza
   * Passare alla pagina del progetto in Workfront
   * Passare alla pagina dei dettagli dell&#39;elemento di lavoro in Priorità
   * Registra ore
   * Aggiungi collegamenti rapidi

1. (Facoltativo) Fai clic su **Crea nuovo** per aggiungere un nuovo elemento di lavoro al calendario. Per ulteriori informazioni, consulta [Creare una nuova attività o un nuovo problema in Priorità](/help/quicksilver/workfront-basics/priorities/create-task-issue-priorities.md).

## Configurare il calendario

{{step1-to-priorities}}

1. Fai clic sull&#39;icona **Calendario** nella parte superiore dell&#39;elenco lavori.
   ![icona calendario](assets/calendar-tab.png)
1. Fai clic sull&#39;icona **Impostazioni** nell&#39;angolo destro del calendario.

1. Nella scheda **Stile barra**, scegliere fino a 5 campi da visualizzare sulla barra degli elementi di lavoro nel calendario.
   ![barra di esempio](assets/sample-task-for-field-config.png)

1. Nella scheda **Colore** scegliere la modalità di visualizzazione degli elementi di lavoro. Se ad esempio si sceglie **Progetto**, gli elementi di lavoro verranno visualizzati in base al colore assegnato al progetto nell&#39;elenco lavori.
   ![progetto colore campione](assets/sample-calendar-projects.png)
