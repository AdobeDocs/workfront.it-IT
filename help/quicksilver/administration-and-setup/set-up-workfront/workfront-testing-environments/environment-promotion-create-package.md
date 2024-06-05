---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Creare o modificare un pacchetto di promozione dell’ambiente
description: La funzionalità di promozione dell’ambiente ha lo scopo di consentire lo spostamento di oggetti correlati alla configurazione da un ambiente all’altro. Scopri come creare un pacchetto di promozione dell’ambiente da installare in un altro ambiente.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: e03573640fd8af9c811cef4cf176cc4f37d757fc
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 0%

---

# Creare o modificare un pacchetto di promozione dell’ambiente

È necessario creare un pacchetto nell&#39;ambiente in cui copiare gli oggetti **da**. Ad esempio, se configuri un progetto nell’ambiente Sandbox di aggiornamento personalizzato e lo promuovi nell’ambiente di produzione, devi creare il pacchetto nell’ambiente Sandbox di aggiornamento personalizzato.

>[!IMPORTANT]
>
>Se la Sandbox di aggiornamento personalizzata viene aggiornata durante la configurazione dell’oggetto per la promozione dell’ambiente, tale configurazione andrà persa con l’aggiornamento. È consigliabile non aggiornare la Sandbox di aggiornamento personalizzata a meno che tutti gli oggetti e i pacchetti di promozione dell’ambiente in sospeso non siano stati promossi correttamente.

## Creare un pacchetto

1. Passa all’ambiente in cui desideri creare il pacchetto. Ambiente in cui si stanno copiando gli oggetti **da**.
1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **[!UICONTROL Configurazione]** ![Icona Configurazione](/help/_includes/assets/gear-icon-setup.png).
1. Seleziona **Sistema** nel menu di navigazione a sinistra, seleziona quindi **Promozione dell&#39;ambiente**.
1. Clic **Crea pacchetto**.

   Viene visualizzata la pagina Nuovo pacchetto promozione.

1. In **Nome pacchetto** immettere un nome per il pacchetto.
1. In **Descrizione** immettere una descrizione per il package.
1. Per aggiungere un oggetto al pacchetto, fare clic su **Aggiungi oggetti** nel menu di navigazione a sinistra e seleziona il tipo di oggetto da aggiungere.
1. Selezionare uno o più oggetti dall&#39;elenco oppure digitare il nome nella barra di ricerca e selezionare l&#39;oggetto quando viene visualizzato nell&#39;elenco. È possibile selezionare più oggetti nell&#39;elenco.
1. Clic **Aggiungi (oggetti X)** per aggiungere gli oggetti selezionati al pacchetto.

   >[!INFO]
   >
   >**Esempio**
   >
   >Se hai selezionato tre progetti da aggiungere al progetto, il pulsante mostra **Aggiungi 3 progetti**.

   Gli oggetti aggiunti vengono visualizzati nell&#39;area Contenuto package a destra della pagina.

1. Per aggiungere un altro tipo di oggetto, ripetere i passaggi 7-9.
1. (Facoltativo) Per rimuovere un oggetto dal package, posizionare il cursore del mouse sull&#39;oggetto nell&#39;area Contenuto package, quindi fare clic sulla X accanto all&#39;oggetto.
1. Dopo aver aggiunto tutti gli oggetti desiderati al pacchetto, fare clic su **Salva e chiudi** per salvare il pacchetto senza assemblarlo.

   Oppure

   Clic **Salva e assembla** per salvare e assemblare il pacchetto.

   >[!NOTE]
   >
   >* I pulsanti Salva e Chiudi e Salva e Assembla sono disponibili se un pacchetto contiene un nome composto da cinque o più caratteri e almeno un oggetto aggiunto.
   >* Non è possibile assemblare un pacchetto in uno stato installabile, ad esempio Testing o Active.

## Modificare o assemblare un pacchetto esistente

1. Passa all’ambiente in cui desideri creare il pacchetto. Ambiente in cui si stanno copiando gli oggetti **da**.
1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **[!UICONTROL Configurazione]** ![Icona Configurazione](/help/_includes/assets/gear-icon-setup.png).
1. Seleziona **Sistema** nel menu di navigazione a sinistra, seleziona quindi **Promozione dell&#39;ambiente**.
1. Seleziona il pacchetto dall’elenco visualizzato.
1. (Condizionale) Per visualizzare i pacchetti disabilitati, abilita **Mostra pacchetti ritirati** opzione.
1. (Facoltativo) Per visualizzare il contenuto, inclusi tutti gli oggetti e i relativi oggetti secondari, fare clic sulla freccia dell&#39;elenco a discesa accanto al tipo di oggetto nella **Sommario** sezione.
1. (Facoltativo) Per visualizzare le installazioni precedenti e i tentativi di installazione del pacchetto, fare clic su **Distribuzioni**.
1. (Facoltativo) Per modificare il pacchetto, fai clic su **Modifica pacchetto** in alto a destra.
1. Per installare il pacchetto, fai clic su **Installa** in alto a destra.

   Per istruzioni sull’installazione di un pacchetto, consulta [Installare un pacchetto di promozione dell’ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).
