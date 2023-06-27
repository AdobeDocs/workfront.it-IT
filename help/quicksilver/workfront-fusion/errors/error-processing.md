---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Errore di elaborazione in [!DNL Adobe Workfront Fusion]
description: A volte può verificarsi un errore durante l’esecuzione di uno scenario. Ciò si verifica in genere se un servizio non è disponibile a causa di un errore di connessione a un servizio o se una convalida non riesce. In questo articolo vengono descritti gli errori comuni che possono verificarsi.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1238'
ht-degree: 0%

---

# Errore di elaborazione in [!DNL Adobe Workfront Fusion]

A volte può verificarsi un errore durante l’esecuzione di uno scenario. Ciò si verifica in genere se un servizio non è disponibile a causa di un errore di connessione a un servizio o se una convalida non riesce. In questo articolo vengono descritti gli errori comuni che possono verificarsi.

[!DNL Adobe Workfront Fusion] distingue tra diversi tipi di errore di base. Reagirà in modo diverso a seconda del tipo di errore che si è verificato.

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
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Errore di connessione

`ConnectionError`

L’errore di connessione è uno degli errori più comuni, in genere causato dall’indisponibilità del servizio di terze parti per vari motivi (sovraccarico, manutenzione, interruzione e così via). La gestione predefinita di questo errore dipende dal modulo in cui è stato rilevato:

* Se l’errore si verifica sul primo modulo, l’esecuzione dello scenario viene terminata con un messaggio di avviso. [!DNL Workfront Fusion] quindi tenta ripetutamente di eseguire nuovamente lo scenario a intervalli di tempo crescenti (descritti di seguito). Se tutti i tentativi falliscono, [!DNL Workfront Fusion] disattiva lo scenario.
* Se l’errore di connessione si verifica su un modulo diverso dal primo, i passaggi successivi dipendono dal [Consenti l’archiviazione di esecuzioni incomplete](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) nelle impostazioni avanzate dello scenario:

   * Se questa opzione è abilitata, l’esecuzione dello scenario viene spostata nel [!UICONTROL Esecuzioni incomplete] cartella in cui [!DNL Workfront Fusion] tenta ripetutamente di eseguire nuovamente lo scenario a intervalli di tempo crescenti. Se tutti i tentativi non vanno a buon fine, l’esecuzione rimarrà nella cartella Esecuzioni incomplete in attesa della risoluzione manuale da parte dell’utente.

     Per ulteriori informazioni sulle esecuzioni incomplete, vedi [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).
   * Se questa opzione è disabilitata, l’esecuzione dello scenario termina con un errore seguito da una fase di rollback. [!DNL Workfront Fusion] quindi tenta ripetutamente di eseguire di nuovo lo scenario a intervalli di tempo crescenti. Se tutti i tentativi falliscono, [!DNL Workfront Fusion] disattiva lo scenario.

### Aumento degli intervalli di tempo

L&#39;algoritmo di aumento moltiplicativo degli intervalli di tempo tra i tentativi quando si verifica un errore è noto come backoff esponenziale. Gli intervalli di tempo crescenti vengono impostati come segue:

1. 10 minuti
1. 1 ora
1. 3 ore
1. 12 ore
1. 24 ore

La ragione principale per cui si utilizzano gli intervalli di tempo crescenti in [!DNL Workfront Fusion] impedisce che gli scenari eseguiti di frequente utilizzino operazioni su tentativi ripetutamente non riusciti.

>[!INFO]
>
>**Esempio:**
>
>Uno scenario contiene [!DNL Google Sheets] trigger [!UICONTROL Righe di controllo]. [!DNL Google Sheets] non è disponibile per 30 minuti a causa di manutenzione quando [!DNL Workfront Fusion] avvia lo scenario, quindi non è in grado di recuperare le nuove righe. Lo scenario si interrompe e riprova tra 10 minuti. Perché [!DNL Google Sheets] non è ancora disponibile, [!DNL Workfront Fusion] non è ancora in grado di ottenere informazioni sulle nuove righe. La prossima esecuzione dello scenario è pianificata in 1 ora. [!DNL Google Sheets] è nuovamente disponibile in questo momento e lo scenario viene eseguito correttamente.

## Errore di dati

`DataError`

Quando un elemento viene mappato in modo errato, viene generato un errore di dati che non passa la convalida eseguita sul [!DNL Workfront Fusion] o sul lato del servizio di terze parti utilizzato.

Se si verifica questo errore, lo scenario, fino al punto in cui il modulo non è riuscito, viene spostato nella cartella esecuzioni incomplete, dove è possibile risolvere il problema. Tuttavia, lo scenario non si arresta e continua a funzionare in base alla sua pianificazione. Per interrompere l’esecuzione dello scenario quando viene visualizzato l’errore Dati, abilita l’opzione Elaborazione sequenziale nel pannello Impostazioni scenario.

Se non hai attivato [!UICONTROL Consenti l’archiviazione di esecuzioni incomplete] nelle impostazioni dello scenario, l’esecuzione dello scenario termina con l’errore e viene eseguito un rollback.

Per ulteriori informazioni sulla mappatura, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

Per informazioni sulle esecuzioni incomplete, vedi [Visualizzare e risolvere esecuzioni incomplete in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Per informazioni sul pannello di impostazione dello scenario, consulta [Pannello delle impostazioni dello scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Per informazioni sulle pianificazioni, consulta [Pianificazione di uno scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Errore di dati duplicati

`DuplicateDataError`

Se [!DNL Workfront Fusion] tenta di inserire lo stesso bundle due volte in un servizio che non consente la duplicazione dei dati. Viene generato un errore di dati duplicati. Se si verifica questo errore, [!DNL Workfront Fusion] procede come per l’errore di dati.

## Errore token di accesso non valido

`InvalidAccessTokenError`

Errore token di accesso non valido quando [!DNL Workfront Fusion] non può accedere al tuo account registrato con un servizio di terze parti. Ciò si verifica in genere quando si revocano i diritti di accesso per [!DNL Workfront Fusion] nell’amministrazione di un determinato servizio, ma gli scenari correlati continuano a funzionare in base alla pianificazione.

Se si verifica questo errore, l’esecuzione di uno scenario viene interrotta immediatamente. Il resto dello scenario che inizia dal modulo in cui si è verificato l’errore viene spostato nella cartella delle esecuzioni incomplete.

Per informazioni sulle esecuzioni incomplete, vedi [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Errore limite di frequenza

`RateLimitError`

Se viene superato un limite impostato da un determinato servizio, viene generato un errore di limite della frequenza. Se si verifica questo errore, [!DNL Workfront Fusion] procede come per l&#39;errore di connessione.

Per ulteriori informazioni, consulta [Errore di connessione](#connection-error).

## Errore di dati incompleti

`IncompleteDataError`

Un errore di dati incompleto si verifica solo con i trigger. Questo errore viene generato se un trigger non riesce a scaricare i dati richiesti da un determinato servizio.

Se uno scenario termina con `IncompleteDataError`, il suo ulteriore comportamento dipenderà dall’impostazione di [!UICONTROL Numero massimo di errori consecutivi].

Per ulteriori informazioni, consulta [Numero di errori consecutivi](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) nell’articolo [Pannello delle impostazioni dello scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Esempio:**
>
>Uno scenario ha il [!DNL Workfront] trigger [!UICONTROL Record di controllo] impostato per la ricerca di documenti. Lo scenario viene eseguito durante il caricamento di un documento di grandi dimensioni, ad esempio un video lungo. Perché [!UICONTROL Workfront Fusion] tenta di scaricare il video mentre è ancora in fase di caricamento su Workfront, lo scenario termina con `IncompleteDataError`.

## Errore di runtime

`RuntimeError`

Se durante l’esecuzione dello scenario viene visualizzato un altro errore (non menzionato in precedenza), questo viene segnalato come `RunTimeError`.

Se uno scenario termina con `RuntimeError`, il suo ulteriore comportamento dipenderà dall’impostazione di [!UICONTROL Numero massimo di errori consecutivi]. Per ulteriori informazioni, consulta [Numero di errori consecutivi](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) nell’articolo [Pannello delle impostazioni dello scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>Se uno scenario inizia con un trigger istantaneo, l’impostazione di [!UICONTROL Numero massimo di errori consecutivi] viene ignorato e lo scenario viene disattivato immediatamente dopo il primo errore. Per ulteriori informazioni, consulta [Trigger istantanei](../../workfront-fusion/modules/module-types.md#instant) nell’articolo [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

## Errore di incoerenza

`InconsistencyError`

Se uno degli errori descritti in precedenza si verifica durante la fase di commit o rollback, uno scenario termina con Errore di incoerenza. Per ulteriori informazioni, consulta [Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Se questo errore viene visualizzato in uno scenario, l’esecuzione dello scenario viene interrotta immediatamente.

## Avvertenza

Durante l’esecuzione di uno scenario, è possibile che venga visualizzato un avviso che ti informa su un problema. Tuttavia, non impedisce il completamento corretto dello scenario.

Ad esempio, può comparire un’avvertenza quando viene superata la dimensione massima consentita del file e viene visualizzato il messaggio [!UICONTROL Abilita perdita di dati] è disabilitata. Per ulteriori informazioni, consulta [Abilita perdita di dati](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) nell’articolo [Pannello delle impostazioni dello scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
