---
title: Panoramica dei livelli di accesso
user-type: administrator
content-type: reference
product-area: system-administration
keywords: accesso,livello,sistema,amministratore,standard,light,collaboratore
navigation-topic: access-levels
description: Per accedere e lavorare in Workfront, ogni utente deve disporre di un livello di accesso. Il livello di accesso ti consente di controllare cosa un utente può visualizzare e fare con determinati oggetti e aree di Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d297d8a4-5a4e-418f-983a-19545aeb0668
source-git-commit: 21c396fc5b52463477d6fedfae8dcd27de989817
workflow-type: tm+mt
source-wordcount: '1765'
ht-degree: 96%

---

# Panoramica dei livelli di accesso

>[!NOTE]
>
> Le informazioni contenute in questo articolo si riferiscono ai livelli di accesso lagacy. Per informazioni sui livelli di accesso precedenti, consulta [Panoramica dei livelli di accesso](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

In qualità di amministratore di Adobe Workfront, puoi assegnare un livello di accesso a un utente per 2 scopi:

* Per accedere e lavorare in Workfront, ogni utente deve disporre di un livello di accesso.
* Il livello di accesso ti consente di controllare cosa un utente può visualizzare e fare con determinati oggetti e aree di Workfront.

## Nuovi livelli di accesso incorporati in Adobe Workfront {#built-in-access}

Workfront dispone di 5 nuovi livelli di accesso incorporati:

* Amministratore di sistema
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
        <td>Visualizzazione</td>
        <td>Gli utenti possono rivedere e condividere l’oggetto Workfront</td>
    </tr>
    <tr>
        <td>Nessun accesso</td>
        <td>Gli utenti non possono accedere all’oggetto Workfront</td>
    </tr>
</table>

Se è necessario un livello di accesso personalizzato, puoi copiare un livello di accesso predefinito e regolare il grado di accesso che desideri consentire per i vari tipi di oggetti Workfront. Per informazioni sulla creazione di un livello di accesso personalizzato, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>È consigliabile lasciare invariati i livelli di accesso predefiniti in modo da potervi fare riferimento dopo aver configurato gli utenti.

### Livello di accesso Amministratore di sistema

Associato alla licenza standard, questo livello di accesso predefinito è progettato per un utente che è responsabile dell’amministrazione del sistema di Adobe Workfront. Questo modello di accesso incorporato non può essere modificato.

Gli utenti con il livello di accesso Amministratore di sistema possono eseguire tutte le operazioni all’interno di Workfront. Possono visualizzare e modificare tutti gli oggetti e le informazioni di Workfront immesse in Workfront da tutti gli altri utenti.

Inoltre, dispongono dell’accesso all’area Configurazione completa, in cui possono modificare qualsiasi impostazione a livello di sistema e accedere a tutte le aree nel Menu principale.

Per ulteriori informazioni, consulta [Concedere a un utente l’accesso amministrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### Livello di accesso standard

Alla licenza Standard è associato anche questo livello di accesso, progettato per gli utenti che:

* Pianificano, creano e tengono traccia di tutti i progetti in un’unica posizione
* Automatizzano i processi di routine
* Gestiscono le risorse
* Tengono traccia e collaborano sulle richieste
* Tengono traccia e creano rapporti sui dati finanziari del progetto
* Avviano richieste di lavoro in entrata
* Collaborano su progetti, attività e problemi

>[!NOTE]
>
>Puoi creare una versione personalizzata del livello di accesso predefinito standard e regolare il grado di accesso consentito per i vari tipi di oggetti di Workfront. Per informazioni sulla creazione di un livello di accesso personalizzato, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Dettagli di accesso**

Di seguito sono riportate le impostazioni di accesso più elevate disponibili per gli oggetti nel livello di accesso standard:

| Tipi di oggetto Workfront | Nessun accesso | Accesso in visualizzazione | Accesso per la modifica |
|---|---|---|---|
| Progetti |   |   | ✓ |
| Tasks |   |   | ✓ |
| Problemi |   |   | ✓ |
| Portfolio |   |   | ✓ |
| Programmi |   |   | ✓ |
| Rapporti (inclusi dashboard e rapporti del calendario) |   |   | ✓ |
| Filtri, viste e raggruppamenti |   |   | ✓ |
| Documenti |   |   | ✓ |
| Utenti |   |   | ✓ |
| Modelli |   |   | ✓ |
| Dati finanziari |   |   | ✓ |
| Gestione delle risorse |   |   | ✓ |
| Pianificazione scenari |   |   | ✓ (L’impostazione predefinita è Nessun accesso). |
| Obiettivi |   |   | ✓ |

{style="table-layout:auto"}

### Livello di accesso Light

Associato alla licenza Light, questo livello di accesso è progettato per gli utenti che:

* Visualizzano tutti gli elementi e gli aggiornamenti associati al lavoro
* Approvano progetti, attività e problemi
* Visualizzano dashboard e rapporti
* Tracciare il tempo dedicato a progetti, attività e problemi e approvare le schede orario
* Creare e gestire i problemi

Utenti con il livello di accesso Light:

* Possono essere assegnati a elementi di lavoro ma non possono completarli.
* Possono accedere a richieste e documenti nel menu principale.
* Hanno capacità limitate di creare oggetti, non possono creare progetti, portfolio, programmi o rapporti.
* È possibile registrare l’ora a livello di progetto solo quando è abilitato l’accesso di modifica. Non possono creare, modificare, eliminare o condividere progetti.
* È possibile aggiornare i moduli personalizzati solo per problemi e documenti.

>[!NOTE]
>
>Puoi creare una versione personalizzata del livello di accesso predefinito Llight e regolare il grado di accesso consentito per i vari tipi di oggetti di Workfront. Per informazioni sulla creazione di un livello di accesso personalizzato, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Dettagli di accesso**

Di seguito sono riportate le impostazioni di accesso più elevate disponibili per gli oggetti nel livello di accesso Light:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipi di oggetto Workfront</th> 
   <th>Nessun accesso</th> 
   <th>Accesso in visualizzazione</th> 
   <th>Accesso per la modifica</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Progetti</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (per la registrazione del tempo a livello di progetto)</td> 
  </tr> 
  <tr> 
   <td>Attività</td> 
   <td> </td> 
   <td></td> 
   <td>✓ (limitato)</td> 
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
   <td>✓ (L’impostazione predefinita è Nessun accesso).</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programmi</td> 
   <td> </td> 
   <td>✓ (L’impostazione predefinita è Nessun accesso).</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Rapporti (inclusi dashboard e rapporti del calendario)</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Filtri, viste e raggruppamenti</td> 
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
   <td></td> 
   <td> <p>✓ (L’impostazione predefinita è Nessun accesso)</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gestione delle risorse</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Pianificazione scenari </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (L’impostazione predefinita è Nessun accesso).</td> 
  </tr>

<tr>   
   <td>Obiettivi </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (L’impostazione predefinita è Nessun accesso)</td> 
 </tbody> 
</table>

### Livello di accesso collaboratore

Associato alla licenza collaboratore, questo livello di accesso è progettato per gli utenti che:

* Inviano richieste
* Tengono traccia delle richieste
* Aggiornano e rivedono le richieste
* Approvano le richieste

Gli utenti con questo livello di accesso predefinito:

* Possono effettuare richieste e aggiornarle
* Possono caricare e approvare documenti
* Possono approvare progetti, attività e problemi

  >[!NOTE]
  >
  >I collaboratori possono partecipare alle approvazioni, ma non possono accedere alla scheda Approvazioni per visualizzare o gestire i processi di approvazione.

* Possono rivedere lo stato dei problemi che hanno inviato
* È possibile aggiornare i moduli personalizzati solo per problemi e documenti.
* Possono essere assegnati ad elementi di lavoro ma non possono completarli
* Possono accedere alle richieste solo dal menu principale. Per ulteriori informazioni sulle code delle richieste, consulta [Creare una coda delle richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!NOTE]
>
>Puoi creare una versione personalizzata del livello di accesso predefinito Collaboratore e regolare il grado di accesso consentito per i vari tipi di oggetti di Workfront. Per informazioni sulla creazione di un livello di accesso personalizzato, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Dettagli di accesso**

Di seguito sono riportate le impostazioni di accesso più elevate disponibili per gli oggetti nel livello di accesso collaboratore:

| Tipi di oggetto Workfront | Nessun accesso | Accesso in visualizzazione | Accesso per la modifica |
|---|---|---|---|
| Progetto |   | ✓ (limitato) |   |
| Attività |   | ✓(limitato) |   |
| Problema |   |   | ✓ |
| Portfolio |   | ✓ |   |
| Programmi |   | ✓ |   |
| Rapporti (inclusi dashboard e rapporti del calendario) |   | ✓ (solo la scheda Dettagli) |   |
| Filtri, viste e raggruppamenti |   |   | ✓ |
| Documento |   |   | ✓ |
| Utente |   | ✓ |   |
| Team |   | ✓ |   |
| Modelli | ✓ |   |   |
| Dati finanziari | ✓ |   |   |
| Gestione delle risorse | ✓ |   |   |
| Pianificazione scenari | ✓ |   |   |
| Obiettivi |   |   | ✓ (L’impostazione predefinita è Nessun accesso) |

{style="table-layout:auto"}

>[!IMPORTANT]
>
>A partire dalla versione 24.7, per impostazione predefinita, i collaboratori hanno accesso in visualizzazione a programmi e portfolio.
>
> 
>Per impostazione predefinita, i collaboratori che hanno eseguito l’onboarding prima della versione 24.7 continueranno a non avere accesso a programmi e portfolio. Puoi aggiornarne l’accesso per la visualizzazione manualmente, se necessario.

### Livello di accesso utente esterno

Questo livello di accesso non è collegato a una licenza Workfront a pagamento. È il livello di accesso più restrittivo, progettato principalmente per collaboratori come consulenti esterni che non accedono a Workfront, ma che devono rivedere, scaricare o visualizzare documenti occasionalmente.

Gli utenti con il livello di accesso utente esterno:

* Possono visualizzare solo i documenti e i rapporti del calendario condivisi con loro
* Visualizzano gli utenti che condividono con loro documenti e rapporti del calendario
* Approvano i documenti condivisi con loro

Gli utenti esterni non possono essere assegnati ad elementi di lavoro.

Non puoi modificare questo livello di accesso.

>[!IMPORTANT]
>
>L’utente esterno è disponibile solo se l’opzione “Collabora con persone senza un account Workfront utilizzandone indirizzo e-mail” è abilitata nell’area Preferenze di sistema in Configurazione. Per ulteriori informazioni, consulta [Configurare le preferenze di sicurezza del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

#### **Dettagli di accesso**

Di seguito sono riportate le impostazioni di accesso più elevate disponibili per gli oggetti nel livello di accesso utente esterno.

| Tipi di oggetto Workfront | Nessun accesso | Accesso in visualizzazione | Accesso per la modifica |
|---|---|---|---|
| Progetto | ✓ |   |   |
| Attività | ✓ |   |   |
| Problema | ✓ |   |   |
| Portfolio | ✓ |   |   |
| Programmi | ✓ |   |   |
| Rapporti (inclusi dashboard e rapporti del calendario) |   | ✓ (Solo per i rapporti del calendario; nessuna possibilità di condividere i rapporti) |   |
| Filtri, viste e raggruppamenti | ✓ |   |   |
| Documento |   | ✓ (Nessuna possibilità di condividere i documenti) |   |
| Utente |   | ✓ |   |
| Team | ✓ |   |   |
| Modelli | ✓ |   |   |
| Dati finanziari | ✓ |   |   |
| Gestione delle risorse | ✓ |   |   |
| Pianificazione scenari | ✓ |   |   |
| Obiettivi | ✓ |   |   |


## Funzionamento congiunto dei livelli di accesso e delle autorizzazioni

I livelli di accesso definiscono ciò che gli utenti possono visualizzare e fare con i tipi di oggetti e le aree generali del sistema, come progetti, attività e problemi. Le autorizzazioni definiscono a cosa puoi accedere all’interno di oggetti specifici creati da altre persone nel sistema, come un progetto creato per eseguire una campagna di marketing.

Nella tabella seguente viene confrontato l’accesso generale di un utente agli oggetti (definito dal livello di accesso dell’utente) con le autorizzazioni per un oggetto condiviso specifico:

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
   <td>Assegnate da un amministratore Workfront nel livello di accesso di un utente</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Assegnate da un utente che condivide un oggetto a livello di oggetto</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Ereditate da un oggetto condiviso con ranking più alto 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Le attività che un utente può svolgere con un oggetto sono definite da una combinazione del livello di accesso e delle autorizzazioni assegnate.

![Gerarchia modelli di sicurezza](assets/security-model-hierachy-copy.png)

### Assegnare autorizzazioni tramite la condivisione di oggetti

Gli utenti possono accedere a singoli oggetti quando altri utenti condividono e assegnano determinate autorizzazioni su tali oggetti.

>[!NOTE]
>
>* Se un utente condivide un oggetto con determinate autorizzazioni e tale oggetto ha oggetti secondari al suo interno, il destinatario eredita le stesse autorizzazioni per tali oggetti secondari.
>* Se un livello di accesso impedisce agli utenti di eliminare determinati oggetti, ciò non impedisce loro di eliminare gli oggetti secondari contenuti in tali oggetti.

Un utente può assegnare al destinatario le seguenti autorizzazioni per il singolo oggetto:

* **Visualizzazione**: questo livello di autorizzazione consente al destinatario di condividere l’oggetto in uno dei modi seguenti:

   * A livello di sistema, in modo che tutti gli utenti possano visualizzarlo (non disponibile per tutti gli oggetti)
   * Con utenti esterni che non dispongono di una licenza Workfront (non disponibile per tutti gli oggetti)
   * Con un indirizzo e-mail (disponibile solo per documenti e calendari)

* **Contributi**: (non disponibile per tutti gli oggetti)
* **Gestione**: quando qualcuno condivide un oggetto, i diritti del destinatario sull’oggetto sono determinati da una combinazione del livello di accesso del destinatario e delle autorizzazioni per l’oggetto assegnate dalla persona che condivide. Il livello di accesso più basso disponibile in tale combinazione è quello che determina ciò che il destinatario può fare con l’oggetto.

### Scenari di esempio

#### **Scenario 1**

Se il livello di accesso del destinatario non consente la modifica del progetto, l’utente non può modificare o eliminare un progetto anche se la persona che condivide ha assegnato le autorizzazioni per gestirlo.

In alternativa, se il livello di accesso del destinatario consente la modifica del progetto, ma la persona che condivide ha assegnato autorizzazioni di sola visualizzazione a un progetto, l’utente non può modificare o eliminare il progetto.

#### **Scenario 2**

Quando Olivia condivide un progetto Workfront con Tony, l’accesso di quest’ultimo è determinato da una combinazione di due fattori:

* Livello di accesso di Tony assegnato dall’amministratore Workfront
* Autorizzazioni di Tony per il progetto, specificate da Olivia

Le azioni di Tony sul progetto possono essere ulteriormente limitate all’interno del progetto stesso, ma non possono essere estese oltre quanto consentito dal suo livello di accesso:

* Se il livello di accesso di Tony non gli consente di creare attività, non può aggiungere attività al progetto, anche se Olivia gli ha concesso le autorizzazioni per aggiungervi attività.
* Se il livello di accesso di Tony non gli consente di creare attività, ma Olivia non assegna le autorizzazioni per aggiungere attività al progetto, Tony non può aggiungere attività a tale progetto, ma può aggiungere attività ad altri progetti per i quali dispone delle autorizzazioni necessarie.
