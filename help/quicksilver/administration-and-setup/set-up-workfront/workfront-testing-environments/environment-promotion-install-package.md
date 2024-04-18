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
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: 92a7a2df142d7736417b903949a5a667cff53913
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# Installare un pacchetto di promozione dell’ambiente

>[!NOTE]
>
>Per installare un pacchetto, devi aver effettuato l’accesso all’ambiente in cui desideri installare il pacchetto. Ambiente in cui si stanno copiando gli oggetti **a**.

1. Passa all’ambiente in cui desideri installare il pacchetto.
1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **[!UICONTROL Configurazione]** ![Icona Configurazione](/help/_includes/assets/gear-icon-setup.png).
1. Seleziona **Sistema** nel menu di navigazione a sinistra, seleziona quindi **Promozione dell&#39;ambiente**.
1. Seleziona il pacchetto dall’elenco visualizzato.
1. Per ogni oggetto che presenta una collisione, selezionare la modalità di risoluzione della collisione.

   Per risolvere una collisione, fare clic sulla freccia a discesa accanto al tipo di oggetto e selezionare l&#39;azione che si desidera eseguire.

   Per ulteriori informazioni, consulta [Conflitti](#collisions) in questo articolo
1. Per distribuire il pacchetto nel nuovo ambiente, fai clic su **Distribuisci** in alto a destra.

## Conflitti

Si verificano conflitti quando un oggetto che fa parte del pacchetto di installazione ha lo stesso nome di un oggetto già esistente nell&#39;ambiente di destinazione. In questo caso, potete selezionare la modalità di risoluzione della collisione. Le collisioni vengono risolte a livello di oggetto.

Puoi visualizzare le collisioni facendo clic sul menu a discesa accanto a ciascun tipo di oggetto. Le collisioni vengono visualizzate nella colonna Collisione.

Per risolvere un conflitto, selezionare un&#39;azione nella colonna Azione di distribuzione oppure utilizzare l&#39;azione predefinita già visualizzata.

* **Crea con nuovo nome**: crea un nuovo oggetto nell’ambiente di destinazione. Se l&#39;oggetto esiste nell&#39;ambiente di destinazione, è possibile creare un nuovo oggetto con un nuovo nome. Se non esiste nell&#39;ambiente di destinazione, è possibile creare l&#39;oggetto con un nuovo nome o con il nome che l&#39;oggetto ha nel pacchetto.
* **Usa esistente**: l’oggetto nel pacchetto non è installato e l’oggetto già esistente nell’ambiente di destinazione rimane invariato.
* **Sovrascrivere**: l’oggetto nel pacchetto sostituisce l’oggetto esistente nell’ambiente di destinazione.

  È inoltre possibile scegliere gli oggetti da sovrascrivere anche se non viene rilevata una collisione.

  Per informazioni dettagliate su come la sovrascrittura influisce sugli oggetti padre e figlio, vedere
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

I valori predefiniti sono `Create new` se l’oggetto non esiste nell’ambiente di destinazione, e `Use existing` se l’oggetto esiste nell’ambiente di destinazione. Per ripristinare la mappatura predefinita, fai clic su **Ripristina mappatura predefinita**.

## Sovrascrittura di oggetti padre e figlio

Alcuni oggetti nel pacchetto di promozione possono avere oggetti secondari. Ad esempio, un progetto (padre) ha delle attività (figli). Quando si sovrascrive un oggetto padre, gli oggetti figlio vengono gestiti come segue:

* Gli oggetti secondari presenti sia nel pacchetto che nella destinazione verranno aggiornati nella destinazione in modo che corrispondano al pacchetto.
* Verranno creati oggetti secondari che esistono nel pacchetto ma non nella destinazione.
* Gli oggetti secondari presenti nella destinazione ma non nel pacchetto rimarranno invariati.

Questa funzionalità ha effetto sui seguenti oggetti padre e figlio:

| Oggetto padre | Oggetti secondari |
|---|---|
| Progetto | Attività<br>QueueDef (definizione coda)<br>RoutingRule |
| Modello | TemplateTask<br>QueueDef (definizione coda)<br>RoutingRule |
| Parametro (campo modulo personalizzato) | ParameterOption (opzione campo modulo personalizzato) |
| InformazioniCalendario | CalendarSection |
| QueueDef (definizione coda) | GruppoArgomentiCoda<br>Argomento coda |

