---
title: Accesso configurabile alle funzionalità per ogni tipo di oggetto
description: Questo articolo spiega cosa puoi consentire come amministratore Adobe Workfront per ogni tipo di oggetto, in ogni livello di accesso. Inoltre, spiega qual è la configurazione predefinita per ogni tipo di livello di accesso.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: 5d924e510ad94098b9f417494f9fc6e8696c90d6
workflow-type: tm+mt
source-wordcount: '3485'
ht-degree: 10%

---

# Accesso configurabile alle funzionalità per ogni tipo di oggetto

Durante la configurazione di un livello di accesso per la tua organizzazione, puoi determinare quali azioni specifiche sono disponibili per il livello di accesso.

In questo articolo vengono illustrate le opzioni che un amministratore Adobe Workfront può selezionare per ogni tipo di oggetto, in ogni livello di accesso. Inoltre, spiega qual è la configurazione predefinita per ogni tipo di livello di accesso.

Ad esempio, se un amministratore di Workfront seleziona &quot;Visualizza&quot; per i progetti in un determinato livello di accesso, gli utenti con tale livello di accesso potranno solo visualizzare i progetti, non modificarli.

Per informazioni su tutte le funzionalità disponibili per un tipo di oggetto in ogni livello di accesso, vedere [Funzionalità disponibili per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Progetti

In ogni livello di accesso, puoi configurare le seguenti opzioni per i progetti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Livello di accesso</th> 
   <th>Opzioni</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planner (tipo di licenza Pianificazione)</td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li><p> <b>Visualizza</b></p> <p>Per ottimizzare questo aspetto, puoi configurare la possibilità di condividere i progetti. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso completo alla modifica dei progetti.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita, sono tutti attivati.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Copia</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Visualizza</p> </li> 
       <li> <p>Condividi</p> </li> 
       <li> <p>Condividi a livello di sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collaboratore </td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li><p> <b>Visualizza</b></p> <p>Per ottimizzare questo aspetto, puoi configurare la possibilità di condividere i progetti. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente un accesso limitato alla modifica dei progetti. Per vedere come l'accesso di modifica è limitato in un livello di accesso Worker rispetto a un livello di accesso Planner (che consente l'accesso di modifica completo ai progetti), vedi la sezione <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref">Progetti</a> nell'articolo <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref">Funzionalità disponibile per ogni tipo di oggetto</a>.</p> <p>Per ottimizzare questo aspetto, puoi configurare la possibilità di condividere i progetti. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Modifica, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisore</td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li> <b>Visualizza</b> (selezione predefinita) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Richiedente</td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li><p> <b>Visualizza</b></p> (selezione predefinita) <p>L’accesso in visualizzazione è limitato perché non è possibile ottimizzarlo per abilitare o disabilitare la condivisione dei progetti.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utente esterno</td> 
   <td> <p>L’accesso ai progetti non è disponibile. Gli utenti esterni possono utilizzare Workfront solo per rivedere e scaricare i documenti e per visualizzare i calendari condivisi con loro.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Attività

In ogni livello di accesso è possibile configurare le seguenti opzioni per le attività:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Livello di accesso</th> 
   <th>Opzioni</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Pianificatore </td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li><p> <b>Visualizza</b></p> <p>Per ottimizzare questo aspetto, puoi configurare la possibilità di condividere le attività. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso alle attività con modifica completa.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita, sono tutti attivati.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
       <li> <p>Condividi a livello di sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collaboratore </td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li><p> <b>Visualizza</b></p> <p>Per ottimizzare questo aspetto, puoi configurare la possibilità di condividere le attività. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso alle attività con modifica completa.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita, sono tutti attivati.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisore</td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li> <b>Visualizza</b> (selezione predefinita) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Richiedente</td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li><p> <b>Visualizza</b></p> (selezione predefinita)<p>L’accesso in visualizzazione è limitato perché non è possibile ottimizzarlo per abilitare o disabilitare la condivisione dei progetti.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utente esterno</td> 
   <td> <p>L'accesso alle attività non è disponibile. Gli utenti esterni possono utilizzare Workfront solo per rivedere e scaricare i documenti e per visualizzare i calendari condivisi con loro.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problemi

In ogni livello di accesso, puoi configurare le seguenti opzioni per i problemi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Livello di accesso</th> 
   <th>Opzioni</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Pianificatore </td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li> <p><b>Visualizza</b></p><p>Per ottimizzare questo aspetto, puoi configurare la possibilità di condividere i problemi. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso di modifica completo ai problemi.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita, sono tutti attivati.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
       <li> <p>Condividi a livello di sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collaboratore </td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li><p> <b>Visualizza</b></p> <p>Per ottimizzare questo aspetto, puoi configurare la possibilità di condividere i problemi. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso di modifica completo ai problemi.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita, sono tutti attivati.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisore</td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li><p> <b>Visualizza</b></p> <p>Per ottimizzare questo aspetto, puoi configurare la possibilità di condividere i problemi. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso di modifica completo ai problemi.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita, sono tutti attivati.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Richiedente</td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li><p> <b>Visualizza</b></p> <p>Per ottimizzare questo aspetto, puoi configurare la possibilità di condividere i problemi. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso di modifica completo ai problemi.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita, sono tutti attivati.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utente esterno</td> 
   <td> <p>L’accesso ai problemi non è disponibile. Gli utenti esterni possono utilizzare Workfront solo per rivedere e scaricare i documenti e per visualizzare i calendari condivisi con loro.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Portfolio

In ogni livello di accesso, puoi configurare le seguenti opzioni per i portfolio:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Livello di accesso</th> 
   <th>Opzioni</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Pianificatore </td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li><p> <b>Visualizza</b></p> <p>Per ottimizzare questo aspetto, puoi configurare la possibilità di condividere i portfolio. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso di modifica completa ai portfolio.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita, sono tutti attivati.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
       <li> <p>Condividi a livello di sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collaboratore </td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li> <b>Visualizza</b> (selezione predefinita) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisore</td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li> <b>Visualizza</b> (selezione predefinita)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Richiedente</td> 
   <td> <p>L’accesso ai portfolio non è disponibile.</p> </td> 
  </tr> 
  <tr> 
   <td>Utente esterno</td> 
   <td> <p>L’accesso ai portfolio non è disponibile. Gli utenti esterni possono utilizzare Workfront solo per rivedere e scaricare i documenti e per visualizzare i calendari condivisi con loro.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Programmi

In ogni livello di accesso è possibile configurare le opzioni seguenti per i programmi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Livello di accesso</th> 
   <th>Opzioni</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Pianificatore </td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li><p> <b>Visualizza</b></p> <p>Per ottimizzare questo aspetto, puoi configurare la possibilità di condividere i programmi. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso completo alle modifiche ai programmi.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita, sono tutti attivati.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
       <li> <p>Condividi a livello di sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collaboratore </td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li> <b>Visualizza</b> (selezione predefinita) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisore</td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li> <b>Visualizza</b> (selezione predefinita)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Richiedente</td> 
   <td> <p>L'accesso ai programmi non è disponibile.</p> </td> 
  </tr> 
  <tr> 
   <td>Utente esterno</td> 
   <td> <p>L'accesso ai programmi non è disponibile. Gli utenti esterni possono utilizzare Workfront solo per rivedere e scaricare i documenti e per visualizzare i calendari condivisi con loro.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Report, dashboard e calendari

In ogni livello di accesso è possibile configurare le opzioni seguenti per i rapporti, le dashboard e i calendari:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Livello di accesso</th> 
   <th>Opzioni</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Pianificatore </td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li> <p><b>Visualizza</b></p><p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle azioni seguenti. Entrambe sono abilitate per impostazione predefinita:</p> 
      <ul> 
       <li> <p>Visualizza rapporti incorporati</p> </li> 
       <li> <p>Condividi</p> </li> 
      </ul> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso a modifiche complete a report, dashboard e calendari.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita sono attivati tutti, ad eccezione di <b>Visualizza report incorporati</b>, <b>Condividi report pubblicamente</b> e <b>Condividi a livello di sistema</b>.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Visualizza rapporti incorporati</p> </li> 
       <li> <p>Condividi</p> </li> 
       <li> <p>Condividere i rapporti pubblicamente (esternamente)</p> </li> 
       <li> <p>Condividi a livello di sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collaboratore </td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li><p> <b>Visualizza</b></p> (selezione predefinita)<p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle azioni seguenti. Entrambe sono abilitate per impostazione predefinita:</p> 
      <ul> 
       <li> <p>Visualizza rapporti incorporati</p> </li> 
       <li> <p>Condividi</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisore</td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li> <p><b>Visualizza</b> (selezione predefinita)<p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle azioni seguenti. Per impostazione predefinita, è abilitata solo l’opzione Condividi.</p> 
      <ul> 
       <li> <p>Visualizza rapporti incorporati</p> </li> 
       <li> <p>Condividi</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Richiedente</td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li> <p><b>Visualizza</b> (selezione predefinita): consente l'accesso in sola visualizzazione ai report, alle dashboard e ai calendari condivisi.</p> <p>Per ottimizzare questa funzione, puoi configurare la possibilità di visualizzare i rapporti incorporati. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Visualizza</b>, quindi disabilita o abilita <b>Visualizza predefinito</b>(disabilitato per impostazione predefinita).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utente esterno</td> 
   <td> <p>L’accesso a rapporti, dashboard e calendari non è disponibile. Gli utenti esterni possono utilizzare Workfront solo per rivedere e scaricare i documenti e per visualizzare i calendari condivisi con loro.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Filtri, viste e raggruppamenti

In ogni livello di accesso, puoi configurare le seguenti opzioni per filtri, viste e raggruppamenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Livello di accesso</th> 
   <th>Opzioni</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Pianificatore </td> 
   <td> 
    <ul> 
     <li> <p><b>Visualizza</b></p><p>Per ottimizzare questa funzione, puoi configurare la possibilità di condividere filtri, viste e raggruppamenti. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso di modifica completa a filtri, visualizzazioni e raggruppamenti.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita, sono tutti attivati.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
       <li> <p>Condividi a livello di sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collaboratore </td> 
   <td> 
    <ul> 
     <li> <p><b>Visualizza</b></p><p>Per ottimizzare questa funzione, puoi configurare la possibilità di condividere filtri, viste e raggruppamenti. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso di modifica completa a filtri, visualizzazioni e raggruppamenti.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita, sono tutti attivati.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
       <li> <p>Condividi a livello di sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisore</td> 
   <td> 
    <ul> 
     <li><p> <b>Visualizza</b></p> <p>Per ottimizzare questa funzione, puoi configurare la possibilità di condividere filtri, viste e raggruppamenti. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso di modifica completa a filtri, visualizzazioni e raggruppamenti.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita, sono tutti attivati.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
       <li> <p>Condividi a livello di sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Richiedente</td> 
   <td> 
    <ul> 
     <li> <p><b>Visualizzazione</b>:</p> <p>Per ottimizzare questa funzione, puoi configurare la possibilità di condividere filtri, viste e raggruppamenti. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso di modifica completa a filtri, visualizzazioni e raggruppamenti.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita, sono tutti attivati.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
       <li> <p>Condividi a livello di sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utente esterno</td> 
   <td> <p>L’accesso a filtri, viste e raggruppamenti non è disponibile. Gli utenti esterni possono utilizzare Workfront solo per rivedere e scaricare i documenti e per visualizzare i calendari condivisi con loro.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Documenti

In ogni livello di accesso è possibile configurare le opzioni seguenti per i documenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Livello di accesso</th> 
   <th>Opzioni</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Pianificatore </td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li><p> <b>Visualizza</b></p> <p>Per ottimizzare questo aspetto, puoi configurare la possibilità di condividere i documenti. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso ai documenti con modifica completa.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Tutti questi elementi sono abilitati per impostazione predefinita, ad eccezione di <b>Condividi documenti pubblicamente</b> e <b>Condividi a livello di sistema</b>.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
       <li> <p>Condividere documenti pubblicamente (esternamente)</p> </li> 
       <li> <p>Condividi a livello di sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collaboratore </td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li> <p><b>Visualizza</b></p><p>Per ottimizzare questo aspetto, puoi configurare la possibilità di condividere i documenti. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso ai documenti con modifica completa.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Tutti questi elementi sono abilitati per impostazione predefinita, ad eccezione di <b>Condividi documenti pubblicamente</b> e <b>Condividi a livello di sistema</b>.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
       <li> <p>Condividere documenti pubblicamente (esternamente)</p> </li> 
       <li> <p>Condividi a livello di sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisore</td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li><p> <b>Visualizza</b></p> <p>Per ottimizzare questo aspetto, puoi configurare la possibilità di condividere i documenti. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso ai documenti con modifica completa.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle azioni seguenti. Tutti questi elementi sono attivati per impostazione predefinita, ad eccezione degli ultimi due: <b>Condividi documenti pubblicamente</b> e <b>Condividi a livello di sistema</b>.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
       <li> <p>Condividere documenti pubblicamente (esternamente)</p> </li> 
       <li> <p>Condividi a livello di sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Richiedente</td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li> <p><b>Visualizza</b></p><p>Per ottimizzare questo aspetto, puoi configurare la possibilità di condividere i documenti. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso ai documenti con modifica completa.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita, sono tutti attivati.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utente esterno</td> 
   <td> <p>L'accesso ai documenti non è configurabile in questo livello di accesso. Tuttavia, gli utenti esterni possono utilizzare Workfront per visualizzare, esaminare e scaricare i documenti.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Utenti

In ogni livello di accesso, puoi configurare le seguenti opzioni per gli utenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Livello di accesso</th> 
   <th>Opzioni</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Pianificatore </td> 
   <td> 
    <ul> 
     <li> <p><b>Visualizza</b></p><p>Per ottimizzare questa funzione, puoi configurare la possibilità di visualizzare le informazioni di contatto degli utenti. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Visualizza</b>, quindi disabilita o abilita l'opzione <b>Visualizza informazioni di contatto</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente agli utenti l'accesso in modalità di modifica completa.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle azioni seguenti. Per impostazione predefinita, solo le prime due opzioni, <b>Crea</b> e <b>Elimina</b>, sono abilitate.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li>Amministratore utenti (Tutti gli utenti)</li> 
       <li> <p>Amministratore utenti (Utenti gruppi)</p> </li> 
      </ul> <p>Per informazioni sulle due opzioni Amministratore utenti, vedere la sezione <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Configurare l'accesso degli utenti alla modifica mediante un livello di accesso personalizzato</a> nell'articolo <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l'accesso agli utenti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collaboratore </td> 
   <td> 
    <ul> 
     <li><p> <b>Visualizza</b> (solo opzione disponibile)</p><p>Per ottimizzare questa funzione, puoi configurare la possibilità di visualizzare le informazioni di contatto degli utenti. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Visualizza</b>, quindi disabilita o abilita l'opzione <b>Visualizza informazioni di contatto</b> (attivata per impostazione predefinita).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisore</td> 
   <td> 
    <ul> 
     <li><p> <b>Visualizza</b> (solo opzione disponibile)</p> <p>Per ottimizzare questa funzione, puoi configurare la possibilità di visualizzare le informazioni di contatto degli utenti. Fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Visualizza</b>, quindi abilitare o disabilitare l'opzione <b>Visualizza informazioni di contatto</b> (disabilitata per impostazione predefinita).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Richiedente</td> 
   <td> 
    <ul> 
     <li> <p><b>Visualizza</b> (solo opzione disponibile)</p><p>Per ottimizzare questa funzione, puoi configurare la possibilità di visualizzare le informazioni di contatto degli utenti. Fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Visualizza</b>, quindi abilitare o disabilitare l'opzione <b>Visualizza informazioni di contatto</b> (disabilitata per impostazione predefinita).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utente esterno</td> 
   <td> <p>L’accesso agli utenti non è disponibile. Gli utenti esterni possono utilizzare Workfront solo per rivedere e scaricare i documenti e per visualizzare i calendari condivisi con loro.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Team

In ogni livello di accesso, puoi configurare le seguenti opzioni per i team:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Livello di accesso</th> 
   <th>Opzioni</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Pianificatore </td> 
   <td> 
    <ul> 
     <li><b>Visualizza</b> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Visualizza</b>, quindi disabilitare o abilitare una delle opzioni seguenti*. Entrambi sono disattivati per impostazione predefinita.</p> 
      <ul> 
       <li>Visualizza tutti i team</li> 
       <li> <p>Visualizza i team associati ai miei gruppi</p> </li> 
      </ul> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso ai team in modalità di modifica completa.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Visualizza</b>, quindi disabilitare o abilitare una delle opzioni seguenti*. Tutti questi team sono abilitati per impostazione predefinita, ad eccezione di <b>Modifica team in cui si trova</b>.</p> 
      <ul> 
       <li>Crea</li> 
       <li>Elimina</li> 
       <li> <p>Modifica i team in cui l’utente è attivo</p> </li> 
       <li> <p>Modifica team nei gruppi che gestisco (solo per amministratori di gruppi)</p> </li> 
       <li> <p>Visualizza tutti i team</p> </li> 
       <li> <p>Visualizza i team associati ai miei gruppi</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collaboratore </td> 
   <td> 
    <ul> 
     <li> <b>Visualizza</b>
      <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Visualizza</b>, quindi disabilitare o abilitare una delle opzioni seguenti*. Entrambi sono attivati per impostazione predefinita.</p> 
      <ul> 
       <li>Visualizza tutti i team</li> 
       <li> <p>Visualizza i team associati ai miei gruppi</p> </li> 
      </ul> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso ai team in modalità di modifica completa.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Visualizza</b>, quindi disabilitare o abilitare una delle opzioni seguenti*. Per impostazione predefinita, solo la prima opzione, <b>Modifica team in cui mi trovo</b>, è disabilitata.</p> 
      <ul> 
       <li> <p>Modifica i team in cui l’utente è attivo</p> </li> 
       <li> <p>Visualizza tutti i team</p> </li> 
       <li> <p>Visualizza i team associati ai miei gruppi</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisore</td> 
   <td> 
    <ul> 
     <li> <p><b>Visualizza</b> (solo opzione disponibile)</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Visualizza</b>, quindi disabilitare o abilitare una delle opzioni seguenti*. Entrambi sono attivati per impostazione predefinita.</p> 
      <ul> 
       <li> <p>Visualizza tutti i team</p> </li> 
       <li>Visualizza i team associati ai miei gruppi</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Richiedente</td> 
   <td> 
    <ul> 
     <li> <p><b>Visualizza</b> (solo opzione disponibile)</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Visualizza</b>, quindi disabilitare o abilitare una delle opzioni seguenti*. Entrambi sono attivati per impostazione predefinita.</p> 
      <ul> 
       <li> <p>Visualizza tutti i team</p> </li> 
       <li>Visualizza i team associati ai miei gruppi</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utente esterno</td> 
   <td> <p>L’accesso ai team non è disponibile. Gli utenti esterni possono utilizzare Workfront solo per rivedere e scaricare i documenti e per visualizzare i calendari condivisi con loro.</p> </td> 
  </tr> 
 </tbody> 
</table>


## Modelli

In ogni livello di accesso, puoi configurare le seguenti opzioni per i modelli:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Livello di accesso</th> 
   <th>Opzioni</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Pianificatore </td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li><p> <b>Visualizza</b></p> <p>Per ottimizzare questo aspetto, puoi configurare la possibilità di condividere i modelli. Fai clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante Visualizza, quindi disabilita o abilita l'opzione <b>Condividi</b> (attivata per impostazione predefinita).</p> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso ai modelli in modalità di modifica completa.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita, sono tutti attivati.</p> 
      <ul> 
       <li> <p>Crea</p> </li> 
       <li> <p>Elimina</p> </li> 
       <li> <p>Condividi</p> </li> 
       <li> <p>Condividi a livello di sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collaboratore </td> 
   <td> 
    <ul> 
     <li> <p><b>Nessun accesso</b> (solo opzione disponibile)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisore</td> 
   <td> 
    <ul> 
     <li> <p><b>Nessun accesso</b> (solo opzione disponibile)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Richiedente</td> 
   <td> 
    <ul> 
     <li> <p><b>Nessun accesso</b> (solo opzione disponibile)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utente esterno</td> 
   <td> <p>L’accesso ai modelli non è disponibile. Gli utenti esterni possono utilizzare Workfront solo per rivedere e scaricare i documenti e per visualizzare i calendari condivisi con loro.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Dati finanziari

In ogni livello di accesso, puoi configurare le seguenti opzioni per i dati finanziari:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Livello di accesso</th> 
   <th>Opzioni</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Pianificatore </td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li> <p><b>Visualizzazione</b>:</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Visualizza</b>, quindi disabilitare o abilitare una delle opzioni seguenti*. Entrambi sono attivati per impostazione predefinita.</p> 
      <ul> 
       <li>Visualizza fatturazione mansione e tassi di costo</li> 
       <li> <p>Visualizza fatturazione utente e tassi di costo</p> </li> 
      </ul> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso in modalità di modifica completa ai dati finanziari.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Visualizza</b>, quindi disabilitare o abilitare una delle opzioni seguenti*. Per impostazione predefinita, solo le ultime due opzioni, <b>Visualizza fatturazione mansione e tassi di costo</b> e <b>Visualizza fatturazione utente e tassi di costo</b>, sono abilitate.</p> 
      <ul> 
       <li>Modifica fatturazione mansione e tassi di costo</li> 
       <li> <p>Modifica fatturazione utente e tassi di costo</p> </li> 
       <li>Visualizza fatturazione mansione e tassi di costo</li> 
       <li> <p>Visualizza fatturazione utente e tassi di costo</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collaboratore </td> 
   <td> 
    <ul> 
     <li> <p><b>Nessun accesso</b> (selezione predefinita)</p> </li> 
     <li> <b>Visualizza</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisore</td> 
   <td> 
    <ul> 
     <li> <p><b>Nessun accesso</b> (selezione predefinita)</p> </li> 
     <li><b>Visualizza</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Richiedente</td> 
   <td> 
    <ul> 
     <li> <p><b>Nessun accesso</b> (solo opzione disponibile)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utente esterno</td> 
   <td> <p>L'accesso ai dati finanziari non è disponibile. Gli utenti esterni possono utilizzare Workfront solo per rivedere e scaricare i documenti e per visualizzare i calendari condivisi con loro.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Per informazioni su queste opzioni, vedere [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Gestione risorse

In ogni livello di accesso è possibile configurare le opzioni seguenti per Gestione risorse:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Livello di accesso</th> 
   <th>Opzioni</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Pianificatore </td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li> <b>Visualizza</b> </li> 
     <li> <p><b>Modifica</b> (selezione predefinita): consente l'accesso di modifica completa a Gestione risorse.</p> <p>Per ottimizzare l'operazione, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-in-access-levels.png"> sul pulsante <b>Modifica</b>, quindi disabilitare o abilitare una delle opzioni seguenti. Per impostazione predefinita, è abilitata solo la prima opzione, <b>Modifica priorità e ore preventivate nel Planner</b>.</p> 
      <ul> 
       <li> <p> Modifica priorità e ore preventivate nella Programmazione</p> </li> 
       <li> <p>Gestisci gruppi di risorse</p> <p><b>NOTA</b>: per gestire i pool di risorse, un utente ha bisogno di ulteriore accesso ai dati finanziari e alle autorizzazioni per i dati finanziari del progetto. Se si concede l'accesso Gestione risorse a un utente di Planner che non ha accesso ai dati finanziari, l'utente potrà comunque visualizzare le allocazioni orarie nella Pianificazione risorse, ma non potrà passare alla visualizzazione Costo o al Business Case. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Concedere l'accesso ai dati finanziari</a> e <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Condividere le autorizzazioni finanziarie su un oggetto</a>.</p> </li> 
       <li> <p>Aggiorna le ore pianificate nel Bilanciatore dei carichi di lavoro</p> <p><b>NOTA</b>: per aggiornare le ore pianificate nel Bilanciatore dei carichi di lavoro, un utente deve disporre dell'autorizzazione per contribuire all'oggetto con l'opzione Crea assegnazioni abilitata in Impostazioni avanzate. Per informazioni, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Panoramica delle autorizzazioni di condivisione sugli oggetti</a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collaboratore </td> 
   <td> 
    <ul> 
     <li><b>Nessun accesso</b> </li> 
     <li> <b>Visualizza</b> (selezione predefinita) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisore</td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> </li> 
     <li> <b>Visualizza</b> (selezione predefinita)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Richiedente</td> 
   <td> 
    <ul> 
     <li> <b>Nessun accesso</b> (solo opzione disponibile) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utente esterno</td> 
   <td> <p>Accesso non disponibile. Gli utenti esterni possono utilizzare Workfront solo per rivedere e scaricare i documenti e per visualizzare i calendari condivisi con loro.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Area Pianificazione scenario

L&#39;impostazione predefinita per tutti i livelli di accesso è Nessun accesso. Un amministratore Workfront può modificare questo livello di accesso in Visualizzazione o Modifica per qualsiasi livello di accesso di Planner, Worker e Revisore.

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>Gli utenti possono visualizzare un piano creato da un altro utente solo se con essi è condiviso un collegamento al piano.

## Area Obiettivi Workfront

Tutti e sei i livelli di accesso predefiniti (e tutti e quattro i tipi di licenza) possono modificare e visualizzare gli Obiettivi di Workfront.

Modifica (Edit) è l&#39;opzione predefinita.
