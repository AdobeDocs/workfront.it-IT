---
title: Eliminare una condizione personalizzata
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: È possibile eliminare una condizione personalizzata.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Eliminare una condizione personalizzata

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Eliminare una condizione personalizzata

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Preferenze progetto** > **Condizioni**.

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. Selezionare la scheda del tipo di oggetto (**Progetto**, **Attività** o **Problema**) in cui si trova la condizione che si desidera eliminare.

1. Passa il puntatore del mouse sulla condizione da eliminare, quindi fai clic sull&#39;icona **Elimina** ![](assets/delete.png) visualizzata all&#39;estrema destra.
1. Nel messaggio di conferma visualizzato, fare clic su **Elimina condizione**.

1. Nella casella **Elimina condizione** visualizzata, selezionare una nuova condizione nell&#39;elenco a discesa per tutti i progetti che utilizzano la condizione che si sta eliminando.

   Le condizioni personalizzate sono disponibili nell’elenco a discesa solo se equivalgono alla stessa condizione incorporata di quella che si sta eliminando. Ad esempio, se elimini una condizione che equivale a A rischio, la selezione sarà possibile solo per le condizioni personalizzate che equivalgono anche a A rischio.

1. Fare clic su **Elimina condizione**.

>[!NOTE]
>
>Non è possibile eliminare le condizioni incorporate, che sono On Target, At Risk e In Trouble. Tuttavia, è possibile modificarne i nomi e i colori.

Per informazioni sulle condizioni personalizzate, vedere [Condizioni personalizzate](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
