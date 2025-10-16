---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Eliminare uno stato personalizzato
description: È possibile eliminare uno stato di sistema personalizzato se non risulta più utile per l'organizzazione.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: 366043a786c94f1bc40ad3b20af175bb84c94742
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 2%

---

# Eliminare uno stato personalizzato

È possibile eliminare uno stato di sistema personalizzato se non risulta più utile per l&#39;organizzazione.

Se lo stato è bloccato o sbloccato determina se lo stato viene eliminato per tutti i gruppi nel sistema:

* Quando si elimina uno stato di sistema attualmente bloccato, lo stato viene rimosso per tutti i gruppi del sistema, indipendentemente dal fatto che il gruppo lo abbia rinominato.
* Al contrario, quando si elimina uno stato di sistema attualmente sbloccato, lo stato rimane per tutti i gruppi del sistema.


>[!NOTE]
>
>Non è possibile eliminare i seguenti elementi:
>
>* Stato di sistema bloccato o sbloccato utilizzato in un processo di approvazione di sistema attualmente in attesa di approvazione per almeno un oggetto nel sistema.
>
>  È tuttavia possibile eliminare uno stato di sistema sbloccato utilizzato in un processo di approvazione a livello di singolo utente o di gruppo attualmente in attesa di approvazione.
>
>  È possibile eseguire un report per trovare gli oggetti e risolvere le approvazioni in sospeso, quindi riprovare a eliminare lo stato. Per istruzioni, vedere [Elencare oggetti con processi di approvazione in sospeso che utilizzano un determinato stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* Stati utilizzati nei processi di approvazione che sono attualmente in attesa di approvazione per almeno un oggetto nel sistema.

Per istruzioni sull&#39;eliminazione dello stato di un gruppo, vedere [Eliminare lo stato di un gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

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

## Eliminare uno stato di sistema personalizzato

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Preferenze progetto** > **Stati**.

1. Per eliminare lo stato in tutto il sistema (inclusi i singoli gruppi), passa il cursore del mouse sullo stato, fai clic su **Modifica**, quindi accertati che sia selezionato **Blocca per tutti i gruppi**. Fai clic su **Salva**.

   Oppure

   Per eliminare lo stato del sistema ma mantenerlo per i singoli gruppi, passa il cursore sullo stato, fai clic su **Modifica**, quindi accertati che **Blocca per tutti i gruppi** sia deselezionato. Fai clic su **Salva**.

1. Passa il puntatore del mouse sullo stato che desideri eliminare, quindi fai clic su **Elimina**.
1. Nel messaggio visualizzato fare clic su **Elimina stato**.
1. Nella casella **Elimina stato** visualizzata, selezionare uno stato nel campo **Imposta tutti i progetti con questo stato su**.

   I progetti che utilizzavano lo stato che si sta eliminando vengono impostati sullo stato selezionato.

   Gli stati sono disponibili nell’elenco a discesa solo se equivalgono allo stato che si sta eliminando.

   Ad esempio, se si elimina uno stato che è uguale a Corrente, solo gli stati che sono uguali a Corrente sono disponibili per la selezione.

1. Fare clic su **Elimina stato**.
