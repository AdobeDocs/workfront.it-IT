---
title: Allegare una scheda tariffe a un progetto
description: Quando alleghi una scheda tariffaria a un progetto, tutti i ruoli per ubicazione e le relative tariffe di fatturazione vengono aggiunti al progetto.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '449'
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

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano corrente: Standard</p><p>Oppure</p><p>Piano legacy: piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti e dati finanziari</p> <p>Accesso amministrativo per le mansioni</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il progetto con le autorizzazioni per Gestire le finanze</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Allegare una scheda tariffe a un progetto

1. Vai al progetto.
1. Fai clic su **Tariffe di fatturazione** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro**.
1. Fai clic su **Aggiungi tariffa di fatturazione > Allega una tariffa**.

   Viene visualizzata la pagina Allega scheda tariffa. Per ulteriori informazioni, consulta [Gestione schede tariffarie](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. Seleziona la scheda tariffe da aggiungere al progetto e fai clic su **Allega**.

   La scheda tariffa e tutte le relative tariffe per le mansioni vengono aggiunte all’elenco delle tariffe di fatturazione.

   ![Scheda tariffa aggiunta al progetto](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >Nell&#39;elenco tariffe di fatturazione è possibile rimuovere una o più mansioni provenienti da una scheda tariffe. La rimozione di una tariffa di fatturazione della mansione dal progetto non la rimuove dalla scheda della tariffa predefinita.
