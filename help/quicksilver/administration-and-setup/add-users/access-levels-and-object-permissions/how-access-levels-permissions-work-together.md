---
title: Funzionamento congiunto dei livelli di accesso e delle autorizzazioni
user-type: administrator
content-type: reference
product-area: system-administration
keywords: accesso, modello, funnel, diagramma, livelli, autorizzazioni
navigation-topic: access-levels
description: L’amministratore di Adobe Workfront determina il livello di accesso che ogni utente deve avere. Tale livello di accesso definisce le operazioni che gli utenti possono visualizzare e eseguire con i tipi di oggetto e le aree del sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
source-git-commit: df73ba291f0a0ab6492e6fabfb6de578ba7e1f1b
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 2%

---

# Funzionamento congiunto dei livelli di accesso e delle autorizzazioni

L’amministratore di Adobe Workfront determina il livello di accesso che ogni utente deve avere. Tale livello di accesso definisce le operazioni che gli utenti possono visualizzare e eseguire con i tipi di oggetto e le aree del sistema.

Inoltre, gli utenti possono accedere a singoli oggetti quando altri utenti condividono e concedono determinate autorizzazioni a tali oggetti.

Pertanto, le attività che un utente può eseguire con un oggetto sono definite da una combinazione del proprio livello di accesso e delle autorizzazioni date loro per quel progetto.

![](assets/security-model-hierachy.png)

Ad esempio, se il livello di accesso indica che è possibile creare attività, ma le autorizzazioni ricevute per un progetto specifico non consentono di aggiungerle, non è possibile aggiungere attività al progetto anche se è possibile creare attività altrove in Workfront.

Questo articolo spiega come funziona questa combinazione.

## Livello di accesso

Il livello di accesso assegnato a ciascun utente da un amministratore Workfront è necessario per accedere a Workfront.

I livelli di accesso predefiniti sono:

* Amministratore di sistema (collegato alla licenza Plan)
* Planner (allegato alla licenza Plan)
* Lavoratore (collegato alla licenza Work)
* Revisore (allegato alla licenza di revisione)
* Richiedente (allegato alla licenza di richiesta)
* Utente esterno (collegato alla licenza Email esterna)

La licenza Workfront per ogni livello di accesso predefinito determina cosa è disponibile e configurabile a livello di accesso. Per informazioni sulle licenze Workfront, vedi [Panoramica sulle licenze di Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

Per gli utenti a cui è assegnato, un livello di accesso definisce cosa possono vedere e fare con i seguenti tipi di oggetti e aree in Workfront:

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

In un livello di accesso personalizzato, è possibile configurare le impostazioni per questi oggetti e aree in modo da modificare il numero di accessi che gli utenti hanno a tali oggetti. A seconda della licenza associata al livello di accesso e del tipo di oggetto o area, è possibile configurare il livello di accesso in modo da non consentire l’accesso, la visualizzazione dell’accesso o la modifica dell’accesso a un oggetto o a un’area.

>[!IMPORTANT]
>
>È vivamente consigliato lasciare invariati i livelli di accesso incorporati, in modo da potervi fare riferimento dopo aver configurato gli utenti. Per personalizzare un livello di accesso, copia il livello di accesso predefinito e modifica la copia. (È possibile eseguire questa operazione per ogni livello di accesso, ad eccezione di Amministratore di sistema e Utente esterno.)

Per una spiegazione dettagliata di ciascuno dei livelli di accesso predefiniti, vedi [Livelli di accesso incorporati in Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

Per istruzioni su come assegnare un livello di accesso a un utente, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Autorizzazioni

Quando si condivide un oggetto con un utente del sistema, quest&#39;ultimo può concedere al destinatario una delle seguenti autorizzazioni all&#39;oggetto.

* **Visualizza**: Questo livello di autorizzazione consente al destinatario di condividere l’oggetto in uno dei seguenti modi:

   * A livello di sistema in modo che tutti gli utenti possano visualizzarlo (non disponibile per tutti gli oggetti)
   * Con utenti esterni che non dispongono di una licenza Workfront (non disponibile per tutti gli oggetti)
   * Con un indirizzo e-mail (disponibile solo per i documenti)

* **Collaborare**: (non disponibile per tutti gli oggetti)
* **Gestisci**: Quando un utente condivide un oggetto, i diritti del destinatario sull&#39;oggetto sono determinati da una combinazione del livello di accesso del destinatario e delle autorizzazioni per l&#39;oggetto concesse dal condivisore. Il grado di accesso più basso disponibile in quella combinazione determina cosa può fare il destinatario con l’oggetto.

   >[!INFO]
   >
   >**Esempio:** Se il livello di accesso del destinatario non consente la modifica del progetto, l’utente non può modificare o eliminare un progetto anche se l’utente condiviso dispone delle autorizzazioni necessarie per gestirlo.
   >
   >Oppure, se il livello di accesso del destinatario consente la modifica del progetto, ma a chi condivide vengono concesse autorizzazioni di sola visualizzazione a un progetto, l’utente non può modificare o eliminare il progetto.

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

>[!NOTE]
>
>* Se un utente condivide un oggetto con determinate autorizzazioni e dispone di oggetti secondari al suo interno, il destinatario eredita le stesse autorizzazioni per tali oggetti secondari.
>* Se un livello di accesso limita l’eliminazione di determinati oggetti da parte degli utenti, ciò non impedisce loro di eliminare gli oggetti secondari contenuti in tali oggetti.
>


## Altri scenari di esempio

Quando Olivia condivide un progetto Workfront con Tony, l&#39;accesso di Tony è determinato da una combinazione di due cose:

* Livello di accesso di Tony, assegnato dall&#39;amministratore Workfront
* Le autorizzazioni di Tony per il progetto, specificate da Olivia

Le azioni di Tony sul progetto possono essere ulteriormente limitate al progetto, ma non possono essere illimitate oltre quanto consentito al suo livello di accesso:

* Se il livello di accesso di Tony non gli consente di creare attività, non può aggiungere attività al progetto, anche se Olivia gli ha dato le autorizzazioni per aggiungere attività.
* Se il livello di accesso di Tony gli consente di creare attività, ma Olivia non concede le autorizzazioni per aggiungere attività al progetto, non può aggiungere attività a quel progetto, ma può aggiungere attività ad altri progetti in cui gli sono state concesse le autorizzazioni per farlo.
