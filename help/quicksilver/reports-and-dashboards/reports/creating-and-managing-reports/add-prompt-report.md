---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Aggiungere una richiesta a un report
description: I filtri e i prompt sono simili in quanto limitano la quantità di informazioni visualizzate in un report.
author: Nolan
feature: Reports and Dashboards
exl-id: b4058fb3-7360-474f-8be1-1c6b584749b0
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1251'
ht-degree: 0%

---

# Aggiungere una richiesta a un report

## Differenza tra prompt e filtri

I filtri e i prompt sono simili in quanto limitano la quantità di informazioni visualizzate in un report.

Creare un filtro quando si desidera che le informazioni visualizzate nel report vengano filtrate in base agli stessi criteri ogni volta che si esegue il report. I filtri vengono generati una volta e sono inseriti direttamente nel rapporto. Per ulteriori informazioni sulla creazione di filtri, consulta l’articolo [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

I prompt sono filtri aperti che possono essere personalizzati e applicati in modo diverso ogni volta che si esegue un report.

Quando si aggiungono prompt al report, è possibile personalizzare le informazioni di filtro modificando i criteri di prompt ogni volta che si esegue il report. Il rapporto viene eseguito ogni volta con un filtro diverso, a seconda dei modificatori scelti, anziché codificarli una sola volta nel filtro del rapporto.

I prompt fungono da filtro personalizzabile per i report che possono essere aggiornati immediatamente prima dell&#39;esecuzione del report. È possibile creare rapporti generici e quindi restringere i risultati in base alle informazioni che si desidera visualizzare per quel giorno o alle informazioni rilevanti per un insieme di criteri specifici. Ad esempio, se si dispone di un rapporto Ore e si desidera modificare le informazioni del rapporto in base ai seguenti criteri:

* Le date in cui le ore sono state registrate
* Gli utenti che hanno inserito le ore
* Quantità di ore immesse

Si creano tre prompt in cui le condizioni sono i criteri richiesti e il rapporto apparirà diverso ogni volta che lo si esegue, in base alle informazioni scelte per i prompt.

Un filtro può indicare ad Adobe Workfront di visualizzare solo le ore inserite tra giugno e agosto di quest’anno. Tuttavia, se viene visualizzato un messaggio, è possibile utilizzare un intervallo di tempo diverso ogni volta che si esegue il rapporto, ad esempio tra gennaio e febbraio oppure tra ottobre e dicembre.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario creare un report prima di aggiungervi un prompt.

Per istruzioni sulla creazione di un rapporto, consulta [Creare un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)

## Crea un prompt

1. Passare al report in cui si desidera aggiungere un prompt.
1. Espandi **Azioni report** e quindi fare clic su **Modifica**.

1. Clic **Impostazioni dei rapporti**.
1. In **Prompt dei report** , fare clic su **Aggiungi una richiesta**.\
   ![](assets/qs-add-a-prompt-350x216.png)

1. (Condizionale) Seleziona il campo su cui desideri basare il prompt. Inizia a digitare il nome del campo e fai clic su per selezionarlo quando viene visualizzato nell’elenco.\
   Le opzioni disponibili per gli utenti che eseguono il rapporto variano a seconda del campo selezionato.\
   Ad esempio, se si seleziona un campo data, ad esempio Data di completamento effettiva in un report attività, &quot;Data di completamento effettiva&quot; è il nome del prompt. Quando modifichi questo prompt durante l’esecuzione del report, puoi scegliere da un set di modificatori per creare l’istruzione di filtro. Questo processo è identico alla creazione di un filtro. Per ulteriori informazioni sui modificatori, consulta [Modificatori di filtri e condizioni](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Condizionale) Fai clic su **Prompt personalizzato** per creare un prompt personalizzato.

   Un prompt personalizzato è un prompt predefinito in cui è necessario codificare i criteri di filtro prima di eseguire il report. In questo senso, un prompt personalizzato è più simile a un filtro che a un prompt.

   Tuttavia, il prompt rimane flessibile come un prompt normale perché puoi scegliere tra diverse istruzioni predefinite, invece di avere un solo filtro hardcoded nel rapporto.

   Specificare le seguenti informazioni per il prompt personalizzato: La condizione di un prompt personalizzato può essere modificata solo utilizzando la modalità testo. Questo consente di applicare più condizioni in un singolo campo.

   * **Nome campo:** Questo è il nome del prompt visualizzato prima dell&#39;esecuzione del report.
   * **Etichetta:** Questo è il nome di una delle opzioni all&#39;interno del prompt visualizzato prima di eseguire il report.
   * **Condizione:** Immetti una condizione che definisca il prompt.

   Utilizza la stessa sintassi che utilizzeresti quando inserisci un filtro in modalità testo e unisci le istruzioni con &quot;&amp;&quot;. Per ulteriori informazioni sulla modifica di un filtro in modalità testo, consulta [Modificare un filtro utilizzando la modalità testo](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

   Ad esempio, il **Condizione** del prompt personalizzato per i seguenti scenari potrebbe essere simile al seguente:

   * tutte le attività su progetti futuri in cui lo stato del progetto è Idea, Richiesto, Pianificato e Corrente:

     ```
     project:plannedStartDate=$$TODAY&project:plannedStartDate_Mod=gte&project:status=IDA,REQ,PLN,CUR&project:status_Mod=in
     ```

   * tutte le attività nei progetti completati (passati) in cui lo stato del progetto è Completato o Inattivo:

     ```
     project:actualCompletionDate=$$TODAY&project:actualCompletionDate_Mod=lte&project:status=CPL,DED&project:status_Mod=in
     ```

   Per ulteriori informazioni sui modificatori della modalità testo, vedere [Modificatori di filtri e condizioni](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Non è possibile modificare le condizioni di un prompt personalizzato quando si esegue il report, come si farebbe con un prompt standard. Per un prompt personalizzato è possibile impostare tutte le condizioni predefinite necessarie.

1. (Facoltativo) Ripetete il passo 4 o il passo 5 per creare tutte le richieste necessarie.
1. Clic **Fine**, quindi fai clic su **Salva+Chiudi** per salvare il rapporto.

## Applicare un prompt a un report

Quando si aggiunge un prompt a un report, la scheda predefinita del report è sempre la scheda Prompts.

Per eseguire un report con un prompt:

1. Vai al report con il prompt.

   ![](assets/qs-prompt-drop-downs-350x229.png)

1. Scegli una condizione per uno o tutti i prompt visualizzati sul **Prompt** scheda.\
   (Facoltativo) Puoi lasciare vuoti i prompt e non filtrare il rapporto in base alle condizioni dei prompt.

1. Fai clic su **Esegui rapporto**.\
   (Condizionale) Se hai popolato i prompt, il rapporto viene filtrato in base alle condizioni scelte per i prompt.\
   (Condizionale) Se hai lasciato vuoti i prompt, il rapporto non viene filtrato in base alle condizioni dei prompt. Il rapporto viene visualizzato come se non fosse filtrato.

   >[!NOTE]
   >
   >Un report che contiene un filtro oltre a un prompt filtra i risultati in base ai criteri definiti nel filtro e al prompt combinato.

## Limitazioni della condivisione dei rapporti richiesti

>[!CAUTION]
>
>Quando condividi un rapporto richiesto all’esterno di Workfront, l’utente che lo visualizza deve aver effettuato l’accesso a Workfront per eseguire il rapporto utilizzando il prompt. Se l’utente che visualizza il rapporto non ha effettuato l’accesso, tutti i risultati del rapporto vengono visualizzati senza applicare il prompt.

Di seguito sono riportate le limitazioni relative alla condivisione dei rapporti richiesti da Workfront:

* Quando si condivide un report pubblicamente, gli utenti non possono eseguirlo applicando il prompt, a meno che non dispongano delle credenziali di Workfront e accedano prima per visualizzare il report in Workfront.

  Per ulteriori informazioni sulla condivisione dei rapporti, consulta l’articolo [Condividere un rapporto in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
* Quando pianifichi la consegna di un rapporto richiesto, il rapporto nell’allegato e-mail include i dati del rapporto omesso. Quando l’utente fa clic sul collegamento nell’e-mail per accedere al rapporto, deve prima accedere per visualizzare il rapporto ed eseguire personalmente il prompt.

  Per informazioni sulla programmazione di un rapporto consegnato, vedere [Pianificare la consegna automatica dei rapporti](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).
