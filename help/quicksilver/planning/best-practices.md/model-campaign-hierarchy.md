---
title: 'Framework di successo: modellare la gerarchia delle campagne'
description: Scopri come tradurre i processi aziendali complessi in una gerarchia di campagne scalabile e gestita utilizzando "Centri di gravità" e un’architettura con più aree di lavoro.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 1158a49fc0b39ef49f23326935d4635530501687
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 0%

---


# Framework per il successo: modellare la gerarchia delle campagne



## Obiettivo

Scopri come tradurre i processi aziendali complessi in una gerarchia di campagne scalabile e gestita utilizzando &quot;Centri di gravità&quot; e un’architettura con più aree di lavoro.



## Panoramica

Con la scalabilità delle operazioni di marketing, aumenta anche la complessità dei dati. Senza una blueprint chiara, il tuo Marketing System of Record (MSOR) può rapidamente diventare un &quot;cassetto della posta indesiderata&quot; di record disconnessi, terminologia in conflitto e silos di reporting.



Il &quot;Blueprint of Success&quot; è un framework per la modellazione della gerarchia delle campagne in Workfront Planning. Consente di passare dal caos dei fogli di calcolo a un modello gestito e orientato agli oggetti che garantisce che ogni team parli la stessa lingua, mantenendo al contempo l&#39;agilità necessaria per l&#39;esecuzione.



## Gerarchia: individuazione dei livelli di intento

Per mantenere chiarezza e scalabilità, consigliamo di iniziare con un **percorso core** comprovato. Anche se le organizzazioni possono espandere questa gerarchia man mano che le loro esigenze operative evolvono, a partire da questi tre livelli garantisce un forte ponte tra strategia ed esecuzione.



### Il percorso di base: strategia per l’azione

La maggior parte delle implementazioni di successo si basa su un modello pulito a tre livelli che si estende sia a Planning che a Workflow:



1. **Livello 1: Campagne (Modulo Pianificazione)**

   * **Obiettivo:** pilastri strategici a lungo termine e iniziative annuali (ad esempio, &quot;Consapevolezza del marchio globale per l&#39;anno fiscale 2026&quot;).

   * **Persona:** CMO, Vice Presidente Marketing, Responsabili strategici.

2. **Livello 2: tattiche del canale (modulo di pianificazione)**

   * **Focus:** le istruzioni operative che definiscono il &quot;cosa&quot; per canali specifici (ad esempio, &quot;Blitz social media Q1&quot;). Questo è il livello finale dell&#39;intento strategico prima dell&#39;inizio dei lavori.

   * **Persona:** Operazioni Di Marketing, Lead Di Canale, Manager Campagne.

3. **Livello 3: Progetti flusso di lavoro (Modulo flusso di lavoro)**

   * **Focus:** l&#39;esecuzione effettiva di &quot;Esperienze&quot; o &quot;Attività&quot; (ad esempio, post social specifici, e-mail, pagine Web).

   * **Implementazione:** Le tattiche in Planning sono collegate direttamente a **Progetti** nel modulo Flusso di lavoro, dove i singoli risultati finali vengono gestiti come attività e problemi.

   * **Persona:** Creativi, Singoli Collaboratori.



### Espansione strategica: aggiunta di altri livelli

Una volta stabilito il percorso principale, le organizzazioni possono scegliere di aggiungere altri livelli dopo un’attenta considerazione della loro complessità aziendale specifica:



* **Piani canale:** Un livello tra *Campagne* e *Tattiche* per raggruppare strategie interfunzionali (ad esempio, &quot;Strategia digitale&quot;).

* **Workfront Planning Activities:** In ambienti con volumi ridotti (in genere &lt;5.000 risultati finali/anno), alcuni team preferiscono tenere traccia delle singole &quot;Esperienze&quot; come record di Workfront Planning prima che diventino progetti.


>[!TIP]
>
>**Suggerimento Fondamentale: La Soglia Di 5.000 Risultati Finali**
>
>Se la tua organizzazione produce più di 5.000 attività all&#39;anno, devi **scaricare sempre** il tracciamento dei singoli risultati finali nel **modulo flusso di lavoro**. La gestione di record di &quot;esperienza&quot; di alto volume in Planning può portare all’accumulo di dati che oscura la visibilità strategica. Usare Planning per &quot;Perché&quot; e &quot;Cosa&quot; e il modulo Workflow per il &quot;Come&quot; di volumi elevati.



## Architettura: centri di gravità

Un MSOR di livello enterprise non è incorporato in un&#39;unica area di lavoro. Utilizza un&#39;architettura &quot;Hub-and-Spoke&quot; in cui i tipi di record vengono gestiti nei loro **Centri di gravità** naturali.



### &#x200B;1. Il polo di tassonomia (classificazioni)

Stabilisci un’area di lavoro centralizzata per le &quot;Classificazioni globali&quot; (ad esempio Marchi, Aree geografiche, Prodotti, Utenti tipo).

* **Posizione principale:** Questa area di lavoro è il &quot;Source of Truth&quot; per questi oggetti.

* **Vantaggio:** Sindacando queste definizioni al resto dell&#39;azienda, si risolve &quot;Semantic Drift&quot;, assicurandosi che &quot;Area geografica: EMEA&quot; significhi la stessa cosa per ogni team.



### &#x200B;2. Il Workspace di pianificazione strategica (centro esecutivo)

**Campagne** di alto livello (e **Piani canale**) sono attivi qui.

* **Sede principale:** Questo è il centro di gravità esecutivo, che fornisce un ambiente privo di rumore per il processo decisionale strategico.

* **Vantaggio:** I dirigenti possono gestire il portfolio senza dover affrontare il problema tattico quotidiano.



### &#x200B;3. Raggi funzionali (aree di lavoro del team)

Le unità funzionali (Social, Creative, E-mail) dispongono di aree di lavoro proprie per gestire le **tattiche**.

* **Posizione principale:** Queste aree di lavoro sono il centro di gravità per l&#39;esecuzione del team locale.

* **Vantaggio:** i team &quot;utilizzano&quot; le campagne e le classificazioni globali dagli hub, mantenendo al contempo i propri oggetti locali (ad esempio *Media Outlet* o *Diritti di utilizzo*).



## Governance basata sul nome: parla una lingua

Per garantire che il tuo blueprint rimanga sotto pressione, segui il principio di **Governance basata su sostantivo**.



* **Usa sostantivi, non verbi:** Assegna un nome ai tipi di record dopo le &quot;cose&quot; che stai tracciando (`Campaign`, `Tactic`), non le &quot;azioni&quot; (`Campaigning`, `Planning`).

* **Nomenclatura standard:** Utilizzare gli stessi nomi in tutte le aree di lavoro. Questo consente di aggregare i dati nell’intero portfolio per i rapporti manageriali.



## E i programmi e i portafogli esistenti?

Una domanda comune per le organizzazioni mature è come gestire i portafogli e i programmi già generati nel **modulo Workflow**. In passato, questi oggetti venivano spesso utilizzati per imitare la pianificazione strategica.



### &#x200B;1. Portfolio e programmi → tipi di record

In molte organizzazioni, i **Portfolio** sono utilizzati per rappresentare marchi di alto livello o Business Unit (BU), mentre i **Programmi** rappresentano temi strategici.

* **Il turno:** Questi sono modellati come **Tipi di record** nel tuo **Hub tassonomia**. Trattando &quot;Brand&quot; o &quot;Business Unit&quot; come tipo di record, puoi collegarli a qualsiasi campagna o tattica in tutta l’azienda, fornendo un reporting molto più flessibile rispetto a una struttura Portfolio/Program statica.



### &#x200B;2. La strategia &quot;Reporting Bridge&quot;

Mentre Workfront Planning è il futuro dell&#39;intento strategico, il reporting nativo tramite **Dashboard Canvas** è ancora in fase di maturazione. Molte organizzazioni si affidano ancora alle solide funzionalità di reporting associate alle strutture legacy di Portfolio e Program nel modulo Workflow.

* **Consiglio:** Non eliminare ancora i portafogli e i programmi. Utilizzare invece **Automazioni Fusion** per creare un bridge.

* **Funzionamento:** Quando si crea una tattica o una campagna in Workfront Planning, Fusion può eseguire automaticamente il mirroring di tale record in un Portfolio o in un programma corrispondente nel modulo del flusso di lavoro. Questo consente di:

   1. Approfitta della **visualizzazione strategica** superiore di Workfront Planning (Timeline/Calendari).

   2. Gestisci la **generazione rapporti legacy** nel modulo Flusso di lavoro per le parti interessate che non sono ancora pronte per passare all&#39;area di lavoro.

## Best practice e suggerimenti

### Effettua:

* **Attieniti prima al percorso principale.** Stabilisci il flusso da campagna a tattica a progetto prima di aggiungere ulteriore complessità.

* **Assegna aree di lavoro principali.** Assicurarsi che ogni tipo di record disponga di un&#39;area di lavoro &quot;principale&quot; (il centro di gravità) che funga da aggregatore per il reporting.

* **Assegna la priorità a Forms per l&#39;acquisizione.** Utilizzare i moduli record per gruppi meno sofisticati in Workfront Planning per garantire l&#39;integrità dei metadati. Anche se gli utenti esperti possono trarre vantaggio dall’inserimento diretto dei dati nelle visualizzazioni Tabella, questo approccio deve essere adottato con cautela: le modifiche in blocco in una tabella possono creare facilmente problemi di dati per altre parti interessate.


### Non:

* **Non dire &quot;Core&quot;.** Quando si parla di esecuzione, fare riferimento in modo specifico al **modulo flusso di lavoro** e agli oggetti **Progetto**.

* **Non complicare eccessivamente.** Ogni livello gerarchico aggiuntivo aggiunge una &quot;tassa di gestione&quot;. Aggiungere solo livelli che rispondono a una domanda di business a cui non è attualmente possibile rispondere.

* **Non creare silos.** Verificare che i tipi di record siano condivisi tra le aree di lavoro in modo che i team non digitino nuovamente gli stessi dati.




