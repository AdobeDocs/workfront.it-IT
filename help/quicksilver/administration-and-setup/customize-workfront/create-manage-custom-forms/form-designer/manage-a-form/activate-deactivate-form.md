---
title: Disattivare o riattivare un modulo personalizzato
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile riattivare o disattivare un modulo personalizzato. È consigliabile disattivare i moduli personalizzati anziché eliminare i moduli che non vengono più utilizzati per conservare i dati storici.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: 15ac51cc13eeb57d2de194a9a6ceec7683acfbe6
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Disattivare o riattivare un modulo personalizzato

È possibile riattivare o disattivare un modulo personalizzato. È consigliabile disattivare i moduli personalizzati anziché eliminare i moduli che non vengono più utilizzati per conservare i dati storici.

>[!NOTE]
>
>Se un modulo personalizzato viene disattivato ma fa ancora parte di un argomento della coda o di una definizione della coda di richieste, verrà allegato alle nuove richieste. Se non desideri che il modulo sia presente nelle richieste, devi rimuoverlo manualmente dalla coda delle richieste.

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
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> </td> 
  </tr>  
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Disattivare un modulo personalizzato

È possibile disattivare i moduli personalizzati che non vengono più utilizzati senza perdere i dati storici associati. Gli utenti non possono aggiungere un modulo personalizzato inattivo agli oggetti, ma possono comunque visualizzare e aggiungere dati ai relativi campi su oggetti a cui era già associato.

Anche i campi di un modulo personalizzato inattivo sono ancora disponibili per la modifica in linea in una visualizzazione. Se un utente aggiunge un campo da un modulo personalizzato inattivo durante una modifica in linea, il modulo viene allegato automaticamente all’oggetto anche se il modulo personalizzato è disattivato.

Per disattivare un modulo personalizzato:

{{step-1-to-setup}}

1. Nel pannello a sinistra, scegli **Forms personalizzato**.
1. Nell&#39;area **Forms** selezionare il modulo personalizzato che si desidera disattivare.
1. Nella colonna È attivo, scegliere **False** e fare clic all&#39;esterno della colonna. Modulo non più attivo.

## Riattivare un modulo personalizzato

Se si riattiva un modulo personalizzato, vengono mantenute le impostazioni precedenti e gli utenti possono interagire con esso come se non fosse mai stato disattivato.

{{step-1-to-setup}}

1. Nel pannello a sinistra, scegli **Forms personalizzato**.
1. Nell&#39;area **Forms** selezionare il modulo personalizzato che si desidera riattivare.
1. Nella colonna È attivo scegliere **True** e fare clic all&#39;esterno della colonna. Il modulo è ora attivo.
