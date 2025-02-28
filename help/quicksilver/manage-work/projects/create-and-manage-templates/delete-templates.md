---
product-area: templates
navigation-topic: templates-navigation-topic
title: Eliminare i modelli di progetto
description: È consigliabile disattivare i modelli che non si utilizzano più, anziché eliminarli, in modo da poter conservare nel tempo informazioni storiche sui progetti.
author: Alina
feature: Work Management
exl-id: 41e0979c-f8ef-4a07-8848-e4ee8cc212c5
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Eliminare i modelli di progetto

È consigliabile disattivare i modelli che non si utilizzano più, anziché eliminarli, in modo da poter conservare nel tempo informazioni storiche sui progetti. Per informazioni sulla disattivazione di un modello, vedere [Modifica modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!IMPORTANT]
>
>Quando elimini un modello, i progetti che lo utilizzano non vengono modificati in alcun modo. Tuttavia, non è più possibile visualizzare il nome del modello originale nel campo Modello del progetto. Inoltre, non è più possibile visualizzare i nomi delle attività modello per le attività del progetto in una visualizzazione delle attività. I campi Modello del progetto e Attività modello delle attività rimangono vuoti dopo l&#39;eliminazione del modello originariamente associato al progetto.

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
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica l'accesso ai Modelli che include l'accesso a Elimina</p> <p> <img src="assets/template-access-level-with-advanced-settings-350x113.png" style="width: 350;height: 113;"> </p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci le autorizzazioni per il modello che include le autorizzazioni per eliminarlo</p> <p> <img src="assets/template-manage-permissions-with-advanced-settings-350x352.png" style="width: 350;height: 352;"> </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Considerazioni sull’eliminazione dei modelli

* Le attività aggiunte ai progetti quando il modello è stato allegato rimangono nei progetti. Tuttavia, le informazioni sull&#39;attività modello associate alle attività vengono eliminate.
* Il nome del modello non è più elencato nel campo **Modello** nella scheda secondaria **Panoramica** del progetto.

* È possibile ripristinare un modello eliminato di recente dal Cestino. Per informazioni sul ripristino degli elementi dal Cestino, vedere [Ripristinare gli elementi eliminati](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Eliminare un modello

{{step1-to-templates}}

Verrà aperto un elenco di modelli

1. Selezionare il modello da eliminare facendo clic sulla casella di controllo a sinistra del nome del modello, quindi fare clic su **Elimina > Sì, Elimina** per confermare l&#39;eliminazione.

   Oppure

   Fai clic sul nome di un modello per accedervi, quindi fai clic sul menu **Altro** ![Icona Altro](assets/qs-more-icon-on-an-object.png) , quindi **Elimina modello > Sì, Elimina**.

   Il modello non è più disponibile per essere associato a un progetto.
