---
title: Funzionamento congiunto dei livelli di accesso e delle autorizzazioni
user-type: administrator
content-type: reference
product-area: system-administration
keywords: accesso,modello,funnel,diagramma,livelli,autorizzazioni
navigation-topic: access-levels
description: L’amministratore Adobe Workfront determina il livello di accesso di ogni utente. Tale livello di accesso definisce cosa gli utenti possono vedere e fare con i tipi di oggetto e le aree del sistema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
source-git-commit: 09afa5808fd4078def16da7a9ccf393c99f47d03
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 2%

---

# Funzionamento congiunto dei livelli di accesso e delle autorizzazioni

L’amministratore Adobe Workfront determina il livello di accesso di ogni utente. Tale livello di accesso definisce cosa gli utenti possono vedere e fare con i tipi di oggetto e le aree del sistema.

Gli utenti possono inoltre accedere a singoli oggetti quando altri utenti condividono e concedono determinate autorizzazioni su tali oggetti.


![](assets/security-model-hierachy.png)

Se ad esempio il livello di accesso indica che è possibile creare attività, ma le autorizzazioni ricevute per un progetto specifico non consentono di aggiungervi attività, non è possibile aggiungere attività al progetto anche se è possibile crearle altrove in Workfront.

Questo articolo spiega come funziona questa combinazione.

## Livello di accesso

Per accedere a Workfront è necessario il livello di accesso assegnato a ogni utente da un amministratore Workfront.

I livelli di accesso predefiniti sono:

* Amministratore di sistema (collegato alla licenza Pianificazione)
* Planner (allegato alla licenza Pianificazione)
* Lavoratore (collegato alla licenza Lavoro)
* Revisore (allegato alla licenza Revisione)
* Richiedente (allegato alla licenza Richiesta)
* Utente esterno (allegato alla licenza e-mail esterna)

La licenza Workfront per ogni livello di accesso predefinito determina ciò che è disponibile e configurabile nel livello di accesso. Per informazioni sulle licenze Workfront, consulta [Panoramica sulle licenze di Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

Per gli utenti che sono assegnati a esso, un livello di accesso definisce cosa possono vedere e cosa fare con i seguenti tipi di oggetti e aree in Workfront:

* Progetti
* Attività
* Problemi
* Portfolio
* Report, dashboard e calendari
* Filtri, visualizzazioni e raggruppamenti
* Documenti
* Altri utenti
* Modelli
* Dati finanziari
* Gestione risorse
* Pianificazione scenario
* Workfront Goals

In un livello di accesso personalizzato, è possibile configurare le impostazioni per questi oggetti e aree per modificare il livello di accesso degli utenti a tali oggetti e aree. A seconda della licenza associata al livello di accesso, nonché del tipo di oggetto o di area, è possibile configurare il livello di accesso in modo da non consentire l&#39;accesso, l&#39;accesso di visualizzazione o la modifica a un oggetto o a un&#39;area.

>[!IMPORTANT]
>
>È consigliabile lasciare invariati i livelli di accesso incorporati in modo da potervi fare riferimento dopo aver configurato gli utenti. Per personalizzare un livello di accesso, copiare il livello di accesso predefinito e modificare la copia. Questa operazione può essere eseguita per ogni livello di accesso, ad eccezione di Amministratore di sistema e Utente esterno.

Per una spiegazione dettagliata di ciascuno dei livelli di accesso predefiniti, vedi [Livelli di accesso incorporati](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

Per istruzioni sull’assegnazione di un livello di accesso a un utente, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Autorizzazioni

Quando si condivide un oggetto con un utente del sistema, l&#39;utente può concedere al destinatario le seguenti autorizzazioni.

* **Visualizza**: questo livello di autorizzazione consente al destinatario di condividere l’oggetto in uno dei seguenti modi:

   * A livello di sistema, in modo che tutti gli utenti possano visualizzarlo (non disponibile per tutti gli oggetti)
   * Con utenti esterni che non dispongono di una licenza Workfront (non disponibile per tutti gli oggetti)
   * Con un indirizzo e-mail (disponibile solo per i documenti)

* **Contribuisci**: (non disponibile per tutti gli oggetti)
* **Gestisci**: quando qualcuno condivide un oggetto, i diritti del destinatario sull’oggetto sono determinati da una combinazione del livello di accesso del destinatario e delle autorizzazioni per l’oggetto concesse dal condivisore. Il livello di accesso più basso disponibile in tale combinazione è quello che determina il comportamento del destinatario con l’oggetto.

  >[!INFO]
  >
  >**Esempio:** Se il livello di accesso del destinatario non consente la modifica del progetto, l’utente non può modificare o eliminare un progetto anche se il condivisore ha concesso le autorizzazioni per gestirlo.
  >
  >In alternativa, se il livello di accesso del destinatario consente la modifica del progetto, ma il condivisore concede autorizzazioni di sola visualizzazione a un progetto, l’utente non può modificare o eliminare il progetto.

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
   <td>Concessi da un amministratore Workfront nel livello di accesso di un utente</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Concesso da un utente che condivide un oggetto a livello di oggetto</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Ereditato da un oggetto condiviso di livello superiore 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Se un utente condivide un oggetto con determinate autorizzazioni e tale oggetto ha oggetti figlio al di sotto di esso, il destinatario eredita le stesse autorizzazioni per tali oggetti figlio.
>* Se un livello di accesso impedisce agli utenti di eliminare determinati oggetti, ciò non impedisce loro di eliminare gli oggetti secondari contenuti in tali oggetti.
>

## Altri scenari esemplificativi

Quando Olivia condivide un progetto Workfront con Tony, l’accesso di quest’ultimo è determinato da una combinazione di due fattori:

* Livello di accesso di Tony assegnato dall’amministratore Workfront
* Autorizzazioni di Tony per il progetto, specificate da Olivia

Le azioni di Tony sul progetto possono essere ulteriormente limitate sul progetto, ma non possono essere illimitate al di là di ciò che è consentito sul suo livello di accesso:

* Se il livello di accesso di Tony non gli consente di creare attività, non può aggiungere attività al progetto , anche se Olivia gli ha dato le autorizzazioni per aggiungervi attività.
* Se il livello di accesso di Tony non gli consente di creare attività, ma Olivia non concede le autorizzazioni per aggiungere attività al progetto, non può aggiungere attività a tale progetto, ma può aggiungere attività ad altri progetti per i quali dispone delle autorizzazioni necessarie.
