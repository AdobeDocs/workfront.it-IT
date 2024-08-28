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
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: e9df34c206dd65ccc2edec00087248eb4ed16f54
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# Creare o modificare un pacchetto di promozione dell’ambiente

È necessario creare un pacchetto nell&#39;ambiente da cui copiare gli oggetti **da**. Ad esempio, se configuri un progetto nell’ambiente Sandbox di aggiornamento personalizzato e lo promuovi nell’ambiente di produzione, devi creare il pacchetto nell’ambiente Sandbox di aggiornamento personalizzato.

>[!IMPORTANT]
>
>Se la Sandbox di aggiornamento personalizzata viene aggiornata durante la configurazione dell’oggetto per la promozione dell’ambiente, tale configurazione andrà persa con l’aggiornamento. È consigliabile non aggiornare la Sandbox di aggiornamento personalizzata a meno che tutti gli oggetti e i pacchetti di promozione dell’ambiente in sospeso non siano stati promossi correttamente.

## Requisiti di accesso

Devi avere i seguenti:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] piano</strong>
   </td>
   <td> Prime o Ultimate (solo per i nuovi piani)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenze</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Configurazioni del livello di accesso
   </td>
   <td>Devi essere un amministratore [!DNL Workfront].
   </td>
  </tr>
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Creare un pacchetto

1. Passa all’ambiente in cui desideri creare il pacchetto. Questo è l&#39;ambiente dal quale si stanno copiando gli oggetti **da**.
1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic sull&#39;icona **[!UICONTROL Setup]** ![Setup](/help/_includes/assets/gear-icon-setup.png).
1. Seleziona **Sistema** nell&#39;area di navigazione a sinistra, quindi seleziona **Promozione ambiente**.
1. Fare clic su **Crea pacchetto**.

   Viene visualizzata la pagina Nuovo pacchetto promozione.

1. Nel campo **Nome pacchetto** immettere un nome per il pacchetto.
1. Nel campo **Descrizione** immettere una descrizione per il pacchetto.
1. Per aggiungere un oggetto al pacchetto, fare clic su **Aggiungi oggetti** nel menu di navigazione a sinistra e selezionare il tipo di oggetto che si desidera aggiungere.
1. Selezionare uno o più oggetti dall&#39;elenco oppure digitare il nome nella barra di ricerca e selezionare l&#39;oggetto quando viene visualizzato nell&#39;elenco. È possibile selezionare più oggetti nell&#39;elenco.
1. Fare clic su **Aggiungi (X oggetti)** per aggiungere gli oggetti selezionati al pacchetto.

   >[!INFO]
   >
   >**Esempio**
   >
   >Se hai selezionato tre progetti da aggiungere al progetto, il pulsante indica **Aggiungi 3 progetti**.

   Gli oggetti aggiunti vengono visualizzati nell&#39;area Contenuto package a destra della pagina.

1. Per aggiungere un altro tipo di oggetto, ripetere i passaggi 7-9.
1. (Facoltativo) Per rimuovere un oggetto dal package, posizionare il cursore del mouse sull&#39;oggetto nell&#39;area Contenuto package, quindi fare clic sulla X accanto all&#39;oggetto.
1. Dopo aver aggiunto tutti gli oggetti desiderati al pacchetto, fare clic su **Salva e chiudi** per salvare il pacchetto senza assemblarlo.

   Oppure

   Fare clic su **Salva e assembla** per salvare e assemblare il pacchetto.

   >[!NOTE]
   >
   >* I pulsanti Salva e Chiudi e Salva e Assembla sono disponibili se un pacchetto contiene un nome composto da cinque o più caratteri e almeno un oggetto aggiunto.
   >* Non è possibile assemblare un pacchetto in uno stato installabile, ad esempio Testing o Active.

## Modificare o assemblare un pacchetto esistente

1. Passa all’ambiente in cui desideri creare il pacchetto. Questo è l&#39;ambiente dal quale si stanno copiando gli oggetti **da**.
1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic sull&#39;icona **[!UICONTROL Setup]** ![Setup](/help/_includes/assets/gear-icon-setup.png).
1. Seleziona **Sistema** nell&#39;area di navigazione a sinistra, quindi seleziona **Promozione ambiente**.
1. Seleziona il pacchetto dall’elenco visualizzato.
1. (Condizionale) Per visualizzare i pacchetti disabilitati, abilita l&#39;opzione **Mostra pacchetti ritirati**.
1. (Facoltativo) Per visualizzare il contenuto, inclusi tutti gli oggetti e i relativi oggetti secondari, fare clic sulla freccia a discesa accanto al tipo di oggetto nella sezione **Contents**.
1. (Facoltativo) Per visualizzare le installazioni precedenti e i tentativi di installazione di questo pacchetto, fare clic su **Distribuzioni**.
1. (Facoltativo) Per modificare il pacchetto, fare clic su **Modifica pacchetto** in alto a destra nella schermata.
1. Per installare il pacchetto, fare clic su **Installa** in alto a destra.

   Per istruzioni sull&#39;installazione di un pacchetto, vedere [Installare un pacchetto di promozione dell&#39;ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).
