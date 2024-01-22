---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: Rimuovere le autorizzazioni dagli oggetti
description: È possibile rimuovere le autorizzazioni di altri utenti per gli oggetti a cui si ha accesso Condividi. La rimozione delle autorizzazioni dagli oggetti è identica per tutti gli oggetti condivisibili.
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 0%

---

# Rimuovere le autorizzazioni dagli oggetti

<!--Audited: 01/2024-->

È possibile rimuovere le autorizzazioni di altri utenti per gli oggetti a cui si ha accesso Condividi. La rimozione delle autorizzazioni dagli oggetti è identica per tutti gli oggetti condivisibili.

Considerazioni simili a quelle relative alla condivisione degli oggetti vengono applicate per la rimozione delle autorizzazioni dagli oggetti. Per ulteriori informazioni, consulta la sezione [Considerazioni sulla condivisione degli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) nell’articolo [Panoramica delle autorizzazioni di condivisione sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

## Requisiti di accesso

Per condividere gli oggetti, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Workfront*</td> 
   <td> <p>Nuova licenza: Collaboratore o versione successiva</p>
   Oppure  
   <p>Licenza corrente: richiesta o successiva</p>
   <p><b>NOTA</b></p>

<p>Alcuni oggetti richiedono un accesso più elevato rispetto a Richiedi. </p>

<p>Ad esempio, per la nuova licenza, un collaboratore può condividere i problemi, ma solo gli utenti con licenza Standard possono condividere un progetto.</p>

<p>Per la licenza corrente, un richiedente può condividere i problemi, ma solo i lavoratori o i responsabili della pianificazione possono condividere un progetto.</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore agli oggetti da condividere</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni o versioni successive per gli oggetti da condividere</p> <p>Gestire le autorizzazioni per rimuovere le autorizzazioni ereditate per gli oggetti</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront. Per ulteriori informazioni, consulta [Requisiti di accesso alla documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Rimuovere le entità dall&#39;elenco di condivisione di un oggetto {#remove-entities-from-the-sharing-list-of-an-object}

È possibile rimuovere entità (utenti, mansioni, team, gruppi, aziende) dall&#39;elenco di condivisione di un oggetto. In questo modo vengono rimosse le relative autorizzazioni per l’oggetto.

1. Passare all&#39;oggetto da cui si desidera rimuovere le autorizzazioni.

   Per informazioni sugli oggetti che possono essere condivisi, vedi [Panoramica delle autorizzazioni di condivisione sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Condizionale) Per programmi, portfolio e documenti, effettua le seguenti operazioni:

   1. Fai clic su **Altro** icona ![](assets/more-icon.png)accanto al nome dell&#39;oggetto, quindi fare clic su **Condivisione** o **Condividi.**

      ![](assets/share-a-document-350x160.png)

   1. Fai clic su **x** accanto al nome di un utente, team, gruppo, società, ruolo per rimuoverli nella casella accesso agli oggetti.

      ![](assets/remove-permissions-on-portfolio.png)

   1. In **L&#39;accesso Workfront di &lt; Nome utente > verrà rimosso da questo** selezionare se si desidera che il relativo accesso venga rimosso solo dall&#39;oggetto selezionato o da tutti gli oggetti figlio associati.

1. (Condizionale) Per progetti, attività e problemi, effettua le seguenti operazioni:

   1. Clic **Condividi** a destra del nome dell&#39;oggetto.

      ![](assets/new-share-button.png)
   1. Individuare l&#39;utente, la mansione, il team, il gruppo o l&#39;azienda che si desidera rimuovere dall&#39;oggetto.
   1. Clic **Rimuovi**.
In **Rimuovi &lt; Nome utente > da** selezionare se si desidera che il relativo accesso venga rimosso solo dall&#39;oggetto selezionato o da tutti gli oggetti figlio associati.

      ![](assets/remove-permissions-on-project-nwe-350x479.png)

   Esistono i seguenti scenari:

   * Se rimuovi l’entità solo dall’oggetto, tale entità perde le relative autorizzazioni sull’oggetto e le autorizzazioni ereditate sugli oggetti secondari. Se in precedenza erano state concesse autorizzazioni per gli elementi figlio singolarmente, quando si seleziona questa opzione manterranno le stesse autorizzazioni per tutti gli oggetti figlio associati.
   * Se si rimuove l&#39;entità dall&#39;oggetto e da tutti gli oggetti figlio, tale entità perde le relative autorizzazioni per l&#39;oggetto e per tutti gli oggetti figlio, anche quando in precedenza era stata concessa loro un&#39;autorizzazione individuale per ciascun oggetto figlio.

1. Fai clic su **Salva**.

## Rimozione in blocco delle autorizzazioni da più oggetti

È possibile rimuovere entità (utenti, mansioni, team, gruppi, aziende) da più oggetti contemporaneamente quando li si seleziona in blocco in un elenco.

>[!NOTE]
>
>Non è possibile visualizzare le entità di accesso disponibili per tutti gli oggetti selezionati quando vengono selezionati in blocco. Prima di rimuovere le relative autorizzazioni, è necessario sapere quale entità si desidera rimuovere dalla condivisione degli oggetti selezionati.

1. Passare all&#39;elenco di oggetti che si desidera condividere.

   Per informazioni sugli oggetti che possono essere condivisi, vedi [Panoramica delle autorizzazioni di condivisione sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Seleziona diversi oggetti nell’elenco, quindi fai clic su **Condividi** icona ![](assets/share-icon.png)nella parte superiore dell’elenco.
1. Digitare il nome dell&#39;utente, del ruolo, del team, del gruppo o della società per cui si desidera rimuovere l&#39;accesso in **Modifica `<Object Name>` accesso a** campo.
1. Dal menu a discesa Accesso, seleziona **Nessun accesso**.

   ![](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. In `<User Name>`L&#39;accesso a Workfront verrà rimosso da questo menu a discesa, selezionare se si desidera che l&#39;accesso venga rimosso solo dagli oggetti selezionati o da tutti gli altri oggetti secondari associati.\
   Esistono i seguenti scenari:

   * Se rimuovi l’entità solo dall’oggetto, tale entità perde le relative autorizzazioni sull’oggetto e le autorizzazioni ereditate sugli oggetti secondari. Se in precedenza erano state concesse autorizzazioni per gli elementi figlio singolarmente, quando si seleziona questa opzione manterranno le stesse autorizzazioni per tutti gli oggetti figlio associati. 
   * Se si rimuove l&#39;entità dall&#39;oggetto e da tutti gli oggetti figlio, tale entità perde le relative autorizzazioni per l&#39;oggetto e per tutti gli oggetti figlio, anche quando in precedenza era stata concessa loro un&#39;autorizzazione individuale per ciascun oggetto figlio.

   **Esempio:** Seleziona se rimuovere le autorizzazioni solo per le attività selezionate in un elenco o per i problemi e i documenti allegati alle attività.

   ![](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. (Facoltativo) Per modificare le autorizzazioni in blocco per più oggetti, selezionare un altro livello di condivisione per l&#39;entità selezionata.

   Se ad esempio dispongono delle autorizzazioni Gestione, selezionate Contribute o Visualizza.

1. Fai clic su **Salva**.

## Rimuovi autorizzazioni ereditate

Le autorizzazioni ereditate possono essere rimosse dagli oggetti consentendo ai proprietari di identificare in modo specifico chi avrà accesso agli oggetti figlio indipendentemente dall&#39;accesso di un utente a un oggetto padre.

>[!IMPORTANT]
>
>Solo gli utenti con l&#39;autorizzazione Gestione possono rimuovere le autorizzazioni ereditate.

Per rimuovere le autorizzazioni ereditate:

1. Passare a un oggetto per il quale si dispone delle autorizzazioni di gestione. Ad esempio, passare a un&#39;attività.
1. Passare alla casella di accesso agli oggetti come descritto nella [Rimuovere le entità dall&#39;elenco di condivisione di un oggetto](#remove-entities-from-the-sharing-list-of-an-object) in questo articolo.
1. Seleziona la **x** accanto a **Autorizzazione ereditata** nella casella di condivisione per rimuovere tutti gli utenti elencati.

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

   In questo modo, per impostazione predefinita, nessuno a cui sono state concesse le autorizzazioni per l&#39;oggetto padre, ad esempio il progetto, dispone delle autorizzazioni per questa attività. Per concedere le autorizzazioni per l&#39;attività, è necessario elencare singole entità nell&#39;elenco di condivisione dell&#39;attività.

   >[!TIP]
   >
   >Non è possibile rimuovere singole entità dall&#39;elenco Autorizzazioni ereditate. È possibile disabilitare le autorizzazioni ereditate solo per tutte le entità elencate.

1. Clic **Salva**. 

## Rendere privato un oggetto

Se un oggetto è stato condiviso a livello di sistema o se è stato condiviso con utenti esterni rendendolo pubblico, è possibile renderlo nuovamente privato rimuovendo le autorizzazioni pubbliche o a livello di sistema. 

Per ulteriori informazioni su come rendere un oggetto disponibile a livello di sistema o pubblicamente, vedere [Condividere un oggetto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

Per rendere privato un oggetto:

1. Passare all&#39;oggetto che si desidera rendere privato.\
   Ad esempio, passa a un rapporto.
1. Clic **Azioni report**, quindi **Condivisione**.

   ![](assets/report-permissions-make-private-nwe-350x477.png)

1. Clic **Rimuovi accesso pubblico** per rimuovere l’accesso degli utenti esterni alla visualizzazione del rapporto.
1. Clic **Rimuovi l&#39;accesso a livello di sistema** per interrompere la condivisione con tutti gli utenti di Workfront. 
1. Fai clic su **Salva**.
