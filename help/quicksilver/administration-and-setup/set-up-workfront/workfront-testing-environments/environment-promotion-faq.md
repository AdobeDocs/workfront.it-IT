---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Domande frequenti sulla promozione dell’ambiente
description: Esplora le domande frequenti sulla promozione dell’ambiente Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e9794262-80cc-4641-a5c6-7130cf008ba2
source-git-commit: 4ea4d7d8fd16d4c4d7c2fe5f7adb15c2b44b6705
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 3%

---

# Domande frequenti sulla promozione dell’ambiente

Di seguito sono riportate le domande frequenti sulla promozione dell’ambiente:

## È supportata la promozione tra più domini?

### Risposta

La promozione dell’ambiente tra più domini non è attualmente supportata. Devi promuovere tra ambienti dello stesso dominio.

## Adobe Business Platform/IMS è un prerequisito per la promozione dell’ambiente?

### Risposta

No. La promozione dell’ambiente è disponibile sia per le istanze di Workfront IMS che per quelle non-IMS.

## Come possiamo sapere se la nostra istanza di Workfront è su licenza Prime o Ultimate?

### Risposta

* Un amministratore Workfront può individuare la licenza dell’organizzazione.

   1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic sull&#39;icona **[!UICONTROL Setup]** ![Setup](/help/_includes/assets/gear-icon-setup.png).
   1. Fai clic su **Sistema** nel pannello a sinistra
   1. Per visualizzare il piano Workfront, selezionare **Licenze**.
Il piano viene visualizzato nell’angolo superiore destro della pagina.
      ![](assets/locate-plan.png)

  Oppure
* Contatta il rappresentante del tuo account Workfront.

## La promozione ambientale è bidirezionale?

### Risposta

Sì. Ad esempio, puoi passare da Sandox a Produzione, oppure da Produzione a Sandbox.

## La condivisione è supportata?

### Risposta

No, la condivisione non è attualmente supportata.

## Il rollback del pacchetto è disponibile?

### Risposta

Il rollback del pacchetto è disponibile per il pacchetto più recente, entro 24 ore dall’installazione del pacchetto.

## Sarà possibile saltare la promozione dei singoli componenti? Dove sono presenti le opzioni `Use Existing`, `Overwrite` e `Save with a new Name`&quot;, è possibile aggiungere `Skip` in modo da saltare la promozione dei singoli parametri?

### Risposta


* &quot;Usa esistente&quot; equivale a &quot;ignorare&quot; o &quot;ignorare&quot; la distribuzione, perché viene mappato sull’oggetto esistente nell’ambiente di destinazione e non apporta modifiche.
* Per ignorare gli oggetti, si consiglia di rimuovere
tutti gli oggetti che non desideri installare dal pacchetto di promozione o direttamente dall’ambiente di origine. Dopo aver rimosso gli oggetti, riassemblate il pacchetto.
