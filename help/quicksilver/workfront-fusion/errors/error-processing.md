---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Errore di elaborazione in [!DNL Adobe Workfront Fusion]
description: A volte può verificarsi un errore durante l’esecuzione di uno scenario. In genere questo accade se un servizio non è disponibile a causa di un errore di connessione a un servizio o se una convalida non riesce. Questo articolo illustra gli errori comuni che potresti riscontrare.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: 184033c8957e955b3011f7e0845a73029f6b7aba
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Errore di elaborazione in [!DNL Adobe Workfront Fusion]

A volte può verificarsi un errore durante l’esecuzione di uno scenario. In genere questo accade se un servizio non è disponibile a causa di un errore di connessione a un servizio o se una convalida non riesce. Questo articolo illustra gli errori comuni che potresti riscontrare.

[!DNL Adobe Workfront Fusion] distingue tra diversi tipi di errore di base. La risposta varia a seconda del tipo di errore che si è verificato.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Errore di connessione

`ConnectionError`

L&#39;errore di connessione è uno degli errori più comuni solitamente causati dall&#39;indisponibilità del servizio di terze parti per vari motivi (sovraccarico, manutenzione, interruzione e così via). La gestione predefinita di questo errore dipende dal modulo su cui è stato rilevato:

* Se l&#39;errore si verifica sul primo modulo, l&#39;esecuzione dello scenario viene terminata con un messaggio di avviso. [!DNL Workfront Fusion] quindi tenta ripetutamente di ripetere lo scenario a intervalli di tempo crescenti (questi sono spiegati di seguito). Se tutti i tentativi falliscono, [!DNL Workfront Fusion] disattiva lo scenario.
* Se l’errore di connessione si verifica su un altro modulo rispetto al primo, i passaggi successivi dipendono dal [Consenti archiviazione esecuzioni incomplete](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) nelle impostazioni avanzate dello scenario:

   * Se questa opzione è abilitata, l’esecuzione dello scenario viene spostata nella [!UICONTROL Esecuzioni incomplete] cartella in cui [!DNL Workfront Fusion] tenta ripetutamente di ripetere lo scenario a intervalli di tempo crescenti. Se tutti i tentativi non riescono, l’esecuzione rimarrà nella cartella esecuzioni incomplete in attesa di risoluzione manuale da parte dell’utente.

      Per ulteriori informazioni sulle esecuzioni incomplete, vedi [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).
   * Se questa opzione è disabilitata, l’esecuzione dello scenario termina con un errore seguito da una fase di rollback. [!DNL Workfront Fusion] quindi tenta ripetutamente di ripetere lo scenario a intervalli di tempo crescenti. Se tutti i tentativi falliscono, [!DNL Workfront Fusion] disattiva lo scenario.

### Aumento degli intervalli di tempo

L’algoritmo di un aumento moltiplicativo degli intervalli di tempo tra i tentativi in cui si verifica un errore è noto come backoff esponenziale. Gli intervalli di tempo crescenti sono fissati come segue:

1. 10 minuti
1. 1 ora
1. 3 ore
1. 12 ore
1. 24 ore

Il motivo principale dell&#39;impiego degli intervalli di tempo crescenti in [!DNL Workfront Fusion] è per evitare che gli scenari eseguiti di frequente utilizzino operazioni in caso di tentativi non riusciti ripetutamente.

>[!INFO]
>
>**Esempio:**
>
>Uno scenario contiene [!DNL Google Sheets] attivare [!UICONTROL Righe di controllo]. [!DNL Google Sheets] non è disponibile per 30 minuti a causa di manutenzione quando [!DNL Workfront Fusion] avvia lo scenario, quindi non è in grado di recuperare nuove righe. Lo scenario si arresta e prova di nuovo tra 10 minuti. Perché [!DNL Google Sheets] non è ancora disponibile, [!DNL Workfront Fusion] non è ancora in grado di ottenere informazioni sulle nuove righe. L&#39;esecuzione successiva dello scenario è pianificata tra 1 ora. [!DNL Google Sheets] è disponibile di nuovo in questo momento e lo scenario viene eseguito correttamente.

## Errore dati

`DataError`

Viene generato un errore di dati quando un elemento non è mappato correttamente e non supera la convalida eseguita sul [!DNL Workfront Fusion] lato o lato del servizio di terze parti utilizzato.

Se si verifica questo errore, lo scenario, fino al punto in cui il modulo non è riuscito, viene spostato nella cartella esecuzioni incomplete in cui è possibile risolvere il problema. Tuttavia, lo scenario non si interrompe e continua a funzionare in base alla sua pianificazione. Per interrompere l&#39;esecuzione dello scenario quando viene visualizzato l&#39;errore Dati, abilita l&#39;opzione di elaborazione sequenziale nel pannello Impostazioni Scenario.

Se non hai abilitato la [!UICONTROL Consenti archiviazione esecuzioni incomplete] nelle impostazioni dello scenario, l&#39;esecuzione dello scenario termina con l&#39;errore e viene eseguito un rollback.

Per ulteriori informazioni sulla mappatura, vedi [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

Per informazioni sulle esecuzioni incomplete, vedi [Visualizzare e risolvere le esecuzioni incomplete in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Per informazioni sul pannello di impostazione dello scenario, vedi [Pannello delle impostazioni dello scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Per informazioni sulle pianificazioni, consulta [Pianificare uno scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Errore di dati duplicati

`DuplicateDataError`

Se [!DNL Workfront Fusion] tenta di inserire due volte lo stesso bundle in un servizio che non consente dati duplicati, viene generato un errore di dati duplicati. Se si verifica questo errore, [!DNL Workfront Fusion] procede come per l’errore di dati.

## Errore token di accesso non valido

`InvalidAccessTokenError`

Errore token di accesso non valido quando [!DNL Workfront Fusion] impossibile accedere all&#39;account registrato con un servizio di terze parti. Questo di solito accade quando revochi i diritti di accesso per [!DNL Workfront Fusion] nella gestione di un determinato servizio, ma gli scenari correlati continuano a funzionare secondo la pianificazione.

Se si verifica questo errore, l&#39;esecuzione di uno scenario viene interrotta immediatamente. Il resto dello scenario che inizia dal modulo in cui si è verificato l’errore viene spostato nella cartella esecuzioni incomplete.

Per informazioni sulle esecuzioni incomplete, vedi [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Errore limite velocità

`RateLimitError`

Se viene superato un limite impostato da un determinato servizio, viene generato un errore di limite di tasso. Se si verifica questo errore, [!DNL Workfront Fusion] procede come per l&#39;errore di connessione.

Per ulteriori informazioni, consulta [Errore di connessione](#connection-error).

## Errore dati incompleto

`IncompleteDataError`

Un errore di dati incompleto si verifica solo con i trigger. Questo errore viene generato se un trigger non riesce a scaricare i dati richiesti da un determinato servizio.

Se uno scenario termina con il `IncompleteDataError`, il suo ulteriore comportamento dipenderà dalla sua impostazione [!UICONTROL Numero massimo di errori consecutivi].

Per ulteriori informazioni, consulta [Numero di errori consecutivi](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) nell&#39;articolo [Pannello delle impostazioni dello scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Esempio:**
>
>Uno scenario ha [!DNL Workfront] attivare [!UICONTROL Registra] impostato per controllare i documenti. Lo scenario viene eseguito durante il caricamento di un documento di grandi dimensioni, ad esempio un video lungo. Perché [!UICONTROL Workfront Fusion] tenta di scaricare il video mentre è ancora in fase di caricamento in Workfront, lo scenario termina con `IncompleteDataError`.

## Errore di esecuzione

`RuntimeError`

Se durante l’esecuzione dello scenario viene visualizzato un altro errore (non menzionato sopra), viene riportato come `RunTimeError`.

Se uno scenario termina con il `RuntimeError`, il suo ulteriore comportamento dipenderà dalla sua impostazione [!UICONTROL Numero massimo di errori consecutivi]. Per ulteriori informazioni, consulta [Numero di errori consecutivi](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) nell&#39;articolo [Pannello delle impostazioni dello scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>Se uno scenario inizia con un trigger immediato, l&#39;impostazione di [!UICONTROL Numero massimo di errori consecutivi] viene ignorato e lo scenario viene disattivato immediatamente dopo il primo errore. Per ulteriori informazioni, consulta [Trigger istantanei](../../workfront-fusion/modules/module-types.md#instant) nell&#39;articolo [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

## Errore di incoerenza

`InconsistencyError`

Se durante la fase di commit o rollback si verifica un errore descritto sopra, lo scenario si interrompe con un errore di incoerenza. Per ulteriori informazioni, consulta [Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Se questo errore appare in uno scenario, l&#39;esecuzione dello scenario viene immediatamente interrotta.

## Avvertenza

Durante l&#39;esecuzione di uno scenario, potresti ricevere un avviso che ti informa di un problema. Tuttavia, non impedisce il completamento dello scenario.

Ad esempio, è possibile visualizzare un avviso quando viene superata la dimensione massima consentita del file e la [!UICONTROL Abilita perdita dati] è disabilitata. Per ulteriori informazioni, consulta [Abilita perdita dati](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) nell&#39;articolo [Pannello delle impostazioni dello scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
