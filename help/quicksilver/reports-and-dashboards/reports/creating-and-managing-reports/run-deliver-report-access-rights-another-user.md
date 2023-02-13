---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Eseguire e distribuire un rapporto con i diritti di accesso di un altro utente
description: Per impostazione predefinita, gli utenti possono visualizzare solo gli oggetti di un rapporto che dispongono delle autorizzazioni di visualizzazione.
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: 269340bc6a0c237edf44f5aa325d4ff95b647df8
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 0%

---

# Eseguire e distribuire un rapporto con i diritti di accesso di un altro utente

Per impostazione predefinita, gli utenti possono visualizzare solo gli oggetti di un rapporto che dispongono delle autorizzazioni di visualizzazione.

È possibile consentire a tutti gli utenti di visualizzare gli stessi risultati in un rapporto di un altro utente, indipendentemente dal livello di accesso o di autorizzazione degli oggetti all’interno del rapporto.

Se si esegue un rapporto con i diritti di accesso di un altro utente con accesso più elevato (ad esempio, i diritti di accesso di un amministratore Adobe Workfront), tutti gli utenti che dispongono delle autorizzazioni di visualizzazione del rapporto possono visualizzare le informazioni nel rapporto come l&#39;utente specificato nel generatore di report. Puoi configurarlo sia per i rapporti che gli utenti trovano nell’interfaccia di Workfront, sia per i rapporti che vengono consegnati agli utenti come allegati a un’e-mail.

>[!TIP]
>
>È necessario sostituire **Esegui questo rapporto con i diritti di accesso di:** campo con un utente attivo solo quando si desidera visualizzare il rapporto con i diritti di accesso di tale utente. Ad esempio, un utente con licenza di lavoro potrebbe non disporre delle autorizzazioni necessarie per visualizzare tutti gli elementi di un report generato da un utente con licenza di piano o da un amministratore di sistema, a meno che il report non venga visualizzato con i diritti di accesso di un planner o di un amministratore di sistema.\
Se il rapporto è condiviso con utenti con accesso simile a quello specificato nell&#39; **Esegui questo rapporto con i diritti di accesso di:** è possibile lasciare vuoto questo campo.

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
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni per un rapporto (per visualizzare il rapporto consegnato)</p> <p>Gestire le autorizzazioni per un report (per eseguire il report)</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Visualizzare un rapporto con i diritti di accesso di un altro utente

Popolazione del **Esegui questo rapporto con i diritti di accesso di:** assicura che un report contenga gli stessi dati, indipendentemente dall&#39;utente che accede al report. Il rapporto viene visualizzato come per l’utente specificato.

Per poter visualizzare il rapporto, gli utenti che accedono al rapporto devono disporre almeno delle autorizzazioni di visualizzazione. Se l’utente ha elencato nella **Esegui questo rapporto con i diritti di accesso di:** Il rapporto non viene più visualizzato per gli altri utenti con cui è condiviso il rapporto.

Per eseguire un rapporto con i diritti di accesso di un altro utente:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **Rapporti**.

1. Seleziona il rapporto da visualizzare con i diritti di accesso di un altro utente.
1. Fai clic su **Azioni dei rapporti**, quindi fai clic su **Modifica**.

1. Fai clic su **Impostazioni dei rapporti**.

1. In **Esegui questo rapporto con i diritti di accesso di:** inizia a digitare il nome dell’utente con cui desideri visualizzare il rapporto, quindi selezionalo quando lo trovi nell’elenco.\
   ![](assets/qs-access-rights-of-350x251.png)

   >[!NOTE]
   Gli utenti con un livello di accesso inferiore consentito per la generazione di rapporti non possono selezionare un utente diverso da se per il **Esegui questo rapporto con i diritti di accesso di:** campo .

1. Fai clic su **Fine**.
1. Fai clic su **Salva e chiudi**.\
   Il rapporto ora viene visualizzato per tutti gli utenti con cui è condiviso il rapporto, come se fosse stato visualizzato dall’utente specificato nel **Esegui questo rapporto con i diritti di accesso di:** campo .

>[!IMPORTANT]
Inserimento di un utente diverso dall&#39;utente connesso per **Esegui questo rapporto con i diritti di accesso di:** Questo campo influisce sulle informazioni visualizzate nel rapporto se contiene un filtro che utilizza un carattere jolly che fa riferimento all’utente connesso. Il rapporto viene visualizzato in base al valore specificato nel **Esegui questo rapporto con i diritti di accesso di:** anziché ciò che è definito nel filtro con caratteri jolly.
Per ulteriori informazioni sui caratteri jolly per i campi utente, consulta la sezione &quot;Variabili basate su utente&quot; in [Variabili filtro caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Fornire un rapporto con i diritti di accesso di un altro utente

Puoi impostare i rapporti da consegnare come allegati a un’e-mail. Puoi impostare questi rapporti consegnati in modo che vengano visualizzati così come sono per gli utenti con un livello di accesso più elevato, in modo che tutti gli utenti possano vedere le stesse informazioni nei rapporti consegnati. Gli utenti che visualizzeranno il rapporto consegnato nell’e-mail devono essere aggiunti all’elenco Invia a destinatari all’interno della consegna del rapporto. Per ulteriori informazioni sull’impostazione di un rapporto per la consegna, consulta l’articolo [Panoramica sulla consegna dei rapporti](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Per fornire un rapporto con i diritti di accesso di un altro utente:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **Rapporti**.

1. Seleziona il rapporto da consegnare con i diritti di accesso di un altro utente.
1. Fai clic sul nome del rapporto per selezionarlo.
1. Fai clic su **Azioni dei rapporti**.
1. Fai clic su **Invia rapporto**.

1. In **Fornire questo rapporto con i diritti di accesso di:** inizia a digitare il nome dell’utente che desideri visualizzare il rapporto come quando viene inviato in un messaggio e-mail, quindi selezionalo quando lo vedi nell’elenco. Il valore predefinito è il nome dell’utente che crea il rapporto.\
   ![](assets/qs-send-report-access-rights-of-350x446.png)

   >[!NOTE]
   Gli utenti con un livello di accesso inferiore consentito per la generazione di rapporti non possono selezionare un altro utente e quindi se stessi per il **Fornire questo rapporto con i diritti di accesso di:** campo .

1. Seleziona la **Formato** desideri che il rapporto venga visualizzato nell’e-mail:

   * HTML
   * PDF
   * MS Excel
   * MS Excel (.xlsx)
   * TSV

1. Fai clic su **Invia subito** per inviarlo immediatamente.\
   Oppure\
   Fai clic su **Effettuare consegne ripetute** per pianificare una consegna ricorrente per il rapporto.\
   Per ulteriori informazioni sulle consegne dei rapporti, consulta l’articolo [Panoramica sulla consegna dei rapporti](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).