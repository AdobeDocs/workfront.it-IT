---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Direttive sulla gestione degli errori [!DNL Adobe Workfront Fusion]
description: Questo articolo descrive le direttive che puoi utilizzare per la gestione degli errori nel tuo [!DNL Adobe Workfront Fusion] scenari.
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: 50b43cd4bafdfc3379eb1d73c12e15c791e28dbe
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# Direttive sulla gestione degli errori [!DNL Adobe Workfront Fusion]

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
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Direttive sulla gestione degli errori

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Ripristino</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>L'esecuzione dello scenario viene interrotta immediatamente e un <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">Ripristino</a> viene avviata una fase su tutti i moduli nel tentativo di ripristinarli tutti allo stato iniziale. I moduli successivi non vengono elaborati.</p> <p>Per alcuni tipi di errore, lo scenario viene disattivato dopo il numero di errori consecutivi specificati nelle impostazioni Scenario. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">Numero di errori consecutivi</a>.</p> <p>Lo stato di esecuzione dello scenario è contrassegnato come "error".</p> <p>Nota: Questo è il comportamento predefinito se al modulo e al <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL Consenti archiviazione esecuzioni incomplete]</a> L'impostazione in Impostazioni scenario non è selezionata.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Conferma</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>L’esecuzione dello scenario viene interrotta immediatamente e viene avviata una fase di commit su tutti i moduli. I moduli successivi non vengono elaborati.</p> <p>Tutti i bundle non elaborati vengono ignorati.</p> <p>Lo stato di esecuzione dello scenario è contrassegnato come "riuscito". Per informazioni sulle fasi di commit, vedi <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">Commit</a> nell'articolo <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Esecuzione di scenari, cicli e fasi in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Riprendi</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>Viene specificato e fornito un output sostitutivo al modulo che rileva un errore.</p> <p>I moduli successivi vengono elaborati.</p> <p>Lo stato di esecuzione dello scenario è contrassegnato come "riuscito".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ignora</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>L’errore viene ignorato e i moduli successivi non vengono elaborati.</p> <p>Se sono presenti bundle non elaborati, l'esecuzione dello scenario continua normalmente.</p> <p>Lo stato di esecuzione dello scenario è contrassegnato come "riuscito".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Interruzione</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>Lo stato dell’esecuzione dello scenario viene memorizzato nella coda delle esecuzioni incomplete in cui l’errore può essere risolto manualmente. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Visualizzare e risolvere le esecuzioni incomplete in Adobe Workfront Fusion</a>. </p> <p>Vi sono tuttavia alcune eccezioni. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">Consenti archiviazione esecuzioni incomplete</a> nell'articolo <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Pannello delle impostazioni dello scenario in Adobe Workfront Fusion</a>.</p> <p>I moduli successivi non vengono elaborati.</p> <p>Se sono presenti bundle non elaborati, l'esecuzione dello scenario continua normalmente.</p> <p>Lo stato di esecuzione dello scenario viene contrassegnato come "avviso" quando l’opzione [!UICONTROL Completa automaticamente l’esecuzione] è disabilitata.</p> <p>Consulta la sezione <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> per ulteriori informazioni.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Riprovare</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>In alcuni casi potrebbe essere utile ripetere l’esecuzione di un modulo non riuscito per un paio di volte quando esiste la possibilità che il motivo dell’errore possa passare nel tempo.</p> <p>Workfront Fusion attualmente non offre la direttiva Retry, anche se è possibile utilizzare diverse soluzioni per imitarne le funzionalità. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Riprova la gestione degli errori in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Attualmente le direttive sulla gestione degli errori non possono essere utilizzate al di fuori dell&#39;ambito di un percorso di gestione degli errori e [!DNL Workfront Fusion] al momento non offre un modulo Throw che ti consentirebbe di generare facilmente (generare) errori in modo condizionale, anche se può essere utilizzata una soluzione alternativa per imitarne la funzionalità. Per ulteriori informazioni, consulta [route del gestore errori](../../workfront-fusion/errors/error-handling.md#error) nell&#39;articolo [Gestione degli errori in Adobe Workfront Fusion](../../workfront-fusion/errors/error-handling.md). Vedi anche [Soluzione per il lancio](../../workfront-fusion/errors/throw.md#workarou) nell&#39;articolo [Gestione degli errori di thread in Adobe Workfront Fusion](../../workfront-fusion/errors/throw.md).

## Interruzione {#break}

Quando un errore viene gestito dal [!DNL Break] , viene creato un record [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) cartella che memorizza lo stato dell’esecuzione dello scenario insieme ai dati dei moduli precedenti. Per ogni bundle di dati che causa l&#39;errore, viene creato un record separato.

Il record fa riferimento al modulo da cui è stato generato l&#39;errore e contiene informazioni relative ai dati ricevuti dal modulo come input. Per ulteriori informazioni, consulta [Visualizzare e risolvere le esecuzioni incomplete in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

In questo caso, è possibile risolvere l’errore manualmente aggiornando lo scenario (se necessario) ed eseguendo l’errore una volta.

D&#39;altro canto, consentendo il [!UICONTROL Esecuzione automatica] in base alle impostazioni della direttiva di interruzione, è possibile configurare per elaborare automaticamente un&#39;esecuzione incompleta eseguendo nuovamente lo scenario dopo il numero specificato di minuti.

Con questa opzione abilitata, quando si verifica un errore, l’esecuzione incompleta viene recuperata (dopo il tempo specificato nel [!UICONTROL Intervallo tra tentativi] ed eseguito con i dati di input originali. Ciò si ripeterà fino al completamento dell’esecuzione del modulo senza un errore o fino al raggiungimento del numero di tentativi specificato.

>[!NOTE]
>
>Se il tentativo iniziale di nuovo tentativo non riesce, l&#39;intervallo tra i tentativi aumenta esponenzialmente ogni altro tentativo.

Quando l’opzione &quot;Completa automaticamente l’esecuzione&quot; è attivata, l’esecuzione dello scenario viene contrassegnata come &quot;Completato&quot; perché il nuovo tentativo automatico del gestore di errori di interruzione gestisce il problema automaticamente. In questo caso, gli utenti non ricevono un’e-mail sull’esecuzione non riuscita.

Quando l&#39;opzione &quot;Completa automaticamente l&#39;esecuzione&quot; è disattivata, l&#39;esecuzione viene contrassegnata come &quot;Avviso&quot;.

![](assets/break-directive-350x241.png)

Tuttavia, ci sono alcune eccezioni alle esecuzioni archiviate in Esecuzioni incomplete e con alcuni tipi di errore, il tentativo automatico di un&#39;esecuzione di uno scenario non è possibile. Per ulteriori informazioni, consulta [Consenti archiviazione esecuzioni incomplete](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) nell&#39;articolo [Pannello delle impostazioni dello scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Per ulteriori informazioni, consulta [Gestione avanzata degli errori in Adobe Workfront Fusion](../../workfront-fusion/errors/advanced-error-handling.md).
