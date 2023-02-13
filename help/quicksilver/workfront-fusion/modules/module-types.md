---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Tipi di moduli
description: "Adobe Workfront Fusion distingue cinque tipi di moduli: moduli di azione, moduli di ricerca, moduli di attivazione, aggregatori e iteratori. Aggregatori e iteratori sono per scenari avanzati."
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 0%

---

# Tipi di moduli

A[!UICONTROL Adobe Workfront Fusion] distingue cinque tipi di moduli: moduli di azione, moduli di ricerca, moduli di attivazione, aggregatori e iteratori. Aggregatori e iteratori sono per scenari avanzati.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>Per utilizzare le funzionalità descritte in questo articolo, la tua organizzazione deve acquistare Adobe Workfront Fusion e Adobe Workfront.</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Moduli di azione

I moduli di azione sono il tipo di modulo più comune. Un modulo di azione tipico restituisce un singolo bundle, che quindi passa al modulo successivo per l&#39;elaborazione.

A differenza dei moduli di attivazione, i moduli di azione possono essere posizionati all’inizio, al centro o alla fine di uno scenario. Gli scenari possono contenere un numero illimitato di moduli di azioni.

>[!INFO]
>
>**Esempi:**
>
>* **[!DNL Workfront]> [!UICONTROL Caricare un file]** invia un file a [!DNL Workfront] e restituisce il relativo identificatore.
>* **[!UICONTROL Immagine] > [!UICONTROL Ridimensiona]** riceve un’immagine, la ridimensiona in base a dimensioni specifiche e passa l’immagine ridimensionata all’azione successiva.


Il tipo Azione dispone di quattro sottotipi: Creare, leggere, aggiornare ed eliminare. Il sottotipo Aggiorna abilita le tre operazioni seguenti:

* **Cancellare il contenuto di un campo**. Questa operazione si verifica quando il contenuto del campo viene valutato per cancellare la parola chiave (da non confondere con *vuoto*).

   ![](assets/erase-content-of-field.png)

* **Lascia invariato il contenuto di un campo**. Questa operazione viene eseguita quando il campo viene lasciato vuoto o il contenuto del campo viene valutato come vuoto (rappresentato tramite null in JSON).

   ![](assets/leave-content-field-unchanged-350x231.png)

* **Sostituire il contenuto di un campo**. Questa operazione si svolge in tutti i casi diversi da quelli sopra descritti.

>[!NOTE]
>
>* Se non visualizzi il `erase` nel pannello di mappatura, il modulo non è un modulo di aggiornamento o non è stato aggiornato alle specifiche più recenti per l’app.
>* &quot;[!UICONTROL Vuoto]&quot; non modifica il contenuto del campo. Se è necessario cancellare il campo, è possibile utilizzare la seguente formula:
>
>![](assets/formula-ifempty-name-erase.png)
>
>Al momento non è possibile lasciare un campo invariato quando il relativo contenuto viene valutato come vuoto.

## Moduli di ricerca

Una ricerca tipica restituisce zero, uno o più bundle, che quindi passano al modulo successivo per l&#39;elaborazione.

È possibile posizionare le ricerche all’inizio, al centro o alla fine di uno scenario.

Gli scenari possono contenere un numero illimitato di ricerche.

>[!INFO]
>
>**Esempio:**
>
>**[!DNL Workfront]> [!UICONTROL Leggi record correlati]**  legge i record che corrispondono alla query di ricerca specificata, in un particolare oggetto principale

## Moduli trigger

I trigger generano bundle quando si verifica una modifica in un determinato servizio. La modifica può consistere nella creazione di nuovi record, nell&#39;eliminazione di un record, nell&#39;aggiornamento di un record e così via.

Ogni trigger può restituire zero, uno o più bundle che poi passano al modulo successivo per l’elaborazione.

Gli attivatori possono essere posizionati solo all’inizio di uno scenario.

Ogni scenario può contenere un solo trigger.

[!DNL Workfront Fusion] distingue tra due tipi di trigger: Trigger di polling e attivatori istantanei.

### Trigger di polling

Il polling attiva regolarmente il polling di un determinato servizio anche se non sono state apportate modifiche dall&#39;esecuzione precedente. È consigliabile pianificare l’esecuzione a intervalli regolari di uno scenario contenente un trigger di polling. Se esiste un *cambiare*, il trigger restituisce i bundle contenenti informazioni sulla modifica. Se non esiste *cambiare*, il trigger non genera alcun bundle. Per istruzioni sulla pianificazione di uno scenario, vedi [Pianifica uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

Gli attivatori di polling consentono di selezionare il primo bundle che devono trasmettere tramite il pannello epoch. Il pannello viene visualizzato automaticamente dopo aver salvato un trigger o modificato le impostazioni di attivazione. Per ulteriori informazioni, consulta [Scegli dove inizia il modulo trigger [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>Le impostazioni effettuate nel pannello epoch influiscono solo sulla prima esecuzione del modulo. Una volta eseguito, il modulo ricorda l’ultimo bundle in uscita e annulla le impostazioni effettuate tramite il pannello epoch.

>[!INFO]
>
>**Esempi:**
>
>* **[!DNL Workfront]> [!UICONTROL Registri di controllo]** restituisce i file appena aggiunti dall’ultima esecuzione dello scenario
>
>* **[!DNL Google Sheets]> [!UICONTROL Righe di controllo]** restituisce nuove righe aggiunte dall’utente dall’ultima esecuzione dello scenario


### Trigger istantanei

Gli attivatori istantanei consentono al servizio di inviare una notifica [!DNL Workfront Fusion] informazioni su *cambiare* immediatamente. È consigliabile pianificare l’esecuzione immediata di uno scenario contenente un trigger istantaneo. Per istruzioni, consulta [Pianificare uno scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md). Vedi anche [Trigger istantanei (webhook) in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) per informazioni dettagliate sulla gestione dei dati in arrivo.

>[!INFO]
>
>**Esempi:**
>
>* **[!DNL Workfront]> [!UICONTROL Eventi di controllo]** restituisce informazioni quando si verifica un determinato tipo di evento in Workfront, ad esempio la creazione di un&#39;attività.
>* **[!DNL Google Sheets]> [!UICONTROL Modifiche di controllo]** restituisce informazioni ogni volta che una cella viene aggiornata.


## Aggregatori

Un Aggregator è un tipo di modulo che accumula più bundle in un unico bundle.

Ogni Aggregator restituisce un solo bundle, che quindi passa al modulo successivo per un&#39;ulteriore elaborazione.

È possibile posizionare Aggregatori solo nel mezzo di uno scenario.

Gli scenari possono contenere un numero illimitato di aggregatori.

>[!INFO]
>
>**Esempi:**
>
>* **[!UICONTROL Archivia] > [!UICONTROL Creare un archivio]** comprime i file ricevuti in un archivio zip
>* **[!UICONTROL CSV] > [!UICONTROL Aggregazione in CSV]** unisce più stringhe da un file CSV in una singola riga
>* **[!UICONTROL Strumenti] > [!UICONTROL Aggregatore di testo]** combina più stringhe in un&#39;unica stringa


Per ulteriori informazioni, consulta [Modulo Aggregator in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Iteratori

Un iteratore è un tipo di modulo che divide gli array in più bundle separati.

Ogni iteratore restituisce uno o più bundle, che quindi passano al modulo successivo per l&#39;elaborazione.

È possibile posizionare gli iteratori solo nel mezzo di uno scenario.

Gli scenari possono contenere un numero illimitato di iteratori.

>[!INFO]
>
>**Esempio:**
>
>**[!UICONTROL E-mail] > [!UICONTROL Recupera allegati]** interrompe un array di allegati in bundle separati

Per ulteriori informazioni, consulta [Modulo iteratore in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) e [Mappare un array in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
