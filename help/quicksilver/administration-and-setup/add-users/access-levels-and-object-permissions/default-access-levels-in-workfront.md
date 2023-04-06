---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: accesso, modello, funnel, diagramma, livelli, autorizzazioni
navigation-topic: access-levels
title: Livelli di accesso incorporati in Adobe Workfront
description: Ciascuno dei sei livelli di accesso incorporati è progettato per un particolare tipo di utente, inclusi Amministratore di sistema, Planner, Worker, Reviewer, Requestor e Utente esterno. Questi livelli di accesso consentono di controllare cosa gli utenti possono modificare e visualizzare nel sistema. Se hai bisogno di un livello di accesso personalizzato, puoi copiare il livello di accesso integrato e determinare la quantità di accesso che desideri consentire per i vari tipi di oggetti Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 1bd454246419e199e5cfd0d8d1d73cd30c0b13b1
workflow-type: tm+mt
source-wordcount: '1515'
ht-degree: 5%

---

# Livelli di accesso legacy incorporati in Adobe Workfront

Ciascuno dei sei livelli di accesso legacy incorporati è progettato per un particolare tipo di utente:

* Amministratore di Sistema
* Pianificatore
* Collaboratore
* Revisore
* Richiedente
* Utente esterno

A seconda del livello di accesso legacy, sono disponibili fino a 3 impostazioni per la maggior parte dei tipi di oggetto Workfront:

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

Se è necessario un livello di accesso personalizzato per Planner, Worker, Requester o Reviewer, è possibile copiare il livello di accesso legacy integrato e determinare la quantità di accesso che si desidera consentire per i vari tipi di oggetti Workfront. Per informazioni sulla creazione di un livello di accesso personalizzato o sulla modifica di uno dei livelli di accesso legacy incorporati, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>È vivamente consigliato lasciare invariati i livelli di accesso legacy incorporati, in modo da potervi fare riferimento dopo la configurazione degli utenti.

Per informazioni generali su questi livelli di accesso, vedi [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Livello di accesso legacy amministratore di sistema

In allegato alla licenza Plan, questo livello di accesso legacy integrato è progettato per un utente che si occupa dell’amministrazione del sistema Adobe Workfront. Non è possibile modificare questo livello di accesso integrato.

Gli utenti con il livello di accesso legacy amministratore di sistema possono eseguire tutte le operazioni all’interno di Workfront. Possono visualizzare e modificare tutti gli oggetti e le informazioni Workfront immessi in Workfront da tutti gli altri utenti.

Inoltre, possono accedere all&#39;area di configurazione completa, in cui possono modificare qualsiasi impostazione a livello di sistema. E possono accedere a tutte le aree del menu principale ![](assets/main-menu-icon.png).

Per ulteriori informazioni, consulta [Concedere a un utente pieno accesso amministrativo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Livello di accesso legacy del planner

Collegato anche alla licenza Plan, questo livello di accesso è progettato per:

* Manager di gruppi, team, progetti e risorse
* Chiunque sia responsabile della pianificazione, creazione e gestione di attività, progetti, portfolio e programmi
* Chiunque sia responsabile dell&#39;assegnazione del lavoro (attività e problemi) ad altri utenti
* Utenti che creano rapporti e approvano fogli ore, elementi di lavoro e documenti
* Utenti che necessitano di accesso a tutte le aree del menu principale ![](assets/main-menu-icon.png)

È possibile creare una versione personalizzata del livello di accesso legacy integrato di Planner e determinare la quantità di accesso consentita per i vari tipi di oggetti Workfront. Per ulteriori informazioni, consulta [Livelli di accesso incorporati in Adobe Workfront](#Customiz) in questo articolo.

Di seguito sono riportate le impostazioni di accesso più elevate disponibili per gli oggetti nel livello di accesso legacy di Planner:

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
| Workfront Goals |   |   | ✓ (l&#39;impostazione predefinita è No Access.) |

{style="table-layout:auto"}

## Livello di accesso legacy di lavoro

In allegato alla licenza di lavoro, questo livello di accesso è progettato per gli utenti che eseguono il lavoro in Workfront. Non pianificano il lavoro; lo completano.

Utenti con questo livello di accesso:

* Sono assegnati a elementi di lavoro in cui possono contribuire e registrare il tempo
* Può approvare lavoro e documenti, ma non fogli presenze
* Accesso e condivisione dei rapporti
* Può comunicare con altri utenti del sistema
* Accesso a tutte le aree del menu principale ![](assets/main-menu-icon.png), ma la loro area &quot;Utenti&quot; si chiama Team. Nell’area Team, gli utenti con questo livello di accesso possono visualizzare solo i team a cui appartengono, insieme al lavoro assegnato a tali team.
* La possibilità di creare oggetti è limitata: non possono creare progetti, portfolio, programmi o rapporti.

È possibile creare una versione personalizzata del livello di accesso legacy integrato di Worker e determinare la quantità di accesso consentita per i vari tipi di oggetti Workfront. Per ulteriori informazioni, consulta [Livelli di accesso incorporati in Adobe Workfront](#Customiz) in questo articolo.

Di seguito sono riportate le impostazioni di accesso più elevate disponibili per gli oggetti nel livello di accesso Worker:

| Tipo di oggetto Workfront | Nessun accesso | Visualizza accesso | Modifica accesso |
|---|---|---|---|
| Progetti |   |   | ✓ (limitato: gli utenti possono condividere il progetto, creare attività e problemi al suo interno e modificare i dati in moduli personalizzati già associati.) |
| Attività |   |   | ✓ |
| Problemi |   |   | ✓ |
| Portfolio |   | ✓ (l&#39;impostazione predefinita è No Access.) |   |
| Programmi |   | ✓ (l&#39;impostazione predefinita è No Access.) |   |
| Rapporti (compresi dashboard e rapporti calendario) |   | ✓ |   |
| Filtri, visualizzazioni e raggruppamenti |   |   | ✓ |
| Documenti |   |   | ✓ |
| Utenti |   |   | ✓ |
| Modelli | ✓ |   |   |
| Dati finanziari |   | ✓ (l&#39;impostazione predefinita è No Access. L&#39;impostazione Visualizza consente all&#39;utente di visualizzare solo l&#39;area Finanza in Dettagli progetto.) |   |
| Gestione risorse |   | ✓ |   |
| Pianificazione scenario |   |   | ✓ (l&#39;impostazione predefinita è No Access.) |
| Workfront Goals |   |   | ✓ (l&#39;impostazione predefinita è No Access.) |

{style="table-layout:auto"}

## Livello di accesso legacy del revisore

In allegato alla licenza di revisione, questo livello di accesso è progettato per i dirigenti che richiedono il lavoro da altri utenti e che rivedono e approvano il lavoro. Questi non sono proprietari di progetti o membri del team, ma hanno bisogno dell&#39;accesso a Workfront per vedere gli elementi di lavoro che controllano.

Ad esempio, un stakeholder con questo livello di accesso potrebbe accedere a Workfront per partecipare a una revisione continua dei materiali di marketing, vedere gli aggiornamenti sul lavoro e rivedere documenti, approvazioni, rapporti e calendari.

Utenti con livello di accesso del revisore:

* Non è possibile assegnare elementi di lavoro o approvare fogli di tempo
* Può accedere a richieste e documenti nel menu principale ![](assets/main-menu-icon.png).
* La possibilità di creare oggetti è limitata: non possono creare progetti, portfolio, programmi o rapporti.

È possibile creare una versione personalizzata del livello di accesso legacy predefinito per il revisore e determinare la quantità di accesso consentita per i vari tipi di oggetti Workfront. Per ulteriori informazioni, consulta [Livelli di accesso incorporati in Adobe Workfront](#Customiz) in questo articolo.

Più limitato per progetti e attività rispetto al livello di accesso di Worker, sono disponibili le impostazioni di accesso più elevate disponibili per gli oggetti nel livello di accesso di Reviewer:

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
   <td>✓</td> 
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
   <td>Modelli</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dati finanziari</td> 
   <td> </td> 
   <td> <p>✓ (l'impostazione predefinita è No Access. L'impostazione Visualizza consente all'utente di visualizzare solo l'area Finanza in Dettagli progetto.)</p> </td> 
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
   <td>Workfront Goals </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (l'impostazione predefinita è No Access.)</td> 
  </tr> 
 </tbody> 
</table>

## Livello di accesso legacy del richiedente

Collegato alla licenza di richiesta, questo livello di accesso è progettato per gli utenti che effettuano e ricevono semplici richieste di lavoro in Workfront. Per impostazione predefinita, sono limitati all’area Richieste.

Ad esempio, un utente può segnalare i problemi nella coda delle richieste dell’help desk dell’organizzazione.

Utenti con questo livello di accesso:

* Può effettuare richieste e aggiornarle
* Può caricare e approvare documenti
* Può controllare lo stato dei problemi che hanno inviato
* Impossibile assegnare agli elementi di lavoro
* Può accedere alle richieste solo dal menu principale ![](assets/main-menu-icon.png). Per ulteriori informazioni sulle code di richiesta, vedi [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

È possibile creare una versione personalizzata del livello di accesso legacy integrato del Requester e determinare la quantità di accesso consentita per i vari tipi di oggetto Workfront. Per ulteriori informazioni, consulta [Livelli di accesso incorporati in Adobe Workfront](#Customiz) in questo articolo.

Di seguito sono riportate le impostazioni di accesso più elevate disponibili per gli oggetti nel livello di accesso Richiedente:

| Tipo di oggetto Workfront | Nessun accesso | Visualizza accesso | Modifica accesso |
|---|---|---|---|
| Progetto |   | ✓ (solo nella pagina Dettagli progetto) |   |
| Attività |   | ✓ (solo la pagina Dettagli) |   |
| Problema |   |   | ✓ |
| Portfolio | ✓ |   |   |
| Programmi | ✓ |   |   |
| Rapporti (compresi dashboard e rapporti calendario) |   | ✓ (solo la pagina Dettagli) |   |
| Filtri, visualizzazioni e raggruppamenti |   |   | ✓ |
| Documento |   |   | ✓ |
| Utente |   | ✓ |   |
| Modello | ✓ |   |   |
| Dati finanziari | ✓ |   |   |
| Gestione risorse | ✓ |   |   |
| Pianificazione scenario | ✓ |   |   |
| Workfront Goals |   |   | ✓ (l&#39;impostazione predefinita è No Access.) |

{style="table-layout:auto"}

## Livello di accesso legacy per gli utenti esterni

Questo livello di accesso non è associato a una licenza Workfront a pagamento. Si tratta del livello di accesso più restrittivo, progettato principalmente per collaboratori come consulenti esterni che non accedono a Workfront, ma che devono rivedere, scaricare o visualizzare documenti occasionalmente.

Gli utenti Workfront possono assegnare attività a utenti esterni anche se gli utenti esterni non possono effettuare l’accesso al sistema. Ma noi sconsigliamo questo perché il lavoro resterebbe irrisolto nel sistema.

Utenti con livello di accesso Utente esterno:

* Può visualizzare solo i documenti e i rapporti del calendario condivisi con gli utenti
* Visualizza gli utenti che condividono documenti e rapporti sul calendario con loro
* Approva i documenti condivisi con loro

Non è possibile modificare questo livello di accesso.

>[!IMPORTANT]
>
>L’utente esterno è disponibile solo se l’opzione &quot;Collabora con persone senza account Workfront utilizzando il loro indirizzo e-mail&quot; è abilitata nell’area Preferenze di sistema in Configurazione. Per ulteriori informazioni, consulta [Configurare le preferenze di sicurezza del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

Di seguito sono riportate le impostazioni di accesso più elevate disponibili per gli oggetti nel livello di accesso Utente esterno.

| Tipo di oggetto Workfront | Nessun accesso | Visualizza accesso | Modifica accesso |
|---|---|---|---|
| Progetto | ✓ |   |   |
| Attività | ✓ | ✓ |   |
| Problema | ✓ |   |   |
| Portfolio | ✓ |   |   |
| Programmi | ✓ |   |   |
| Rapporti (compresi dashboard e rapporti calendario) |   | ✓ (solo per i rapporti di calendario; nessuna capacità di condividere rapporti) |   |
| Filtri, visualizzazioni e raggruppamenti | ✓ |   |   |
| Documento |   | ✓ (senza la possibilità di condividere documenti) |   |
| Utente |   | ✓ |   |
| Modello | ✓ |   |   |
| Dati finanziari | ✓ |   |   |
| Gestione risorse | ✓ |   |   |
| Pianificazione scenario | ✓ |   |   |
| Workfront Goals | ✓ |   |   |
