---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli di gestione utente di Adobe
description: In uno scenario  [!DNL Adobe Workfront Fusion] , puoi automatizzare i flussi di lavoro che gestiscono gli utenti nel tuo account Adobe.
author: Becky
feature: Workfront Fusion
source-git-commit: 6470ea408bfd354707387f7916edb08b4879168c
workflow-type: tm+mt
source-wordcount: '2362'
ht-degree: 2%

---

# Moduli di gestione utente di Adobe

In uno scenario [!DNL Adobe Workfront Fusion], puoi automatizzare i flussi di lavoro che gestiscono gli utenti nel tuo account Adobe.


Se hai bisogno di istruzioni per la creazione di uno scenario, consulta [Creare uno scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, vedere [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o versione successiva</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Creare una connessione a Gestione utenti di Adobe

Per creare una connessione per i moduli [!DNL Adobe User Management]:

1. Fai clic su **[!UICONTROL Aggiungi]** accanto alla casella Connessione.

1. Compila i campi seguenti:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Nome connessione]</td>
        <td>
          <p>Immettere un nome per la connessione.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>Seleziona se ti connetti a un ambiente di produzione o non di produzione.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Specificare se ci si connette a un account di servizio o a un account personale.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID client]</td>
        <td>Immetti [!UICONTROL Adobe] [!UICONTROL ID client]. Questo si trova nella sezione dei dettagli [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Segreto client]</td>
        <td>Immetti [!DNL Adobe] [!UICONTROL Client Secret]. Questo si trova nella sezione dei dettagli [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL IMS Organization ID]</td>
        <td>Immetti le tue credenziali IMS di [!DNL Adobe]. L’identificatore univoco di un’organizzazione. Questa è una stringa del formato A495E53@AdobeOrg in cui il prefisso prima di @ è un numero esadecimale. Puoi trovare questo valore come parte del percorso URL per l’organizzazione nell’Admin Console o nella console adobe.io per l’integrazione di User Management.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Ambiti aggiuntivi]</td>
        <td>Per ogni ambito aggiuntivo che si desidera aggiungere, fare clic su <b>Aggiungi elemento</b> e immettere l'ambito.</td>
        </tr>
      </tbody>
    </table>

1. Fai clic su **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo.



## Moduli di gestione utenti di Adobe e relativi campi

Quando configuri i moduli di Gestione utenti di Adobe, Workfront Fusion visualizza i campi elencati di seguito. Insieme a questi, possono essere visualizzati campi aggiuntivi di Gestione utente di Adobe, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ricerche](#searches)
* [Azioni utente](#user-actions)
* [Azioni gruppo utenti](#user-group-actions)
* [Altro](#other)

### Ricerche

* [Ottenere gruppi di utenti e profili di prodotto](#get-user-groups-and-product-profiles)
* [Ottieni informazioni utente](#get-user-information)
* [Ottenere gli utenti in un gruppo di utenti o un profilo di prodotto](#get-users-in-a-user-group-or-product-profile)
* [Ottenere gli utenti in un’organizzazione](#get-users-in-an-organization)

#### Ottenere gruppi di utenti e profili di prodotto

Questo modulo di ricerca recupera un elenco di tutti i gruppi di utenti e i profili di prodotto dell’organizzazione, insieme ai dettagli sui gruppi e i profili.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connessione</td> 
   <td>Per istruzioni sulla creazione di una connessione a Gestione utenti Adobe, vedere <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Creare una connessione a Gestione utenti Adobe</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Numero massimo di risultati restituiti</td> 
   <td>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### Ottieni informazioni utente

Questo modulo di ricerca recupera i dettagli per un singolo utente dell’organizzazione, identificati dal suo indirizzo e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connessione</td> 
   <td>Per istruzioni sulla creazione di una connessione a Gestione utenti Adobe, vedere <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Creare una connessione a Gestione utenti Adobe</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Indirizzo e-mail</td> 
   <td>Inserisci o mappa l’indirizzo e-mail dell’utente per il quale desideri restituire i dettagli. Per Adobe ID, Enterprise e gli utenti federati e-mail, questo deve essere l’indirizzo e-mail completo, compreso il dominio. In tutti i casi, il parametro non distingue tra maiuscole e minuscole.</td> 
  </tr> 
 </tbody> 
</table>

#### Ottenere gli utenti in un gruppo di utenti o un profilo di prodotto

Questo modulo di ricerca recupera un elenco di tutti gli utenti nel gruppo di utenti o nel profilo di prodotto specificato, insieme ai dettagli sugli utenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connessione</td> 
   <td>Per istruzioni sulla creazione di una connessione a Gestione utenti Adobe, vedere <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Creare una connessione a Gestione utenti Adobe</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome gruppo</td> 
   <td>Il gruppo utenti, il nome del profilo di prodotto o un gruppo amministrativo. Per un gruppo di amministratori, il nome può essere uno dei gruppi fissi <code>_org_admin</code>, <code>_deployment_admin</code> o <code>_support_admin</code> oppure un gruppo di amministratori specifico per il gruppo. Questi sono identificati con un prefisso nel nome del gruppo, ad esempio <code>_admin_groupName</code>, <code>_product_admin_productName</code> o <code>_developer_groupName</code>. Se il gruppo esiste ma il gruppo amministratore non lo è, viene restituito un elenco vuoto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Solo diretto</td> 
   <td>Specifica se il campo dei gruppi nella struttura utente restituita contiene solo i profili di prodotto di cui l’utente è membro diretto. Se false, restituisce tutti i gruppi (gruppi di utenti, profili di prodotto e gruppi di amministratori) contenenti l’utente, indipendentemente dal fatto che un diritto per un particolare profilo di prodotto arrivi direttamente (tramite l’assegnazione dell’utente) o indirettamente (tramite un gruppo di utenti che contiene l’utente assegnato al profilo di prodotto). Se true, restituisce tutti i gruppi di utenti e di amministratori che contengono l'utente, ma solo i profili di prodotto a cui l'utente è stato esplicitamente assegnato un diritto. Un utente può essere sia un membro diretto che un membro indiretto di un profilo di prodotto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Escludi gruppi</td> 
   <td>Specifica se la risposta esclude la restituzione dell’array dei gruppi per ogni singolo utente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Stato</td> 
   <td>Questa opzione è valida solo per i profili di prodotto. Seleziona attivo per elencare gli utenti per i quali è stato eseguito il provisioning del prodotto e dispongono di una licenza attiva. Seleziona inattivo per elencare gli utenti che sono stati aggiunti al profilo di prodotto ma non dispongono di una licenza attiva. Se lasciato vuoto, il modulo restituisce tutti gli utenti membri indipendentemente dal loro stato di adesione.
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Numero massimo di risultati restituiti</td> 
   <td>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### Ottenere gli utenti in un’organizzazione

Questo modulo di ricerca restituisce tutti gli utenti dell’organizzazione associati alla connessione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connessione</td> 
   <td>Per istruzioni sulla creazione di una connessione a Gestione utenti Adobe, vedere <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Creare una connessione a Gestione utenti Adobe</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Numero massimo di risultati restituiti</td> 
   <td>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>

### Azioni utente

* [Aggiungere un utente come membro di un gruppo](#add-a-user-as-a-member-of-a-group)
* [Creare un utente](#create-a-user)
* [Rimuovere un utente dai gruppi](#remove-a-user-from-groups)
* [Aggiornare un utente](#update-a-user)

#### Aggiungere un utente come membro di un gruppo

Questo modulo di azione aggiunge un utente come membro del gruppo o dei gruppi specificati. Questo modulo può aggiungere l’utente a un massimo di quattro gruppi.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connessione</td> 
   <td>Per istruzioni sulla creazione di una connessione a Gestione utenti Adobe, vedere <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Creare una connessione a Gestione utenti Adobe</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Utente</td> 
   <td>Inserisci o mappa l’utente che desideri aggiungere ai gruppi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dominio</td> 
   <td>Per gli ID federati che non sono indirizzi e-mail, immetti il dominio a cui appartiene l’utente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gruppi</td> 
   <td>Per ogni gruppo a cui si desidera aggiungere l'utente, fare clic su <b>Aggiungi elemento</b> e immettere o mappare il gruppo. È possibile immettere fino a quattro gruppi e deve immetterne almeno uno.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Utilizzare Adobe ID</td> 
   <td>Seleziona true per garantire che l'ID utente venga interpretato come riferito a un Adobe ID esistente anche se esiste un'azienda o un Federated ID con lo stesso nome.</td> 
  </tr> 
 </tbody> 
</table>

#### Creare un utente

Questo modulo di azione crea un nuovo utente nell’organizzazione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connessione</td> 
   <td>Per istruzioni sulla creazione di una connessione a Gestione utenti Adobe, vedere <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Creare una connessione a Gestione utenti Adobe</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo ID</td> 
   <td>Seleziona se desideri creare un utente con un’Adobe ID, un’Enterprise ID o un Federated ID. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Accedi</td> 
   <td>Se stai creando un utente con un Federated ID, seleziona il tipo di accesso.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">E-mail</td> 
   <td>Inserisci o mappa l’indirizzo e-mail per il nuovo utente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dominio</td> 
   <td>Se stai creando un utente con un Federated ID con un accesso basato su dominio, immetti o mappa il dominio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Utente</td> 
   <td>Se stai creando un utente con un Federated ID con un accesso basato su dominio, immetti o mappa l’utente che questo nuovo utente rappresenterà.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome</td> 
   <td>Inserisci o mappa il nome dell’utente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cognome</td> 
   <td>Inserisci o mappa il cognome dell’utente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nazione</td> 
   <td>Immetti o mappa il codice ISO a due caratteri del paese. Una volta creato l'utente, non è possibile modificare questa impostazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Opzione</td> 
   <td>Seleziona l’azione da intraprendere se l’utente esiste già nell’organizzazione. Se non è selezionata alcuna opzione e l’utente esiste già, il modulo restituisce un errore.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Utilizzare Adobe ID</td> 
   <td>Se è true, l'ID utente viene interpretato come riferito a un Adobe ID esistente anche se esiste un'azienda o un Federated ID con lo stesso nome.</td> 
  </tr> 
 </tbody> 
</table>

#### Rimuovere un utente dai gruppi

Questo modulo di azione rimuove l’appartenenza di un utente dai gruppi specificati. È possibile rimuovere un utente da un massimo di quattro gruppi alla volta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connessione</td> 
   <td>Per istruzioni sulla creazione di una connessione a Gestione utenti Adobe, vedere <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Creare una connessione a Gestione utenti Adobe</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Utente</td> 
   <td>Immettere o mappare l'utente da rimuovere dai gruppi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dominio</td> 
   <td>Per gli ID federati che non sono indirizzi e-mail, immetti il dominio a cui appartiene l’utente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gruppi</td> 
   <td>Per ogni gruppo da cui si desidera rimuovere l'utente, fare clic su <b>Aggiungi elemento</b> e immettere o mappare il gruppo. È possibile immettere fino a quattro gruppi e deve immetterne almeno uno.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Utilizzare Adobe ID</td> 
   <td>Seleziona true per garantire che l'ID utente venga interpretato come riferito a un Adobe ID esistente anche se esiste un'azienda o un Federated ID con lo stesso nome.</td> 
  </tr> 
 </tbody> 
</table>



#### Aggiornare un utente

Questo modulo aggiorna un utente esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connessione</td> 
   <td>Per istruzioni sulla creazione di una connessione a Gestione utenti Adobe, vedere <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Creare una connessione a Gestione utenti Adobe</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Utente</td> 
   <td>Inserisci o mappa l’ID dell’utente che desideri aggiornare. Questo è l’indirizzo e-mail dell’utente, ad esempio <code>user@example.com</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dominio</td> 
   <td>Se stai aggiornando un utente con un Federated ID che non è un indirizzo e-mail, immetti o mappa il dominio a cui appartiene l’utente per identificarlo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">E-mail</td> 
   <td>Inserisci o mappa il nuovo indirizzo e-mail per l’utente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome</td> 
   <td>Inserisci o mappa il nome dell’utente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cognome</td> 
   <td>Inserisci o mappa il cognome dell’utente.</td> 
  </tr> 
 </tbody> 
</table>

### Azioni gruppo utenti

* [Aggiungere appartenenze a un gruppo di utenti](#add-memberships-for-a-user-group)
* [Creare un gruppo di utenti](#create-a-user-group)
* [Eliminare un gruppo di utenti](#delete-a-user-group)
* [Rimuovere le appartenenze per un gruppo di utenti](#remove-memberships-for-a-user-group)
* [Aggiornare un gruppo di utenti](#update-a-user-group)

#### Aggiungere appartenenze a un gruppo di utenti

Questo modulo di azione aggiunge utenti e profili di prodotto a un gruppo di utenti. Gli utenti aggiunti al gruppo di utenti acquisiscono il diritto a tutti i profili di prodotto nel gruppo di utenti. L’aggiunta di un profilo di prodotto dà diritto a tale profilo agli utenti del gruppo di utenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connessione</td> 
   <td>Per istruzioni sulla creazione di una connessione a Gestione utenti Adobe, vedere <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Creare una connessione a Gestione utenti Adobe</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome gruppo</td> 
   <td>Inserisci o mappa il nome del gruppo da cui desideri rimuovere gli utenti o i profili.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Utenti</td> 
   <td>Per ogni utente che desideri aggiungere, fai clic su <b>Aggiungi utente</b> e immetti l'indirizzo e-mail dell'utente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profili</td> 
   <td>Per ogni profilo da aggiungere al gruppo, fare clic su <b>Aggiungi utente</b> e immettere il nome del profilo</td> 
  </tr> 
 </tbody> 
</table>

#### Creare un gruppo di utenti

Questo modulo di azione crea un nuovo gruppo di utenti. Se esiste già un gruppo con il nome specificato, il modulo può aggiornare il gruppo esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connessione</td> 
   <td>Per istruzioni sulla creazione di una connessione a Gestione utenti Adobe, vedere <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Creare una connessione a Gestione utenti Adobe</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome gruppo</td> 
   <td>Immettere o mappare un nome per il nuovo gruppo di utenti.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Descrizione</td> 
   <td>Immettere o mappare una descrizione per il nuovo gruppo di utenti.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Opzione</td> 
   <td>Seleziona l’azione da intraprendere se il gruppo di utenti esiste già nell’organizzazione. Se non è selezionata alcuna opzione e il gruppo di utenti esiste già, il modulo restituisce un errore.</td> 
  </tr> 
 </tbody> 
</table>

#### Eliminare un gruppo di utenti

Questo modulo di azione elimina un gruppo di utenti esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connessione</td> 
   <td>Per istruzioni sulla creazione di una connessione a Gestione utenti Adobe, vedere <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Creare una connessione a Gestione utenti Adobe</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome gruppo</td> 
   <td>Immettere o mappare il nome del gruppo che si desidera eliminare.</td> 
  </tr> 
 </tbody> 
</table>

#### Rimuovere le appartenenze per un gruppo di utenti

Questo modulo di azione rimuove utenti o profili da un gruppo di utenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connessione</td> 
   <td>Per istruzioni sulla creazione di una connessione a Gestione utenti Adobe, vedere <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Creare una connessione a Gestione utenti Adobe</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome gruppo</td> 
   <td>Inserisci o mappa il nome del gruppo da cui desideri rimuovere gli utenti o i profili.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Utenti</td> 
   <td>Per ogni utente che si desidera rimuovere, fare clic su <b>Aggiungi utente</b> e immettere l'indirizzo di posta elettronica dell'utente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profili</td> 
   <td>Per ogni profilo da rimuovere dal gruppo, fare clic su <b>Aggiungi utente</b> e immettere il nome del profilo</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Utilizzare Adobe ID</td> 
   <td>Se è true, l’ID utente viene interpretato come riferito a un Adobe ID esistente anche se esiste un’azienda o un Federated ID con lo stesso nome.</td> 
  </tr> 
 </tbody> 
</table>

#### Aggiornare un gruppo di utenti

Questo modulo di azione aggiorna un gruppo di utenti esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connessione</td> 
   <td>Per istruzioni sulla creazione di una connessione a Gestione utenti Adobe, vedere <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Creare una connessione a Gestione utenti Adobe</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome gruppo originale</td> 
   <td>Immettere o mappare il nome corrente del gruppo che si desidera aggiornare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome nuovo gruppo</td> 
   <td>Immettere o mappare il nuovo nome che si desidera assegnare al gruppo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome gruppo originale</td> 
   <td>Immettere o mappare la descrizione aggiornata del gruppo.</td> 
  </tr> 
 </tbody>

### Altro

Questo modulo di azione effettua una chiamata personalizzata all’API User Management di Adobe.

#### Effettuare una chiamata API personalizzata

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connessione</td>
      <td>Per istruzioni sulla creazione di una connessione a Gestione utenti Adobe, vedere <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Creare una connessione a Gestione utenti Adobe</a> in questo articolo.</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>URL</p>
      </td>
      <td>
        <p>Inserisci un percorso relativo a <code>https://usermanagement.adobe.io/v2/usermanagement/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Metodo</p>
      </td>
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, vedere <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">Intestazioni</td>
      <td>
        <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p>
        <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione e le intestazioni x-api-key.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Stringa di query  </td>
      <td>
        <p>Immettere la stringa di query richiesta.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Corpo</td>
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserire le virgolette al di fuori dell'istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>










