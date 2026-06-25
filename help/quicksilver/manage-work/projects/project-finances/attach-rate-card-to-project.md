---
title: Allegare una scheda tariffa a un progetto
description: Quando alleghi una scheda tariffaria a un progetto, tutti i ruoli e le relative tariffe di fatturazione vengono aggiunti al progetto.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
TQID: https://experienceleague.adobe.com/waVWQfq2YqgDXZx3wl0ahzuQx7UJ78S1kYY8xBgi5OQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0ae6286f0c76f638358839603fba1301d5557d83
workflow-type: tm+mt
source-wordcount: 565
ht-degree: 8%

---

# Allegare una scheda tariffaria a un progetto

Le schede tariffa memorizzano più tariffe di fatturazione per mansione, in base agli attributi. Ad esempio, potresti avere un ruolo di Designer con sede a Parigi per l’Agenzia A, un altro Designer con sede a Parigi per l’Agenzia B e un terzo Designer con sede a New York non assegnato a un’agenzia, ciascuno con tariffe di fatturazione diverse. Tuttavia, gli attributi non sono necessari per le mansioni su una scheda tariffa. Gli attributi fungono da strumenti per stabilire tassi più granulari. Una tariffa di fatturazione su una scheda tariffa può anche essere data di validità, in modo che la tariffa inizi e termini in date specificate.

Quando alleghi una scheda tariffaria a un progetto, tutti i ruoli e le relative tariffe di fatturazione vengono aggiunti al progetto.

>[!NOTE]
>
>Quando si allega una scheda tariffa, vengono ignorate tutte le tariffe di fatturazione della scheda tariffa esistenti sul progetto. Le sostituzioni delle tariffe di fatturazione aggiunte direttamente al progetto non vengono rimosse.

Per informazioni sulla creazione di schede di frequenza, vedere [Gestione delle schede di frequenza](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

Per informazioni generali sulla sostituzione delle tariffe di fatturazione dei ruoli per i progetti e sul calcolo dei ricavi del progetto, vedere [Panoramica sulla sostituzione delle tariffe di fatturazione e sul calcolo dei ricavi per un progetto](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

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
   <td>Modifica accesso a progetti, dati finanziari e schede tassi</td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td>Gestisci le autorizzazioni per il progetto con le autorizzazioni per Modifica tariffe di fatturazione</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Allegare una scheda tariffaria a un progetto

1. Vai al progetto.
1. Fai clic su **Tariffe** nel pannello a sinistra, quindi seleziona **Fatturazione**.
1. Fai clic su **Aggiungi tariffa di fatturazione > Allega una tariffa**.

   Viene visualizzata la casella **Allega scheda tariffa**. È possibile cercare una scheda di tariffa nell’elenco.

   ![Allegare una casella della scheda tariffaria](assets/attach-rate-card-dialog.png)

   >[!NOTE]
   >
   >Il Gruppo e la Società nelle schede di tariffa vengono utilizzati come filtri in questo elenco. Poiché i progetti includono anche campi Gruppo e Società, Workfront utilizza questi valori per restringere l’elenco delle schede di tariffa disponibili a quelle pertinenti per il contesto del progetto e non a tutte le schede di tariffa nel sistema.
   >
   >Non è necessario che la corrispondenza sia esatta. Le schede di tariffa con valori Gruppo e/o Azienda vuoti possono ancora essere visualizzate a seconda della configurazione Gruppo/Azienda del progetto. Ad esempio, se per un progetto è selezionato un gruppo ma la società è vuota, è possibile che vengano visualizzate le schede di tariffa associate a tale gruppo anche se la società della scheda di tariffa è diversa o vuota.

1. Seleziona la scheda tariffe da aggiungere al progetto e fai clic su **Allega**.

   La scheda tariffa e tutte le relative tariffe per le mansioni vengono aggiunte all’elenco delle tariffe di fatturazione.

   ![Scheda tariffa aggiunta al progetto](assets/rate-card-on-project.png)

## Rimuovere una scheda delle tariffe da un progetto

Quando rimuovi una scheda tariffe da un progetto, tutte le relative tariffe per le mansioni vengono rimosse. Non puoi rimuovere una singola tariffa dal progetto che proviene da una scheda delle tariffe.

Le sostituzioni delle tariffe di fatturazione per gli utenti o le mansioni che sono state aggiunte direttamente al progetto possono essere rimosse senza rimuovere l’intera scheda delle tariffe.

1. Vai al progetto.
1. Fai clic su **Tariffe** nel pannello a sinistra, quindi seleziona **Fatturazione**.
1. Fai clic sull&#39;icona **Rimuovi** ![Rimuovi icona](assets/remove-icon.png).
1. Fai clic su **Conferma** nel messaggio di conferma per rimuovere la scheda della tariffa.

