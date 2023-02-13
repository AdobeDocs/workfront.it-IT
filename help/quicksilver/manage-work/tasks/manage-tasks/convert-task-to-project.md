---
product-area: projects
navigation-topic: manage-tasks
title: Convertire un'attività in un progetto
description: Quando un'attività di un progetto richiede uno sforzo maggiore per essere completata rispetto alla pianificazione iniziale, puoi convertirla in un progetto.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Convertire un&#39;attività in un progetto

Quando un&#39;attività di un progetto richiede uno sforzo maggiore per essere completata rispetto alla pianificazione iniziale, puoi convertirla in un progetto.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l’accesso a Attività e Progetti</p> <p>Visualizza o consente un accesso più elevato ai modelli durante la conversione in un progetto utilizzando un modello</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestione delle autorizzazioni per un’attività</p> <p>Visualizza le autorizzazioni di un modello, se si converte in un progetto utilizzando un modello</p> <p>Dopo aver creato il progetto, disponi delle autorizzazioni Gestisci per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Considerazioni sulla conversione di attività in progetti

* L&#39;attività originale viene eliminata.
* Le approvazioni delle attività vengono eliminate.
* Tutte le attività secondarie, i problemi e le note vengono aggregati al nuovo progetto.
* I documenti, le versioni dei documenti e le bozze vengono spostati nel nuovo progetto.
* Lo stato e la percentuale di completamento di tutte le attività secondarie e i problemi vengono mantenuti.
* Gli utenti condivisi dell’attività diventano utenti condivisi nel progetto.
* La data di inizio del progetto è impostata sulla data di inizio dell&#39;attività.
* Se lo stato dell&#39;attività è &quot;Nuovo&quot;, lo stato del progetto è impostato su &quot;Pianificazione&quot;.
* Se lo stato dell&#39;attività è &quot;In corso&quot;, lo stato del progetto è impostato su &quot;Corrente&quot;.
* Se lo stato dell’attività è &quot;Completato&quot;, lo stato del progetto è &quot;Completo&quot;.

## Convertire un&#39;attività in un progetto

1. Passa all’attività da convertire in un progetto.
1. Fai clic sul pulsante **Altro** icona ![](assets/more-icon.png), quindi **Converti in progetto**.
1. Scegli una delle seguenti opzioni:

   * **Nuovo progetto**
   * Un modello nel **Seleziona da modelli** sezione

      ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. Fai clic su **Continua** sulla notifica visualizzata.
1. In **Converti in progetto** specificare quanto segue:

   * **Nome**: Assegna un nome al progetto. Il nome predefinito è il nome dell’attività.
   * (Facoltativo) **Descrizione**: Descrivere lo scopo del progetto.
   * (Facoltativo e condizionale) Se hai selezionato di creare un progetto da un modello, aggiorna i campi disponibili nella sezione **Converti in progetto** finestra di dialogo.

      Per ulteriori informazioni sulla modifica dei campi nei progetti, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >Per aggiornare i campi nella sezione Finanza della casella Converti in progetto, è necessario disporre dell&#39;accesso Modifica ai dati finanziari nel livello di accesso. Se disponi dell&#39;accesso Visualizza dati finanziari nel tuo livello di accesso, tutte le informazioni finanziarie del modello vengono trasferite al nuovo progetto e non puoi modificarle durante la conversione del problema. Per informazioni, consulta [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) e [Condividere un modello](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (Facoltativo) Aggiungi **Forms personalizzato** al nuovo progetto.

      >[!TIP]
      Se un modulo personalizzato con più oggetti associato all’attività è configurato per l’utilizzo con attività e progetti, tutte le informazioni salvate nel modulo vengono mantenute al momento della conversione.
      Se si utilizza un modello per la conversione e un modulo personalizzato allegato al modello contiene un campo personalizzato anch’esso presente in un modulo personalizzato allegato all’attività, per il nuovo progetto viene utilizzato il valore del campo dell’attività. Tuttavia, se il campo personalizzato è vuoto nell&#39;attività, viene utilizzato il valore del modello.

1. Fai clic su **Salva modifiche**.
