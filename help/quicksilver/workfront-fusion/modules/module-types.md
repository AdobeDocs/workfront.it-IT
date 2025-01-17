---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Tipi di moduli
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 0%

---

# Tipi di moduli

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Panoramica modulo](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/module-overview.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

A[!UICONTROL Adobe Workfront Fusion] distingue cinque tipi di moduli: moduli di azione, moduli di ricerca, moduli di attivazione, aggregatori e iteratori. Aggregatori e Iteratori sono per scenari avanzati.

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
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>Per utilizzare le funzionalità descritte in questo articolo, la tua organizzazione deve acquistare Adobe Workfront Fusion e Adobe Workfront.</td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Moduli di azione

I moduli di azione sono il tipo di modulo più comune. Un modulo di azione tipico restituisce un singolo bundle, che quindi passa al modulo successivo per l’elaborazione.

A differenza dei moduli di attivazione, i moduli di azione possono essere posizionati all’inizio, al centro o alla fine di uno scenario. Gli scenari possono contenere un numero illimitato di moduli di azione.

>[!INFO]
>
>**Esempi:**
>
>* **[!DNL Workfront]> [!UICONTROL Carica un file]** invia un file a [!DNL Workfront] e restituisce il relativo identificatore.
>* **[!UICONTROL Immagine] > [!UICONTROL Ridimensiona]** riceve un&#39;immagine, la ridimensiona in base alle dimensioni specificate e la trasmette all&#39;azione successiva.

Il tipo di azione dispone di quattro sottotipi: Crea, Leggi, Aggiorna ed Elimina. Il sottotipo Update consente le tre operazioni seguenti:

* **Cancellare il contenuto di un campo**. Questa operazione viene eseguita quando il contenuto del campo viene valutato per cancellare la parola chiave (da non confondere con *empty*).

  ![](assets/erase-content-of-field.png)

* **Lasciare invariato il contenuto di un campo**. Questa operazione viene eseguita quando il campo viene lasciato vuoto o il contenuto del campo viene valutato come vuoto (rappresentato da null in JSON).

  ![](assets/leave-content-field-unchanged-350x231.png)

* **Sostituisci il contenuto di un campo**. Questa operazione viene eseguita in tutti gli altri casi diversi da quelli sopra descritti.

>[!NOTE]
>
>* Se non vedi la parola chiave `erase` nel pannello di mappatura, il modulo non è un modulo di aggiornamento o non è stato aggiornato alle specifiche più recenti per l&#39;app.
>* &quot;[!UICONTROL Vuoto]&quot; non modifica il contenuto del campo. Se è necessario cancellare il campo, puoi utilizzare la seguente formula:
>
>![](assets/formula-ifempty-name-erase.png)
>
>Non è attualmente possibile lasciare un campo invariato quando il relativo contenuto viene valutato come vuoto.

## Moduli ricerca

Una ricerca tipica restituisce zero, uno o più bundle, che quindi passano al modulo successivo per l’elaborazione.

È possibile inserire Ricerche all&#39;inizio, al centro o alla fine di uno scenario.

Gli scenari possono contenere un numero illimitato di Ricerche.

>[!INFO]
>
>**Esempio:**
>
>**[!DNL Workfront]> [!UICONTROL Leggi record correlati]** legge i record che corrispondono alla query di ricerca specificata, in un particolare oggetto padre

## Moduli trigger

Gli attivatori generano bundle quando si è verificata una modifica in un determinato servizio. La modifica può consistere nella creazione di nuovi record, nell&#39;eliminazione di record, nell&#39;aggiornamento di record e così via.

Ogni trigger può restituire zero, uno o più bundle che quindi passano al modulo successivo per l’elaborazione.

Gli attivatori possono essere posizionati solo all&#39;inizio di uno scenario.

Ogni scenario può contenere un solo trigger.

[!DNL Workfront Fusion] distingue tra due tipi di trigger: Polling triggers e Instant triggers.

### Trigger di polling

I trigger di polling eseguono regolarmente il polling di un determinato servizio anche se non sono state apportate modifiche rispetto all’esecuzione precedente. È consigliabile pianificare uno scenario contenente un trigger di polling da eseguire a intervalli regolari. Se è presente una *modifica*, il trigger restituisce bundle contenenti informazioni sulla modifica. Se non è presente *change*, il trigger non restituisce alcun bundle. Per istruzioni sulla pianificazione di uno scenario, vedere [Pianificare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

I trigger di polling consentono di selezionare il primo bundle che devono generare tramite il pannello epoca. Il pannello viene visualizzato automaticamente dopo aver salvato un trigger o averne modificato le impostazioni. Per ulteriori informazioni, vedere [Scegliere la posizione di inizio di un modulo trigger in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>Le impostazioni effettuate nel pannello epoca influiscono solo sulla prima esecuzione del modulo. Una volta eseguito, il modulo ricorda l’ultimo bundle di output e annulla le impostazioni effettuate tramite il pannello epoca.

>[!INFO]
>
>**Esempi:**
>
>* **[!DNL Workfront]> [!UICONTROL Osserva record]** restituisce file appena aggiunti dall&#39;ultima esecuzione dello scenario
>
>* **[!DNL Google Sheets]> [!UICONTROL Osserva righe]** restituisce nuove righe aggiunte dall&#39;utente dall&#39;ultima esecuzione dello scenario

### Trigger istantanei

I trigger istantanei consentono al servizio di notificare immediatamente a [!DNL Workfront Fusion] una *modifica*. È consigliabile pianificare uno scenario contenente un trigger istantaneo da eseguire immediatamente. Per istruzioni, consulta [Pianificare uno scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md). Vedi anche [Trigger istantanei (webhook) in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) per informazioni dettagliate sulla gestione dei dati in arrivo.

>[!INFO]
>
>**Esempi:**
>
>* **[!DNL Workfront]> [!UICONTROL Osserva eventi]** restituisce informazioni quando si verifica un determinato tipo di evento in Workfront, ad esempio la creazione di un&#39;attività.
>* **[!DNL Google Sheets]> [!UICONTROL Osserva modifiche]** restituisce informazioni ogni volta che una cella viene aggiornata.

## Aggregatori

Un aggregatore è un tipo di modulo che accumula più bundle in un singolo bundle.

Ogni aggregatore restituisce un solo bundle, che quindi passa al modulo successivo per l’ulteriore elaborazione.

È possibile posizionare gli aggregatori solo nel mezzo di uno scenario.

Gli scenari possono contenere un numero illimitato di aggregatori.

>[!INFO]
>
>**Esempi:**
>
>* **[!UICONTROL Archivia] > [!UICONTROL Crea un archivio]** comprime i file ricevuti in un archivio zip
>* **[!UICONTROL CSV] > [!UICONTROL Aggrega in CSV]** unisce più stringhe da un file CSV in un&#39;unica riga
>* **[!UICONTROL Strumenti] > [!UICONTROL Aggregatore di testo]** combina più stringhe in un&#39;unica stringa

Per ulteriori informazioni, vedere [Modulo Aggregator in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Iteratori

Un iteratore è un tipo di modulo che divide gli array in più bundle separati.

Ogni iteratore restituisce uno o più bundle, che quindi passano al modulo successivo per l’elaborazione.

È possibile posizionare gli iteratori solo nel mezzo di uno scenario.

Gli scenari possono contenere un numero illimitato di iteratori.

>[!INFO]
>
>**Esempio:**
>
>**[!UICONTROL E-mail] > [!UICONTROL Recupera allegati]** suddivide un array di allegati in bundle separati

Per ulteriori informazioni, vedere [Modulo Iterator in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) e [Mappare un array in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
