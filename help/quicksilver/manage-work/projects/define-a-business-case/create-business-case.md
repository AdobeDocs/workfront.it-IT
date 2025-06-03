---
navigation-topic: business-case-and-scorecards
title: Creare un Business Case per un progetto
description: È possibile utilizzare il Business Case per richiedere un progetto e definirne lo scopo, il budget e il vantaggio potenziale. Portfolio Manager o lo sponsor del progetto utilizza le informazioni del Business Case per analizzare e assegnare la priorità al progetto prima che venga approvato.
author: Alina
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: 9cfb67f627c06a5926e820860d52ba9f1ab58bcf
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---

# Creare un Business Case per un progetto

È possibile utilizzare il Business Case per richiedere un progetto e definirne lo scopo, il budget e il vantaggio potenziale. Portfolio Manager o lo sponsor del progetto utilizza le informazioni del Business Case per analizzare e assegnare la priorità al progetto prima che venga approvato.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> 
   <p>Corrente: Prime o versione successiva</p> 
   <p>Legacy: Pro o superiore</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Corrente: Standard </p> 
   <p>Legacy: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a progetti, dati finanziari e gestione risorse</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci o autorizzazioni superiori per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Quando si richiede un progetto tramite un Business Case, tenere presente quanto segue:

* L’amministratore di Adobe Workfront o l’amministratore di gruppo deve abilitare le sezioni del Business Case prima che vengano visualizzate nel progetto.\
  Per informazioni sull&#39;abilitazione delle sezioni nel Business Case a livello di sistema, vedere l&#39;articolo [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  Per informazioni sulle aree del Business Case, vedere l&#39;articolo [Panoramica delle aree del Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* Se si desidera che il progetto riceva un punteggio in Portfolio Optimizer, è necessario completare tutte le aree del Business Case, ad eccezione dell&#39;area Obiettivi. Il completamento dell’area Obiettivi è facoltativo. Il progetto riceve un punteggio in Portfolio Optimizer, anche se questa area non è stata completata.

  Per informazioni sull&#39;utilizzo delle scorecard e di Portfolio Optimizer, vedere l&#39;articolo [Applicare una scorecard a un progetto e generare un punteggio di allineamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

## Creazione di un Business Case

{{step1-to-projects}}

1. Fai clic su **Nuovo progetto**, quindi seleziona **Richiedi progetto** dal menu a discesa visualizzato. Il progetto è stato creato e lo stato **Idea** è assegnato per impostazione predefinita.

   >[!CAUTION]
   >
   >Se lo stato Idea è stato eliminato nell’istanza di Workfront, il progetto viene posto nello stato predefinito per i nuovi progetti, come definito nell’area Preferenze progetto. Per informazioni sulla configurazione delle preferenze di progetto, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. Immetti un nome nel campo del titolo del progetto.
1. (Facoltativo) Fai clic sull&#39;icona **Altro** ![Altro icona](assets/qs-more-icon-on-an-object.png), quindi **Allega modello** per creare la struttura funzionale del progetto.

   Oppure

   Inizia ad aggiungere attività al progetto manualmente.

1. (Condizionale) Se hai selezionato di allegare un modello, continua ad allegarlo al progetto.
1. Nel pannello a sinistra, fai clic su **Business Case**.
1. (Facoltativo) Per modificare la sezione **Informazioni progetto**, fare clic su **Modifica informazioni progetto**. 

   Per ulteriori informazioni sulla modifica dei campi della sezione **Informazioni progetto**, vedere la sezione [Informazioni progetto](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) nell&#39;articolo [Panoramica delle aree del caso di business](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Facoltativo) Per modificare la sezione **Obiettivi**, fai clic su **Modifica obiettivi**.

   Per ulteriori informazioni sulla modifica della sezione **Obiettivi** del caso aziendale, vedere la sezione [Obiettivi](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals) nell&#39;articolo [Panoramica delle aree del caso aziendale](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Facoltativo) Per modificare la sezione **Spese**, fare clic su **Modifica spese**.

   Per ulteriori informazioni sulla modifica della sezione **Spese** del Business Case, vedere la sezione [Spese](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses) nell&#39;articolo [Panoramica delle aree del Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Facoltativo) Fare clic su **Modifica budget risorse** per preventivare le risorse e ottenere il costo manodopera preventivato associato alle mansioni del progetto. Per ulteriori informazioni, vedere [Risorse budget nel caso di business](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   >[!TIP]
   >
   >Le informazioni visualizzate qui corrispondono a quelle visualizzate negli strumenti di budget delle risorse a livello di sistema.

1. (Facoltativo) Fai clic su **Modifica rischi** per aggiungere potenziali rischi a questo progetto. Per informazioni sull&#39;aggiunta di rischi al Business Case, vedere la sezione [Rischi](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks) nell&#39;articolo [Panoramica delle aree del Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).
1. (Facoltativo) Seleziona una **scorecard** nel menu a discesa **Aggiungi una scorecard a questo progetto**.

   Le scorecard devono essere create prima di poter essere allegate ai progetti.

   Per ulteriori informazioni sulle scorecard, vedere l&#39;articolo [Applicare una scorecard a un progetto e generare un punteggio di allineamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

1. (Facoltativo) Selezionare un **modulo personalizzato** nel menu a discesa **Forms** personalizzato.

   È necessario creare un Forms personalizzato prima di allegarlo ai progetti.

   Per ulteriori informazioni su Forms personalizzato, vedere l&#39;articolo [Creazione di un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Fai clic su **Invia**. Lo stato del progetto è cambiato in **Richiesto** e viene inviato per l&#39;approvazione del Business Case.

   Per ulteriori informazioni sull&#39;approvazione di un caso aziendale, vedere l&#39;articolo [Approvare un caso aziendale](../../../manage-work/projects/define-a-business-case/approve-business-case.md).


>[!TIP]
>
> Dopo aver completato il Business Case, puoi esportare una copia in un file .pdf. Per ulteriori informazioni sull&#39;esportazione del Business Case in un file .pdf, vedere [Esportare il Business Case di un progetto](/help/quicksilver/manage-work/projects/define-a-business-case/export-business-case.md).


