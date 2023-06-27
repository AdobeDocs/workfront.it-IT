---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Tipi di moduli
description: "Adobe Workfront Fusion distingue cinque tipi di moduli: moduli di azione, moduli di ricerca, moduli di attivazione, aggregatori e iteratori. Aggregatori e Iteratori sono per scenari avanzati."
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 0%

---

# Tipi di moduli

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
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>Per utilizzare le funzionalità descritte in questo articolo, la tua organizzazione deve acquistare Adobe Workfront Fusion e Adobe Workfront.</td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Moduli di azione

I moduli di azione sono il tipo di modulo più comune. Un modulo di azione tipico restituisce un singolo bundle, che quindi passa al modulo successivo per l’elaborazione.

A differenza dei moduli di attivazione, i moduli di azione possono essere posizionati all’inizio, al centro o alla fine di uno scenario. Gli scenari possono contenere un numero illimitato di moduli di azione.

>[!INFO]
>
>**Esempi:**
>
>* **[!DNL Workfront]> [!UICONTROL Carica un file]** invia un file a [!DNL Workfront] e restituisce il relativo identificatore.
>* **[!UICONTROL Immagine] > [!UICONTROL Ridimensiona]** riceve un&#39;immagine, la ridimensiona alle dimensioni specificate e la passa all&#39;azione successiva.

Il tipo di azione dispone di quattro sottotipi: Crea, Leggi, Aggiorna ed Elimina. Il sottotipo Update consente le tre operazioni seguenti:

* **Cancellare il contenuto di un campo**. Questa operazione ha luogo quando il contenuto del campo viene valutato per cancellare la parola chiave (da non confondere con *vuoto*).

  ![](assets/erase-content-of-field.png)

* **Lascia invariato il contenuto di un campo**. Questa operazione viene eseguita quando il campo viene lasciato vuoto o il contenuto del campo viene valutato come vuoto (rappresentato da null in JSON).

  ![](assets/leave-content-field-unchanged-350x231.png)

* **Sostituire il contenuto di un campo**. Questa operazione viene eseguita in tutti gli altri casi diversi da quelli sopra descritti.

>[!NOTE]
>
>* Se non vede il `erase` parola chiave nel pannello di mappatura, il modulo non è un modulo di aggiornamento o non è stato aggiornato alle specifiche più recenti per l’app.
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
>**[!DNL Workfront]> [!UICONTROL Leggi record correlati]**  legge i record corrispondenti alla query di ricerca specificata, in un particolare oggetto padre

## Moduli di attivazione

Gli attivatori generano bundle quando si è verificata una modifica in un determinato servizio. La modifica può consistere nella creazione di nuovi record, nell&#39;eliminazione di record, nell&#39;aggiornamento di record e così via.

Ogni trigger può restituire zero, uno o più bundle che quindi passano al modulo successivo per l’elaborazione.

Gli attivatori possono essere posizionati solo all&#39;inizio di uno scenario.

Ogni scenario può contenere un solo trigger.

[!DNL Workfront Fusion] distingue tra due tipi di trigger: Polling triggers e Instant triggers.

### Trigger di polling

I trigger di polling eseguono regolarmente il polling di un determinato servizio anche se non sono state apportate modifiche rispetto all’esecuzione precedente. È consigliabile pianificare uno scenario contenente un trigger di polling da eseguire a intervalli regolari. Se è presente un *modifica*, il trigger restituisce bundle contenenti informazioni sulla modifica. In caso contrario *modifica*, il trigger non restituisce alcun bundle. Per istruzioni sulla pianificazione di uno scenario, consulta [Pianificare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

I trigger di polling consentono di selezionare il primo bundle che devono generare tramite il pannello epoca. Il pannello viene visualizzato automaticamente dopo aver salvato un trigger o averne modificato le impostazioni. Per ulteriori informazioni, consulta [Scegli da dove inizia un modulo trigger [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>Le impostazioni effettuate nel pannello epoca influiscono solo sulla prima esecuzione del modulo. Una volta eseguito, il modulo ricorda l’ultimo bundle di output e annulla le impostazioni effettuate tramite il pannello epoca.

>[!INFO]
>
>**Esempi:**
>
>* **[!DNL Workfront]> [!UICONTROL Osserva i record]** restituisce i file appena aggiunti dall&#39;ultima esecuzione dello scenario
>
>* **[!DNL Google Sheets]> [!UICONTROL Righe di controllo]** restituisce nuove righe aggiunte dall’utente dall’ultima esecuzione dello scenario

### Trigger istantanei

I trigger istantanei consentono al servizio di notificare [!DNL Workfront Fusion] circa un *modifica* immediatamente. È consigliabile pianificare uno scenario contenente un trigger istantaneo da eseguire immediatamente. Per istruzioni, consulta [Pianificazione di uno scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md). Vedi anche [Trigger istantanei (webhook) in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) per informazioni dettagliate sulla gestione dei dati in arrivo.

>[!INFO]
>
>**Esempi:**
>
>* **[!DNL Workfront]> [!UICONTROL Guarda gli eventi]** restituisce informazioni quando si verifica un determinato tipo di evento in Workfront, ad esempio la creazione di un&#39;attività.
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
>* **[!UICONTROL Archivia] > [!UICONTROL Creare un archivio]** comprime i file ricevuti in un archivio zip
>* **[!UICONTROL CSV] > [!UICONTROL Aggrega in CSV]** unisce più stringhe da un file CSV in un’unica riga
>* **[!UICONTROL Strumenti] > [!UICONTROL Aggregatore di testo]** combina più stringhe in un&#39;unica stringa

Per ulteriori informazioni, consulta [Modulo aggregatore in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

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

Per ulteriori informazioni, consulta [Modulo iteratore in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) e [Mappare un array in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
