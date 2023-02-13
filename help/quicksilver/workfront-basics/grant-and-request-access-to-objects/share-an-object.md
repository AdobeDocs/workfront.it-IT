---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Condividere un oggetto
description: L’amministratore Adobe Workfront consente agli utenti di visualizzare o modificare gli oggetti quando assegnano i livelli di accesso. Per ulteriori informazioni sulla concessione dell’accesso agli oggetti, vedere Creazione o modifica di livelli di accesso personalizzati.
author: Alina
feature: Get Started with Workfront
exl-id: 27a1beb9-e83a-4ef6-bf5f-ad52575a993c
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 0%

---

# Condividere un oggetto

L’amministratore Adobe Workfront consente agli utenti di visualizzare o modificare gli oggetti quando assegnano i livelli di accesso. Per ulteriori informazioni sulla concessione dell&#39;accesso agli oggetti, vedere [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Oltre al livello di accesso concesso agli utenti, puoi anche concedere loro le autorizzazioni per visualizzare o modificare oggetti specifici creati o con accesso da condividere. Per ulteriori informazioni sui livelli di accesso e le autorizzazioni, consulta [Funzionamento congiunto dei livelli di accesso e delle autorizzazioni](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Le autorizzazioni sono specifiche per un elemento in Workfront e definiscono quali azioni è possibile eseguire su tale elemento.

Per informazioni sulla condivisione delle autorizzazioni sugli oggetti, consulta [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Un amministratore Workfront può aggiungere o rimuovere autorizzazioni per qualsiasi elemento del sistema, per tutti gli utenti, senza esserne il proprietario.

Questo articolo descrive come condividere i seguenti oggetti per i quali la condivisione è identica: 

* Progetti, attività, problemi
* Portfoli, programmi
* Documenti

Per informazioni su come condividere tutti gli altri oggetti in Workfront, consulta anche i seguenti articoli:

* Per i modelli, consulta [Condividere i modelli di progetto](../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Per le bozze, vedi [Condividi una bozza in Workfront Proof](../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).
* Per rapporti, dashboard e calendari, consulta i seguenti articoli:

   * [Condivisione di un rapporto in Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Condivisione di un dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Condivisione di un rapporto calendario](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

   Inoltre, vedi [Condividere rapporti, dashboard e calendari](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md) per informazioni generali sulla condivisione di rapporti, dashboard e calendari. 

* Per filtri, visualizzazioni e raggruppamenti, consulta [Condividere un filtro, una visualizzazione o un raggruppamento](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* Per le cartelle di documenti, vedere [Condivisione di una cartella di documenti](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).
* Per i piani, vedi [Condividere un piano in Planner scenario](../../scenario-planner/share-a-plan.md).

   Questo richiede una licenza aggiuntiva.

* Per gli obiettivi, vedi [Condividere un obiettivo in Obiettivi di Workfront](../../workfront-goals/workfront-goals-settings/share-a-goal.md). Questo richiede una licenza aggiuntiva.

## Requisiti di accesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you want to share</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to the objects you want to share</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Per condividere gli oggetti è necessario disporre dei seguenti elementi:

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
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizza l'accesso o una parte superiore agli oggetti che desideri condividere</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza autorizzazioni o superiore agli oggetti che desideri condividere</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Condividere un singolo oggetto {#share-a-single-object}

1. Passa all&#39;oggetto che desideri condividere.

   Per informazioni sugli oggetti condivisibili, consulta [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
1. Fai clic sul pulsante **Altro** icona ![](assets/more-icon.png)accanto al nome dell’oggetto, quindi fai clic su **Condivisione** o **Condividi.**

   ![](assets/share-a-document-350x160.png)

1. In **Dare `<Object Name>` accesso** inizia a digitare il nome dell’utente, del team, del ruolo, del gruppo o della società con cui desideri condividere l’oggetto, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.

   Ad esempio, se condividi un progetto, utilizza il **Consenti accesso al progetto a** campo .

   >[!TIP]
   >
   >È possibile condividere un oggetto solo con utenti attivi, team, ruoli o aziende.

   ![](assets/nwe-project-sharing-modal-350x456.png)

   >[!TIP]
   >
   >Se hai più entità denominate in modo simile, sono elencate sotto il loro tipo. I nomi delle entità vengono visualizzati in ordine alfabetico. Tuttavia, l’ordine in cui i tipi di entità vengono visualizzati è casuale.
   >
   >
   >![](assets/sharing-entities-named-similarly-in-sharing-box-350x179.png)   >

1. (Facoltativo) Ripetere il passaggio 3 per ogni utente, team, ruolo o gruppo a cui si desidera concedere l’accesso all’oggetto.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: esnure this stays accurate; in the editor it looks like step 4 but one step is conditioned entirely for one version or another)
   </MadCap:conditionalText>
   -->

1. Specifica le autorizzazioni per ogni utente, team, ruolo, gruppo o società aggiunto al passaggio 3 facendo clic sul menu a discesa, quindi seleziona il livello di autorizzazione che desideri concedere.

   Sono disponibili le seguenti opzioni:

   * **Visualizza:** Gli utenti possono esaminare e condividere l’elemento. 
   * **Collaborare****:** Gli utenti possono effettuare aggiornamenti, registrare informazioni, apportare modifiche minori e condividere, oltre a tutte le autorizzazioni di visualizzazione.

      >[!TIP]
      >
      >È possibile concedere autorizzazioni Contribute solo ai seguenti oggetti: 
      * Progetti
      * Attività
      * Problemi


   * **Gestisci:**gli utenti hanno accesso completo all&#39;oggetto senza diritti amministrativi, concessi a livello di accesso, oltre a tutte le autorizzazioni Visualizza e Contribuisci.

      >[!NOTE]
       L’amministratore di Workfront o il creatore di oggetti può rimuovere le autorizzazioni da queste entità.

       

      ![](assets/screen-shot-2013-12-04-at-1.13.11-pm.png)

1. (Facoltativo) Fai clic su **Opzioni avanzate** per configurare autorizzazioni specifiche per l’oggetto.

   Le opzioni di visualizzazione, gestione e Contribute variano a seconda dell&#39;oggetto selezionato.\
   Per ulteriori informazioni sui livelli di autorizzazione, vedi [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

   ![](assets/screen-shot-2013-12-04-at-1.14.11-pm.png)

1. (Facoltativo) Per rendere questo oggetto disponibile a tutti gli utenti del sistema, fare clic sul pulsante **Ingranaggio** icona ![](assets/gear-icon-settings-with-dn-arrow.jpg) , quindi fai clic su nel menu a discesa **Rendere visibile il sistema a livello di sistema**.

   Tutti gli utenti possono visualizzare l’oggetto in base alle autorizzazioni impostate.

1. (Facoltativo e condizionale) Quando condividi un progetto, fai clic sul pulsante **Ingranaggio** icona ![](assets/gear-icon-settings-with-dn-arrow.jpg), quindi fai clic su nel menu a discesa **Imposta come modello di accesso al progetto** per impostare le autorizzazioni come modello.\
   Dopo aver definito le autorizzazioni per un progetto, queste stesse autorizzazioni vengono applicate automaticamente alla successiva creazione di un progetto da zero.

   >[!NOTE]
   Il modello di accesso al progetto sostituisce i valori predefiniti di condivisione concessi dall’amministratore Workfront nel livello di accesso.\
   Per ulteriori informazioni su come specificare le impostazioni predefinite per la condivisione dei progetti a livello di accesso, consulta [Concedere l’accesso ai progetti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md) . >
   <!--   >
   ><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   >
   >(NOTE: (this note also appears in Understanding Project Permissions.))   >
   ></MadCap:conditionalText>   >
   >-->   >


   Puoi specificare le autorizzazioni per i progetti che verranno creati da un modello quando condividi il modello. Per ulteriori informazioni, consulta [Condividere i modelli di progetto](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

1. (Facoltativo) Per rendere l’oggetto pubblico, fare clic su **Rendi pubblico a utenti esterni**.

   >[!TIP]
   Questa opzione non è disponibile per tutti gli oggetti.

   ![](assets/make-public-system-wide-settings-sharing-box-on-document-nwe-350x481.png)

1. (Condizionale) Se l’oggetto è stato reso pubblico a utenti esterni, fai clic su **collegamento copia,** quindi distribuisci il collegamento agli utenti esterni.\
   Tutti gli utenti con il collegamento possono visualizzare l’oggetto.

   >[!CAUTION]
   È consigliabile prestare attenzione quando si condivide con utenti esterni un oggetto contenente informazioni confidenziali. Questo consente loro di visualizzare le informazioni senza essere un utente Workfront o parte dell’organizzazione.

1. Fai clic su **Salva**.

## Condividere oggetti in blocco

Da un elenco di oggetti, è possibile condividere più oggetti contemporaneamente con altri utenti, team, gruppi, ruoli o aziende.

>[!IMPORTANT]
Quando si condividono oggetti in blocco, i nomi delle entità che dispongono delle autorizzazioni per i singoli oggetti non vengono visualizzati. Quando si condividono oggetti in blocco, le entità aggiunte all’elenco di condivisione vengono aggiunte agli oggetti selezionati. Non sovrascrivono le entità associate ai singoli oggetti. 

Per condividere oggetti in blocco:

1. Passare a un elenco di oggetti.
1. Selezionare due o più oggetti nell’elenco.
1. Fai clic sul pulsante **Condividi** icona ![](assets/share-icon.png).\
   Gli utenti che hanno già accesso all’oggetto non sono elencati come disponibili quando si esegue la condivisione in blocco.

   >[!NOTE]
   Se non si dispone delle autorizzazioni necessarie per condividere un oggetto selezionato, la **Condividi** pulsante non visibile.

1. In **Modifica `<Object Name>` accesso** inizia a digitare il nome di un utente, un team, un gruppo, un ruolo o una società a cui si desidera concedere le autorizzazioni.

   Ad esempio, se condividi un progetto, utilizza il **Consenti accesso al progetto** campo .

   ![](assets/share-multiple-projects-people-box-nwe-350x480.png)

1. Continua a condividere gli oggetti selezionati come descritto nei passaggi 4-9 della sezione . [Condividere un singolo oggetto](#share-a-single-object) in questo articolo.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure these steps stay accurate; always look at them in the viewer; because of condiitoning, the steps numbers in the editor are different!!!!!!*****)
   </MadCap:conditionalText>
   -->

1. Fai clic su **Salva**.
