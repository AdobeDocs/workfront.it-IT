---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Installare un pacchetto di promozione dell’ambiente
description: La funzionalità di promozione dell’ambiente ha lo scopo di consentire lo spostamento di oggetti correlati alla configurazione da un ambiente all’altro. Scopri come installare un pacchetto di promozione dell’ambiente in un ambiente di destinazione.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Installare un pacchetto di promozione dell’ambiente

Dopo aver creato un pacchetto, puoi installarlo in un ambiente diverso.

È necessario installare un pacchetto nell&#39;ambiente in cui si desidera copiare gli oggetti da **a**. Ad esempio, se configuri un progetto nell’ambiente Sandbox di aggiornamento personalizzato e lo promuovi nell’ambiente di produzione, devi installare il pacchetto nell’ambiente di produzione.

>[!IMPORTANT]
>
>* Se la Sandbox di aggiornamento personalizzata viene aggiornata durante la configurazione dell’oggetto per la promozione dell’ambiente, tale configurazione andrà persa con l’aggiornamento. È consigliabile non aggiornare la Sandbox di aggiornamento personalizzata a meno che tutti gli oggetti e i pacchetti di promozione dell’ambiente in sospeso non siano stati promossi correttamente.
>* Gli oggetti creati nell&#39;ambiente di destinazione come parte dell&#39;installazione del pacchetto **not** hanno lo stesso ID dell&#39;oggetto nell&#39;ambiente originale. Ciò è dovuto al fatto che gli ID vengono assegnati dal sistema al momento della creazione degli oggetti.

## Requisiti di accesso

Devi avere i seguenti:

<table>
  <tr>
   <td>Pacchetto Adobe Workfront
   </td>
   <td> <p>PRIME o ULTIMATE</p>
   </td>
  </tr>
  <tr>
   <td><strong>Licenze Workfront</strong>
   </td>
   <td> <p>Standard</p>&gt;
   </td>
  </tr>
   <tr>
   <td>Configurazioni del livello di accesso
   </td>
   <td><p>Devi essere un amministratore di Workfront.</p>
   </td>
  </tr>
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisiti

È necessario creare un pacchetto di promozione dell’ambiente prima di installarlo.

Per istruzioni, vedere [Creare o modificare un pacchetto di promozione dell&#39;ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md).

## Stato del pacchetto per l&#39;installazione

Per poter essere installato nell’ambiente di produzione, un pacchetto deve trovarsi nello stato ATTIVO.

Per testare il pacchetto, è consigliabile spostarlo sullo stato TEST e installarlo in un’altra sandbox.  Se il test ha esito positivo, senza errori, sposta il pacchetto in ACTIVE per installarlo nell’ambiente di produzione.

Per modificare lo stato di un pacchetto:

1. Selezionare il pacchetto come descritto in [Modificare o assemblare un pacchetto esistente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package) nell&#39;articolo Creare e modificare pacchetti di promozione dell&#39;ambiente.
1. Fare clic su **Modifica pacchetto**.
1. Fai clic su **Stato**.
1. Seleziona lo stato desiderato dal menu a discesa.

Per ulteriori informazioni sugli stati, vedere [Stati di promozione dell&#39;ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) nell&#39;articolo Panoramica sullo spostamento di oggetti tra ambienti Workfront.

## Installare un pacchetto

>[!NOTE]
>
>* Per installare un pacchetto, devi aver effettuato l’accesso all’ambiente in cui desideri installare il pacchetto. Questo è l&#39;ambiente in cui si stanno copiando gli oggetti da **a**.

1. Passa all’ambiente in cui desideri installare il pacchetto.
1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic sull&#39;icona **[!UICONTROL Setup]** ![Setup](/help/_includes/assets/gear-icon-setup.png).
1. Seleziona **Sistema** nell&#39;area di navigazione a sinistra, quindi seleziona **Promozione ambiente**.
1. Seleziona il pacchetto dall’elenco visualizzato.
1. Per ogni oggetto che presenta una collisione, selezionare la modalità di risoluzione della collisione.

   Per risolvere una collisione, fare clic sulla freccia a discesa accanto al tipo di oggetto e selezionare l&#39;azione che si desidera eseguire.

   Per ulteriori informazioni, vedi [Conflitti](#collisions) in questo articolo
1. Per distribuire il pacchetto nel nuovo ambiente, fare clic su **Distribuisci** in alto a destra.

## Conflitti

Una collisione è un oggetto presente nell&#39;ambiente di destinazione di un&#39;installazione che corrisponde a uno degli oggetti installati dall&#39;ambiente di origine. Le collisioni vengono rilevate confrontando i nomi e gli ID degli oggetti di origine con gli oggetti nell&#39;ambiente di destinazione. Le collisioni vengono rilevate anche confrontando gli oggetti di origine con i record di oggetti installati in precedenza.

Quando si verifica una collisione, è possibile selezionare la modalità di risoluzione della collisione. Le collisioni vengono risolte a livello di oggetto.

È possibile visualizzare i conflitti facendo clic sul menu a discesa accanto a ciascun tipo di oggetto. Le collisioni vengono visualizzate nella colonna Collisione.

>[!NOTE]
>
>È possibile che i conflitti rilevati non siano gli oggetti che si desidera ignorare o utilizzare nell&#39;installazione. Si consiglia di convalidare le collisioni rilevate per garantire che le destinazioni di installazione siano corrette.

Per risolvere un conflitto, selezionare un&#39;azione nella colonna Azione di distribuzione oppure utilizzare l&#39;azione predefinita già visualizzata.

* **Crea con nuovo nome**: crea un nuovo oggetto nell&#39;ambiente di destinazione. Se l&#39;oggetto esiste nell&#39;ambiente di destinazione, è possibile creare un nuovo oggetto con un nuovo nome. Se non esiste nell&#39;ambiente di destinazione, è possibile creare l&#39;oggetto con un nuovo nome o con il nome che l&#39;oggetto ha nel pacchetto.
* **Usa esistente**: l&#39;oggetto nel pacchetto non è installato e l&#39;oggetto già esistente nell&#39;ambiente di destinazione non è stato modificato.
* **Sovrascrivi**: l&#39;oggetto nel pacchetto sostituisce l&#39;oggetto esistente nell&#39;ambiente di destinazione.

  È inoltre possibile scegliere gli oggetti da sovrascrivere anche se non viene rilevata una collisione.

  Per informazioni dettagliate su come la sovrascrittura influisce sugli oggetti padre e figlio, vedere [Sovrascrittura degli oggetti padre e figlio](#overwriting-parent-and-child-objects) in questo articolo.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

I valori predefiniti sono `Create new` se l&#39;oggetto non esiste nell&#39;ambiente di destinazione e `Use existing` se l&#39;oggetto esiste nell&#39;ambiente di destinazione. Per ripristinare il mapping predefinito, fare clic su **Ripristina mapping predefinito**.

## Sovrascrittura di oggetti padre e figlio

Alcuni oggetti nel pacchetto di promozione possono avere oggetti secondari. Ad esempio, un progetto (padre) ha delle attività (figli). Quando si sovrascrive un oggetto padre, gli oggetti figlio vengono gestiti come segue:

* Gli oggetti secondari presenti sia nel pacchetto che nella destinazione verranno aggiornati nella destinazione in modo che corrispondano al pacchetto.
* Verranno creati oggetti secondari che esistono nel pacchetto ma non nella destinazione.
* Gli oggetti secondari presenti nella destinazione ma non nel pacchetto rimarranno invariati.

Questa funzionalità ha effetto sui seguenti oggetti padre e figlio:

| Oggetto padre | Oggetti secondari |
|---|---|
| Progetto | Task<br>QueueDef (definizione coda)<br>RoutingRule |
| Modello | TemplateTask<br>QueueDef (definizione coda)<br>RoutingRule |
| Parametro (campo modulo personalizzato) | ParameterOption (opzione campo modulo personalizzato) |
| InformazioniCalendario | CalendarSection |
| QueueDef (definizione coda) | QueueTopicGroup<br>ArgomentoCoda |

