---
title: Eliminare una condizione personalizzata
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: È possibile eliminare una condizione personalizzata.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: 1eab0317bfe72609133e71411ee24263517f1508
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Eliminare una condizione personalizzata

{{highlighted-preview}}

Se una condizione personalizzata non è più necessaria, è possibile eliminarla.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>Oppure</p>
       <p>Corrente: Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminare una condizione personalizzata

{{step-1-to-setup}}

1. Fai clic su **Preferenze progetto** > **Condizioni**.

1. Selezionare la scheda del tipo di oggetto (**Progetto**, **Attività** o **Problema**) in cui si trova la condizione che si desidera eliminare.

1. Fai clic su <span class="preview">**Elimina** accanto al nome della condizione</span> che desideri eliminare oppure passa il puntatore del mouse sulla condizione e fai clic sull&#39;icona **Elimina** ![Elimina](assets/delete.png) visualizzata all&#39;estrema destra.

1. Nella casella **Elimina condizione** visualizzata, selezionare una nuova condizione nell&#39;elenco a discesa per tutti i progetti, le attività o i problemi che utilizzano la condizione che si sta eliminando.

   Le condizioni personalizzate sono disponibili nell’elenco a discesa solo se equivalgono alla stessa condizione incorporata di quella che si sta eliminando. Ad esempio, se elimini una condizione che equivale a A rischio, la selezione sarà possibile solo per le condizioni personalizzate che equivalgono anche a A rischio.

1. Fare clic su **Elimina condizione**.

>[!NOTE]
>
>Non è possibile eliminare le condizioni incorporate, che sono On Target, At Risk e In Trouble. Tuttavia, è possibile modificarne i nomi e i colori.
>
>Per informazioni sulla modifica delle condizioni personalizzate, vedere [Creare o modificare una condizione personalizzata](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).
