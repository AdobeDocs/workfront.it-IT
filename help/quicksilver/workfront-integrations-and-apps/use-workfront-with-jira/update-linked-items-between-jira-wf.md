---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Aggiorna elementi collegati tra [!DNL Jira] e [!DNL Adobe Workfront]
description: Quando colleghi [!DNL Jira] problemi ad [!DNL Adobe Workfront] attività o problemi, gli utenti possono aggiornare gli elementi in un'applicazione e la controparte di quell'elemento viene aggiornata anche per gli utenti che lavorano nella seconda applicazione.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '1700'
ht-degree: 0%

---

# Aggiorna elementi collegati tra [!DNL Jira] e [!DNL Adobe Workfront]

>[!IMPORTANT]
>
>Per offrire integrazioni più stabili e scalabili, stiamo passando a un approccio di integrazione moderno e flessibile che utilizza l’automazione e l’integrazione di Workfront (Fusion). Nell&#39;ambito di questo processo di transizione, l&#39;integrazione Workfront for Jira non sarà disponibile dopo il **28 febbraio 2026**.
>
>È consigliabile utilizzare l’automazione e l’integrazione di Workfront per le esigenze di integrazione della tua organizzazione con Jira.
>
>Entro agosto saranno disponibili otto modelli di automazione e integrazione Workfront pronti all’uso per Jira, per consentire la replica dei flussi di lavoro comuni e accelerare l’implementazione. I modelli sono completamente personalizzabili per soddisfare specifiche esigenze aziendali e possono essere estesi in base all&#39;evoluzione dei requisiti.
> 
>Per una panoramica dell&#39;automazione e dell&#39;integrazione di Workfront, vedere [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Per informazioni sulle funzionalità specifiche dei moduli di automazione e integrazione di Workfront per Jira, vedere [Moduli software Jira](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

Quando colleghi [!DNL Jira] problemi ad attività o problemi [!DNL Adobe Workfront], gli utenti possono aggiornare gli elementi in un&#39;applicazione e la controparte di quell&#39;elemento viene aggiornata anche per gli utenti che lavorano nella seconda applicazione.

Per ulteriori informazioni sul collegamento di elementi tra [!DNL Workfront] e [!DNL Jira], vedere [Collegare elementi tra Adobe Workfront e Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Durante la configurazione di [!DNL Workfront] per [!DNL Jira], in qualità di amministratore di sistema di [!DNL Jira], è possibile configurare alcuni campi di un&#39;applicazione per la sincronizzazione con i campi degli elementi collegati dell&#39;altra applicazione.

Per ulteriori informazioni sulla sincronizzazione dei campi tra gli elementi collegati [!DNL Jira] e [!DNL Workfront], vedere [Configure [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td><p>Nuovo: Qualsiasi</p>
       <p>oppure</p>
       <p>Corrente: [!UICONTROL Pro] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td><p>Nuovo: [!UICONTROL Standard]</p>
       <p>oppure</p>
       <p>Corrente: [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] accesso</td> 
   <td> <p>Accesso amministratore di sistema</p> <p>Importante: è consigliabile creare account di amministratore di sistema separati in [!DNL Jira] e [!DNL Workfront] per dedicarsi a questa integrazione, anziché utilizzare account esistenti che potrebbero essere collegati agli utenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore [!DNL Workfront].</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisiti

Prima di collegare gli elementi tra [!DNL Workfront] e [!DNL Jira], è necessario:

* Installa [!DNL Workfront for Jira].

  Per istruzioni sull&#39;installazione di [!DNL Workfront for Jira], vedere [Installa [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configura [!DNL Workfront for Jira].

  Per istruzioni sulla configurazione di [!DNL Workfront for Jira], vedere [Configura [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Collega elementi tra [!DNL Workfront] e [!DNL Jira].

  Per istruzioni, vedi [Collega elementi tra [!DNL Adobe Workfront] e [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Aggiorna elementi collegati in [!DNL Workfront]

Se si lavora principalmente in [!DNL Workfront], è possibile aggiornare gli elementi di lavoro in [!DNL Workfront] e anche le relative controparti in [!DNL Jira]. Questo aggiornamento avviene tramite l&#39;integrazione di [!DNL Workfront] per [!DNL Jira] che non richiede una licenza di [!DNL Jira].

Se l&#39;amministratore di [!DNL Workfront] ha configurato [!DNL Workfront for Jira] per sincronizzare i campi tra gli elementi collegati, alcuni campi aggiornati in [!DNL Workfront] vengono aggiornati anche per il problema [!DNL Jira] collegato. Per ulteriori informazioni sull&#39;aggiornamento degli elementi in [!DNL Workfront], vedere [Modifica problemi](../../manage-work/issues/manage-issues/edit-issues.md) e [Modifica attività](../../manage-work/tasks/manage-tasks/edit-tasks.md).

L&#39;elenco seguente mostra quali campi [!DNL Workfront] si sincronizzano con i campi [!DNL Jira] degli elementi collegati:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Campo [!DNL Workfront] aggiornato</strong> </th> 
   <th><strong>Campo/aggiornamento [!DNL Jira] sincronizzato</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Nome problema o attività]</td> 
   <td> <p>[!UICONTROL Issue name]</p> <p>Un commento sulla modifica del Nome è stato aggiunto alla scheda <strong>[!DNL Workfront]</strong> del problema [!DNL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Description]</td> 
   <td> <p> [!UICONTROL Descrizione problema]</p> <p>Un commento sulla Descrizione aggiornata è stato aggiunto alla scheda <strong>[!DNL Workfront]</strong> del problema [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Documenti Caricati]</p> <p>Nota: i documenti collegati a [!DNL Workfront] elementi da un server esterno non vengono trasferiti a [!DNL Jira] problemi. Solo i documenti caricati direttamente sugli elementi [!DNL Workfront] vengono aggiornati ai [!DNL Jira] problemi collegati. </p> </td> 
   <td> <p>[!UICONTROL Allegati]</p> <p>Un commento sugli allegati caricati è stato aggiunto alla scheda <strong>[!DNL Workfront]</strong> del problema [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di completamento Pianificata]</td> 
   <td> <p>[!UICONTROL Scadenza]</p> <p>Un commento sulla [!UICONTROL Scadenza] modificata è aggiunto alla scheda [!DNL Workfront] del problema [!DNL Jira]. </p> <p>Nota: è necessario abilitare <strong>[!UICONTROL Scadenza]</strong> per [!DNL Jira] problemi per poter visualizzare questo campo aggiornato in [!UICONTROL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>Forms personalizzato e campi personalizzati</td> 
   <td> <p> Visualizza nel pannello a destra [!DNL Workfront] del problema [!DNL Jira]. <br>Nel pannello vengono visualizzati solo i campi personalizzati con un valore effettivo.<br></p> <p>Nota: le sezioni dei moduli personalizzati vengono visualizzate con il livello di accesso dell'amministratore [!DNL Workfront]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Priority]</td> 
   <td>Viene visualizzato nel pannello a destra [!DNL Workfront] del problema [!DNL Jira]. <br>Il campo <strong>[!UICONTROL Priority]</strong> non viene aggiornato in [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo di registrazione] </td> 
   <td> <p>Nella scheda <strong>[!DNL Workfront]</strong> del problema [!DNL Jira] è stato aggiunto un commento sull'ora registrata. Questo include il nome dell’utente che registra l’ora e dell’utente per il quale l’ora è registrata, nel caso siano diversi. Nessun orario registrato nella scheda <strong>[!UICONTROL Work Log]</strong> in [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commenti]</td> 
   <td> <p>Il commento viene aggiunto alla scheda <strong>[!DNL Workfront]</strong> del problema [!DNL Jira]. Non è stato aggiunto alla scheda <strong>[!UICONTROL Commenti]</strong> del problema [!DNL Jira]</p> <p>Nota: quando si collegano manualmente due elementi esistenti, i commenti aggiunti all'elemento [!DNL Workfront] prima di collegarlo a [!DNL Jira] non vengono sincronizzati con il problema [!DNL Jira]. </p> <p>I commenti Jira vengono sincronizzati con Workfront.</td> 
  </tr> 
 </tbody> 
</table>

## Aggiorna elementi collegati in [!DNL Jira]

Se si lavora principalmente in [!DNL Jira], è possibile aggiornare gli elementi di lavoro in [!DNL Jira] e anche le relative controparti in [!DNL Workfront]. Non è necessario disporre di una licenza [!DNL Workfront] per [!DNL Workfront] elementi collegati ai problemi [!DNL Jira] per ricevere gli aggiornamenti che si stanno effettuando in [!DNL Jira].

A condizione che l&#39;amministratore di [!DNL Workfront] abbia configurato [!DNL Workfront] per [!DNL Jira] per sincronizzare i campi tra gli elementi collegati, alcuni campi che si aggiornano in [!DNL Jira] vengono aggiornati anche per l&#39;elemento [!DNL Workfront] collegato.

L&#39;elenco seguente mostra quali campi [!DNL Jira] si sincronizzano con i campi [!DNL Workfront] degli elementi collegati:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Campo [!DNL Jira] Aggiornato</strong> </th> 
   <th><strong>Campo [!DNL Workfront] Sincronizzato/ Aggiornamento</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Stato problema]</td> 
   <td> <p> [!UICONTROL Stato problema o attività]</p> <p>Lo stato del problema in [!DNL Jira] viene sincronizzato con i seguenti stati, o stati equivalenti ai seguenti, in Workfront:</p> 
    <ul> 
     <li> <p>[!UICONTROL Nuovo] ([!UICONTROL NUOVO])</p> </li> 
     <li> <p>[!UICONTROL In Corso] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL chiuso]/[!UICONTROL completo] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Nota: lo stato [!DNL Jira] viene sincronizzato con il primo stato [!DNL Workfront] che corrisponde allo stato appropriato.</p> <p>Per ulteriori informazioni sugli stati degli elementi in [!DNL Workfront], vedere <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Creare o modificare uno stato</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Issue Attachments]</td> 
   <td> [!UICONTROL Issue or Task Documents]<br>Un commento sul caricamento di un nuovo documento in [!DNL Jira] è stato aggiunto alla scheda [!UICONTROL Updates] del problema o dell'attività [!DNL Workfront].  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scadenza]</td> 
   <td> <p> Un commento sulla modifica di [!UICONTROL Scadenza] in [!DNL Jira] è stato aggiunto alla scheda [!UICONTROL Aggiornamenti] del problema o dell'attività [!DNL Workfront]. </p> <p>Nota: nessuna modifica di date sul problema o sull'attività [!DNL Workfront]. </p> </td> 
  </tr> 
  <tr> 
   <td> Registra tempo nel pannello a destra di [!DNL Workfront] o dal menu [!UICONTROL Altro] nel problema [!DNL Jira]<br></td> 
   <td> <p>Ore<br>Oltre ad aggiungere le ore registrate in Jira all'elemento [!DNL Workfront] collegato, nella scheda [!UICONTROL Aggiornamenti] dell'elemento [!DNL Workfront] viene aggiunto un commento sull'ora di registrazione.</p> <p>Per ulteriori informazioni sull'ora di registrazione per [!DNL Jira] problemi collegati, incluso l'aggiornamento dell'utente [!DNL Jira] che registra l'ora in [!DNL Workfront], vedere <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Ora di registrazione per [!DNL Jira] e [!DNL Workfront] elementi collegati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Commenti <br><br></td> 
   <td> <p>I commenti vengono aggiunti alla scheda [!UICONTROL Aggiornamenti] del problema o dell'attività [!DNL Workfront] se l'impostazione <strong>[!UICONTROL Commenti]</strong> nella sezione [!UICONTROL SINCRONIZZA DA JIRA A WORKFRONT] della scheda [!UICONTROL Setup] è impostata su <strong>[!UICONTROL Always]</strong>.</p> <p>Per informazioni sulla configurazione delle impostazioni di Workfront in [!DNL Jira], vedere <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configurazione di [!DNL Workfront for Jira]</a>.</p> <p>Per informazioni sul commento di elementi da [!DNL Jira] problemi collegati, vedere <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Commento da un [!DNL Jira] problema collegato</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Registra tempo da [!DNL Jira] problemi collegati

L&#39;ora registrata per un elemento [!DNL Jira] in [!DNL Jira] verrà trasferita anche all&#39;elemento [!DNL Workfront] collegato, indipendentemente da dove in [!DNL Jira] si registra l&#39;ora.\
Quando si effettua l&#39;accesso in Jira nel pannello [!DNL Workfront], l&#39;ora viene registrata solo in [!DNL Workfront].\
Il tempo di registrazione in [!DNL Workfront] non influisce sul tempo del problema collegato in [!DNL Jira].

>[!NOTE]
>
>Se l&#39;ora viene aggiunta a un elemento [!DNL Jira] collegato a un&#39;attività [!DNL Workfront], il tipo di [!UICONTROL ora] per l&#39;ora in [!DNL Workfront] è [!UICONTROL ora attività]. Se l&#39;ora viene aggiunta a un elemento [!DNL Jira] collegato a un problema [!DNL Workfront], il tipo [!UICONTROL Hour] per l&#39;ora in [!DNL Workfront] è [!UICONTROL Issue Time].

È stato aggiunto un commento alla scheda **[!DNL Workfront]** in [!DNL Jira] e alla scheda **[!UICONTROL Aggiornamenti]** dell&#39;elemento in [!DNL Workfront] per registrare l&#39;ora.\
L&#39;ora viene visualizzata anche nella scheda **[!UICONTROL Ore]** dell&#39;elemento [!DNL Workfront].

* [Tempo di connessione per elementi collegati [!DNL Jira] e [!DNL Workfront] elementi](#log-time-for-linked-jira-and-workfront-items)
* [Tempo di connessione da [!DNL Jira] a un [!DNL Workfront] elemento](#log-time-from-jira-to-a-workfront-item)

### Tempo di connessione per [!DNL Jira] e [!DNL Workfront] elementi collegati

È possibile registrare l&#39;ora da un problema [!DNL Jira] collegato a un elemento [!DNL Workfront] e l&#39;ora viene registrata sia sul problema [!DNL Jira] che sull&#39;elemento [!DNL Workfront].

>[!IMPORTANT]
>
>Se l&#39;utente che registra l&#39;ora in [!DNL Jira] non esiste in [!DNL Workfront], l&#39;integrazione crea un nuovo utente attivo in Workfront se **[!UICONTROL Crea automaticamente un utente in [!DNL Workfront]&#x200B;se l&#39;utente [!DNL Jira] non ha un *[!DNL Workfront]&#x200B;account]** è impostato su&#x200B;**[!UICONTROL &#x200B; Sempre &#x200B;]**. Questo utente non occupa una licenza [!DNL Workfront]. È possibile assegnare utenti attivi agli elementi di lavoro in [!DNL Workfront], ma non è possibile includerli negli aggiornamenti. Per informazioni sulla configurazione della creazione automatica di [!DNL Workfront] utenti da [!DNL Jira], vedere [Configurazione [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

Per registrare l&#39;ora di un elemento in [!DNL Jira] e registrarlo sia in [!DNL Jira] che in [!DNL Workfront]:

1. Accedi a [!DNL Jira].
1. Passare al problema [!DNL Jira] collegato all&#39;elemento [!DNL Workfront].
1. Espandere il menu **[!UICONTROL Altro]** e fare clic su **[!UICONTROL Registra lavoro]**.

1. Nel campo **[!UICONTROL Tempo trascorso]**, specifica la quantità di tempo impiegato per risolvere il problema. È necessario specificare l&#39;ora utilizzando i seguenti periodi di tempo:

   * [!UICONTROL Settimane] (l)
   * [!UICONTROL Giorni] (d)
   * [!UICONTROL Ore] (h)

1. Continua ad aggiungere informazioni alla tua voce orario, inclusa una **[!UICONTROL Descrizione lavoro]**, quindi fai clic su **[!UICONTROL Registro]**.\
   L&#39;ora viene aggiunta alla scheda **[!UICONTROL Registro di lavoro]** dell&#39;elemento [!DNL Jira] e all&#39;elemento [!DNL Workfront] a esso collegato.\
   La descrizione di lavoro della voce dell&#39;ora viene registrata come nota nella voce dell&#39;ora in [!DNL Workfront].

### Registra tempo da [!DNL Jira] a un elemento [!DNL Workfront]

È possibile registrare l&#39;ora solo per l&#39;elemento [!DNL Workfront] collegato dal problema [!DNL Jira] senza registrare l&#39;ora per il problema [!DNL Jira].

1. Accedi a [!DNL Jira].
1. Passare a un problema [!DNL Jira] collegato a un elemento [!DNL Workfront].

   I dettagli dell&#39;elemento [!DNL Workfront] devono essere visualizzati nel pannello destro [!DNL Workfront] del problema.

1. Fai clic sull&#39;icona **[!UICONTROL Tempo di registrazione]**.

1. Specifica la quantità di **[!UICONTROL ore]** e **[!UICONTROL minuti]** da registrare per il problema.

1. Fare clic su **[!UICONTROL Tempo di registrazione]**.

   Ora aggiunta all&#39;elemento [!DNL Workfront].

   Questa volta non viene aggiunta alla scheda [!UICONTROL Registro di lavoro] del problema [!DNL Jira].

## Commento da un problema [!DNL Jira] collegato {#comment-from-a-linked-jira-issue}

Quando si commenta un elemento [!DNL Jira] dal pannello destro [!DNL Workfront] in [!DNL Jira], il commento viene aggiunto anche alla scheda [!UICONTROL Aggiornamenti] dell&#39;elemento collegato in Workfront.

Per aggiungere un commento da [!DNL Jira] a un elemento [!DNL Workfront]:

1. Accedi a [!DNL Jira].
1. Passare a un problema [!DNL Jira] collegato a un elemento [!DNL Workfront].

   I dettagli dell&#39;elemento [!DNL Workfront] devono essere visualizzati nel pannello destro [!DNL Workfront] del problema.

1. Fare clic sull&#39;icona **[!UICONTROL Commenti]** nel pannello [!DNL Workfront] o nella scheda **[!UICONTROL Commenti]**.

1. Inizia a digitare un commento, quindi fai clic su **[!UICONTROL Invia]**.

   Il commento è aggiunto al seguente:

   * Scheda **[!DNL Workfront]** del problema [!DNL Jira].
   * Scheda **[!UICONTROL Commenti]** del problema [!DNL Jira].
   * Scheda **[!UICONTROL Aggiornamenti]** dell&#39;elemento collegato in Workfront.
