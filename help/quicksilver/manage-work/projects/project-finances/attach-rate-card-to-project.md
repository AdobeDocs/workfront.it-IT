---
title: Allegare una scheda tariffa a un progetto
description: Quando alleghi una scheda tariffaria a un progetto, tutti i ruoli per ubicazione e le relative tariffe di fatturazione vengono aggiunti al progetto.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Allegare una scheda tariffe a un progetto

{{highlighted-preview-article-level}}

Le schede tariffa memorizzano più tariffe di fatturazione per mansione, in base alla posizione. Potresti avere un ruolo di Designer con sede a Parigi e un secondo Designer con sede a New York, ciascuno con tariffe di fatturazione diverse. Tuttavia, non è necessario specificare una posizione per le mansioni su una scheda tariffaria. Una tariffa di fatturazione per una mansione (e possibilmente l&#39;ubicazione) su una scheda della tariffa può includere anche date di validità.

Quando alleghi una scheda tariffaria a un progetto, tutti i ruoli per ubicazione e le relative tariffe di fatturazione vengono aggiunti al progetto.

>[!NOTE]
>
>Quando si allega una scheda tariffa, vengono ignorate tutte le tariffe di fatturazione esistenti sul progetto.

Puoi modificare le tariffe di fatturazione direttamente dalla scheda delle tariffe nel progetto. Questo non influisce sulle tariffe memorizzate sulla scheda delle tariffe predefinita.

Per informazioni sulla creazione di schede di frequenza, vedere [Gestione delle schede di frequenza](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

Per informazioni generali sulla sostituzione delle tariffe di fatturazione dei ruoli per i progetti e sul calcolo dei ricavi del progetto, vedere [Panoramica sulla sostituzione delle tariffe di fatturazione dei ruoli e sul calcolo dei ricavi per un progetto](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a progetti e dati finanziari</p> <p>Accesso amministrativo per le mansioni</p></td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni oggetto</td> 
   <td>Gestisci le autorizzazioni per il progetto che includono Modifica dati finanziari </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Allegare una scheda tariffe a un progetto

1. Vai al progetto.
1. Fai clic su **Tariffe di fatturazione** nel pannello a sinistra.
1. Fai clic su **Aggiungi tariffa di fatturazione > Allega una tariffa**.

   Viene visualizzata la pagina Allega scheda tariffa. Per ulteriori informazioni, consulta [Gestione schede tariffarie](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. Seleziona la scheda tariffe da aggiungere al progetto e fai clic su **Allega**.

   La scheda tariffa e tutte le relative tariffe per le mansioni vengono aggiunte all’elenco delle tariffe di fatturazione.

   ![Scheda tariffa aggiunta al progetto](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >Nell&#39;elenco tariffe di fatturazione è possibile rimuovere una o più mansioni provenienti da una scheda tariffe. La rimozione di una tariffa di fatturazione della mansione dal progetto non la rimuove dalla scheda della tariffa predefinita.
