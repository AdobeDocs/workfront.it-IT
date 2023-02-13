---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Eliminare uno stato personalizzato
description: Se non è più utile per la tua organizzazione, puoi eliminare uno stato di sistema personalizzato.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# Eliminare uno stato personalizzato

Se non è più utile per la tua organizzazione, puoi eliminare uno stato di sistema personalizzato.

Se lo stato è bloccato o sbloccato determina se lo stato viene eliminato per tutti i gruppi nel sistema:

* Quando si elimina uno stato di sistema attualmente bloccato, lo stato viene rimosso per tutti i gruppi del sistema, indipendentemente dal fatto che il gruppo lo abbia rinominato o meno.
* Viceversa, quando si elimina uno stato di sistema attualmente sbloccato, lo stato rimane per tutti i gruppi nel sistema.


>[!NOTE]
>
>Non è possibile eliminare quanto segue:
>
>* Stato di sistema bloccato o sbloccato utilizzato in un processo di approvazione del sistema in attesa di approvazione per almeno un oggetto nel sistema.
>
>  Tuttavia, è possibile eliminare uno stato di sistema sbloccato utilizzato in un singolo utilizzo o in un processo di approvazione a livello di gruppo attualmente in attesa di approvazione.
>
>  È possibile eseguire un rapporto per individuare gli oggetti e risolvere le approvazioni in sospeso, quindi riprovare a eliminare lo stato. Per istruzioni, consulta [Elencare oggetti con processi di approvazione in sospeso utilizzando un determinato stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* Stati utilizzati nei processi di approvazione in attesa di approvazione per almeno un oggetto del sistema.


Per istruzioni sull&#39;eliminazione di uno stato di gruppo, vedere [Eliminare uno stato di gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

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

## Eliminare uno stato di sistema personalizzato

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Preferenze del progetto** > **Stati**.

1. Per eliminare lo stato nell’intero sistema (incluso per i singoli gruppi), passa il mouse sullo stato e fai clic su **Modifica**, quindi assicurati che **Blocca per tutti i gruppi** è selezionato. Fai clic su **Salva**.

   Oppure

   Per eliminare lo stato del sistema ma conservarlo per i singoli gruppi, passare il mouse sullo stato e fare clic su **Modifica**, quindi assicurati che **Blocca per tutti i gruppi** viene deselezionato. Fai clic su **Salva**.

1. Passa il puntatore del mouse sullo stato da eliminare, quindi fai clic su **Elimina**.
1. Nel messaggio visualizzato, fai clic su **Elimina stato**.
1. In **Elimina stato** casella visualizzata, selezionare uno stato nel campo contrassegnato **Imposta tutti i progetti con questo stato su**.

   I progetti che utilizzavano lo stato da eliminare vengono impostati sullo stato selezionato.

   Gli stati sono disponibili nell’elenco a discesa solo se corrispondono allo stesso stato dell’eliminazione.

   Ad esempio, se si elimina uno stato che equivale a Corrente, è possibile selezionare solo gli stati che corrispondono anche a Corrente.

1. Fai clic su **Elimina stato**.
