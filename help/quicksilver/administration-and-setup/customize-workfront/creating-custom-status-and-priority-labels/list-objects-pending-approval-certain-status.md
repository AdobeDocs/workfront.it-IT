---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Elencare oggetti con processi di approvazione in sospeso utilizzando un determinato stato
description: Se tenti di eliminare uno stato, un messaggio di errore potrebbe indicarti che non può essere eliminato perché viene utilizzato nei processi di approvazione in sospeso sugli oggetti nel sistema. Se si desidera individuare e rivedere tali oggetti per decidere cosa è necessario eseguire, è possibile eseguire un rapporto che li elenchi.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Elencare oggetti con processi di approvazione in sospeso utilizzando un determinato stato

Se tenti di eliminare uno stato, un messaggio di errore potrebbe indicarti che non può essere eliminato perché si trova in almeno un processo di approvazione in sospeso nel sistema. È possibile eseguire un rapporto per elencare gli oggetti in cui si trova in un processo di approvazione in sospeso, quindi decidere cosa fare per ciascuno di essi.

## In modalità standard

1. Vai a **Reporting** nella barra di navigazione globale, quindi seleziona la **Rapporti** scheda .
1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon.png) nell&#39;angolo in alto a destra, quindi fai clic su **Rapporti**.
1. Fai clic su **Nuovo rapporto**, quindi seleziona **Rapporto sul progetto**, **Report attività** oppure **Report del problema**.
1. Apri **Filtri** scheda .
1. Fai clic su **Aggiungere una regola filtro**, quindi procedi come segue per impostare la regola:
   1. Inizia a digitare `status`, quindi seleziona **Stato** quando viene visualizzato.
   1. Esci **Uguale** nel secondo campo.
   1. Selezionare il nome dello stato nel terzo campo.
1. Fai clic su **Aggiungere una regola filtro** di nuovo, quindi procedi come segue per impostare la regola
   1. Inizia a digitare `pending status`, quindi selezionare l&#39;elemento quando viene visualizzato sotto il tipo di oggetto in cui si sta cercando (**Progetto**, **Attività** oppure **Problema**).
   1. Esci **Uguale** nel secondo campo.
   1. Tipo `in` nel terzo campo.
1. Fai clic su **Aggiungere una regola filtro** di nuovo, quindi procedi come segue per impostare la regola
   1. Inizia il processo di approvazione della digitazione, quindi seleziona **ID gruppo** quando viene visualizzato sotto **Processo di approvazione**.
   1. Seleziona **È vuoto** nel secondo campo.
1. Fai clic su **Salva e chiudi** per eseguire il rapporto ed elencare tutti gli oggetti del tipo specificato con i processi di approvazione in sospeso in base allo stato specificato (**Progetto**, **Attività** oppure **Problema**).
1. Ripetere questi passaggi per trovare le stesse informazioni per gli altri due tipi di oggetti.


## In modalità Testo

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon.png) nell&#39;angolo in alto a destra, quindi fai clic su **Rapporti**.
1. Fai clic su **Nuovo rapporto**, quindi seleziona **Rapporto sul progetto**, **Report attività** oppure **Report del problema**.
1. Apri **Filtri** scheda .
1. Seleziona **Passa alla modalità testo**.
1. Copia e incolla quanto segue nella finestra di modifica, sostituendo XXX con la chiave a 3 lettere per lo stato:

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   È possibile visualizzare la chiave nell’elenco degli stati, come illustrato in questi articoli:
   * [Accedere all’elenco degli stati del progetto di sistema](project-statuses.md)
   * [Accedere all&#39;elenco degli stati delle attività del sistema](task-statuses.md)
   * [Accedere all’elenco degli stati dei problemi del sistema](issue-statuses.md)

1. Fai clic su **Salva e chiudi** per eseguire il rapporto ed elencare tutti gli oggetti del tipo specificato con i processi di approvazione in sospeso in base allo stato specificato (**Progetto**, **Attività** oppure **Problema**).
1. Ripetere questi passaggi per trovare le stesse informazioni per gli altri due tipi di oggetti.
