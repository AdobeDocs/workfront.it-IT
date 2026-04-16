---
content-type: overview
product-area: projects
navigation-topic: financials
title: Imposta una mansione per la fatturazione
description: Workfront consente di fatturare un utente con una mansione diversa da quella principale. Questo è utile quando una persona svolge temporaneamente un lavoro che dovrebbe essere fatturato a una tariffa diversa.
author: Lisa
feature: Work Management
exl-id: d6e2947d-2f40-4591-b048-9a769caadf43
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 5%

---

# Imposta una mansione per la fatturazione

Workfront consente di fatturare un utente con una mansione diversa da quella principale. Questo è utile quando una persona svolge temporaneamente un lavoro che dovrebbe essere fatturato a una tariffa diversa.

È possibile assegnare una mansione per la fatturazione in due modi:

* A livello di progetto: utilizza questa opzione quando la persona deve essere fatturata con lo stesso ruolo per l’intero progetto.
* A livello di assegnazione: utilizzare questa opzione per fatturare in modo diverso task specifici.

>[!NOTE]
>
>* Una mansione per la fatturazione si applica solo alle persone (utenti). Non si applica a mansioni o segnaposto generici.
>* L’aggiunta di una mansione per la fatturazione influisce solo sulla tariffa di fatturazione, non sui costi.
>* La fatturazione a livello di assegnazione ha sempre la priorità rispetto alla fatturazione a livello di progetto.

Per ulteriori informazioni, vedere [Panoramica sulla gerarchia ricavi e costi](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) e [Creare assegnazioni avanzate](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

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
   <td> Modifica accesso alle schede tariffe</td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td>Gestire le autorizzazioni per il progetto </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Assegna una mansione per la fatturazione a livello di progetto

Quando crei una mansione per la fatturazione su un progetto:

* Il ruolo di fatturazione si applica a tutte le attività e assegnazioni all’interno del progetto per tale utente.
* La fatturazione utilizza la tariffa di fatturazione della mansione selezionata, ma il costo segue ancora il ruolo principale dell&#39;utente.

Per assegnare una mansione per la fatturazione a livello di progetto:

1. Apri un progetto.
1. Fai clic su **Risorsa per fatturazione** nel pannello a sinistra.
1. Selezionare la scheda **Ruolo per fatturazione** se non è già visualizzata.
1. Fai clic su **Aggiungi > Aggiungi mansione per la fatturazione**.
1. Nella casella **Aggiungi mansione per la fatturazione**, selezionare **Utente**.
1. Selezionare la **mansione** da utilizzare come mansione per la fatturazione per questo utente in questo progetto.
1. (Facoltativo) Fai clic su **Aggiungi mansione** per definire le date di validità della mansione per la fatturazione. Immetti le date **Inizio** e **Fine** per la mansione.

[Aggiungi mansione per la fatturazione a livello di progetto](assets/jrfb-project-level.png)

1. Fai di nuovo clic su **Aggiungi mansione** per specificare ulteriori ruoli di fatturazione per diversi periodi di tempo.
1. Fai clic su **Salva**.

### Esempio a livello di progetto

>[!BEGINSHADEBOX]

Il ruolo principale di John è Designer 1. Il progetto richiede un Senior Designer, e John sta compilando.

È necessario impostare la mansione per la fatturazione su **Designer senior** a livello di progetto.

Risultato:

* I ricavi di fatturazione sono il tasso Designer senior
* Costo è la tariffa di Designer 1 (tariffa di John)

>[!ENDSHADEBOX]

## Assegna una mansione per la fatturazione a livello di assegnazione

Quando si aggiunge una mansione per la fatturazione di un&#39;assegnazione, l&#39;impostazione sostituisce un ruolo di fatturazione a livello di progetto solo per l&#39;assegnazione specifica.

Per assegnare una mansione per la fatturazione a livello di assegnazione:

1. Apri un progetto e individua l’attività.
1. Vai a **Assegnazioni avanzate** dell&#39;attività.

   Per informazioni, vedere [Creare assegnazioni avanzate](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Nella griglia di assegnazione dell&#39;attività individuare la colonna **Ruolo per fatturazione**.
1. Selezionare una mansione per ogni assegnazione per la quale si desidera una fatturazione diversa.

   >[!NOTE]
   >
   >Se a livello di progetto è stata assegnata una mansione per la fatturazione, questa viene visualizzata nell&#39;assegnazione. Puoi fare clic nel campo **Ruolo per fatturazione** e selezionare un&#39;altra mansione da utilizzare per l&#39;assegnazione.
   >L&#39;icona delle informazioni indica se è stata definita una mansione per la fatturazione a livello di progetto o di assegnazione.

   ![Ruolo per fatturazione su un&#39;assegnazione](assets/jrfb-assignment-level.png)

### Esempio a livello di assegnazione

>[!BEGINSHADEBOX]

Il ruolo principale di John è Designer 1. Viene fatturato come Senior Designer a livello di progetto, ma c&#39;è un&#39;attività speciale che richiede una tariffa di fatturazione Principal Designer.

È necessario impostare la mansione per la fatturazione su Principal Designer solo per tale assegnazione.

Risultato:

* Tutte le altre attività di John fatturano come Designer senior
* Questa attività viene fatturata come Designer principale
* Il costo rimane Designer 1

>[!ENDSHADEBOX]
