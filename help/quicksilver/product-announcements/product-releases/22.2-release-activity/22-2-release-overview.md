---
title: Panoramica sulla versione 22.2
description: Panoramica sulla versione 22.2
author: Luke
draft: Probably
feature: Product Announcements
exl-id: e490a955-b2cb-4b9b-9794-12ff2a2c2338
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '3937'
ht-degree: 0%

---

# Panoramica sulla versione 22.2

Questa pagina fornisce informazioni sulle funzionalità incluse nella versione 22.2. Tutte le funzioni elencate sono disponibili nella nuova esperienza Adobe Workfront. Alcune funzioni sono disponibili anche in Adobe Workfront Classic; tuttavia, [Workfront Classic verrà interrotto a marzo 2022](https://one.workfront.com/s/new-workfront-experience), seguita a breve dalla data di fine del ciclo di vita di Workfront Classic nel luglio 2022.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
to help you unlock productivity and collaboration.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment. As the 22.2 release nears its planned Production release later this year
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
the week of January 17, 2022
</MadCap:conditionalText>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in October 2021
</MadCap:conditionalText>
, this page will be updated with all functionality included with 22.2. </p>
-->

Questi miglioramenti sono stati resi disponibili nell&#39;ambiente di produzione la settimana del 4 aprile 2022.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment and will be made available in the Production environment
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
later this year
</MadCap:conditionalText>
the week of April 4, 2022, unless otherwise specified. For specific release dates and times for each cluster, see the <a href="https://status.adobe.com/en/products/5943" target="_blank">Adobe Workfront status page</a> on <a href="http://status.adobe.com/" target="_blank">status.adobe.com</a>. You must log in to see specific release times. </p>
-->

## Miglioramenti di Adobe Workfront

* [Miglioramenti dell’amministratore](#administrator-enhancements)
* [Miglioramenti al progetto](#project-enhancements)
* [Miglioramenti a Gestione risorse](#resource-management-enhancements)
* [Miglioramenti a domicilio](#home-enhancements)
* [Miglioramenti a Mobile](#mobile-enhancements)
* [Miglioramenti alle integrazioni](#integrations-enhancements)
* [Altri miglioramenti](#other-enhancements)

### Miglioramenti dell’amministratore {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzione</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Configurare un modulo personalizzato per l’utilizzo con più tipi di oggetto</a> </p> <p>Ora è possibile configurare un modulo personalizzato nuovo o esistente per l’utilizzo con più tipi di oggetto, rendendo il modulo molto più utile. Gli utenti potranno allegare e compilare il modulo sugli oggetti di tutti i tipi per i quali lo si configura.</p> <p>In precedenza era possibile configurare un modulo personalizzato in modo che funzionasse con un solo tipo di oggetto.</p> <p>Questa funzionalità funziona con tutti i moduli personalizzati creati in precedenza nel sistema Workfront. Ad esempio, se si dispone già di un modulo personalizzato creato per il tipo di oggetto Task, è ora possibile configurarlo in modo che funzioni anche con altri tipi di oggetto, ad esempio Progetto e Problema.</p> </td> 
   <td> <p><b>Disponibile alle seguenti date:</b> </p> 
    <ul> 
     <li> <p>Anteprima versione: 10 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">Il catalogo Blueprint è disponibile per tutti gli utenti e gli amministratori possono consentire le richieste</a> </p> <p>Tutti gli utenti di Adobe Workfront possono ora sfogliare il catalogo delle blueprint disponibili. </p> <p>Inoltre, l'amministratore di sistema può consentire agli utenti di accedere per richiedere l'installazione dei progetti. L’assegnazione di una coda di richiesta per memorizzare le richieste consente agli utenti di effettuare richieste dal catalogo blueprint. </p> </td> 
   <td> <p><b>Disponibile alle seguenti date:</b> </p> 
    <ul> 
     <li> <p>Anteprima versione: 10 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#add" class="MCXref xref" xrefformat="{para}">Aggiungere un’immagine a un modulo personalizzato</a> </p> <p>In un modulo personalizzato creato o modificato, è ora possibile aggiungere un’immagine e includere una descrizione delle informazioni o delle istruzioni che gli utenti possono leggere quando passano il puntatore del mouse su di essa.</p> <p>Questo potrebbe essere utile, ad esempio, per mostrare il branding per un nuovo prodotto o per fornire informazioni visive di cui gli utenti hanno bisogno durante la compilazione del modulo.</p> <p>In precedenza, i moduli personalizzati erano completamente basati su testo.</p> </td> 
   <td> <p><b>Disponibile alle seguenti date:</b> </p> 
    <ul> 
     <li> <p>Anteprima versione: 10 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#deactiva" class="MCXref xref" xrefformat="{para}">Disattivare un gruppo</a> </p> <p>Quando le organizzazioni interne cambiano, potrebbe essere necessario interrompere l’utilizzo di determinati gruppi in Workfront e crearne di nuovi. Per facilitare questa fase, abbiamo aggiunto la possibilità di disattivare un gruppo senza perdere i dati storici. Per gli utenti abituali che non hanno bisogno di visualizzarli, i gruppi inattivi vengono cancellati dai campi tipo-avanti del gruppo.</p> <p>È comunque possibile trovare e configurare opzioni, preferenze e associazioni di oggetti per i gruppi inattivi gestiti. La disattivazione di un gruppo non comporta alcuna modifica per gli oggetti a cui è associato il gruppo.</p> <p>In precedenza, non era possibile disattivare un gruppo.</p> </td> 
   <td> <p><b>Disponibile alle seguenti date:</b> </p> 
    <ul> 
     <li> <p>Anteprima versione: 10 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuove configurazioni predefinite del livello di accesso</a> </p> <p>Per soddisfare meglio le esigenze della maggior parte degli amministratori che creano i livelli di accesso, abbiamo modificato la configurazione predefinita per diverse opzioni di "Ottimizza le impostazioni" che vengono visualizzate quando fai clic sull’icona a forma di ingranaggio su un pulsante Modifica.</p> <p>Le opzioni, precedentemente abilitate per impostazione predefinita, ora sono disabilitate. Se questo non soddisfa le esigenze della tua organizzazione, puoi attivarli quando imposti un nuovo livello di accesso o in un secondo momento.</p> </td> 
   <td> <p><b>Disponibile alle seguenti date:</b> </p> 
    <ul> 
     <li> <p>Anteprima versione: 27 gennaio 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic verrà interrotto a marzo 2022</a>, seguita a breve dalla data di fine del ciclo di vita di Workfront Classic nel luglio 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#blueprin2" class="MCXref xref" xrefformat="{para}">Miglioramenti alla cronologia dell’installazione di Blueprint</a> </p> <p>Quando si installa una blueprint, ora viene visualizzato un messaggio per visualizzare gli oggetti specifici (ad esempio ruoli, team o gruppi) che sono stati installati correttamente con la blueprint ed eventuali oggetti che non sono stati installati. È inoltre possibile visualizzare l’elenco degli oggetti installati nella pagina Dettagli blueprint facendo clic su Visualizza dettagli accanto a una specifica installazione nella tabella della cronologia dell’installazione.</p> </td> 
   <td> <p><b>Disponibile alle seguenti date:</b> </p> 
    <ul> 
     <li> <p>Anteprima versione: 10 febbraio 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#a" class="MCXref xref" xrefformat="{para}">Viene ora visualizzato un avviso durante l’installazione di una blueprint solo anteprima in Produzione</a> </p> <p>Alcuni blueprint sono disponibili solo per l’installazione nell’ambiente di anteprima a scopo di test.</p> <p>Se accedi al contenuto solo anteprima nell’ambiente di produzione, Sandbox 1 o Sandbox 2, il pulsante di installazione non è attivo e potresti visualizzare un messaggio di avviso.</p> </td> 
   <td><b>Disponibile alle seguenti date:</b> 
    <ul> 
     <li> <p>Anteprima versione: 10 febbraio 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Miglioramenti al progetto {#project-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzione</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#adobe" class="MCXref xref" xrefformat="{para}">Sono ora disponibili le bacheche Adobe Workfront. </a> </p> <p>Le bacheche sono strumenti flessibili che consentono la collaborazione del team fornendo l'accesso a una bacheca condivisa contenente colonne e schede. </p> <p>Utilizzando le bacheche, potete configurare rapidamente una bacheca con più colonne, configurare le colonne per mostrare uno stato o una categoria, aggiungere altri utenti alla bacheca e assegnarli alle schede e altro ancora.</p> </td> 
   <td> <p><b>Disponibile alle seguenti date:</b> </p> 
    <ul> 
     <li> <p>Anteprima versione: 10 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#addition" class="MCXref xref" xrefformat="{para}">Ulteriori miglioramenti alle schede Workfront</a></p> <p>Per le bacheche Workfront sono ora disponibili i seguenti miglioramenti aggiuntivi:</p> 
    <ul> 
     <li> <p>Assegnare tag alle schede sulle bacheche</p> </li> 
     <li> <p>Sposta schede</p> </li> 
     <li> <p>Copia schede</p> </li> 
     <li> <p>Cerca nelle bacheche</p> </li> 
     <li> <p>Impostare una data di scadenza per una scheda nelle bacheche</p> </li> 
    </ul> </td> 
   <td><b>Disponibile alle seguenti date:</b> 
    <ul> 
     <li> <p>Anteprima versione: 24 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#undo" class="MCXref xref" xrefformat="{para}">Opzione Annulla per aggiornare i post</a> </p> <p>È ora più facile rilevare gli errori durante la pubblicazione di un aggiornamento. Quando si completa un commento nella scheda Aggiorna di un oggetto, ora viene creata una finestra a comparsa per 7 secondi che consente di annullare il post e tornare alla modifica prima che il sistema lo marchi in tempo o invii e-mail e notifiche in-app. Se si chiude la finestra a comparsa, si esce dalla pagina o si attendono 7 secondi prima che la finestra si interrompa, il post verrà effettuato normalmente.</p> </td> 
   <td> <p><b>Disponibile alle seguenti date:</b> </p> 
    <ul> 
     <li> <p>Anteprima versione: 10 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuova esperienza durante la copia di un progetto</a> </p> <p>Per rendere coerente l’utilizzo di Workfront con la nuova esperienza Adobe Workfront, abbiamo riprogettato l’interfaccia per la copia dei progetti. Questa opzione è disponibile quando si copia un progetto dalla pagina del progetto o quando si copia un progetto da un elenco o da un rapporto. Prima di questo aggiornamento era possibile copiare un progetto solo dalla pagina del progetto.</p> </td> 
   <td> <p><b>Disponibile alle seguenti date:</b> </p> 
    <ul> 
     <li> <p>Anteprima versione: 10 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#ability" class="MCXref xref" xrefformat="{para}">Possibilità di gestire progetti da elenchi e rapporti da un nuovo menu Altro</a> </p> <p>È stato aggiunto un nuovo menu Altro negli elenchi e nei rapporti dei progetti per consentire di eseguire le azioni seguenti da queste aree:</p> 
    <ul> 
     <li> <p>Per diversi progetti alla volta:</p> </li> 
     <li> <p>Ricalcola timeline</p> </li> 
     <li> <p>Ricalcola Finanze</p> </li> 
     <li> <p>Ricalcolare Espressioni Customizzate</p> </li> 
     <li> <p>Per un singolo progetto:</p> </li> 
     <li> <p>Allega Modello</p> </li> 
     <li> <p>Esporta in MS Project</p> </li> 
     <li> <p>Iscrizione</p> </li> 
    </ul> </td> 
   <td> <p><b>Disponibile alle seguenti date:</b> </p> 
    <ul> 
     <li> <p>Anteprima versione: 10 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Nuova esperienza durante la conversione di un problema in un progetto utilizzando un modello a livello di problema</a> </p> <p>Per rendere coerente l’utilizzo di Workfront con la nuova esperienza Workfront, abbiamo riprogettato l’interfaccia per la conversione di un problema in un progetto quando si utilizza un modello quando lo si converte dalla pagina del problema.</p> <p>Ora puoi accedere più facilmente all’elenco dei preferiti immediatamente dopo aver selezionato per convertire il problema.</p> <p>L’interfaccia riprogettata corrisponde all’esperienza acquisita durante la creazione di un progetto da un modello, anch’esso aggiornato di recente.</p> </td> 
   <td><strong>Disponibile alle seguenti date:</strong> 
    <ul> 
     <li> <p>Anteprima versione: 8 dicembre 2021<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.1 <span style="color: #ff0000; font-weight: bold;">Questa funzione è stata temporaneamente rimossa dall’ambiente di produzione il 4 marzo 2022. È stato successivamente pubblicato in un roll-out graduale a partire dal 28 aprile 2022. L’implementazione è stata completata il 5 maggio 2022. Questa funzione è ora disponibile in Anteprima e Produzione per tutti i clienti.</span></p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#convert" class="MCXref xref" xrefformat="{para}">Convertire i problemi in progetti utilizzando un modello da elenchi, rapporti e dashboard</a> </p> <p>Per aumentare l’efficienza del lavoro e semplificare la conversione dei problemi in un ambiente ad alta velocità, abbiamo aggiunto la possibilità di convertire un problema in un progetto utilizzando un modello da un elenco, un rapporto o un dashboard.</p> <p>Prima di questo miglioramento, questa funzionalità esisteva solo quando il problema era stato convertito dalla pagina del problema.</p> </td> 
   <td><strong>Disponibile alle seguenti date:</strong> 
    <ul> 
     <li> <p>Anteprima versione: 8 dicembre 2021<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.1 <span style="color: #ff0000; font-weight: bold;">Questa funzione è stata temporaneamente rimossa dall’ambiente di produzione il 4 marzo 2022. È stato successivamente pubblicato in un roll-out graduale a partire dal 28 aprile 2022. L’implementazione è stata completata il 5 maggio 2022. Questa funzione è ora disponibile in Anteprima e Produzione per tutti i clienti.</span></p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">È stata aggiornata l’esperienza durante la copia e lo spostamento dei problemi</a> </p> <p>Per rendere coerente l’utilizzo di Workfront con la nuova esperienza Adobe Workfront, abbiamo riprogettato l’interfaccia per problemi di copia e spostamento. Questa opzione è attualmente disponibile quando si copia o si sposta un singolo problema o quando si copiano o si spostano problemi in blocco da un elenco o da un report.</p> </td> 
   <td><strong>Disponibile alle seguenti date:</strong> 
    <ul> 
     <li> <p>Anteprima versione: 18 febbraio 2022<br></p> </li> 
     <li> <p>Versione di produzione: Con la versione 22.2</p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#keep" class="MCXref xref" xrefformat="{para}">Mantieni gli utenti nel dashboard, nell’elenco o nel rapporto dopo la conversione del problema in progetto</a> </p> <p>Per aumentare l’efficienza ed eliminare il numero di clic, è stato rilasciato un miglioramento durante la conversione dei problemi in progetti da un elenco, report o dashboard.</p> <p>Dopo la conversione di un problema in un progetto, gli utenti rimangono nell’elenco, nel rapporto o in una dashboard anziché essere reindirizzati alla pagina del progetto. Al termine della conversione viene visualizzata una notifica di successo con il collegamento al progetto, per consentirti di passare facilmente al progetto, se necessario. </p> </td> 
   <td><strong>Disponibile alle seguenti date:</strong> 
    <ul> 
     <li> <p>Anteprima versione: 10 febbraio 2022<br></p> </li> 
     <li> <p>Versione di produzione: 24 febbraio 2022</p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#allocati" class="MCXref xref" xrefformat="{para}">Le ore di allocazione non verranno più rimosse quando si apportano modifiche alle assegnazioni</a> </p> <p>Per garantire l'accuratezza dei dati, è stata apportata una modifica per mantenere le ore di allocazione e per mantenere invariata l'ora pianificata delle attività quando si apportano modifiche alle assegnazioni dell'attività.</p> <p>Sono state apportate le seguenti modifiche alle attività con un tipo di durata semplice:</p> 
    <ul> 
     <li> <p>Le allocazioni di assegnazione individuali vengono mantenute quando si sostituiscono utenti e ruoli.</p> </li> 
     <li> <p>Le allocazioni di assegnazione individuali vengono mantenute sul ruolo durante la rimozione dell'utente.</p> </li> 
     <li> <p>Le ore pianificate vengono mantenute quando si rimuovono tutti gli assegnatari. <span style="color: #ff0000;">(Rimosso dal rilascio. Ora, l'ora pianificata sarà impostata su 0 dopo aver rimosso tutti gli assegnatari.)</span></p> </li> 
    </ul> </td> 
   <td><strong>Disponibile alle seguenti date:</strong> 
    <ul> 
     <li> <p>Anteprima versione: 10 febbraio 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 <span style="color: #ff0000; font-weight: bold;">Questa funzione verrà rilasciata in produzione poco dopo la versione 22.2</span></p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic verrà interrotto a marzo 2022</a>, seguita a breve dalla data di fine del ciclo di vita di Workfront Classic nel luglio 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#share" class="MCXref xref" xrefformat="{para}">Condividere le cartelle solo nei primi cinque livelli di una gerarchia di cartelle</a> </p> <p>Per garantire le migliori prestazioni agli utenti che condividono le cartelle, al momento la condivisione è limitata ai primi cinque livelli della gerarchia delle cartelle su un oggetto.</p> <p>Ogni cartella al sesto livello o inferiore eredita le configurazioni di condivisione dalla cartella direttamente sopra di essa.</p> </td> 
   <td><strong>Disponibile alle seguenti date:</strong> 
    <ul> 
     <li> <p>Anteprima versione: 10 febbraio 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 <span style="color: #ff0000; font-weight: bold;">Funzione temporaneamente non disponibile. Questa pagina viene aggiornata quando la funzione è disponibile in Produzione.</span></p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic verrà interrotto a marzo 2022</a>, seguita a breve dalla data di fine del ciclo di vita di Workfront Classic nel luglio 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Miglioramenti a Gestione risorse {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzione</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">Miglioramenti alla navigazione del bilanciamento del carico di lavoro</a> </p> <p>Per migliorare la tua esperienza quando utilizzi il servizio di bilanciamento del carico di lavoro, sono stati introdotti i seguenti miglioramenti:</p> 
    <ul> 
     <li> <p>I pulsanti Annulla e Salva quando si regolano le allocazioni sono ora permanenti, anche quando l’attività è più lunga dell’intervallo di tempo incluso nella schermata o quando viene visualizzato il pannello Riepilogo .</p> </li> 
     <li> <p>Il pannello a sinistra che visualizza i nomi degli utenti e degli elementi di lavoro è ora appiccicoso, consente di scorrere in orizzontale per intervalli di tempo più lunghi e di poter comunque leggere i nomi degli elementi elencati nel pannello.</p> </li> 
     <li> <p>Puoi comprimere ed espandere tutti gli elementi elencati nel pannello a sinistra con un solo clic invece che a livello di utente o di progetto.</p> </li> 
     <li> <p>È ora possibile ridimensionare anche il pannello a sinistra.</p> </li> 
     <li> <p>È ora disponibile una modalità a schermo intero per il bilanciamento del carico di lavoro.</p> </li> 
    </ul> </td> 
   <td> <p><b>Disponibile alle seguenti date:</b> </p> 
    <ul> 
     <li> <p>Anteprima versione: 10 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#access" class="MCXref xref" xrefformat="{para}">Accedere alle assegnazioni avanzate nel load balancer</a> </p> <p>Per semplificare e rendere più precisa l'assegnazione degli elementi di lavoro, è ora possibile effettuare assegnazioni avanzate quando si assegnano gli elementi di lavoro manualmente nel servizio di bilanciamento del carico di lavoro. Prima di questo miglioramento, era possibile accedere ad Assegnazioni avanzate durante la modifica di elementi, dalle intestazioni degli elementi o negli elenchi.</p> </td> 
   <td> <p><b>Disponibile alle seguenti date:</b> </p> 
    <ul> 
     <li> <p>Anteprima versione: 10 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuova formula per il calcolo della disponibilità dell'utente quando è selezionata la preferenza Pianificazione predefinita</a> </p> <p>Per fornire informazioni più precise negli strumenti di gestione delle risorse, abbiamo modificato la formula utilizzata da Workfront per calcolare la disponibilità degli utenti quando l’amministratore di Workfront seleziona La pianificazione predefinita nelle preferenze di gestione delle risorse. Con il nuovo aggiornamento, Workfront utilizza la seguente formula per calcolare la disponibilità degli utenti:</p> <p>Orari disponibili dell'utente = (ore di programmazione predefinite - Eccezioni) * FTE - Ora di pausa</p> <p>Prima di questo aggiornamento, Workfront utilizzava la seguente formula per calcolare la disponibilità dell’utente quando era selezionata la pianificazione predefinita:</p> <p>Orari disponibili dell’utente = (ore di pianificazione predefinite - (eccezioni di pianificazione + ore di inattività) * Valore FTE dell’utente</p> </td> 
   <td> <p><b>Disponibile alle seguenti date:</b> </p> 
    <ul> 
     <li> <p>Anteprima versione: 10 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic verrà interrotto a marzo 2022</a>, seguita a breve dalla data di fine del ciclo di vita di Workfront Classic nel luglio 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Miglioramenti a domicilio {#home-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzione</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-home-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">Miglioramenti ai filtri nell'elenco Home Work</a> </p> <p>Per dare maggiore controllo e focus sulla tua lista di lavoro, abbiamo implementato diversi miglioramenti ai filtri nell'area Home. Con i nuovi miglioramenti, è possibile selezionare i filtri per tipo di oggetto e limitare ulteriormente i risultati in base allo stato degli elementi di lavoro (ad esempio, Pronti per iniziare, Lavoro su o Richiesto). I nuovi filtri Home forniscono ora un conteggio corretto delle attività, dei problemi, degli elementi di lavoro personali e delle approvazioni quando si applica una combinazione di filtri per il tipo di oggetto e lo stato dell'elemento di lavoro.</p> <p>Prima di questa esperienza, i filtri nell'area Home non fornivano un conteggio accurato del numero di elementi di lavoro nell'elenco quando si selezionavano uno o più filtri e creavano confusione sullo stato degli elementi di lavoro.</p> </td> 
   <td> <p><b>Disponibile alle seguenti date:</b> </p> 
    <ul> 
     <li> <p>Anteprima versione: 10 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Miglioramenti a Mobile {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzione</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-mobile-enhancements.md#drawings" class="MCXref xref" xrefformat="{para}">Disegni e commenti sui documenti di prova nell’app mobile</a></p> <p>L’app mobile Adobe Workfront ora consente di aggiungere disegni e commenti ai documenti di prova. Una nuova barra degli strumenti della bozza contiene strumenti di disegno per le forme. È possibile scegliere impostazioni quali colore e spessore della linea per ogni forma. Il disegno di una forma sulla bozza consente di collegare il commento all'area del documento di prova.</p> <p>Potete anche rispondere alle osservazioni che altri hanno formulato sulla prova.</p> </td> 
   <td><strong>Disponibile alle seguenti date:</strong> 
    <ul> 
     <li> <p>Anteprima versione: N/D<br></p> </li> 
     <li> <p>Versione di produzione: da metà a fine aprile 2022 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>App mobile iOS</p> </li> 
     <li> <p>App mobile Android</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-mobile-enhancements.md#enhancem" class="MCXref xref" xrefformat="{para}">Miglioramenti alla funzionalità di bozza nell’app mobile</a> </p> <p>Nell’app mobile Adobe Workfront, ora puoi:</p> 
    <ul> 
     <li> <p>Condivisione di bozze con destinatari interni ed esterni</p> </li> 
     <li> <p>Visualizza commenti della bozza</p> </li> 
     <li> <p>Scarica bozze</p> </li> 
    </ul> </td> 
   <td><strong>Disponibile alle seguenti date:</strong> 
    <ul> 
     <li> <p>Anteprima versione: N/D<br></p> </li> 
     <li> <p>Versione di produzione: primi di febbraio 2022 (questi miglioramenti sono stati originariamente comunicati con la versione 22.1).</p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>App mobile iOS</p> </li> 
     <li> <p>App mobile Android</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Miglioramenti alle integrazioni {#integrations-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzione</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#adobe" class="MCXref xref" xrefformat="{para}">È ora disponibile l’integrazione Adobe Workfront con Anaplan</a> </p> <p>Per offrirti una maggiore flessibilità e una migliore comprensione degli aspetti finanziari dei tuoi progetti Workfront, Workfront può ora integrarsi con il tuo account Anaplan. Collegando gli oggetti Workfront agli oggetti Anaplan, è possibile aggiornare automaticamente le informazioni tra i due account, garantendo che le informazioni in entrambi siano aggiornate e identiche. </p> <p>Puoi anche attivare i processi automatizzati in Anaplan in base alle azioni in Workfront (o viceversa).</p> <p>Ad esempio, puoi creare una campagna in Anaplan, quindi creare un progetto o un programma Workfront collegato alla campagna. Eventuali costi tracciati in Workfront possono quindi essere caricati nuovamente su Anaplan per esaminare le prestazioni della campagna.</p> </td> 
   <td><strong>Disponibile alle seguenti date:</strong> 
    <ul> 
     <li> <p>Anteprima versione: 10 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: Con la versione 22.2</p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Workfront per Experience Manager aggiornamenti avanzati dei connettori</a> </p> <p>Workfront, ad Experience Manager, include ora i seguenti aggiornamenti:</p> 
    <ul> 
     <li> <p>È ora possibile creare cartelle collegate tra Adobe Workfront e Adobe Experience Manager Assets as a Cloud Service anche se sono presenti più configurazioni di cartelle collegate al progetto.</p> </li> 
     <li> <p>È stato aggiunto il supporto per l’impaginazione dell’abbonamento a un evento</p> </li> 
     <li> <p>È stato aggiunto il supporto per AEM 6.4.x</p> </li> 
     <li> <p>È stato aggiunto il supporto per gli ambienti proxy</p> </li> 
     <li> <p>Diverse correzioni di bug in base al feedback di partner e clienti</p> </li> 
    </ul> </td> 
   <td><strong>Disponibile alle seguenti date:</strong> 
    <ul> 
     <li> <p>Anteprima versione: N/D<br></p> </li> 
     <li> <p>Versione di produzione: 28 marzo 2022</p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#see" class="MCXref xref" xrefformat="{para}">Vedi i dettagli del segreto client per le integrazioni personalizzate OAuth2 o JWT</a> </p> <p>Per garantire la trasparenza nell’utilizzo delle integrazioni personalizzate OAuth2 e JWT, abbiamo reso possibile la visualizzazione dei dettagli dei Segreti client utilizzati dalle integrazioni. Ora puoi vedere le date di creazione e dell’ultimo utilizzo del Segreto client. È inoltre possibile aggiungere e visualizzare le proprie note sul Segreto client.</p> <p>In precedenza, questi dettagli non erano disponibili.</p> </td> 
   <td><strong>Disponibile alle seguenti date:</strong> 
    <ul> 
     <li> <p>Anteprima versione: 3 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: Con la versione 22.2</p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#adobe2" class="MCXref xref" xrefformat="{para}">Le integrazioni Adobe Creative Cloud ora utilizzano OAuth2</a> </p> <p>Per una maggiore sicurezza e per fare un’esperienza più coerente tra le integrazioni, abbiamo aggiornato le integrazioni Adobe Creative Cloud per utilizzare l’autenticazione OAuth2, un metodo standard di settore per l’autenticazione degli utenti. Ora, quando gli utenti effettuano l’accesso, possono visualizzare le azioni e le aree specifiche a cui le integrazioni hanno accesso e consentire l’accesso. In seguito, non è necessario effettuare l’accesso con la stessa frequenza.</p> </td> 
   <td><strong>Disponibile alle seguenti date:</strong> 
    <ul> 
     <li> <p>Anteprima versione: 24 febbraio 2022<br></p> </li> 
     <li> <p>Versione di produzione: Con la versione 22.2</p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#see2" class="MCXref xref" xrefformat="{para}">Vedi il tipo di autenticazione nell’elenco delle applicazioni OAuth2 personalizzate</a> </p> <p>Ora, quando visualizzi l’elenco delle applicazioni OAuth2 personalizzate nella tua organizzazione, puoi vedere se ogni applicazione utilizza l’autenticazione utente o l’autenticazione server.</p> <p>In precedenza, era possibile visualizzare queste informazioni solo andando nelle opzioni di modifica su ogni applicazione.</p> </td> 
   <td><strong>Disponibile alle seguenti date:</strong> 
    <ul> 
     <li> <p>Anteprima versione: 17 febbraio 2022<br></p> </li> 
     <li> <p>Versione di produzione: Con la versione 22.2</p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#set" class="MCXref xref" xrefformat="{para}">Imposta la scadenza per i token di aggiornamento nelle integrazioni personalizzate OAuth2</a> </p> <p>Per controllare meglio l’accesso e la sicurezza per le integrazioni OAuth2 personalizzate, ora puoi personalizzare la durata dei token di aggiornamento. Dopo la scadenza del token di aggiornamento di un utente, dovrà accedere nuovamente all’integrazione.</p> </td> 
   <td> <p><b>Disponibile alle seguenti date:</b> </p> 
    <ul> 
     <li> <p>Anteprima versione: 10 febbraio 2022 <br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#use" class="MCXref xref" xrefformat="{para}">Utilizza le chiavi pubbliche e private nelle integrazioni personalizzate OAuth2 per le app da server a server</a> </p> <p>È ora possibile configurare le applicazioni OAuth2 server-to-server nelle integrazioni personalizzate. Impostando le chiavi pubblica e privata, puoi consentire a Workfront di comunicare con un’altra applicazione senza utilizzare le credenziali di accesso.</p> <p>In precedenza, tutte le autenticazioni nelle applicazioni OAuth2 personalizzate utilizzavano le credenziali di accesso dell’utente.</p> </td> 
   <td> <p><b>Disponibile alle seguenti date:</b> </p> 
    <ul> 
     <li> <p>Anteprima versione: 10 febbraio 2022 <br></p> </li> 
     <li> <p>Versione di produzione: con la versione 22.2 </p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Altri miglioramenti {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzione</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-look-and-feel-updates.md#enhancem" class="MCXref xref" xrefformat="{para}">Aggiornamenti look-and-feel durante l’intervallo di rilascio della versione 22.2</a> </p> <p>Sono in corso aggiornamenti minori all’aspetto e all’aspetto di varie aree dell’applicazione Adobe Workfront entro l’intervallo di tempo previsto per la versione 22.2. Questi miglioramenti saranno resi disponibili nell'ambiente di produzione almeno 2 settimane dopo il rilascio in anteprima. </p> </td> 
   <td><strong>Disponibile alle seguenti date:</strong> 
    <ul> 
     <li> <p>Anteprima versione: nell’arco temporale della versione 22.2<br></p> </li> 
     <li> <p>Versione di produzione: almeno 2 settimane dopo il rilascio in anteprima</p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-other-enhancements.md#enhancem" class="MCXref xref" xrefformat="{para}">Miglioramenti alla barra di navigazione superiore</a> </p> <p>Sono stati apportati diversi miglioramenti alla barra di navigazione superiore di Adobe Workfront.</p> 
    <ul> 
     <li> <p>I Preferiti e i Recenti dispongono ora di icone separate nella barra di navigazione superiore. Ciascuna visualizza comunque lo stesso contenuto (pagine contrassegnate come preferiti e pagine visitate di recente) e puoi continuare ad aggiungere e rimuovere le pagine preferite nello stesso modo.</p> </li> 
     <li> <p>L'aspetto dei perni e del menu principale è stato aggiornato agli standard di design Adobi, compresi colori e caratteri. La modalità di aggiunta e rimozione dei perni e delle aree a cui hai accesso nel menu principale non sono state modificate.</p> </li> 
     <li> <p>Le icone a destra della barra di navigazione superiore sono state riordinate in modo da essere più intuitive. L’ordine delle icone è: collegamento di aiuto, notifiche, preferiti, recenti, ricerca, menu principale.</p> </li> 
    </ul> </td> 
   <td><strong>Disponibile alle seguenti date:</strong> 
    <ul> 
     <li> <p>Anteprima versione: 10 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: Con la versione 22.2</p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-other-enhancements.md#redesign" class="MCXref xref" xrefformat="{para}">Elenchi schede attività riprogettati</a> </p> <p>Per rendere coerente l’utilizzo di Workfront con la nuova esperienza Adobe Workfront, abbiamo riprogettato gli elenchi delle schede attività nell’area Foglio presenze . È possibile prevedere la stessa funzionalità nell'elenco della scheda attività, solo con un'esperienza utente più pulita e più semplice.</p> <p>Alcuni degli elementi di rilievo di questa riprogettazione sono:</p> 
    <ul> 
     <li> <p>L'elenco delle schede attività ora corrisponde all'esperienza in tutti gli altri elenchi in Workfront.</p> </li> 
     <li> <p>L’esperienza di filtro ora corrisponde ai filtri presenti in tutti gli altri elenchi. Potrai creare filtri personalizzati con i campi e gli attributi più appropriati e condividerli con altri utenti.</p> </li> 
    </ul> </td> 
   <td><strong>Disponibile alle seguenti date:</strong> 
    <ul> 
     <li> <p>Anteprima versione: 10 marzo 2022<br></p> </li> 
     <li> <p>Versione di produzione: Con la versione 22.2</p> </li> 
    </ul> <p><strong>Disponibile nei seguenti ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Miglioramenti a Workfront Fusion

Le nuove funzioni di Workfront Fusion sono disponibili in Produzione a cadenza inferiore alla pianificazione della versione 22.2. Per ulteriori informazioni sulle funzioni più recenti, consulta [Attività di rilascio di Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

## Miglioramenti a Workfront Scenario Planner

A questo punto della versione non sono disponibili aggiornamenti per la pianificazione degli scenari. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features are coming to Workfront Scenario Planner release with the 21.4 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Scenario Planner release activity</a>.</p>
-->

## Miglioramenti a prova di Workfront

A questo punto della versione non sono disponibili aggiornamenti di prova Workfront. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features in Workfront Proof are now available. For more information, see <a href="../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-22-1.md" class="MCXref xref" xrefformat="{para}">Workfront Proof release activity:&nbsp;Week of November 29, 2021</a>.</p>
-->

## Miglioramenti agli obiettivi di Workfront

A questo punto della versione non sono disponibili aggiornamenti di obiettivi Workfront. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Most new features coming to Workfront Goals release with the 21.2 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Adobe Workfront Goals with the 21.2 release</a>.</p>
-->

## API versione 14

Per l’API versione 14, abbiamo modificato alcune risorse e alcuni endpoint. Alcune delle modifiche supportano nuove funzionalità, altre le semplificano nell’utilizzo delle informazioni disponibili tramite l’API.

Per informazioni sulle novità e gli aggiornamenti, consulta [Novità dell’API versione 14](../../../wf-api/api/new-api-version-14.md).

Per informazioni sulle versioni API, consulta [Controllo delle versioni e pianificazione del supporto API](../../../wf-api/api/api-version-support-schedule.md).

## Aggiornamenti di manutenzione per Workfront

Per informazioni sugli aggiornamenti di manutenzione effettuati durante la versione 22.2, consulta [Aggiornamenti alla manutenzione di Workfront](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## Webinar sulla versione 22.2

Il webinar sulla versione Workfront 22.2 verrà presentato il 24 marzo 2022 alle 08:00 MST. È possibile registrarsi per l&#39;evento nella [Pagina Eventi in Workfront One](https://webinars.on24.com/adobe_workfront/WF22point2?partnerref=WFOne).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This area will be updated as more information becomes available.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
was presented on January 12, 2022. You can view the webinar recording on the
<a href="https://one.workfront.com/s/event">Events page on Workfront One</a>.
</MadCap:conditionalText>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Functionality being removed from Production</h2>
<h3>Feature rollback: Carry over the existing proof workflow when generating a new version</h3>
<p>Due to customer feedback, <b>Workfront is removing this change from Preview environments on March 30, 2021 and from Production environments on March 31, 2021</b>.</p>
<p>On March 11, 2021, Workfront released a change to existing proof workflows in both Workfront Classic and the new Workfront experience. The change allowed for an existing workflow to carry over to any new proof versions created by a user, regardless of the method used to generate them.</p>
<p>In the new Workfront experience after this change is removed, proofs created with the Simple proof selection will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>In Workfront Classic after this change is removed, the option to Generate Proof will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>Similar functionality to easily copy existing workflows might be added to Production at a future time.</p>
</div>
-->

## Aggiornamenti alla formazione

Scopri gli ultimi aggiornamenti apportati a programmi di apprendimento, percorsi di apprendimento, video e guide per ogni versione del prodotto Adobe Workfront. Per ulteriori informazioni, consulta la sezione [Pagina degli aggiornamenti della versione di formazione](https://one.workfront.com/s/training-release-updates).

## Funzionalità non più supportata

### Internet Explorer 11

Con la rimozione del supporto per Internet Explorer, Workfront ora supporta ufficialmente Microsoft Edge.

Per ulteriori informazioni sui browser supportati, consulta [Requisiti del browser Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).
