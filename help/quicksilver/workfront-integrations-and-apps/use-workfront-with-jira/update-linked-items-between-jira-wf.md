---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Aggiorna elementi collegati tra [!DNL Jira] e [!DNL Adobe Workfront]
description: Quando si collega [!DNL Jira] problemi a [!DNL Adobe Workfront] attività o problemi, gli utenti possono aggiornare gli elementi in un'applicazione e la controparte di quell'elemento viene aggiornata anche per gli utenti che lavorano nella seconda applicazione.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: e01f5eaf3133fa1bdaedf4dad56e9a8175b70667
workflow-type: tm+mt
source-wordcount: '1570'
ht-degree: 0%

---

# Aggiorna elementi collegati tra [!DNL Jira] e [!DNL Adobe Workfront]

Quando si collega [!DNL Jira] problemi a [!DNL Adobe Workfront] attività o problemi, gli utenti possono aggiornare gli elementi in un&#39;applicazione e la controparte di quell&#39;elemento viene aggiornata anche per gli utenti che lavorano nella seconda applicazione.

Per ulteriori informazioni sul collegamento di elementi tra [!DNL Workfront] e [!DNL Jira], vedi [Collegare elementi tra Adobe Workfront e Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Come si configura [!DNL Workfront] per [!DNL Jira], come [!DNL Jira] amministratore di sistema, è possibile configurare alcuni campi di un&#39;applicazione per eseguire la sincronizzazione con i campi degli elementi collegati dell&#39;altra applicazione.

Per ulteriori informazioni sulla sincronizzazione dei campi tra [!DNL Jira] e [!DNL Workfront] elementi, vedi [Configura [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

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
   <td> <p>Accesso amministratore di sistema</p> <p>Importante: è consigliabile creare account di amministratore di sistema separati in [!DNL Jira] e [!DNL Workfront] per dedicarsi a questa integrazione, anziché utilizzare quelle esistenti che potrebbero essere collegate agli utenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisiti

Prima di collegare gli elementi tra [!DNL Workfront] e [!DNL Jira], è necessario:

* Installa [!DNL Workfront for Jira].

  Per istruzioni sull&#39;installazione [!DNL Workfront for Jira], vedi [Installa [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configura [!DNL Workfront for Jira].

  Per istruzioni sulla configurazione [!DNL Workfront for Jira], vedi [Configura [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Collega elementi tra [!DNL Workfront] e [!DNL Jira].

  Per istruzioni, consulta [Collega elementi tra [!DNL Adobe Workfront] e [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Aggiornare gli elementi collegati in [!DNL Workfront]

Se lavori principalmente in [!DNL Workfront], è possibile aggiornare gli elementi di lavoro in [!DNL Workfront] e le loro controparti in [!DNL Jira] aggiorna anche. Questo aggiornamento avviene tramite l’integrazione di [!DNL Workfront] per [!DNL Jira] che non richiede una [!DNL Jira] licenza.

Fino a quando [!DNL Workfront] l’amministratore ha configurato [!DNL Workfront for Jira] per sincronizzare i campi tra elementi collegati, alcuni campi che vengono aggiornati in [!DNL Workfront] aggiorna anche per il [!DNL Jira] problema. Per ulteriori informazioni sull&#39;aggiornamento degli elementi in [!DNL Workfront], vedi [Modifica problemi](../../manage-work/issues/manage-issues/edit-issues.md) e [Modifica attività](../../manage-work/tasks/manage-tasks/edit-tasks.md).

L&#39;elenco seguente mostra quali [!DNL Workfront] campi sincronizzati con [!DNL Jira] campi sugli elementi collegati:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aggiornato [!DNL Workfront] campo</strong> </th> 
   <th><strong>Sincronizzato [!DNL Jira] campo/aggiornamento</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Nome problema o attività]</td> 
   <td> <p>[!UICONTROL Issue name]</p> <p>Un commento sulla modifica del Nome viene aggiunto al <strong>[!DNL Workfront]</strong> scheda di [!DNL Jira] problema. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Description]</td> 
   <td> <p> [!UICONTROL Descrizione problema]</p> <p>Un commento sulla Descrizione aggiornata viene aggiunto al <strong>[!DNL Workfront]</strong> scheda di [!DNL Jira] problema.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Documenti Caricati]</p> <p>Nota: documenti collegati a [!DNL Workfront] gli elementi da un server esterno non vengono trasferiti a [!DNL Jira] problemi. Solo i documenti caricati direttamente in [!DNL Workfront] Gli elementi vengono aggiornati anche nel [!DNL Jira] problemi. </p> </td> 
   <td> <p>[!UICONTROL Allegati]</p> <p>Un commento sugli allegati caricati viene aggiunto al <strong>[!DNL Workfront]</strong> scheda di [!DNL Jira] problema.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di completamento Pianificata]</td> 
   <td> <p>[!UICONTROL Scadenza]</p> <p>È stato aggiunto un commento sulla [!UICONTROL Scadenza] modificata [!DNL Workfront] scheda di [!DNL Jira] problema. </p> <p>Nota: è necessario abilitare <strong>[!UICONTROL Scadenza]</strong> per [!DNL Jira] problemi per visualizzare questo campo aggiornato in [!UICONTROL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>Forms personalizzato e campi personalizzati</td> 
   <td> <p> Visualizza in [!DNL Workfront] pannello a destra della [!DNL Jira] problema. <br>Nel pannello vengono visualizzati solo i campi personalizzati con un valore effettivo.<br></p> <p>Nota: le sezioni del modulo personalizzato vengono visualizzate con il livello di accesso del [!DNL Workfront] amministratore. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Priority]</td> 
   <td>Visualizzazioni in [!DNL Workfront] pannello a destra della [!DNL Jira] problema. <br>Il problema non viene aggiornato <strong>Priorità [!UICONTROL]</strong> campo in [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo di registrazione] </td> 
   <td> <p>Un commento sull'ora registrata viene aggiunto nel <strong>[!DNL Workfront]</strong> scheda di [!DNL Jira] problema. Questo include il nome dell’utente che registra l’ora e dell’utente per il quale l’ora è registrata, nel caso siano diversi. Non è stato effettuato l’accesso all’ora <strong>[!UICONTROL Registro di lavoro]</strong> scheda in [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commenti]</td> 
   <td> <p>Il commento viene aggiunto al <strong>[!DNL Workfront]</strong> scheda di [!DNL Jira] problema. Non viene aggiunto al <strong>[!UICONTROL Commenti]</strong> scheda di [!DNL Jira] problema</p> <p>Nota: quando colleghi manualmente due elementi esistenti, i commenti aggiunti al [!DNL Workfront] elemento prima del collegamento [!DNL Jira] non sincronizzare con [!DNL Jira] problema. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Aggiornare gli elementi collegati in [!DNL Jira]

Se lavori principalmente in [!DNL Jira], è possibile aggiornare gli elementi di lavoro in [!DNL Jira] e le loro controparti in [!DNL Workfront] aggiorna anche. Non è necessario disporre di [!DNL Workfront] licenza per [!DNL Workfront] elementi collegati al tuo [!DNL Jira] problemi per ricevere gli aggiornamenti che stai effettuando in [!DNL Jira].

A condizione che [!DNL Workfront] l’amministratore ha configurato [!DNL Workfront] per [!DNL Jira] per sincronizzare i campi tra gli elementi collegati, alcuni campi che vengono aggiornati in [!DNL Jira] aggiorna anche per il [!DNL Workfront] elemento.

L&#39;elenco seguente mostra quali [!DNL Jira] campi sincronizzati con [!DNL Workfront] campi sugli elementi collegati:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aggiornato [!DNL Jira] Campo</strong> </th> 
   <th><strong>Sincronizzato [!DNL Workfront] Campo/Aggiornamento</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Stato problema]</td> 
   <td> <p> [!UICONTROL Stato problema o attività]</p> <p>Stato del problema in [!DNL Jira] sincronizza con i seguenti stati, o stati che corrispondono ai seguenti stati, in Workfront:</p> 
    <ul> 
     <li> <p>[!UICONTROL Nuovo] ([!UICONTROL NUOVO])</p> </li> 
     <li> <p>[!UICONTROL In Corso] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL chiuso]/[!UICONTROL completo] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Nota: il [!DNL Jira] stato sincronizzato con il primo [!DNL Workfront] stato che corrisponde allo stato appropriato.</p> <p>Per ulteriori informazioni sugli stati degli elementi in [!DNL Workfront], vedi <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Creare o modificare uno stato</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Issue Attachments]</td> 
   <td> [!UICONTROL Documenti problema o attività]<br>Un commento sul caricamento di un nuovo documento in [!DNL Jira] viene aggiunto alla scheda [!UICONTROL Aggiornamenti] del [!DNL Workfront] problema o attività.  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scadenza]</td> 
   <td> <p> Un commento sulla modifica di [!UICONTROL Scadenza] in [!DNL Jira] viene aggiunto alla scheda [!UICONTROL Aggiornamenti] del [!DNL Workfront] problema o attività. </p> <p>Nota: non cambia nessuna data nella [!DNL Workfront] problema o attività. </p> </td> 
  </tr> 
  <tr> 
   <td> Tempo di connessione in [!DNL Workfront] nel pannello a destra o dal menu Altro di [!DNL Jira] problema<br></td> 
   <td> <p>Ore<br>Oltre ad aggiungere le ore registrate in Jira al [!DNL Workfront] elemento, un commento sull'ora di registrazione viene aggiunto alla scheda [!UICONTROL Aggiornamenti] del [!DNL Workfront] elemento.</p> <p>Per ulteriori informazioni sull'ora di accesso al collegamento [!DNL Jira] problemi, incluso l'aggiornamento di [!DNL Jira] utente che sta registrando l’ora in [!DNL Workfront], vedi <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Tempo di connessione per Collegato [!DNL Jira] e [!DNL Workfront] elementi</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Commenti <br><br></td> 
   <td> <p>I commenti vengono aggiunti alla scheda [!UICONTROL Aggiornamenti] del [!DNL Workfront] problema o attività se <strong>[!UICONTROL Commenti]</strong> impostazione nella sezione [!UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT] della scheda [!UICONTROL Setup] su <strong>[!UICONTROL Always]</strong>.</p> <p>Per informazioni sulla configurazione delle impostazioni di Workfront in [!DNL Jira], vedi <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configurazione [!DNL Workfront for Jira]</a>.</p> <p>Per informazioni sui commenti agli elementi da collegati [!DNL Jira] problemi, vedi <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Commento da un collegato [!DNL Jira] problema</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tempo di connessione da collegato [!DNL Jira] problemi

L’ora di registrazione per un [!DNL Jira] elemento in [!DNL Jira] trasferirà anche al collegato [!DNL Workfront] elemento, indipendentemente dalla posizione in [!DNL Jira] registra l’ora.\
Quando accedi a Jira in [!DNL Workfront] l&#39;ora viene registrata solo in [!DNL Workfront].\
Ora di registrazione in [!DNL Workfront] non influisce sul momento del problema collegato in [!DNL Jira].

>[!NOTE]
>
>Se l’ora viene aggiunta a un [!DNL Jira] elemento collegato a un [!DNL Workfront] attività, il [!UICONTROL Tipo di Ora] per il tempo in [!DNL Workfront] è [!UICONTROL Ora attività]. Se l’ora viene aggiunta a un [!DNL Jira] elemento collegato a un [!DNL Workfront] problema, il [!UICONTROL Tipo di Ora] per il tempo in [!DNL Workfront] è [!UICONTROL Ora problema].

Un commento viene aggiunto al **[!DNL Workfront]** scheda in [!DNL Jira] e al **[!UICONTROL Aggiornamenti]** scheda dell’elemento in [!DNL Workfront] per registrare l&#39;ora.\
L&#39;ora viene visualizzata anche nel **[!UICONTROL Ore]** scheda di [!DNL Workfront] elemento.

* [Tempo di connessione per Collegato [!DNL Jira] e [!DNL Workfront] elementi](#log-time-for-linked-jira-and-workfront-items)
* [Tempo di connessione da [!DNL Jira] a un [!DNL Workfront] elemento](#log-time-from-jira-to-a-workfront-item)

### Tempo di connessione per Collegato [!DNL Jira] e [!DNL Workfront] elementi

È possibile registrare l’ora da un [!DNL Jira] problema collegato a un [!DNL Workfront] e l&#39;ora viene registrata sia sul [!DNL Jira] problema e il [!DNL Workfront] elemento.

>[!IMPORTANT]
>
>Se l’utente effettua l’accesso [!DNL Jira] non esiste in [!DNL Workfront], l’integrazione crea un nuovo utente attivo in Workfront se **[!UICONTROL Crea automaticamente un utente in [!DNL Workfront]&#x200B;se [!DNL Jira] l’utente non dispone di un *[!DNL Workfront]&#x200B;account]** è impostato su**[!UICONTROL  Sempre ]**. Questo utente non occupa un [!DNL Workfront] licenza. È possibile assegnare utenti attivi agli elementi di lavoro in [!DNL Workfront], ma non è possibile includerli negli aggiornamenti. Per informazioni sulla configurazione della creazione automatica di [!DNL Workfront] utenti da [!DNL Jira], vedi [Configurazione [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

Per registrare l&#39;ora di un elemento in [!DNL Jira] e registrarli entrambi [!DNL Jira] e [!DNL Workfront]:

1. Accedi a [!DNL Jira].
1. Vai a [!DNL Jira] problema collegato al [!DNL Workfront] elemento.
1. Espandi **[!UICONTROL Altro]** e fai clic su **[!UICONTROL Registra lavoro]**.

1. In **[!UICONTROL Tempo trascorso]** , specificare la quantità di tempo impiegata per questo problema. È necessario specificare l&#39;ora utilizzando i seguenti periodi di tempo:

   * [!UICONTROL Weeks] (l)
   * [!UICONTROL Giorni] d)
   * [!UICONTROL Ore] h)

1. Continua ad aggiungere informazioni all’immissione dell’ora, tra cui **[!UICONTROL Descrizione lavoro]**, quindi fai clic su **[!UICONTROL Log]**.\
   L’ora viene aggiunta al **[!UICONTROL Registro di lavoro]** scheda di [!DNL Jira] e al [!DNL Workfront] elemento ad esso collegato.\
   La descrizione dell&#39;ora viene registrata come nota nella voce dell&#39;ora in [!DNL Workfront].

### Tempo di connessione da [!DNL Jira] a un [!DNL Workfront] elemento

Puoi registrare l’ora solo sul collegamento [!DNL Workfront] elemento da [!DNL Jira] problema senza registrare questa volta su [!DNL Jira] problema.

1. Accedi a [!DNL Jira].
1. Passa a [!DNL Jira] problema collegato a un [!DNL Workfront] elemento.

   I dettagli della [!DNL Workfront] l&#39;elemento deve essere visualizzato nel [!DNL Workfront] pannello a destra del problema.

1. Fai clic su **[!UICONTROL Tempo di connessione]** icona.

1. Specifica la quantità di **[!UICONTROL Ore]** e **[!UICONTROL Minutes]** desideri segnalare il problema.

1. Clic **[!UICONTROL Tempo di connessione]**.

   L’ora viene aggiunta al [!DNL Workfront] elemento.

   Questa volta non viene aggiunta al [!UICONTROL Registro di lavoro] scheda di [!DNL Jira] problema.

## Commento da un collegato [!DNL Jira] problema {#comment-from-a-linked-jira-issue}

Quando si commenta un [!DNL Jira] elemento da [!DNL Workfront] pannello destro in [!DNL Jira], il commento viene aggiunto anche al [!UICONTROL Aggiornamenti] dell’elemento collegato in Workfront.

Per commentare da [!DNL Jira] a un [!DNL Workfront] elemento:

1. Accedi a [!DNL Jira].
1. Passa a [!DNL Jira] problema collegato a un [!DNL Workfront] elemento.

   I dettagli della [!DNL Workfront] l&#39;elemento deve essere visualizzato nel [!DNL Workfront] pannello a destra del problema.

1. Fai clic su **[!UICONTROL Commenti]** icona in [!DNL Workfront] o sul pannello **[!UICONTROL Commenti]** scheda.

1. Inizia a digitare un commento, quindi fai clic su **[!UICONTROL Invia]**.

   Il commento è aggiunto al seguente:

   * Il **[!DNL Workfront]** scheda di [!DNL Jira] problema.
   * Il **[!UICONTROL Commenti]** scheda di [!DNL Jira] problema.
   * Il **[!UICONTROL Aggiornamenti]** dell’elemento collegato in Workfront.
