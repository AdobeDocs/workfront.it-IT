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
source-git-commit: 366043a786c94f1bc40ad3b20af175bb84c94742
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 1%

---

# Eliminare una condizione personalizzata

Se una condizione personalizzata non è più necessaria, è possibile eliminarla.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Amministratore di Sistema</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminare una condizione personalizzata

{{step-1-to-setup}}

1. Fai clic su **Preferenze progetto** > **Condizioni**.

1. Selezionare la scheda del tipo di oggetto (**Progetto**, **Attività** o **Problema**) in cui si trova la condizione che si desidera eliminare.

1. Fai clic su **Elimina** accanto al nome della condizione che desideri eliminare.
1. Nella casella **Elimina condizione** visualizzata, selezionare una nuova condizione nell&#39;elenco a discesa per tutti i progetti, le attività o i problemi che utilizzano la condizione che si sta eliminando.

   Le condizioni personalizzate sono disponibili nell’elenco a discesa solo se equivalgono alla stessa condizione incorporata di quella che si sta eliminando. Ad esempio, se elimini una condizione che equivale a A rischio, la selezione sarà possibile solo per le condizioni personalizzate che equivalgono anche a A rischio.

1. Fare clic su **Elimina condizione**.

>[!NOTE]
>
>Non è possibile eliminare le condizioni incorporate, che sono On Target, At Risk e In Trouble. Tuttavia, è possibile modificarne i nomi e i colori.
>
>Per informazioni sulla modifica delle condizioni personalizzate, vedere [Creare o modificare una condizione personalizzata](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).
