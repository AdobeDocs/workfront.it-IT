---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Aggiorna gli elementi collegati tra [!DNL Jira] e [!DNL Adobe Workfront]
description: Quando si collega [!DNL Jira] questioni [!DNL Adobe Workfront] attività o problemi, gli utenti possono aggiornare gli elementi in un'applicazione e la controparte di tale elemento viene aggiornata anche per gli utenti che lavorano nella seconda applicazione.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '1703'
ht-degree: 0%

---

# Aggiorna gli elementi collegati tra [!DNL Jira] e [!DNL Adobe Workfront]

Quando si collega [!DNL Jira] questioni [!DNL Adobe Workfront] attività o problemi, gli utenti possono aggiornare gli elementi in un&#39;applicazione e la controparte di tale elemento viene aggiornata anche per gli utenti che lavorano nella seconda applicazione.

Per ulteriori informazioni sul collegamento di elementi tra [!DNL Workfront] e [!DNL Jira], vedi [Collegamento di elementi tra Adobe Workfront e Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Durante la configurazione [!DNL Workfront] per [!DNL Jira], come [!DNL Jira] amministratore di sistema, è possibile configurare determinati campi da un&#39;applicazione per eseguire la sincronizzazione con i campi degli elementi collegati nell&#39;altra applicazione.

Per ulteriori informazioni sulla sincronizzazione dei campi tra collegati [!DNL Jira] e [!DNL Workfront] elementi, vedi [Configura [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] piano</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] panoramica delle licenze</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] accesso</td> 
   <td> <p>Accesso amministratore di sistema</p> <p>Importante: È consigliabile creare account di amministratore di sistema separati in [!DNL Jira] e [!DNL Workfront] per dedicare a questa integrazione, anziché utilizzare quelle esistenti che potrebbero essere collegate agli utenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Prerequisiti

Prima di poter collegare elementi tra [!DNL Workfront] e [!DNL Jira], devi

* Installa [!DNL Workfront for Jira].

   Per istruzioni sull’installazione [!DNL Workfront for Jira], vedi [Installa [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configura [!DNL Workfront for Jira].

   Per istruzioni sulla configurazione [!DNL Workfront for Jira], vedi [Configura [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Collega elementi tra [!DNL Workfront] e [!DNL Jira].

   Per istruzioni, consulta [Collega elementi tra [!DNL Adobe Workfront] e [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Aggiorna elementi collegati in [!DNL Workfront]

Se lavori principalmente in [!DNL Workfront], è possibile aggiornare gli elementi di lavoro in [!DNL Workfront] e loro omologhi [!DNL Jira] anche aggiornare. Questo aggiornamento avviene tramite l&#39;integrazione di [!DNL Workfront] per [!DNL Jira] che non richiede un [!DNL Jira] licenza.

Finché il tuo [!DNL Workfront] amministratore configurato [!DNL Workfront for Jira] per sincronizzare i campi tra gli elementi collegati, alcuni campi che vengono aggiornati in [!DNL Workfront] viene inoltre aggiornato per [!DNL Jira] problema. Per ulteriori informazioni sull’aggiornamento degli elementi in [!DNL Workfront], vedi [Modifica dei problemi](../../manage-work/issues/manage-issues/edit-issues.md) e [Modifica delle attività](../../manage-work/tasks/manage-tasks/edit-tasks.md).

Nell&#39;elenco seguente viene illustrato quale [!DNL Workfront] campi sincronizzati con [!DNL Jira] campi relativi agli elementi collegati:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aggiornato [!DNL Workfront] field</strong> </th> 
   <th><strong>Sincronizzato [!DNL Jira] field/ update</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Problema o nome dell'attività]</td> 
   <td> <p>[!UICONTROL Nome del problema]</p> <p>Alla variabile <strong>[!DNL Workfront]</strong> della scheda [!DNL Jira] problema. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema o descrizione attività]</td> 
   <td> <p> [!UICONTROL Issue Description]</p> <p>Al gruppo viene aggiunto un commento sulla descrizione aggiornata <strong>[!DNL Workfront]</strong> della scheda [!DNL Jira] problema.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Documenti caricati]</p> <p>Nota: Documenti collegati a [!DNL Workfront] gli elementi di un server esterno non vengono trasferiti in [!DNL Jira] problemi. Solo documenti caricati direttamente in [!DNL Workfront] gli elementi vengono anche aggiornati al [!DNL Jira] problemi. </p> </td> 
   <td> <p>[!UICONTROL Allegati]</p> <p>Un commento sugli allegati caricati viene aggiunto al <strong>[!DNL Workfront]</strong> della scheda [!DNL Jira] problema.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di completamento pianificata]</td> 
   <td> <p>[!UICONTROL Data di scadenza]</p> <p>Un commento sulla modifica della [!UICONTROL Due Date] viene aggiunto al [!DNL Workfront] della scheda [!DNL Jira] problema. </p> <p>Nota: È necessario attivare <strong>[!UICONTROL Data di scadenza]</strong> per [!DNL Jira] problemi per poter visualizzare questo campo aggiornato in [!UICONTROL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>Campi personalizzati Forms e personalizzati</td> 
   <td> <p> Visualizza in [!DNL Workfront] pannello di destra [!DNL Jira] problema. <br>Nel pannello vengono visualizzati solo i campi personalizzati con un valore effettivo.<br></p> <p>Nota: Le sezioni Modulo personalizzato vengono visualizzate con il livello di accesso [!DNL Workfront] amministratore. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema o Priorità attività]</td> 
   <td>Visualizza nella [!DNL Workfront] pannello di destra [!DNL Jira] problema. <br>Non aggiorna il problema <strong>[!UICONTROL Priority]</strong> campo [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Log time] </td> 
   <td> <p>Nella sezione <strong>[!DNL Workfront]</strong> della scheda [!DNL Jira] problema. Ciò include il nome dell’utente che registra l’ora, nonché l’utente per il quale l’ora è registrata, nel caso in cui siano diverse. Nessun tempo di accesso al <strong>[!UICONTROL Work log]</strong> scheda in [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commenti]</td> 
   <td> <p>Il commento viene aggiunto al <strong>[!DNL Workfront]</strong> della scheda [!DNL Jira] problema. Non viene aggiunto al <strong>[!UICONTROL Commenti]</strong> della scheda [!DNL Jira] problema</p> <p>Nota: Quando colleghi manualmente due elementi esistenti, i commenti aggiunti al [!DNL Workfront] elemento prima di collegarlo a [!DNL Jira] non eseguire la sincronizzazione con [!DNL Jira] problema. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Aggiorna elementi collegati in [!DNL Jira]

Se lavori principalmente in [!DNL Jira], è possibile aggiornare gli elementi di lavoro in [!DNL Jira] e loro omologhi [!DNL Workfront] anche aggiornare. Non devi avere un [!DNL Workfront] licenza per [!DNL Workfront] elementi collegati al [!DNL Jira] problemi relativi alla ricezione degli aggiornamenti che stai effettuando in [!DNL Jira].

A condizione che il tuo [!DNL Workfront] amministratore configurato [!DNL Workfront] per [!DNL Jira] per sincronizzare i campi tra elementi collegati, alcuni campi che vengono aggiornati in [!DNL Jira] viene inoltre aggiornato per [!DNL Workfront] oggetto.

Nell&#39;elenco seguente viene illustrato quale [!DNL Jira] campi sincronizzati con [!DNL Workfront] campi relativi agli elementi collegati:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aggiornato [!DNL Jira] Campo</strong> </th> 
   <th><strong>Sincronizzato [!DNL Workfront] Campo/aggiornamento</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Stato del problema]</td> 
   <td> <p> [!UICONTROL Problema o stato dell'attività]</p> <p>Stato del problema in [!DNL Jira] sincronizza con i seguenti stati, o stati che corrispondono ai seguenti stati, in Workfront:</p> 
    <ul> 
     <li> <p>[!UICONTROL New] ([!UICONTROL NEW])</p> </li> 
     <li> <p>[!UICONTROL In Corso] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Closed]/[!UICONTROL Complete] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Nota: La [!DNL Jira] lo stato si sincronizza con il primo [!DNL Workfront] che equivale allo stato appropriato.</p> <p>Per ulteriori informazioni sugli stati degli elementi in [!DNL Workfront], vedi <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Creare o modificare uno stato</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issignee]</td> 
   <td> <p> [!UICONTROL Problema o Assegnatario attività]</p> <p>Importante: Quando si assegna un elemento in [!DNL Jira] a un utente che non ha [!DNL Workfront] l'integrazione crea un nuovo utente attivo in [!DNL Workfront] solo quando l'opzione "[!UICONTROL Crea automaticamente un utente in [!DNL Workfront] se [!DNL Jira] l'utente non ha un [!DNL Workfront] account]" è impostato su [!UICONTROL Always]. Questo utente non occupa un [!DNL Workfront] licenza. Gli utenti attivi possono essere assegnati agli elementi di lavoro in [!DNL Workfront], ma non può essere incluso negli aggiornamenti. Per ulteriori informazioni sulla configurazione della creazione automatica di [!DNL Workfront] utenti da [!DNL Jira], vedi <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configurazione [!DNL Workfront for Jira]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problemi allegati]</td> 
   <td> [!UICONTROL Problemi o documenti di attività]<br>Un commento sul caricamento di un nuovo documento in [!DNL Jira] viene aggiunto alla scheda [!UICONTROL Updates] del [!DNL Workfront] problema o attività.  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di scadenza]</td> 
   <td> <p> Un commento sulla modifica della [!UICONTROL Due Date] in [!DNL Jira] viene aggiunto alla scheda [!UICONTROL Updates] del [!DNL Workfront] problema o attività. </p> <p>Nota: Nessuna modifica delle date nella [!DNL Workfront] problema o attività. </p> </td> 
  </tr> 
  <tr> 
   <td> Tempo di accesso [!DNL Workfront] pannello a destra o dal menu [!UICONTROL More] (Altro) [!DNL Jira] problema<br></td> 
   <td> <p>Ore<br>Oltre ad aggiungere le ore registrate in Jira al link [!DNL Workfront] un commento sul tempo di registrazione viene aggiunto alla scheda [!UICONTROL Updates] di [!DNL Workfront] oggetto.</p> <p>Per ulteriori informazioni sul tempo di accesso ai collegamenti [!DNL Jira] questioni, compreso l'aggiornamento [!DNL Jira] utente che accede al registro [!DNL Workfront], vedi <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Tempo di log per Linked [!DNL Jira] e [!DNL Workfront] items</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Commenti <br><br></td> 
   <td> <p>I commenti vengono aggiunti alla scheda [!UICONTROL Updates] di [!DNL Workfront] emissione o attività se <strong>[!UICONTROL Commenti]</strong> impostazione nella sezione [!UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT] della scheda [!UICONTROL Setup] su <strong>[!UICONTROL Always]</strong>.</p> <p>Per informazioni sulla configurazione delle impostazioni Workfront in [!DNL Jira], vedi <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configurazione [!DNL Workfront for Jira]</a>.</p> <p>Per informazioni su commenti su elementi collegati [!DNL Jira] problemi, vedi <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Commento da un collegamento [!DNL Jira] problema</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tempo di log da collegato [!DNL Jira] questioni

L&#39;ora in cui si registra un [!DNL Jira] elemento in [!DNL Jira] trasferirà anche al link [!DNL Workfront] articolo, indipendentemente da dove [!DNL Jira] si registra l&#39;ora.\
Quando si registra il tempo in Jira nel [!DNL Workfront] il tempo viene registrato solo in [!DNL Workfront].\
L&#39;ora in cui si registra [!DNL Workfront] non influisce sul tempo del problema collegato in [!DNL Jira].

>[!NOTE]
>
>Se l’ora viene aggiunta a un [!DNL Jira] elemento collegato a un [!DNL Workfront] l&#39;attività [!UICONTROL Tipo ora] per l&#39;ora [!DNL Workfront] è [!UICONTROL Ora attività]. Se l’ora viene aggiunta a un [!DNL Jira] elemento collegato a un [!DNL Workfront] il problema [!UICONTROL Tipo ora] per l&#39;ora [!DNL Workfront] è [!UICONTROL Ora del problema].

Un commento viene aggiunto al **[!DNL Workfront]** scheda in [!DNL Jira] e **[!UICONTROL Aggiornamenti]** scheda dell&#39;elemento in [!DNL Workfront] per registrare l&#39;ora.\
L’ora viene visualizzata anche nella **[!UICONTROL Ore]** della scheda [!DNL Workfront] oggetto.

* [Tempo di log per Linked [!DNL Jira] e [!DNL Workfront] items](#log-time-for-linked-jira-and-workfront-items)
* [Tempo di log da [!DNL Jira] a [!DNL Workfront] item](#log-time-from-jira-to-a-workfront-item)

### Tempo di log per Linked [!DNL Jira] e [!DNL Workfront] items

È possibile registrare l&#39;ora da un [!DNL Jira] problema collegato a un [!DNL Workfront] e l&#39;ora viene registrata sia sul [!DNL Jira] e [!DNL Workfront] oggetto.

>[!IMPORTANT]
>
>Se l&#39;utente accede al momento [!DNL Jira] non esiste in [!DNL Workfront], l&#39;integrazione crea un nuovo utente attivo in Workfront se **[!UICONTROL Crea automaticamente un utente in [!DNL Workfront]&#x200B; se [!DNL Jira] l&#39;utente non ha un *[!DNL Workfront]&#x200B; account]** è impostato su**[!UICONTROL  Sempre ]**. Questo utente non occupa un [!DNL Workfront] licenza. È possibile assegnare utenti attivi a elementi di lavoro in [!DNL Workfront], ma non puoi includerli negli aggiornamenti. Per informazioni sulla configurazione della creazione automatica di [!DNL Workfront] utenti da [!DNL Jira], vedi [Configurazione [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

Per registrare il tempo di un elemento in [!DNL Jira] e registrarli entrambi [!DNL Jira] e [!DNL Workfront]:

1. Accedi a [!DNL Jira].
1. Vai a [!DNL Jira] problema collegato al [!DNL Workfront] oggetto.
1. Espandi la **[!UICONTROL Altro]** menu e fai clic su **[!UICONTROL Registro di lavoro]**.

1. In **[!UICONTROL Tempo trascorso]** specifica la quantità di tempo impiegato per questo problema. È necessario specificare l’ora utilizzando i seguenti periodi di tempo:

   * [!UICONTROL Settimane] (w)
   * [!UICONTROL Giorni] d)
   * [!UICONTROL Ore] h)

1. Continua ad aggiungere informazioni alla voce dell’ora, tra cui una **[!UICONTROL Descrizione del lavoro]**, quindi fai clic su **[!UICONTROL Registro]**.\
   L’ora viene aggiunta al **[!UICONTROL Registro di lavoro]** della scheda [!DNL Jira] e al [!DNL Workfront] elemento collegato ad esso.\
   La descrizione del lavoro dell&#39;inserimento dell&#39;ora viene registrata come nota sulla voce dell&#39;ora in [!DNL Workfront].

### Tempo di log da [!DNL Jira] a [!DNL Workfront] item

È possibile registrare l&#39;ora solo al link [!DNL Workfront] dell&#39;articolo [!DNL Jira] problema senza registrare questa volta [!DNL Jira] problema.

1. Accedi a [!DNL Jira].
1. Passa a un [!DNL Jira] problema collegato a un [!DNL Workfront] oggetto.

   I dettagli della [!DNL Workfront] l&#39;elemento deve essere visualizzato in [!DNL Workfront] pannello a destra del problema.

1. Fai clic sul pulsante **[!UICONTROL Tempo di log]** icona.

1. Specifica l&#39;importo di **[!UICONTROL Ore]** e **[!UICONTROL Minutes]** desideri registrare il problema.

1. Fai clic su **[!UICONTROL Tempo di log]**.

   L’ora viene aggiunta al [!DNL Workfront] oggetto.

   Questa ora non viene aggiunta al [!UICONTROL Registro di lavoro] della scheda [!DNL Jira] problema.

## Commento da un collegamento [!DNL Jira] problema {#comment-from-a-linked-jira-issue}

Quando commenta un [!DNL Jira] dell&#39;articolo [!DNL Workfront] pannello destro in [!DNL Jira], il commento viene aggiunto anche al [!UICONTROL Aggiornamenti] scheda dell’elemento collegato in Workfront.

Per commentare da [!DNL Jira] a [!DNL Workfront] articolo:

1. Accedi a [!DNL Jira].
1. Passa a un [!DNL Jira] problema collegato a un [!DNL Workfront] oggetto.

   I dettagli della [!DNL Workfront] l&#39;elemento deve essere visualizzato in [!DNL Workfront] pannello a destra del problema.

1. Fai clic sul pulsante **[!UICONTROL Commenti]** nella [!DNL Workfront] o **[!UICONTROL Commenti]** scheda .

1. Inizia a digitare un commento, quindi fai clic su **[!UICONTROL Invia]**.

   Il commento è aggiunto al seguente:

   * La **[!DNL Workfront]** della scheda [!DNL Jira] problema.
   * La **[!UICONTROL Commenti]** della scheda [!DNL Jira] problema.
   * La **[!UICONTROL Aggiornamenti]** scheda dell’elemento collegato in Workfront.
