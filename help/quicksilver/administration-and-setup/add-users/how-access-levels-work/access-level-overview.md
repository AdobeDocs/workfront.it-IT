---
title: Panoramica dei nuovi livelli di accesso
user-type: administrator
content-type: reference
product-area: system-administration
keywords: accesso, livello, sistema, amministratore, standard, luce, contributore
navigation-topic: access-levels
description: Per poter accedere e lavorare in Workfront, ogni utente deve disporre di un livello di accesso. È possibile utilizzare il livello di accesso per controllare ciò che un utente può vedere e fare con determinati oggetti e aree di Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: d297d8a4-5a4e-418f-983a-19545aeb0668
source-git-commit: 4af7a72a3633f1b669cbc681f230727cc4f54d1e
workflow-type: tm+mt
source-wordcount: '1626'
ht-degree: 4%

---

# Panoramica dei nuovi livelli di accesso

In qualità di amministratore di Adobe Workfront, assegni un livello di accesso a un utente per 2 scopi:

* Per poter accedere e lavorare in Workfront, ogni utente deve disporre di un livello di accesso.
* È possibile utilizzare il livello di accesso per controllare ciò che un utente può vedere e fare con determinati oggetti e aree di Workfront.

## Nuovi livelli di accesso incorporati in Adobe Workfront {#built-in-access}

Workfront offre 6 nuovi livelli di accesso incorporati:

* Amministratore di Sistema
* Standard
* Light
* Collaboratore
* Esterno

A seconda del livello di accesso, sono disponibili fino a 3 autorizzazioni per la maggior parte dei tipi di oggetto Workfront:

<table style="table-layout:auto">
    <tr>
        <td>Modifica</td>
        <td>Gli utenti possono creare, modificare, eliminare e condividere l’oggetto Workfront</td>
    </tr>
    <tr>
        <td>Visualizza</td>
        <td>Gli utenti possono rivedere e condividere l'oggetto Workfront</td>
    </tr>
    <tr>
        <td>Nessun accesso</td>
        <td>Gli utenti non possono accedere all’oggetto Workfront</td>
    </tr>
</table>

Se hai bisogno di un livello di accesso personalizzato, puoi copiare il livello di accesso integrato e regolare la quantità di accesso che desideri che consenta ai vari tipi di oggetti Workfront. Per informazioni sulla creazione di un livello di accesso personalizzato, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>È vivamente consigliato lasciare invariati i livelli di accesso incorporati, in modo da potervi fare riferimento dopo aver configurato gli utenti.

### Livello di accesso amministratore di sistema

In allegato alla licenza Standard, questo livello di accesso integrato è progettato per un utente che si occupa dell&#39;amministrazione del sistema Adobe Workfront. Non è possibile modificare questo livello di accesso integrato.

Gli utenti con il livello di accesso amministratore di sistema possono eseguire tutte le operazioni all’interno di Workfront. Possono visualizzare e modificare tutti gli oggetti e le informazioni Workfront immessi in Workfront da tutti gli altri utenti.

Hanno inoltre accesso all&#39;area di configurazione completa, dove possono modificare qualsiasi impostazione a livello di sistema, e possono accedere a tutte le aree del menu principale.

Per ulteriori informazioni, consulta [Concedere a un utente pieno accesso amministrativo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### Livello di accesso standard

Collegato anche alla licenza Standard, questo livello di accesso è progettato per gli utenti che:

* Pianificare, creare e tenere traccia di tutti i progetti in un’unica posizione
* Automatizzare i processi di routine
* Gestione delle risorse
* Tracciare e collaborare alle richieste
* Tracciare e riferire in merito alle finanze dei progetti
* Richieste di lavoro in entrata kickoff
* Collaborazione a progetti, attività e problemi

>[!NOTE]
>
>È possibile creare una versione personalizzata del livello di accesso integrato standard e regolare la quantità di accesso consentita per i vari tipi di oggetti Workfront. Per informazioni sulla creazione di un livello di accesso personalizzato, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Dettagli di accesso**

Di seguito sono riportate le impostazioni di accesso più elevate disponibili per gli oggetti nel livello di accesso Standard:

| Tipo di oggetto Workfront | Nessun accesso | Visualizza accesso | Modifica accesso |
|---|---|---|---|
| Progetti |   |   | ✓ |
| Attività |   |   | ✓ |
| Problemi |   |   | ✓ |
| Portfolio |   |   | ✓ |
| Programmi |   |   | ✓ |
| Rapporti (compresi dashboard e rapporti calendario) |   |   | ✓ |
| Filtri, visualizzazioni e raggruppamenti |   |   | ✓ |
| Documenti |   |   | ✓ |
| Utenti |   |   | ✓ |
| Modelli |   |   | ✓ |
| Dati finanziari |   |   | ✓ |
| Gestione risorse |   |   | ✓ |
| Pianificazione scenario |   |   | ✓ (l&#39;impostazione predefinita è No Access.) |
| Bacheche |   |   | ✓ |
| Home |   |   | ✓ |
| Obiettivi |   |   | ✓ |

{style="table-layout:auto"}

### Livello di accesso leggero

Collegato alla licenza Light, questo livello di accesso è progettato per gli utenti che:

* Visualizza tutti gli elementi e gli aggiornamenti associati al lavoro
* Approvare progetti, attività e problemi
* Visualizzare dashboard e rapporti
* Tempo di traccia
* Creare e gestire i problemi
* Effettuare aggiornamenti sul lavoro

Utenti con livello di accesso leggero:

* Impossibile assegnare elementi di lavoro o approvare fogli presenze
* Può accedere a richieste e documenti nel menu principale.
* La possibilità di creare oggetti è limitata: non possono creare progetti, portfolio, programmi o rapporti.

>[!NOTE]
>
>È possibile creare una versione personalizzata del livello di accesso integrato Light e regolare la quantità di accesso consentita per i vari tipi di oggetti Workfront. Per informazioni sulla creazione di un livello di accesso personalizzato, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Dettagli di accesso**

Di seguito sono riportate le impostazioni di accesso più elevate disponibili per gli oggetti con livello di accesso chiaro:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo di oggetto Workfront</th> 
   <th>Nessun accesso</th> 
   <th>Visualizza accesso</th> 
   <th>Modifica accesso</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Progetti</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Attività</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problemi</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td> </td> 
   <td>✓ (l'impostazione predefinita è No Access.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programmi</td> 
   <td> </td> 
   <td>✓ (l'impostazione predefinita è No Access.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Rapporti (compresi dashboard e rapporti calendario)</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Filtri, visualizzazioni e raggruppamenti</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documenti</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Utenti</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
    <tr> 
   <td>Team</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr>
  <tr> 
   <td>Modelli</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dati finanziari</td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gestione risorse</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Pianificazione scenario </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (l'impostazione predefinita è No Access.)</td> 
  </tr> 
  <tr> 
   <td>Bacheche </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
     <tr> 
   <td>Home </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr>   
   <td>Obiettivi </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
 </tbody> 
</table>

### Livello di accesso collaboratore

In allegato alla licenza da collaboratore, questo livello di accesso è progettato per gli utenti che:

* Inviare richieste
* Tracciare le richieste
* Aggiornare e rivedere le richieste.

Utenti con questo livello di accesso integrato:

* Può effettuare richieste e aggiornarle
* Può caricare e approvare documenti
* Può controllare lo stato dei problemi che hanno inviato
* Impossibile assegnare agli elementi di lavoro
* Può accedere alle richieste solo dal menu principale. Per ulteriori informazioni sulle code di richiesta, vedi [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!NOTE]
>
>Puoi creare una versione personalizzata del livello di accesso integrato da collaboratore e regolare la quantità di accesso consentita per i vari tipi di oggetti Workfront. Per informazioni sulla creazione di un livello di accesso personalizzato, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Dettagli di accesso**

Di seguito sono riportate le impostazioni di accesso più elevate disponibili per gli oggetti nel livello di accesso Collaboratore :

| Tipo di oggetto Workfront | Nessun accesso | Visualizza accesso | Modifica accesso |
|---|---|---|---|
| Progetto |   | ✓ (solo nella pagina Dettagli progetto) |   |
| Attività |   | ✓ (solo la pagina Dettagli) |   |
| Problema |   |   | ✓ |
| Portfolio | ✓ |   |   |
| Programmi | ✓ |   |   |
| Rapporti (compresi dashboard e rapporti calendario) |   | ✓ (solo la scheda Dettagli) |   |
| Filtri, visualizzazioni e raggruppamenti |   |   | ✓ |
| Documento |   |   | ✓ |
| Utente |   | ✓ |   |
| Team |   | ✓ |   |
| Modello | ✓ |   |   |
| Dati finanziari | ✓ |   |   |
| Gestione risorse | ✓ |   |   |
| Pianificazione scenario | ✓ |   |   |
| Bacheche |   |   | ✓ (schede semplici) |
| Home |   | ✓ (Aggiornamenti personali) |   |
| Obiettivi |   |   | ✓ |

{style="table-layout:auto"}

### Livello di accesso utente esterno

Questo livello di accesso non è associato a una licenza Workfront a pagamento. Si tratta del livello di accesso più restrittivo, progettato principalmente per collaboratori come consulenti esterni che non accedono a Workfront, ma che devono rivedere, scaricare o visualizzare documenti occasionalmente.

Gli utenti Workfront possono assegnare attività a utenti esterni anche se gli utenti esterni non possono effettuare l’accesso al sistema. Ma noi sconsigliamo questo perché il lavoro resterebbe irrisolto nel sistema.

Utenti con livello di accesso Utente esterno:

* Può visualizzare solo i documenti e i rapporti del calendario condivisi con gli utenti
* Visualizza gli utenti che condividono con loro documenti e rapporti calendario
* Approva i documenti condivisi con loro

Non è possibile modificare questo livello di accesso.

>[!IMPORTANT]
>
>L’utente esterno è disponibile solo se l’opzione &quot;Collabora con persone senza account Workfront utilizzando il loro indirizzo e-mail&quot; è abilitata nell’area Preferenze di sistema in Configurazione. Per ulteriori informazioni, consulta [Configurare le preferenze di sicurezza del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

#### **Dettagli di accesso**

Di seguito sono riportate le impostazioni di accesso più elevate disponibili per gli oggetti nel livello di accesso Utente esterno.

| Tipo di oggetto Workfront | Nessun accesso | Visualizza accesso | Modifica accesso |
|---|---|---|---|
| Progetto | ✓ |   |   |
| Attività | ✓ |   |   |
| Problema | ✓ |   |   |
| Portfolio | ✓ |   |   |
| Programmi | ✓ |   |   |
| Rapporti (compresi dashboard e rapporti calendario) |   | ✓ (solo per i rapporti di calendario; nessuna capacità di condividere rapporti) |   |
| Filtri, visualizzazioni e raggruppamenti | ✓ |   |   |
| Documento |   | ✓ (nessuna possibilità di condividere documenti) |   |
| Utente |   | ✓ |   |
| Team | ✓ |   |   |
| Modello | ✓ |   |   |
| Dati finanziari | ✓ |   |   |
| Gestione risorse | ✓ |   |   |
| Pianificazione scenario | ✓ |   |   |
| Bacheche | ✓ |   |   |
| Home | ✓ |   |   |
| Obiettivi | ✓ |   |   |


## Funzionamento congiunto dei livelli di accesso e delle autorizzazioni

I livelli di accesso definiscono cosa gli utenti possono vedere e fare con i tipi di oggetti e le aree generali del sistema, ad esempio progetti, attività e problemi. Le autorizzazioni definiscono a cosa puoi accedere su oggetti specifici creati da altre persone nel sistema, come un progetto creato per eseguire una campagna di marketing.

Nella tabella seguente viene confrontato l&#39;accesso generale di un utente agli oggetti (definito dal livello di accesso dell&#39;utente) con le autorizzazioni per un oggetto condiviso specifico:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>Livello di accesso </th> 
   <th>Autorizzazioni </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Concesso da un amministratore Workfront nel livello di accesso di un utente</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Concesso da un utente che condivide un oggetto a livello di oggetto</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Ereditato da un oggetto condiviso di ranking superiore 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Le attività che un utente può eseguire con un oggetto sono definite da una combinazione del livello di accesso e delle autorizzazioni assegnate a tale oggetto.

![](assets/security-model-hierachy-copy.png)

### Concedere autorizzazioni tramite la condivisione di oggetti

Gli utenti possono accedere ai singoli oggetti quando altri utenti condividono e concedono determinate autorizzazioni a tali oggetti.

>[!NOTE]
>
>* Se un utente condivide un oggetto con determinate autorizzazioni e dispone di oggetti secondari al suo interno, il destinatario eredita le stesse autorizzazioni per tali oggetti secondari.
>* Se un livello di accesso limita l’eliminazione di determinati oggetti da parte degli utenti, ciò non impedisce loro di eliminare gli oggetti secondari contenuti in tali oggetti.


Un utente può concedere al destinatario una delle seguenti autorizzazioni per il singolo oggetto:

* **Visualizza**: Questo livello di autorizzazione consente al destinatario di condividere l’oggetto in uno dei seguenti modi:

   * A livello di sistema in modo che tutti gli utenti possano visualizzarlo (non disponibile per tutti gli oggetti)
   * Con utenti esterni che non dispongono di una licenza Workfront (non disponibile per tutti gli oggetti)
   * Con indirizzo e-mail (disponibile solo per documenti e calendari)

* **Collaborare**: (non disponibile per tutti gli oggetti)
* **Gestisci**: Quando un utente condivide un oggetto, i diritti del destinatario sull&#39;oggetto sono determinati da una combinazione del livello di accesso del destinatario e delle autorizzazioni per l&#39;oggetto concesse dal condivisore. Il grado di accesso più basso disponibile in quella combinazione determina cosa può fare il destinatario con l’oggetto.

### Scenari di esempio

#### **Scenario 1**

Se il livello di accesso del destinatario non consente la modifica del progetto, l’utente non può modificare o eliminare un progetto anche se l’utente condiviso dispone delle autorizzazioni necessarie per gestirlo.

Oppure, se il livello di accesso del destinatario consente la modifica del progetto, ma a chi condivide vengono concesse autorizzazioni di sola visualizzazione a un progetto, l’utente non può modificare o eliminare il progetto.

#### **Scenario 2**

Quando Olivia condivide un progetto Workfront con Tony, l&#39;accesso di Tony è determinato da una combinazione di due cose:

* Livello di accesso di Tony, assegnato dall&#39;amministratore Workfront
* Le autorizzazioni di Tony per il progetto, specificate da Olivia

Le azioni di Tony sul progetto possono essere ulteriormente limitate al progetto, ma non possono essere illimitate oltre quanto consentito al suo livello di accesso:

* Se il livello di accesso di Tony non gli consente di creare attività, non può aggiungere attività al progetto, anche se Olivia gli ha dato le autorizzazioni per aggiungere attività.
* Se il livello di accesso di Tony gli consente di creare attività, ma Olivia non concede le autorizzazioni per aggiungere attività al progetto, non può aggiungere attività a quel progetto, ma può aggiungere attività ad altri progetti in cui gli sono state concesse le autorizzazioni per farlo.
