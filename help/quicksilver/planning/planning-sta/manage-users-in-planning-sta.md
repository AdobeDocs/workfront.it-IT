---
title: Gestire gli utenti in Adobe Workfront Planning come prodotto standalone
description: Questo articolo descrive come gestire utenti e team in Adobe Workfront Planning quando Planning viene acquistato come prodotto standalone.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 697499fadf4d5d22292ededed381cb72e53fcae3
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 1%

---


# Gestione degli utenti in Adobe Workfront Planning come prodotto standalone

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono ad Adobe Workfront Planning, se acquistato come prodotto standalone. Fare riferimento a questo articolo quando la società ha acquistato un pacchetto solo Adobe Workfront Planning e non ha acquistato un pacchetto flusso di lavoro Workfront.
>
>Per informazioni su Adobe Workfront Planning acquistato insieme a un pacchetto Workfront, vedere [Introduzione ad Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
>

Puoi gestire gli utenti in Adobe Workfront Planning come prodotto standalone in modo analogo a come li gestisci in Adobe Workfront.

Esistono alcune limitazioni nei livelli di accesso che è possibile assegnare agli utenti in Workfront Planning.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning</p></td> 
   <td> 
<p>Qualsiasi pacchetto Workfront Planning come pacchetto autonomo</p>

</td> </tr>
  <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Amministratore pianificazione</p>
   </td> 
  </tr>

</tbody> 
</table>

Per ulteriori informazioni sull&#39;accesso necessario per Workfront come pacchetto autonomo, vedere [Accesso necessario per Adobe Workfront Planning come prodotto autonomo](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md).
+++    

## Livelli di accesso in Adobe Workfront Planning

È possibile assegnare i seguenti livelli di accesso agli utenti di Workfront Planning acquistati come prodotto standalone:

* Amministratore pianificazione
* Standard di pianificazione

Per ulteriori informazioni sulle funzionalità incluse in ogni accesso, vedere [Accesso necessario per Adobe Workfront Planning come prodotto standalone](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md).

Quando si utilizzano i livelli di accesso in Workfront Planning come prodotto standalone, tenere presente quanto segue:

* Non è possibile creare o modificare livelli di accesso in Workfront Planning. Sono preconfigurati.

* Dopo aver aggiunto un utente a Adobe Admin Console come amministratore per il prodotto Workfront, questi vengono automaticamente assegnati a questo livello di accesso in Workfront Planning e non possono essere modificati in Planning.
* È possibile assegnare un livello di accesso Planning Standard solo agli utenti di Planning, dopo aver aggiunto gli utenti a Admin Console. Questo è l’unico livello di accesso che puoi assegnare manualmente a un utente.

## Gestione degli utenti in Workfront Planning come prodotto standalone

1. In qualità di amministratore di Planning, eseguire una delle operazioni seguenti:

   * Se sei un nuovo cliente di Workfront Planning, riceverai un’e-mail da Adobe Workfront per avvisarti che ora disponi di un account in Adobe Workfront. Utilizza il collegamento nell’e-mail per accedere ad Admin Console.

   * Se si è un amministratore di Workfront Planning esistente e si desidera aggiungere altri utenti al proprio account, accedere ad Admin Console.

   Per informazioni, vedere [Gestione degli utenti in Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

1. In Admin Console, inizia ad aggiungere utenti in una delle seguenti schede:

   * **Amministratori**: gli utenti vengono creati automaticamente come utente amministratore di Planning in Planning.
   * **Utenti**: è necessario assegnare un livello di accesso in Workfront Planning.

1. (Condizionale) Accedi a Workfront dalla home di Adobe CX Enterprise.

   Verrà aperto Workfront Planning.
1. Fai clic su **Menu principale** > **Utenti** > **Nuovo utente**.

   ![Casella Nuovo utente in Planning autonomo](assets/new-user-box-planning-sta.png)

1. Nella casella **Nuovo utente**, aggiorna le seguenti informazioni:

   * **Nome/i**: lo stesso nome aggiunto all&#39;Admin Console.
   * **Cognome**: lo stesso nome aggiunto all&#39;Admin Console.
   * **Indirizzo di posta elettronica (nome utente)**: stesso indirizzo di posta elettronica aggiunto all&#39;Admin Console.
   * **L&#39;utente è attivo**: per indicare che l&#39;utente è attivo, può accedere a Workfront Planning e può essere assegnato a record, attivare l&#39;impostazione.
   * **Livello di accesso**: selezionare Planning Standard per un utente non amministratore. È l&#39;unica opzione.

     >[!TIP]
     >
     >L&#39;aggiunta di un utente che era già stato impostato come amministratore in Admin Console comporta l&#39;aggiunta automatica del livello di accesso Amministratore di Planning all&#39;utente. Questo non può essere modificato.

   * **Team**: dal menu a discesa, seleziona i team da associare all&#39;utente. È necessario creare i team prima di assegnarli agli utenti.

     Per informazioni, vedere [Gestione team](/help/quicksilver/planning/planning-sta/manage-teams-in-planning-sta.md).

1. Fai clic su **Carica ora** per aggiungere un&#39;immagine del profilo, quindi fai clic su **Salva**.

1. Fai clic su **Salva** o **Aggiungi persona e avviane un&#39;altra** per salvare l&#39;utente e aggiungerne un altro.

   Gli utenti vengono aggiunti e riceveranno un messaggio e-mail per accedere a Workfront Planning.
1. (Facoltativo) Per modificare un utente esistente, effettuate una delle seguenti operazioni:

   * Passa il mouse sul nome dell&#39;utente nell&#39;elenco, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) > **Modifica utente**
   * Selezionare l&#39;utente nell&#39;elenco, quindi fare clic su **Modifica utente** sulla barra degli strumenti blu nella parte inferiore della pagina.
1. (Facoltativo) Per eliminare un utente, effettuare una delle seguenti operazioni:

   * Passa il mouse sul nome dell&#39;utente nell&#39;elenco, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) > **Elimina utente**
   * Seleziona il team nell&#39;elenco, quindi fai clic su **Elimina utente** nella barra degli strumenti blu nella parte inferiore della pagina
1. Fai clic su **Elimina** per confermare.
1. (Facoltativo) Per disattivare un utente, effettuare una delle seguenti operazioni:

   * Passa il mouse sul nome dell&#39;utente nell&#39;elenco, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) > **Disattiva**
   * Seleziona il team nell&#39;elenco, quindi fai clic su **Disattiva** nella barra degli strumenti blu nella parte inferiore della pagina
1. Fai clic su **Disattiva** per confermare.

   Per conservare i record cronologici del tuo lavoro, ti consigliamo di disattivare gli utenti, invece di eliminarli.

