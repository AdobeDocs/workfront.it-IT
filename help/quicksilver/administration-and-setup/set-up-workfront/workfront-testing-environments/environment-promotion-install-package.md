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
source-git-commit: 610469811a937fde70a938af829b156e69cca391
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---

# Installare un pacchetto di promozione dell’ambiente


1. Passa all’ambiente in cui desideri installare il pacchetto. Ambiente in cui si stanno copiando gli oggetti **a**.
1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **[!UICONTROL Configurazione]** ![Icona Configurazione](/help/_includes/assets/gear-icon-setup.png).
1. Seleziona **Sistema** nel menu di navigazione a sinistra, seleziona quindi **Promozione dell&#39;ambiente**.
1. Seleziona il pacchetto dall’elenco visualizzato.
1. Per installare il pacchetto, fai clic su **Installa** in alto a destra.
1. Mappare ogni oggetto del pacchetto all&#39;oggetto corrispondente nell&#39;ambiente di destinazione.

   Per ulteriori informazioni, consulta [Mappatura](#mapping) in questo articolo


## Mappatura

Ogni tipo di oggetto è elencato nella barra di navigazione a sinistra e su una scheda. Nella scheda vengono visualizzati gli oggetti di quel tipo e se tali oggetti esistono nell’ambiente di destinazione. È possibile determinare come questi oggetti verranno spostati nell&#39;ambiente di destinazione.

* Crea nuovo: crea un nuovo oggetto nell’ambiente di destinazione. Se l&#39;oggetto esiste nell&#39;ambiente di destinazione, è possibile creare un nuovo oggetto con un nuovo nome. Se non esiste nell&#39;ambiente di destinazione, è possibile creare l&#39;oggetto con un nuovo nome o con il nome che l&#39;oggetto ha nel pacchetto.
* Usa esistente: l&#39;oggetto nel pacchetto non è installato e l&#39;oggetto già esistente nell&#39;ambiente di destinazione rimane invariato.
* Sovrascrivi esistente: (non attualmente disponibile) L’oggetto nel pacchetto sostituisce l’oggetto esistente nell’ambiente di destinazione.
* Do not use: l&#39;oggetto nel pacchetto non è installato nell&#39;ambiente di destinazione. Se si seleziona Non utilizzare, verrà visualizzato un messaggio di errore che descrive in dettaglio l&#39;effetto di questa scelta su altri oggetti o campi.

I valori predefiniti sono `Create new` se l’oggetto non esiste nell’ambiente di destinazione, e `Use existing` se l’oggetto esiste nell’ambiente di destinazione. Per ripristinare la mappatura predefinita, fai clic su **Ripristina mappatura predefinita**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
