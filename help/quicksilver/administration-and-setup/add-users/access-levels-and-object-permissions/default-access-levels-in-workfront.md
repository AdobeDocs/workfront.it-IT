---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: accesso,modello,funnel,diagramma,livelli,autorizzazioni
navigation-topic: access-levels
title: Livelli di accesso incorporati
description: Ciascuno dei sei livelli di accesso predefiniti è progettato per un particolare tipo di utente, inclusi amministratore di sistema, planner, lavoratore, revisore, richiedente e utente esterno. Questi livelli di accesso consentono di controllare quali utenti possono modificare e visualizzare nel sistema. Se è necessario un livello di accesso personalizzato, è possibile copiare un livello di accesso predefinito e modificarlo in base alla quantità di accesso che si desidera consentire per i vari tipi di oggetti di Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '1715'
ht-degree: 6%

---

# Livelli di accesso incorporati

<!--Audited: 01/2024-->

>[!NOTE]
>
>Questo articolo descrive gli attuali livelli di accesso incorporati in Adobe Workfront. Per informazioni sui nuovi livelli di accesso incorporati, vedere [Panoramica sui nuovi livelli di accesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).


Ognuno dei sei livelli di accesso incorporati è progettato per un particolare tipo di utente. Questi livelli di accesso consentono di controllare quali utenti possono modificare e visualizzare nel sistema.

Ciascuno dei sei livelli di accesso incorporati è progettato per i seguenti tipi di utenti:

* Amministratore di Sistema
* Pianificatore
* Collaboratore
* Revisore
* Richiedente
* Utente esterno

A seconda del livello di accesso, sono disponibili fino a 3 impostazioni per la maggior parte dei tipi di oggetto Workfront:

<table style="table-layout:auto">
    <tr>
        <td>Modifica</td>
        <td>Gli utenti possono creare, modificare, eliminare e condividere l’oggetto Workfront</td>
    </tr>
    <tr>
        <td>Visualizza</td>
        <td>Gli utenti possono rivedere e condividere l’oggetto Workfront</td>
    </tr>
    <tr>
        <td>Nessun accesso</td>
        <td>Gli utenti non possono accedere all’oggetto Workfront</td>
    </tr>
</table>

Se è necessario un livello di accesso Planner, Worker, Richiedente o Revisore personalizzato, è possibile copiare il livello di accesso incorporato e determinare la quantità di accesso che si desidera consentire per i vari tipi di oggetto Workfront.

>[!TIP]
>
>Non è possibile modificare i livelli di accesso Amministratore di sistema o Utente esterno.

Per informazioni sulla creazione di un livello di accesso personalizzato o sulla modifica di uno dei livelli di accesso incorporati, vedere [Creare e modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>È consigliabile lasciare invariati i livelli di accesso incorporati in modo da potervi fare riferimento dopo aver configurato gli utenti.

Per informazioni generali su questi livelli di accesso, vedere [Panoramica sui livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Livello di accesso Amministratore di sistema

Collegato alla licenza Pianificazione, il livello di accesso integrato Amministratore di sistema è progettato per un utente responsabile dell&#39;amministrazione del sistema Adobe Workfront. Impossibile modificare questo livello di accesso predefinito.

Gli utenti con il livello di accesso Amministratore di sistema possono eseguire tutte le operazioni in Workfront. Possono visualizzare e modificare tutti gli oggetti e le informazioni di Workfront immesse in Workfront da tutti gli altri utenti.

Inoltre, hanno accesso completo all&#39;area Setup (Configurazione), in cui è possibile modificare qualsiasi impostazione a livello di sistema. Possono inoltre accedere a tutte le aree dell&#39;icona del menu principale ![Main menu icon](assets/main-menu-icon.png) o del menu principale ![Main menu icon](assets/main-menu-icon.png), se disponibile.

Per ulteriori informazioni, vedere [Concedere a un utente l&#39;accesso amministrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Livello di accesso al planner

In aggiunta alla licenza Pianificazione, il livello di accesso Pianificazione è progettato per:

* Manager di gruppi, team, progetti e risorse
* Tutti gli utenti responsabili della pianificazione, creazione e gestione di attività, progetti, portfolio e programmi
* Chiunque sia responsabile dell&#39;assegnazione del lavoro (attività e problemi) ad altri utenti
* Utenti che creano rapporti e che approvano schede orario, elementi di lavoro e documenti
* Utenti che devono accedere a tutte le aree del menu principale ![icona menu principale](assets/main-menu-icon.png) o ![icona menu principale](assets/main-menu-icon.png), se disponibile

È possibile creare una versione personalizzata del livello di accesso integrato di Planner e determinare la quantità di accesso consentita per i vari tipi di oggetto Workfront. Per ulteriori informazioni, vedere [Creare e modificare livelli di accesso personalizzati](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Di seguito sono riportate le impostazioni di accesso più elevate disponibili per gli oggetti nel livello di accesso Planner:

| Tipo di oggetto Workfront | Nessun accesso | Visualizza accesso | Modifica accesso |
|---|---|---|---|
| Progetti |   |   | ✓ |
| Attività |   |   | ✓ |
| Problemi |   |   | ✓ |
| Portfolio |   |   | ✓ |
| Programmi |   |   | ✓ |
| Report, dashboard e calendari |   |   | ✓ |
| Filtri, visualizzazioni e raggruppamenti |   |   | ✓ |
| Documenti |   |   | ✓ |
| Utenti |   |   | ✓ |
| Team |   |   | ✓ |
| Modelli |   |   | ✓ |
| Dati finanziari |   |   | ✓ |
| Gestione risorse |   |   | ✓ |
| Pianificazione scenario |   |   | ✓ (l&#39;impostazione predefinita è Nessun accesso). |
| Workfront Goals |   |   | ✓ (l&#39;impostazione predefinita è Nessun accesso). |

{style="table-layout:auto"}

## Livello di accesso lavoratore

Collegato alla licenza Lavoro, il livello di accesso Worker è progettato per gli utenti che eseguono il lavoro in Workfront. Non pianificano il lavoro, lo completano.

Utenti con questo livello di accesso:

* Sono assegnati ad elementi di lavoro in cui possono contribuire e registrare il tempo
* Può approvare lavoro e documenti, ma non schede orario
* Può accedere e condividere i rapporti
* Può comunicare con altri utenti nel sistema
* Impossibile accedere a tutte le aree del menu principale ![icona menu principale](assets/main-menu-icon.png) o ![icona menu principale](assets/main-menu-icon.png), se disponibile, e la relativa area &quot;Utenti&quot; è denominata Team. Nell’area Team, gli utenti con questo livello di accesso possono visualizzare solo i team a cui appartengono, insieme al lavoro assegnato a tali team.
* Hanno capacità limitate di creare oggetti, non possono creare progetti, portfolio, programmi o report.

È possibile creare una versione personalizzata del livello di accesso integrato di Worker e determinare la quantità di accesso consentita per i vari tipi di oggetto Workfront. Per ulteriori informazioni, vedere [Creare e modificare livelli di accesso personalizzati](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Di seguito sono riportate le impostazioni di accesso più elevate disponibili per gli oggetti nel livello di accesso Worker:

| Tipo di oggetto Workfront | Nessun accesso | Visualizza accesso | Modifica accesso |
|---|---|---|---|
| Progetti |   |   | ✓ (Limitato: gli utenti possono solo condividere il progetto, crearne attività e problemi e modificare i dati nei moduli personalizzati già allegati.) |
| Attività |   |   | ✓ |
| Problemi |   |   | ✓ |
| Portfolio |   | ✓ (l&#39;impostazione predefinita è Nessun accesso). |   |
| Programmi |   | ✓ (l&#39;impostazione predefinita è Nessun accesso). |   |
| Report, dashboard e calendari |   | ✓ |   |
| Filtri, visualizzazioni e raggruppamenti |   |   | ✓ |
| Documenti |   |   | ✓ |
| Utenti |   |   | ✓ |
| Team |   |   | ✓ (accesso limitato) |
| Modelli | ✓ |   |   |
| Dati finanziari |   | ✓ (l&#39;impostazione predefinita è Nessun accesso). L&#39;impostazione Visualizza consente all&#39;utente di visualizzare solo l&#39;area Finanza   in Project Details (Dettagli progetto). |   |
| Gestione risorse |   | ✓ |   |
| Pianificazione scenario |   |   | ✓ (l&#39;impostazione predefinita è Nessun accesso). |
| Workfront Goals |   |   | ✓ (l&#39;impostazione predefinita è Nessun accesso). |

{style="table-layout:auto"}

## Livello di accesso revisore

Collegato alla licenza Revisione, il livello di accesso Revisore è progettato per i dirigenti che richiedono lavoro ad altri utenti e che revisionano e approvano il lavoro. Non si tratta di proprietari di progetti o di membri del team, ma di utenti che devono accedere a Workfront per visualizzare gli elementi di lavoro di cui sono responsabili.

Ad esempio, un soggetto interessato con questo livello di accesso può accedere a Workfront per partecipare a una revisione continua del materiale di marketing, vedere gli aggiornamenti sul lavoro e rivedere documenti, approvazioni, rapporti e calendari.

Utenti con il livello di accesso Revisore:

* Impossibile assegnare elementi di lavoro o approvare schede orario
* Può accedere alle aree Richieste e Documenti nel menu principale ![icona menu principale](assets/main-menu-icon.png) o ![icona menu principale](assets/main-menu-icon.png), se disponibile
* Hanno capacità limitate di creare oggetti, non possono creare progetti, portfolio, programmi o report.

È possibile creare una versione personalizzata del livello di accesso predefinito del revisore e determinare la quantità di accesso consentita per i vari tipi di oggetti di Workfront. Per ulteriori informazioni, vedere [Creare e modificare livelli di accesso personalizzati](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Più limitate per progetti e attività rispetto al livello di accesso Lavoratore, le seguenti sono le impostazioni di accesso più elevate disponibili per gli oggetti nel livello di accesso Revisore:

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
   <td>✓ (l'impostazione predefinita è Nessun accesso).</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programmi</td> 
   <td> </td> 
   <td>✓ (l'impostazione predefinita è Nessun accesso).</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Report, dashboard, calendari</td> 
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
   <td> </td> 
   <td> <p>✓ (l'impostazione predefinita è Nessun accesso). L'impostazione Visualizza consente all'utente di visualizzare solo l'area Finanza   in Project Details (Dettagli progetto).</p> </td> 
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
   <td>✓ (l'impostazione predefinita è Nessun accesso).</td> 
  </tr> 
  <tr> 
   <td>Workfront Goals </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (l'impostazione predefinita è Nessun accesso).</td> 
  </tr> 
 </tbody> 
</table>

## Livello di accesso richiedente

In allegato alla licenza Request, il livello di accesso Requestor è progettato per gli utenti che effettuano e ricevono semplici richieste di lavoro in Workfront. Per impostazione predefinita, sono limitati all’area Richieste.

Ad esempio, un utente può segnalare i problemi alla coda di richieste dell’helpdesk della tua organizzazione.

Utenti con questo livello di accesso:

* Può effettuare richieste e aggiornarle
* Può caricare e approvare i documenti
* Può rivedere lo stato dei problemi che ha inviato
* Impossibile assegnare ad elementi di lavoro
* È possibile accedere alle richieste solo dall&#39;area Richieste nel menu principale ![icona del menu principale](assets/main-menu-icon.png) o dall&#39;icona del menu principale ![icona del menu principale](assets/main-menu-icon.png), se disponibile. Per ulteriori informazioni sulle code di richieste, vedere [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

È possibile creare una versione personalizzata del livello di accesso predefinito del richiedente e determinare la quantità di accesso consentita per i vari tipi di oggetti di Workfront. Per ulteriori informazioni, vedere [Creare e modificare livelli di accesso personalizzati](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Di seguito sono riportate le impostazioni di accesso più elevate disponibili per gli oggetti nel livello di accesso Richiedente:

| Tipo di oggetto Workfront | Nessun accesso | Visualizza accesso | Modifica accesso |
|---|---|---|---|
| Progetto |   | ✓ (solo la pagina Dettagli progetto) |   |
| Attività |   | ✓(solo la pagina Dettagli attività) |   |
| Problema |   |   | ✓ |
| Portfolio | ✓ |   |   |
| Programmi | ✓ |   |   |
| Report, dashboard e calendari |   | ✓ |   |
| Filtri, viste e raggruppamenti |   |   | ✓ |
| Documenti |   |   | ✓ |
| Utente |   | ✓ |   |
| Team |   | ✓ |   |
| Modelli | ✓ |   |   |
| Dati finanziari | ✓ |   |   |
| Gestione risorse | ✓ |   |   |
| Pianificazione scenario | ✓ |   |   |
| Workfront Goals |   |   | ✓ (l&#39;impostazione predefinita è Nessun accesso). |

{style="table-layout:auto"}

## Livello di accesso utente esterno

Il livello di accesso Utente esterno non è collegato a una licenza Workfront a pagamento. Si tratta del livello di accesso più restrittivo, progettato principalmente per i collaboratori, ad esempio consulenti esterni che non accedono a Workfront, ma che devono rivedere, scaricare o visualizzare documenti di tanto in tanto.

Gli utenti di Workfront possono assegnare attività a utenti esterni anche se questi non possono accedere al sistema. Tuttavia, si sconsiglia di assegnare attività e problemi a utenti esterni, in quanto tale lavoro rimarrebbe irrisolto nel sistema.

Utenti con il livello di accesso Utente esterno:

* È possibile visualizzare solo i documenti e i report del calendario condivisi con gli altri
* Può visualizzare gli utenti che condividono documenti e report calendario con loro
* Può approvare i documenti condivisi con loro

Non puoi modificare questo livello di accesso.

>[!IMPORTANT]
>
>L’utente esterno è disponibile solo se l’opzione &quot;Collaborazione con persone senza account Workfront utilizzando il loro indirizzo e-mail&quot; è abilitata nell’area Preferenze di sistema in Configurazione. Per ulteriori informazioni, vedere [Configurare le preferenze di sicurezza del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

Sebbene queste impostazioni non siano visibili nell&#39;area Livelli di accesso per il livello di accesso Utente esterno, un utente con questo livello di accesso dispone del livello di accesso più elevato ai tipi di oggetto Workfront riportato di seguito.

| Tipo di oggetto Workfront | Nessun accesso | Visualizza accesso | Modifica accesso |
|---|---|---|---|
| Progetto | ✓ |   |   |
| Attività | ✓ | |   |
| Problema | ✓ |   |   |
| Portfolio | ✓ |   |   |
| Programmi | ✓ |   |   |
| Report, dashboard e calendari |   | ✓ (solo per i report calendario; impossibile condividere i report) |   |
| Filtri, visualizzazioni e raggruppamenti | ✓ |   |   |
| Documenti |   | ✓ (senza possibilità di condividere i documenti) |   |
| Utenti |   | ✓ |   |
| Team |   | ✓ |   |
| Modelli | ✓ |   |   |
| Dati finanziari | ✓ |   |   |
| Gestione risorse | ✓ |   |   |
| Pianificazione scenario | ✓ |   |   |
| Workfront Goals | ✓ |   |   |
