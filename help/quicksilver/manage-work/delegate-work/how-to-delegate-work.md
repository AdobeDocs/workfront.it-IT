---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: Delega attività e problemi
description: Puoi delegare temporaneamente il lavoro a cui sei assegnato mentre sei fuori ufficio. Questo articolo descrive come delegare le assegnazioni di attività ed emissioni.
author: Alina
exl-id: 42b3112f-4f39-4078-aaa0-623559384a12
source-git-commit: 72a2927d33f40c4fe08888712bdf62e9a5db9c40
workflow-type: tm+mt
source-wordcount: '1483'
ht-degree: 1%

---

# Gestione dell&#39;attività e della delega dei problemi

<!--
<NOTE: 
<you might need to change the tile to Delegate PTI, etc, when that functionality is added. Named it this so it will not conflict with the TOC article for Delegate section which was also "Delegate work"
I wrote thhis as a "Manage..." article and I did not add three separate articles, to match what we have for delegating approval requests)
-->

Puoi delegare temporaneamente il lavoro a cui sei assegnato mentre sei fuori ufficio.

È possibile delegare le attività e rilasciare le assegnazioni oppure delegare le approvazioni. Questo articolo descrive come delegare le assegnazioni di attività ed emissioni.

Per informazioni generali sulla delega del lavoro, vedere [Panoramica sul lavoro delegato](../../manage-work/delegate-work/delegate-work-overview.md).

## Requisiti di accesso

>[!IMPORTANT]
>
>* Gli utenti selezionati come delegati ricevono le stesse autorizzazioni delle tue autorizzazioni sulle attività e sui problemi che deleghi loro.
>* Le autorizzazioni devono funzionare entro i loro livelli di accesso e a volte i loro livelli di accesso potrebbero essere inferiori ai tuoi.

   >
   >   
   >   Ad esempio, se un utente dispone solo dell&#39;accesso Visualizza alle attività nel proprio livello di accesso e si dispone delle autorizzazioni Gestione per le attività che si delegano, riceverà le autorizzazioni Gestisci per le attività che deleghi a tali attività. Tuttavia, non saranno in grado di eseguire le stesse azioni eseguite dall’utente sulle attività delegate. Per poter aggiornare le attività in assenza, è necessario che l&#39;amministratore di sistema richieda l&#39;accesso a Modifica attività.
   >
   >   
   >   Per informazioni su come modificare il livello di accesso, consulta [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
>
>* Per gli elementi assegnati dopo l&#39;avvio della delega, può essere necessaria fino a un&#39;ora dopo l&#39;assegnazione dell&#39;elemento [!DNL Workfront] per condividere gli elementi appena assegnati con il delegato.



Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>Revisione o superiore</p>

>[!NOTE]
>
>Anche se puoi essere assegnato al lavoro quando disponi di una licenza di richiesta, non puoi delegare il tuo lavoro ad altri. [!DNL Workfront] sconsiglia di assegnare il lavoro agli utenti di revisione o richiesta.

</tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l'accesso alle attività e ai problemi Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per le attività o i problemi a cui sei assegnato</p> 
    <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## Prerequisiti

Prima di poter eseguire le attività descritte in questo articolo, è necessario assicurarsi quanto segue:

* Le [!DNL Workfront] o l&#39;amministratore del gruppo ha abilitato [!UICONTROL Consenti agli utenti di eliminare attività e problemi relativi alle ore registrate] nella [!UICONTROL Configurazione] area [!DNL Workfront] istanza.

   Per ulteriori informazioni, consulta [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Delega attività e problemi a un altro utente

Prima di delegare il lavoro ad altri, ti consigliamo di contattarli e informarli che saranno designati come delegati sui tuoi oggetti di lavoro. Chiedi la loro approvazione verbale prima di delegare il lavoro per assicurarsi che abbiano il tempo necessario per completare il lavoro mentre sei fuori ufficio.

Per informazioni generali sulla delega di attività e problemi, consulta [Panoramica sulla delega di attività e problemi](delegate-work.md).

Per delegare attività e problemi ad altri:

1. Vai a [!UICONTROL **Pagina principale**] area, quindi fare clic su [!UICONTROL **Delega**] nella parte superiore del [!UICONTROL **Elenco lavori**].

   ![](assets/delegate-button-in-home.png)

1. In [!UICONTROL **Delega di compiti e problemi**] , aggiorna quanto segue:

   * [!UICONTROL **Delega di attività e problemi a**]: Inizia a digitare il nome di un utente a cui desideri delegare le attività e i problemi, quindi selezionalo quando viene visualizzato nell’elenco. È possibile selezionare un solo utente.\

      L&#39;utente selezionato come delegato riceve le stesse autorizzazioni delle tue autorizzazioni sulle attività e sui problemi che deleghi ad essi. Per ulteriori informazioni, consulta [Panoramica sull’attività e sul problema delegato](delegate-work-overview.md).

   * [!UICONTROL **Data di inizio**]: Selezionare una data dal calendario in cui deve iniziare la delega degli elementi di lavoro.

      >[!TIP]
      >
      >La data di inizio non può essere passata.

   * [!UICONTROL **Nessuna data di fine**]: Selezionare questa opzione se non si desidera specificare la data di fine della delega.

   * [!UICONTROL **Data di fine**]: Seleziona una data dal calendario in cui la delega deve essere interrotta.

      >[!TIP]
      >
      >Se non si seleziona una data di fine, la delega viene abilitata solo per il giorno corrente.

      ![](assets/delegate-box-expanded-in-home.png)

1. Fai clic su [!UICONTROL **Salva**].

   Accade quanto segue:

   * Il lavoro viene delegato all&#39;utente specificato. Vengono delegati tutti i task o i problemi incompleti che hanno date entro l&#39;intervallo di tempo selezionato (inclusi quelli appena assegnati, dopo l&#39;abilitazione della delega).
   >[!TIP]
   >
   >   Gli elementi di lavoro completati con date entro l&#39;intervallo di tempo della delega non vengono delegati.


   * Ricevi un messaggio nell’angolo in alto a destra dello schermo per confermare di aver abilitato la delega del lavoro a un altro utente. Il nome dell’utente delegato viene visualizzato nel messaggio di conferma.

   * L&#39;indicazione che le attività e i problemi sono delegati ad altri utenti viene visualizzata nella maggior parte delle aree in cui è possibile visualizzare le assegnazioni in [!DNL Workfront]. Per ulteriori informazioni sulle aree che non includono i nomi dei delegati, vedi [Panoramica sull’attività e sul problema delegato](delegate-work-overview.md).

   * La [!UICONTROL **Delega**] nel [!UICONTROL Pagina principale] modifiche all&#39;area in [!UICONTROL **Modifica delega**] per indicare l&#39;esistenza di una delega.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
   </MadCap:conditionalText>
   -->

   ![](assets/work-delegated-button-in-home.png)

   * Se le notifiche dell’evento e le notifiche personali sono abilitate, riceverai anche una conferma e-mail della tua delegazione.

   * L’utente selezionato come delegato riceve un’e-mail sulla delega, se le relative notifiche evento sono abilitate.

      Per informazioni sull’abilitazione delle notifiche e-mail personali, consulta [Attivare o disattivare le notifiche degli eventi personali](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).





## Modifica o interrompi la delega

È possibile lasciare scadere una delega, se è stata selezionata una data di fine, oppure arrestarla manualmente. Puoi anche modificare l&#39;intervallo di tempo per la delega, se le date della delega sono cambiate.

1. Vai a [!UICONTROL Pagina principale] area, quindi fare clic su [!UICONTROL Modifica delega] nell&#39;angolo in alto a destra dell&#39;Elenco di lavoro.
1. In [!UICONTROL Delega di compiti e problemi] eseguire una delle operazioni seguenti:
   * Modifica la [!UICONTROL **Data di inizio**] o [!UICONTROL **Data di fine**]
   * Fai clic su [!UICONTROL **Interrompi delega**]

   >[!TIP]
   >
   >    Puoi modificare solo la data di fine di una delega se la delega è già iniziata.

   ![](assets/stop-delegation-screen-in-home.png)

1. (Condizionale) fai clic su [!UICONTROL **Salva**] per salvare le nuove date di delega

   Oppure

   Fai clic su [!UICONTROL **Interrompi delega**] nella casella di conferma per confermare l’arresto della delega.

   La delega ha aggiornato le date o si è interrotta e gli utenti delegati sono stati rimossi dalle attività e dai problemi. Le loro autorizzazioni per le attività e i problemi rimangono in vigore.


## Individuare il lavoro delegato e delegare le informazioni

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

Quando vengono delegati compiti e problemi, ci sono diverse aree in [!DNL Workfront] dove puoi vedere il lavoro delegato o chi sono i delegati.

* [Individua delegati nella casella Assegnazioni](#locate-delegates-in-the-assignments-box)
* [Individua il lavoro delegato in [!UICONTROL Pagina principale]](#locate-delegated-work-in-home)


### Individua i delegati nella [!UICONTROL Assegnazioni] scatola

Quando l&#39;amministratore di sistema o di gruppo abilita la delega del lavoro nel sistema, la [!UICONTROL Assegnazioni] in questa casella vengono visualizzate le seguenti schede ovunque sia possibile accedervi:

* [!UICONTROL **Assegnazioni**]: Gli utenti assegnati all&#39;attività o al problema vengono visualizzati qui.
* [!UICONTROL **Delegazioni**]: Gli utenti designati come delegati dagli assegnatari sull&#39;attività o sul problema vengono visualizzati qui.

Puoi accedere al [!UICONTROL Assegnazioni] nelle seguenti aree:

* Intestazione dell&#39;attività o del problema

   ![](assets/assignments-and-delegates-panel-in-task-header.png)

   La [!UICONTROL Assegnazioni] nel campo dell&#39;attività o dell&#39;intestazione del problema viene modificato in [!UICONTROL Assegnazioni e delegazioni].

* La [!DNL Workload Balancer] quando si assegnano manualmente attività o problemi

   ![](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> Non è possibile visualizzare i delegati nel [!UICONTROL Assegnazioni] sezione di un&#39;attività o della casella di modifica del problema.

Se un&#39;attività o un problema viene delegato e il [!UICONTROL Delegazioni] la sottoscheda è vuota, potrebbe esistere uno dei seguenti scenari:

* Non sei assegnato all&#39;attività o al problema.
* Le date dell&#39;attività o del rilascio non rientrano nell&#39;intervallo di tempo di delega.

>[!TIP]
>
>Gli strumenti di gestione delle risorse non tengono conto delle ore pianificate o effettive per le attività e i problemi delegati, come [!DNL Workload Balancer] o [!DNL Resource Planner] per gli utenti delegati. Le ore rimangono associate solo all’utente assegnato.

### Individua il lavoro delegato in [!UICONTROL Pagina principale]

1. Vai a [!UICONTROL **Pagina principale**] , quindi fai clic sul menu a discesa del filtro e seleziona una o più delle seguenti opzioni:
   * [!UICONTROL **Delegato**]: per visualizzare le attività e i problemi delegati a te o da te.
   * [!UICONTROL **Delegato a me**]: per visualizzare le attività e i problemi delegati da un altro utente.
   * [!UICONTROL **Delegato da me**]: per visualizzare le attività e i problemi delegati da te ad altri utenti.

   ![](assets/delegated-to-me-or-by-me-filters-in-home.png)

1. Fai clic sul pulsante [!UICONTROL ordinamento] menu a discesa per ordinare l’elenco in base ai seguenti criteri:
   * [!UICONTROL Completamento pianificato]. Questa è l’opzione di ordinamento predefinita.
   * [!UICONTROL Inizio pianificato]
   * [!UICONTROL Conferma data]
   * [!UICONTROL Progetto]
   * [!UICONTROL La mia priorità]
1. Espandi i raggruppamenti nel [!UICONTROL **Elenco lavori**] per visualizzare gli elementi di lavoro delegati. Esistono i seguenti scenari:
   * Per gli elementi delegati ad altri, il nome del delegato viene visualizzato nella sezione [!UICONTROL **Elenco lavori**] nonché [!UICONTROL **Assegnazioni e delegazioni**] campo a destra.

   * Per gli elementi delegati, il nome dell’assegnatario viene visualizzato nella sezione [!UICONTROL **Elenco lavori**] nonché **[!UICONTROL Assegnazioni e delegazioni]** campo a destra.
   >[!TIP]
   >
   >    Se la delega deve iniziare a una data successiva alla data odierna, la data di inizio della delega viene visualizzata anche nella [!UICONTROL Elenco lavori]. Gli elementi delegati vengono visualizzati nel raggruppamento selezionato per la [!UICONTROL Elenco lavori], in base al tipo di raggruppamento. Ad esempio, se si raggruppa per [!UICONTROL Data completamento pianificata], gli elementi delegati vengono visualizzati nel raggruppamento che corrisponde alle rispettive date di completamento pianificate.
