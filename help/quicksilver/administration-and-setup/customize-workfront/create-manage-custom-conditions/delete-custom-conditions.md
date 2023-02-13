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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Eliminare una condizione personalizzata

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Preferenze del progetto** > **Condizioni**.

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. Seleziona la scheda del tipo di oggetto (**Progetto**, **Attività** oppure **Problema**), in cui si trova la condizione da eliminare.

1. Passa il puntatore del mouse sulla condizione da eliminare, quindi fai clic sul pulsante **Elimina** icona ![](assets/delete.png) all&#39;estrema destra.
1. Nel messaggio di conferma visualizzato, fai clic su **Elimina condizione**.

1. In **Elimina condizione** selezionare una nuova condizione nell&#39;elenco a discesa per tutti i progetti che utilizzavano la condizione da eliminare.

   Le condizioni personalizzate sono disponibili nell’elenco a discesa solo se corrispondono alla stessa condizione incorporata di quella che si sta eliminando. Ad esempio, se si elimina una condizione che equivale a A rischio, è possibile selezionare solo le condizioni personalizzate che corrispondono anche a Rischio.

1. Fai clic su **Elimina condizione**.

>[!NOTE]
>
>Non è possibile eliminare le condizioni incorporate, ovvero On Target, At Risk e In Trouble. Tuttavia, è possibile modificarne i nomi e i colori.

Per informazioni sulle condizioni personalizzate, consulta [Condizioni personalizzate](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
