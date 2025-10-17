---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Elencare oggetti con un processo di approvazione in sospeso utilizzando un determinato stato
description: Se si tenta di eliminare uno stato, è possibile che venga visualizzato un messaggio di errore che indica che non è possibile eliminarlo perché è utilizzato in processi di approvazione in sospeso sugli oggetti nel sistema. Se si desidera trovare ed esaminare tali oggetti per decidere cosa è necessario fare, è possibile eseguire un report che li elenca.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Elenca gli oggetti con un processo di approvazione in sospeso utilizzando un determinato stato

Se si tenta di eliminare uno stato, è possibile che venga visualizzato un messaggio di errore che indica che non è possibile eliminarlo perché è incluso in almeno un processo di approvazione in sospeso nel sistema. È possibile eseguire un report per elencare gli oggetti in cui si trova in un processo di approvazione in sospeso, quindi decidere cosa è necessario fare per ciascuno di essi.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td>
     <p>Standard</p>
     <p>Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td><p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p><p>Modifica accesso a Filtri, Viste, Raggruppamenti</p></td>
  </tr>
  <tr> 
   <td>Autorizzazioni oggetto</td> 
   <td>Ottieni le autorizzazioni di gestione per i rapporti creati.</td>
  </tr>
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## In modalità standard

{{step1-to-reports}}

1. Fai clic su **Nuovo rapporto**, quindi seleziona **Rapporto progetto**, **Rapporto attività** o **Rapporto problemi**.
1. Apri la scheda **Filtri**.
1. Fai clic su **Aggiungi regola filtro**, quindi effettua le seguenti operazioni per impostare la regola:
   1. Inizia a digitare `status`, quindi seleziona **Stato** quando viene visualizzato.
   1. Lascia **Equal** nel secondo campo.
   1. Seleziona il nome dello stato nel terzo campo.
1. Fai di nuovo clic su **Aggiungi una regola filtro**, quindi effettua le seguenti operazioni per impostare la regola
   1. Inizia a digitare `pending status`, quindi seleziona l&#39;elemento quando viene visualizzato nel tipo di oggetto in cui stai cercando (**Progetto**, **Attività** o **Problema**).
   1. Lascia **Equal** nel secondo campo.
   1. Digitare `in` nel terzo campo.
1. Fai di nuovo clic su **Aggiungi una regola filtro**, quindi effettua le seguenti operazioni per impostare la regola
   1. Inizia a digitare il processo di approvazione, quindi seleziona **ID gruppo** quando viene visualizzato in **Processo di approvazione**.
   1. Selezionare **È vuoto** nel secondo campo.
1. Fai clic su **Salva + Chiudi** per eseguire il report ed elencare tutti gli oggetti del tipo specificato con processi di approvazione in sospeso in base allo stato specificato (**Progetto**, **Attività** o **Problema**).
1. Ripetere questi passaggi per trovare le stesse informazioni per gli altri due tipi di oggetto.


## In modalità testo

{{step1-to-reports}}

1. Fai clic su **Nuovo rapporto**, quindi seleziona **Rapporto progetto**, **Rapporto attività** o **Rapporto problemi**.
1. Apri la scheda **Filtri**.
1. Selezionare **Passa alla modalità testo**.
1. Copiare e incollare quanto segue nella finestra di modifica, sostituendo XXX con la chiave di 3 lettere per lo stato:

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   Puoi visualizzare la chiave nell’elenco degli stati, come illustrato in questi articoli:
   * [Accedere all’elenco degli stati del progetto di sistema](project-statuses.md)
   * [Accedere all&#39;elenco degli stati delle attività di sistema](task-statuses.md)
   * [Accedere all’elenco degli stati dei problemi di sistema](issue-statuses.md)

1. Fai clic su **Salva + Chiudi** per eseguire il report ed elencare tutti gli oggetti del tipo specificato con processi di approvazione in sospeso in base allo stato specificato (**Progetto**, **Attività** o **Problema**).
1. Ripetere questi passaggi per trovare le stesse informazioni per gli altri due tipi di oggetto.
