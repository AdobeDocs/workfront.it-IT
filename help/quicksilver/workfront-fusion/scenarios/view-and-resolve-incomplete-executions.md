---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]
description: La [!UICONTROL Esecuzioni incomplete] La cartella memorizza esecuzioni di scenari che non sono state completate correttamente a causa di un errore. Ciascuna esecuzione incompleta archiviata può essere risolta manualmente o automaticamente.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]

La [!UICONTROL Esecuzioni incomplete] La cartella memorizza esecuzioni di scenari che non sono state completate correttamente a causa di un errore. Ciascuna esecuzione incompleta archiviata può essere risolta manualmente o automaticamente.

>[!NOTE]
>
>Per impostazione predefinita, la memorizzazione delle esecuzioni incomplete è disabilitata. Per abilitarlo, abilita la [!UICONTROL Consenti archiviazione esecuzioni incomplete] nelle impostazioni avanzate dello scenario.
>
>Per ulteriori informazioni sulle impostazioni degli scenari, consulta [Il pannello delle impostazioni dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Visualizza esecuzioni incomplete

Se un modulo rileva un errore durante il suo funzionamento, viene aggiunta una nuova esecuzione incompleta alla cartella esecuzioni incomplete. Ogni esecuzione incompleta contiene il blueprint dello scenario e tutti i bundle che possono essere mappati nel modulo non riuscito. L&#39;elenco delle esecuzioni incomplete può essere aperto facendo clic su [!UICONTROL Esecuzioni incomplete] nella pagina dei dettagli dello scenario:

![](assets/incomplete-executions-tab-350x102.png)

Per ulteriori informazioni, consulta [Errori che si traducono in esecuzioni incomplete](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>Il limite di dimensione corrente della cartella esecuzioni incomplete non risolte per organizzazione è di 500 MB. Se l’organizzazione supera questo limite, potresti visualizzare il seguente errore:
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>Per ulteriori informazioni, consulta [Abilita perdita dati](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) in [Il pannello delle impostazioni dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Risolvere esecuzioni incomplete

Quando viene memorizzata una nuova esecuzione incompleta, è possibile risolverla come segue:

1. Fai clic sul pulsante **[!UICONTROL Esecuzioni incomplete]** scheda .
1. Individua l&#39;esecuzione incompleta da risolvere e fai clic su **[!UICONTROL Dettaglio]**.


   Se desideri visualizzare il registro di tutte le operazioni del modulo prima di tentare di risolvere l’esecuzione incompleta, puoi risolvere l’esecuzione incompleta dal [!UICONTROL Cronologia] cartella:

1. Fai clic sul pulsante **[!UICONTROL Cronologia]** scheda .
1. Individua il registro di esecuzione non riuscito dello scenario e fai clic su **[!UICONTROL Dettagli]**.
1. Apri il registro del modulo in cui vengono visualizzate tutte le operazioni del modulo.
1. Individua l&#39;operazione non riuscita e fai clic su **[!UICONTROL Risolvi]**:

   ![](assets/resolve-btn-350x188.png)

## Opzioni relative alle esecuzioni incomplete

Le seguenti opzioni nel [!UICONTROL Impostazioni dello scenario] Il pannello determina se e come vengono memorizzate le esecuzioni incomplete:

* Consenti archiviazione esecuzioni incomplete
* Elaborazione sequenziale
* Abilita perdita dati

Per ulteriori informazioni su queste opzioni, consulta [Il pannello delle impostazioni dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Errori che si traducono in esecuzioni incomplete

Ci sono diverse categorie di errori che si traducono nella memorizzazione di esecuzioni incomplete. Tali misure possono comprendere:

* Errori di convalida derivanti da dati incompleti o errati, principalmente a causa di un elemento mancante che è previsto per elaborare correttamente tutti i dati che attraversano un modulo.
* Errori derivanti dall&#39;indisponibilità della destinazione finale a causa di un errore temporaneo o di connessione a lungo termine (ad esempio, durante la connessione a un server FTP remoto o via e-mail).

Se si verifica un errore sul primo modulo dello scenario, l&#39;esecuzione si arresta immediatamente e non viene memorizzata alcuna esecuzione incompleta.

Se si verifica un errore su qualsiasi altro modulo e non è collegata alcuna route del gestore di errori, si verifica una delle seguenti situazioni:

* Se il tipo di errore è `ConnectionError`, `RateLimitError`, `OutOfSpaceError` o `ModuleTimeoutError`, viene memorizzato un record di esecuzione incompleto con esecuzione automatica di un nuovo tentativo.
* Se il tipo di errore è `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError`oppure `MaxResultsExceededError`, viene memorizzato un record di esecuzione incompleto senza esecuzione di un nuovo tentativo automatico.
* Se il tipo di errore è diverso da quanto indicato sopra, l’esecuzione non riesce.
