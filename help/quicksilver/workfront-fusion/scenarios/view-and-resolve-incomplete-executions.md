---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]
description: Il [!UICONTROL Esecuzioni incomplete] La cartella archivia le esecuzioni dello scenario che non sono state finalizzate correttamente a causa di un errore. Ogni esecuzione incompleta archiviata può essere risolta manualmente o automaticamente.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]

Il [!UICONTROL Esecuzioni incomplete] La cartella archivia le esecuzioni dello scenario che non sono state finalizzate correttamente a causa di un errore. Ogni esecuzione incompleta archiviata può essere risolta manualmente o automaticamente.

>[!NOTE]
>
>Per impostazione predefinita, la memorizzazione di esecuzioni incomplete è disabilitata. Per abilitarlo, abilita [!UICONTROL Consenti l’archiviazione di esecuzioni incomplete] nelle impostazioni avanzate.
>
>Per ulteriori informazioni sulle impostazioni dello scenario, consulta [Il pannello delle impostazioni dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!DNL Pro] o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Visualizzare le esecuzioni incomplete

Se un modulo rileva un errore durante l’operazione, viene aggiunta una nuova esecuzione incompleta alla cartella Esecuzioni incomplete. Ogni esecuzione incompleta contiene il blueprint dello scenario e tutti i bundle che possono essere mappati nel modulo non riuscito. L’elenco delle esecuzioni incomplete può essere aperto facendo clic sul pulsante [!UICONTROL Esecuzioni incomplete] nella pagina dei dettagli dello scenario:

![](assets/incomplete-executions-tab-350x102.png)

Per ulteriori informazioni, consulta [Errori risultanti in esecuzioni incomplete](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>Il limite di dimensione corrente della cartella esecuzioni incomplete non risolte per organizzazione è di 500 MB. Se l’organizzazione supera questo limite, è possibile che venga visualizzato il seguente errore:
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>Per ulteriori informazioni, consulta [Abilita perdita di dati](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) in [Il pannello delle impostazioni dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Risolvere le esecuzioni incomplete

Quando viene memorizzata una nuova esecuzione incompleta, è possibile risolverla come segue:

1. Fai clic su **[!UICONTROL Esecuzioni incomplete]** scheda.
1. Individua l’esecuzione incompleta da risolvere e fai clic su **[!UICONTROL Dettaglio]**.


   Se desideri visualizzare il registro di tutte le operazioni del modulo prima di tentare di risolvere l’esecuzione incompleta, puoi risolverla da [!UICONTROL Cronologia] cartella:

1. Fai clic su **[!UICONTROL Cronologia]** scheda.
1. Individua il registro di esecuzione dello scenario non riuscito e fai clic su **[!UICONTROL Dettagli]**.
1. Apri il registro del modulo in cui vengono visualizzate tutte le operazioni del modulo.
1. Individuare l&#39;operazione non riuscita e fare clic su **[!UICONTROL Risolvi]**:

   ![](assets/resolve-btn-350x188.png)

## Opzioni relative alle esecuzioni incomplete

Le seguenti opzioni in [!UICONTROL Impostazioni scenario] Il pannello determina se e come vengono memorizzate le esecuzioni incomplete:

* Consenti l’archiviazione di esecuzioni incomplete
* Elaborazione sequenziale
* Abilita perdita di dati

Per ulteriori informazioni su queste opzioni, vedi [Il pannello delle impostazioni dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Errori risultanti in esecuzioni incomplete

Esistono diverse categorie di errori che si traducono nella memorizzazione di esecuzioni incomplete. Questi possono includere:

* Errori di convalida derivanti da dati incompleti o errati, principalmente a causa di un elemento mancante previsto per elaborare correttamente tutti i dati che passano attraverso un modulo.
* Errori che si verificano dall’indisponibilità della destinazione finale a causa di un errore di connessione temporaneo o a lungo termine (ad esempio, durante la connessione a un server e-mail o FTP remoto).

Se si verifica un errore nel primo modulo dello scenario, l’esecuzione viene interrotta immediatamente e non viene memorizzata alcuna esecuzione incompleta.

Se si verifica un errore in un altro modulo e non è collegata alcuna route del gestore degli errori, si verifica una delle seguenti situazioni:

* Se il tipo di errore è `ConnectionError`, `RateLimitError`, `OutOfSpaceError` o `ModuleTimeoutError`, viene memorizzato un record di esecuzione incompleto con un nuovo tentativo automatico.
* Se il tipo di errore è `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError`, o `MaxResultsExceededError`, viene memorizzato un record di esecuzione incompleto senza un nuovo tentativo automatico.
* Se il tipo di errore è diverso da quello riportato sopra, l’esecuzione non riesce.
