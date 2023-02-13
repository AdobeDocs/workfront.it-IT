---
title: Creare e gestire modelli di layout
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: In qualità di amministratore di Workfront o di gruppo, puoi creare e modificare modelli di layout per personalizzare gli elementi di layout in Workfront per i tuoi utenti.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Creare e gestire modelli di layout

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

In qualità di amministratore di Workfront o di amministratore di gruppo, puoi creare e modificare modelli di layout per personalizzare i seguenti elementi di layout in Workfront per i tuoi utenti:

* Menu principale
* Pannello di navigazione a sinistra
* Area abitativa
* Visualizzazioni, filtri e raggruppamenti utilizzati dagli utenti con elenchi e rapporti.
* Terminologia su schermo

Dopo aver creato o modificato un modello di layout, è possibile assegnarlo a singoli utenti, team, gruppi o ruoli di lavoro.

Il layout Workfront predefinito di ogni utente dipende dal livello di accesso e dal tipo di licenza. Ad esempio, alcuni utenti potrebbero non visualizzare alcune aree nel menu principale. Per ulteriori informazioni, consulta [Informazioni sul layout predefinito di Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

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
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.
Per eseguirle per un gruppo, devi essere un responsabile di quel gruppo.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Considerazioni sulla creazione e la gestione dei modelli di layout

* Gli utenti possono personalizzare alcune aree del proprio layout. Quando si modifica un modello di layout, le modifiche si uniscono a tutte le personalizzazioni effettuate senza sovrascriverle o ripristinarle. Questo vale anche se assegni utenti a un nuovo modello di layout.
* I vecchi modelli di layout creati in Adobe Workfront Classic sono disponibili automaticamente nella tua istanza della nuova esperienza Adobe Workfront dopo la migrazione all’inizio di autunno 2019. I modelli di layout creati in Adobe Workfront Classic in seguito a tale migrazione sono stati migrati nell’aprile 2020. È consigliabile aggiornare questi modelli di layout nella nuova esperienza Adobe Workfront per sfruttare le nuove funzionalità e renderli ancora più utili in tale ambiente.
* Gli amministratori di gruppo e gli utenti con una licenza Plan che possono modificare altri utenti possono aggiungere modelli di layout a livello di sistema e di gruppo agli utenti che possono gestire quando modificano il loro profilo.
* Gli amministratori di gruppo non possono assegnare modelli di layout a ruoli di lavoro o team.

Per ulteriori informazioni sui modelli di layout, consulta [Modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

## Creare o modificare un modello di layout

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Interfaccia** > **Modelli di layout**.

1. Fai clic su **Nuovo modello di layout**.

   Oppure

   Fare clic sul nome del modello di layout che si desidera modificare.

1. Se si sta creando un nuovo modello di layout, digitare un **Nome del modello di layout** e (facoltativo) a **Descrizione** per questo.

1. Personalizza le aree dell’interfaccia utente, come descritto nei seguenti articoli:

   * [Personalizzare il menu principale utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Personalizzare il pannello a sinistra utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Personalizzare le pagine bloccate utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Personalizzare Home e Riepilogo utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [Personalizzare la pagina di destinazione utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Personalizzare filtri, visualizzazioni e gruppi utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [Personalizzare la terminologia dell’interfaccia utente utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Continua a testare il modello di layout e renderlo disponibile agli utenti, come descritto negli articoli seguenti:

   * [Verifica di un nuovo modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Consentire l’accesso amministrativo per un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Assegnare gli utenti a un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

È inoltre possibile creare un nuovo modello di layout copiandolo e modificando la copia. Per ulteriori informazioni, consulta [Copiare un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).
