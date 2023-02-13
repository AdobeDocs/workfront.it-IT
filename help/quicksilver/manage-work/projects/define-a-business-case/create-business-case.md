---
navigation-topic: business-case-and-scorecards
title: Creare un business case per un progetto
description: È possibile utilizzare il Business Case per richiedere un progetto e definire lo scopo, il budget e il potenziale beneficio del progetto. Il Portfoli Manager o Project Sponsor utilizza le informazioni contenute nel Business Case per analizzare e assegnare una priorità al progetto prima che venga approvato.
author: Alina
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 0%

---

# Creare un business case per un progetto

È possibile utilizzare il Business Case per richiedere un progetto e definire lo scopo, il budget e il potenziale beneficio del progetto. Il Portfoli Manager o Project Sponsor utilizza le informazioni contenute nel Business Case per analizzare e assegnare una priorità al progetto prima che venga approvato.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l'accesso a progetti, dati finanziari e gestione risorse</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci o autorizzazioni superiori per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Quando richiedi un progetto tramite un Business Case, considera quanto segue:

* L’amministratore di Adobe Workfront o l’amministratore di gruppo deve abilitare le sezioni del Business Case prima che vengano visualizzate nel progetto.\
   Per informazioni sull&#39;abilitazione delle sezioni nel Business Case a livello di sistema, vedere l&#39;articolo [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   Per informazioni sulle aree del Business Case, vedere l&#39;articolo [Panoramica delle aree del Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* Se desideri che il progetto riceva un punteggio in Portfoli Optimizer, devi completare tutte le aree del Business Case eccetto l&#39;area Obiettivi . Il completamento dell’area Obiettivi è facoltativo. Il progetto riceve un punteggio in Portfoli Optimizer, anche se questa area non è stata completata.

   Per informazioni sull’utilizzo delle scorecard e di Portfoli Optimizer, consulta l’articolo [Applicare una scorecard a un progetto e generare un punteggio di allineamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

## Creare un caso aziendale

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png), quindi fai clic su **Progetti**.
1. Fai clic su **Nuovo progetto** e seleziona **Richiedi progetto**.\
   Per impostazione predefinita, il progetto viene inserito nella **Idea** stato.

   >[!CAUTION]
   >
   >Se lo stato Idea è stato eliminato nell’istanza di Workfront, il progetto viene posizionato nello stato predefinito per i nuovi progetti, come definito nell’area Preferenze progetto. Per informazioni sulla configurazione delle preferenze del progetto, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. Specifica un nome per il progetto, quindi premi Invio.
1. (Facoltativo) Fai clic sul pulsante **Altro** icona ![](assets/qs-more-icon-on-an-object.png), quindi **Allega modello**, per creare la struttura di suddivisione del lavoro del progetto.

   Oppure

   Inizia ad aggiungere manualmente le attività al progetto.

1. (Condizionale) Se hai selezionato di allegare un modello, continua ad allegare il modello al progetto
1. Fai clic su **Business case** nel pannello a sinistra.
1. (Facoltativo) Fai clic su **Modifica informazioni progetto**. 

   Per ulteriori informazioni sulla modifica dei campi nella sezione Informazioni progetto del Business Case, vedere la sezione [Informazioni progetto](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) nell&#39;articolo [Panoramica delle aree del Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Facoltativo) Fai clic su **Modifica obiettivi**.

   Per ulteriori informazioni sulla modifica della sezione Obiettivi del Business Case, consulta la sezione [Obiettivi](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals) nell&#39;articolo [Panoramica delle aree del Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Facoltativo) Fai clic su **Modifica spese**.

   Per ulteriori informazioni sulla modifica della sezione Spese del Business Case, consulta la sezione [Spese](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses) nell&#39;articolo [Panoramica delle aree del Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Facoltativo) Utilizzare l&#39;area Budget risorse per eseguire il budget delle risorse e ottenere il costo del lavoro a budget associato ai ruoli del lavoro nel progetto. Per ulteriori informazioni, consulta [Risorse di budget nel Business Case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   >[!TIP]
   >
   >Le informazioni visualizzate sono le stesse visualizzate negli strumenti di budget delle risorse a livello di sistema.

1. (Facoltativo) Fai clic su **Modifica rischi** aggiungere rischi potenziali a questo progetto. Per informazioni sull&#39;aggiunta di rischi al Business Case, vedere la [Rischi](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks) sezione dell&#39;articolo [Panoramica delle aree del Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).
1. (Facoltativo) Seleziona un **Scorecard** in **Aggiungi una scorecard****a questo progetto** menu a discesa.

   Le scorecard devono essere create prima di poter essere aggiunte ai progetti.

   Per ulteriori informazioni sulle scorecard, consulta l’articolo [Applicare una scorecard a un progetto e generare un punteggio di allineamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

1. (Facoltativo) Seleziona un **Modulo personalizzato** in **Forms personalizzato** menu a discesa.

   È necessario creare Forms personalizzato prima di poterli allegare ai progetti.

   Per ulteriori informazioni su Custom Forms, consulta l’articolo [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Fai clic su **Invia**.

   Lo stato del progetto viene modificato in **Richiesto** e viene sottoposto all&#39;approvazione del Business Case.

   Per ulteriori informazioni sull&#39;approvazione di un Business Case, consulta l&#39;articolo [Approvare un caso aziendale](../../../manage-work/projects/define-a-business-case/approve-business-case.md).

1. (Facoltativo) Dopo aver completato il Business Case, puoi esportarne una copia in un file .pdf . Per ulteriori informazioni sull&#39;esportazione del Business Case in un file .pdf, vedere la sezione &quot;Export the Business Case&quot; nell&#39;articolo [Panoramica delle aree del Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).
