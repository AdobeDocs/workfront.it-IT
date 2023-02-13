---
title: Visualizza informazioni di accesso utente
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Puoi vedere la frequenza con cui gli utenti accedono a Workfront e l’ultima volta che hanno effettuato l’accesso, indicando che desideri includere queste informazioni nella visualizzazione di un elenco di utenti o in un rapporto per gli utenti.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# Visualizza informazioni di accesso utente

Puoi vedere la frequenza con cui gli utenti accedono ad Adobe Workfront e l’ultima volta che hanno effettuato l’accesso, indicando che desideri includere queste informazioni nella visualizzazione di un elenco di utenti o in un rapporto per gli utenti.

## Requisiti di accesso

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
   <td> <p>Piano </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi disporre di una delle seguenti caratteristiche:</p> 
    <ul> 
     <li> <p>Livello di accesso amministratore di sistema. Per informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>. </p> </li> 
     <li> <p><b>Utenti</b> impostazione nel livello di accesso configurato per <b>Modifica</b> accesso, con <b>Crea</b> e almeno uno dei due <b>Amministratore utente</b> opzioni attivate in <b>Ottimizzare le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se Utente <b>Amministratore (utenti del gruppo)</b> è abilitato, devi essere un amministratore di gruppo di un gruppo in cui l’utente è membro.</p> <p>Per ulteriori informazioni sulla <b>Utenti</b> impostazione in un livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Come Workfront registra le informazioni di accesso

Workfront registra le seguenti informazioni sugli utenti che accedono al sistema:

* **Conteggio accessi**: Workfront conta un utente che accede all’applicazione una volta ogni 24 ore. Se un utente accede più volte utilizzando browser, computer o dispositivi mobili diversi, Workfront conta tutti gli accessi che si sono verificati in un giorno come un unico accesso. Il conteggio di accesso include informazioni che iniziano con la creazione dell’utente.
* **Data ultimo accesso**: L’ultima data in cui un utente ha effettuato l’accesso. La data di ogni accesso da qualsiasi browser, dispositivo mobile o altre applicazioni viene registrata in questo campo.

L&#39;accesso a Workfront in uno dei seguenti modi viene conteggiato come accesso a Workfront:

* Applicazione Web Workfront
* App Workfront Mobile (dispositivi iOS o Android)
* Qualsiasi integrazione Workfront supportata con un’altra applicazione di terze parti (Slack, Jira)
* Qualsiasi integrazione personalizzata tra Workfront e un’altra applicazione di terze parti.
* API Workfront

   >[!NOTE]
   >
   >L’accesso a Workfront tramite l’API Workfront è disponibile solo per le organizzazioni non ancora integrate nell’Adobe Business Platform.

## Visualizzazione delle informazioni di utilizzo in un elenco o report utente

È possibile visualizzare i campi Conteggio accessi e Data ultimo accesso nella visualizzazione di un elenco di utenti o in un rapporto per gli utenti.\
Per ulteriori informazioni sulla creazione di un rapporto, vedi [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Per visualizzare le informazioni sull’utilizzo nella visualizzazione di un elenco di utenti:

1. Vai a un elenco di utenti in Workfront.
1. Da **Visualizza** menu a discesa, seleziona **Nuova vista**.

1. Fai clic su **Aggiungi colonna** nell’angolo in basso a destra dello schermo.
1. In **Mostra in questa colonna** campo, inizia a digitare **Conteggio accessi**, quindi selezionalo quando viene visualizzato nell’elenco in **Utente**.

1. Fai clic su **Aggiungi colonna** di nuovo.
1. In **Mostra nella colonna** campo, inizia a digitare **Data ultimo accesso**, quindi selezionalo quando viene visualizzato nell’elenco in **Utente**.

1. (Facoltativo) Fai clic su **Opzioni avanzate**, quindi seleziona una **Formato campo** dal menu a discesa per includere l’ora o il giorno della settimana dell’ultimo accesso nella colonna.

1. Fai clic su **Salva visualizzazione**.\
   La visualizzazione include informazioni sul numero di volte in cui gli utenti hanno effettuato l’accesso e sul momento dell’ultimo accesso.
