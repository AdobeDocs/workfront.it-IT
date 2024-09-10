---
title: Visualizza informazioni di accesso utente
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Puoi verificare la frequenza con cui gli utenti accedono a Workfront, nonché l’ultima volta che hanno effettuato l’accesso, indicando che desideri includere queste informazioni nella visualizzazione di un elenco di utenti o in un rapporto per gli utenti.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 1%

---

# Visualizza informazioni di accesso utente

Puoi vedere con quale frequenza gli utenti accedono ad Adobe Workfront, nonché l’ultima volta che hanno effettuato l’accesso, indicando che desideri includere queste informazioni nella visualizzazione di un elenco di utenti o in un rapporto per gli utenti.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p><p>Oppure</p><p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>È necessario disporre di uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Livello di accesso Amministratore di sistema. </li> 
     <li> <p>Impostazione di <b>Utenti</b> nel livello di accesso configurato per l'accesso di <b>Modifica</b>, con <b>Crea</b> e almeno una delle due opzioni di <b>Amministratore utenti</b> abilitate in <b>Ottimizza le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se <b>User Admin (Group Users)</b> è abilitato, è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Registrazione delle informazioni di accesso in Workfront

Workfront registra le seguenti informazioni sugli utenti che accedono al sistema:

* **Conteggio accessi**: Workfront conta un utente che accede all&#39;applicazione una volta ogni 24 ore. Se un utente effettua l’accesso più volte utilizzando browser, computer o dispositivi mobili diversi, Workfront conta tutti gli accessi che si sono verificati in un giorno come un unico accesso. Il conteggio degli accessi include informazioni che iniziano con la data di creazione dell’utente.
* **Ultima data di accesso**: l&#39;ultima data di accesso di un utente. In questo campo viene registrata la data di ogni accesso da qualsiasi browser, dispositivo mobile o altre applicazioni.

L’accesso a Workfront può essere considerato come un accesso a Workfront in uno dei seguenti modi:

* Applicazione Web Workfront
* App mobili Workfront (dispositivi iOS o Android)
* Qualsiasi integrazione Workfront supportata con un’altra applicazione di terze parti (Slack, Jira)
* Qualsiasi integrazione personalizzata tra Workfront e un’altra applicazione di terze parti.
* API di Workfront

  >[!NOTE]
  >
  >L’accesso a Workfront tramite l’API Workfront è disponibile solo per le organizzazioni che non sono ancora state caricate su Adobe Business Platform.

## Visualizzare le informazioni sull&#39;utilizzo in un elenco di utenti o in un report

Puoi visualizzare i campi Conteggio e Data ultimo accesso nella visualizzazione di un elenco di utenti o in un rapporto per gli utenti.\
Per ulteriori informazioni sulla creazione di un report, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Per visualizzare le informazioni sull&#39;utilizzo nella visualizzazione di un elenco di utenti:

1. Vai a un elenco di utenti in Workfront.
1. Dal menu a discesa **Visualizza**, selezionare **Nuova visualizzazione**.

1. Fai clic su **Aggiungi colonna** nell&#39;angolo inferiore destro dello schermo.
1. Nel campo **Mostra in questa colonna**, inizia a digitare **Conteggio accessi**, quindi selezionalo quando viene visualizzato nell&#39;elenco in **Utente**.

1. Fai di nuovo clic su **Aggiungi colonna**.
1. Nel campo **Mostra nella colonna**, inizia a digitare **Data ultimo accesso**, quindi selezionala quando viene visualizzata nell&#39;elenco in **Utente**.

1. (Facoltativo) Fai clic su **Opzioni avanzate**, quindi seleziona un **Formato campo** dal menu a discesa per includere l&#39;ora o il giorno della settimana dell&#39;ultimo accesso nella colonna.

1. Fai clic su **Salva vista**.\
   La visualizzazione include informazioni sul numero di accessi degli utenti e sulla data dell’ultimo accesso.
