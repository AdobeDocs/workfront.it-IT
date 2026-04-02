---
content-type: overview
product-area: projects
navigation-topic: financials
title: Sostituisci tassi di costo utente a livello di progetto
description: In questo articolo viene descritto come sostituire i tassi di costo degli utenti del sistema per un progetto.
author: Lisa
feature: Work Management
source-git-commit: cb21414992587c62c37580f156100f2b5b755e9b
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 5%

---

# Sostituisci i tassi di costo utente a livello di progetto

{{highlighted-preview-article-level}}

Puoi specificare la tariffa per un utente su un progetto specifico. Questa tariffa a livello di progetto sostituisce la tariffa a livello di sistema per questo utente. Per calcolare il costo, Workfront utilizza la tariffa a livello di progetto della mansione, anziché la tariffa a livello di sistema.

In questo articolo viene descritto come sostituire i tassi di costo degli utenti del sistema per un progetto.

Per ulteriori informazioni sul calcolo dei costi del progetto, vedere [Panoramica sulla gerarchia dei ricavi e dei costi](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) e [Tracciare i costi](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td>Flusso di lavoro Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a progetti e dati finanziari</p>
       <p><p>È inoltre necessario disporre di uno dei seguenti elementi:</p> 
        <ul> 
          <li> <p>Livello di accesso Amministratore di sistema. </li> 
          <li> <p>Impostazione di <b>Utenti</b> nel livello di accesso configurato per l'accesso di <b>Modifica</b>, con <b>Crea</b> e almeno una delle due opzioni di <b>Amministratore utenti</b> abilitate in <b>Ottimizza le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se <b>User Admin (Group Users)</b> è abilitato, è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td>Gestisci le autorizzazioni per il progetto che includono Modifica dati finanziari </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

L&#39;utente deve avere il campo **Sostituzione tariffa consentita** abilitato nel proprio profilo utente. Se il campo Sostituzione costi non è abilitato per un utente, le sostituzioni dei costi non sono consentite per tale utente in alcun progetto e il sistema utilizza la tariffa nel profilo utente per calcolare i costi.

Per ulteriori informazioni, vedere [Modificare il profilo di un utente](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Sostituisci i tassi di costo utente a livello di progetto

1. Passare al progetto per il quale si desidera sostituire i tassi di costo.
1. Fai clic su **Tariffe** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro**.
1. Fare clic sulla scheda **Costo** se non è già selezionata.
1. Fare clic su **Aggiungi tariffa** > **Nuova tariffa utente**.

   Viene visualizzata la casella Nuova tariffa utente (New User Cost Rate).

1. Nel campo **Utente**, selezionare l&#39;utente per il quale si desidera modificare la tariffa.
1. Selezionare **Valuta** per la sostituzione del tasso di costo.
1. Nel campo **Tariffa di costo** immettere la prima sostituzione della tariffa di costo.
1. (Facoltativo) Fai clic su **Aggiungi tariffa effettiva data** per aggiungere altre sostituzioni della tariffa.

   >[!NOTE]
   >
   >Se si immette una sostituzione di tariffa singola, questa viene applicata per l&#39;intera durata del progetto.
   >Se desideri che le tariffe siano diverse nel tempo, puoi aggiungere più sostituzioni valide per data.

1. (Condizionale) Se si stanno aggiungendo più sostituzioni del tasso di costo, specificare le seguenti informazioni per ogni riga:

   * **Tariffa di costo**: il valore della tariffa di costo durante il periodo di tempo specificato.
   * **Data inizio**: la data di inizio della sostituzione della tariffa di costo.
   * **Data di fine**: la data in cui termina la sostituzione della tariffa di costo.

   ![La casella Nuova tariffa utente visualizza le date effettive](assets/new-user-cost-rate-box.png)

   Workfront applica il tasso di ruolo di sostituzione alle ore che si verificano durante questi intervalli di tempo durante il calcolo del costo sul progetto.

   Non devono esserci intervalli tra gli intervalli di tempo di due tassi di sostituzione. La **Data inizio** di una tariffa di sostituzione deve essere il giorno immediatamente successivo alla **Data fine** della data di sostituzione precedente.

   Non è necessario specificare una data di inizio per il primo tasso di sostituzione né una data di fine per l&#39;ultimo tasso di sostituzione.

   È consigliabile utilizzare la tariffa predefinita per la prima tariffa di sostituzione.

   Workfront presuppone che il primo tasso di sostituzione venga applicato a tutte le ore con una data precedente alla data di fine della prima sostituzione e che l’ultimo tasso di sostituzione venga applicato a tutte le ore con una data successiva alla data di inizio dell’ultima sostituzione.

   Se viene registrata un’ora prima della data di inizio pianificata del progetto, viene utilizzata la prima tariffa di costo.

   Se viene registrata un’ora dopo la data di completamento pianificata del progetto, viene utilizzata l’ultima tariffa di costo.

1. Fai clic su **Salva**.


