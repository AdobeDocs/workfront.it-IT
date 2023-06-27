---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Direttive per la gestione degli errori in [!DNL Adobe Workfront Fusion]
description: Questo articolo descrive le direttive che puoi utilizzare per la gestione degli errori nel [!DNL Adobe Workfront Fusion] scenari.
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# Direttive per la gestione degli errori in [!DNL Adobe Workfront Fusion]

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

## Direttive per la gestione degli errori

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Rollback</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>L’esecuzione dello scenario viene interrotta immediatamente e un <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">Rollback</a> La fase viene avviata su tutti i moduli nel tentativo di ripristinarne lo stato iniziale. I moduli successivi non vengono elaborati.</p> <p>Salvo alcuni tipi di errore, lo scenario viene disattivato dopo il numero di errori consecutivi specificati in Impostazioni scenario. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">Numero di errori consecutivi</a>.</p> <p>Lo stato di esecuzione dello scenario è contrassegnato come "error" (Errore).</p> <p>Nota: questo è il comportamento predefinito se al modulo e al modulo non è associata alcuna route del gestore degli errori <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL Consenti l'archiviazione di esecuzioni incomplete]</a> L'impostazione in [!UICONTROL Scenario settings] non è selezionata.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Conferma</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>L’esecuzione dello scenario viene interrotta immediatamente e viene avviata una fase di commit su tutti i moduli. I moduli successivi non vengono elaborati.</p> <p>Tutti i bundle non elaborati vengono ignorati.</p> <p>Lo stato di esecuzione dello scenario è contrassegnato come "Completato". Per informazioni sulle fasi di commit, vedi <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">Conferma</a> nell’articolo <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Esecuzione di scenari, cicli e fasi in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Riprendi</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>Viene specificato e fornito un output sostitutivo al modulo che rileva un errore.</p> <p>Vengono elaborati i moduli successivi.</p> <p>Lo stato di esecuzione dello scenario è contrassegnato come "Completato".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ignora</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>L’errore viene ignorato e i moduli successivi non vengono elaborati.</p> <p>Se sono presenti bundle non elaborati, l’esecuzione dello scenario continua normalmente.</p> <p>Lo stato di esecuzione dello scenario è contrassegnato come "Completato".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Interrompi</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>Lo stato dell’esecuzione dello scenario viene memorizzato nella coda di esecuzioni incomplete, dove l’errore può essere risolto manualmente. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Visualizzare e risolvere esecuzioni incomplete in Adobe Workfront Fusion</a>. </p> <p>Vi sono tuttavia alcune eccezioni. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">Consenti l’archiviazione di esecuzioni incomplete</a> nell’articolo <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Pannello delle impostazioni dello scenario in Adobe Workfront Fusion</a>.</p> <p>I moduli successivi non vengono elaborati.</p> <p>Se sono presenti bundle non elaborati, l’esecuzione dello scenario continua normalmente.</p> <p>Lo stato di esecuzione dello scenario è contrassegnato come "avvertenza" quando l'opzione [!UICONTROL Automatically complete execution] è disabilitata.</p> <p>Consulta la <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> per ulteriori informazioni.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Riprovare</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>In alcuni casi potrebbe essere utile rieseguire un modulo non riuscito per un paio di volte, quando esiste la possibilità che il motivo del problema passi nel tempo.</p> <p>Workfront Fusion attualmente non offre la direttiva sui nuovi tentativi, anche se è possibile utilizzare diverse soluzioni alternative per imitarne la funzionalità. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Gestione degli errori dei tentativi in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Attualmente le direttive di gestione degli errori non possono essere utilizzate al di fuori di un percorso di gestione degli errori.
>
>   Per ulteriori informazioni, consulta [Route gestore errori](../../workfront-fusion/errors/error-handling.md#error) nell’articolo [Gestione degli errori in Adobe Workfront Fusion](../../workfront-fusion/errors/error-handling.md).
>* [!DNL Workfront Fusion] attualmente non offre un modulo Throw che consentirebbe di generare facilmente errori in modo condizionale, anche se è possibile utilizzare una soluzione alternativa per imitarne la funzionalità.
>
>   Per ulteriori informazioni, consulta [Soluzione alternativa per il lancio](../../workfront-fusion/errors/throw.md#workaround-for-throw) nell’articolo [Gestione degli errori in Adobe Workfront Fusion](../../workfront-fusion/errors/throw.md).

## Interrompi {#break}

Quando un errore viene gestito da [!DNL Break] direttiva, viene creato un record nella cartella Esecuzioni incomplete. Questo record memorizza lo stato dell’esecuzione dello scenario, insieme ai dati dei moduli precedenti. Il record fa riferimento al modulo in cui si è verificato l’errore e contiene informazioni sui dati ricevuti dal modulo come input. Per ogni bundle di dati che causa l’errore, viene creato un record separato.

Per ulteriori informazioni, consulta [Visualizzare e risolvere esecuzioni incomplete in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Risolvere gli errori derivanti dalla direttiva Break

Puoi risolvere l’errore manualmente aggiornando lo scenario (se necessario) ed eseguendolo una volta.

Puoi anche configurare lo scenario in modo da elaborare automaticamente un’esecuzione incompleta rieseguendo lo scenario. Per configurare il modulo in modo da elaborare le esecuzioni incomplete:

1. All&#39;interno del modulo Break, abilita [!UICONTROL **Completamento automatico dell’esecuzione**] opzione.
1. In **Numero di tentativi** , immettere o mappare il numero massimo di tentativi che si desidera vengano ripetuti dal modulo

   Questo numero deve essere compreso tra 1 e 100.
1. In **Intervallo tra i tentativi** immettere o mappare il numero di minuti tra ogni nuovo tentativo.

Con questa opzione abilitata, quando si verifica un errore, viene recuperata l’esecuzione incompleta (dopo il tempo specificato in [!UICONTROL Intervallo tra i tentativi] ) ed eseguito con i dati di input originali. Questo verrà ripetuto fino al completamento dell’esecuzione del modulo senza errori o fino al raggiungimento del numero di tentativi specificato.

>[!NOTE]
>
>Se il tentativo iniziale di nuovo tentativo non riesce, l’intervallo tra i nuovi tentativi aumenta in modo esponenziale ogni altro tentativo.


Quando è attivata l’opzione &quot;Esecuzione automatica del completamento&quot;, l’esecuzione dello scenario è contrassegnata come &quot;Completata&quot; perché il tentativo automatico del gestore degli errori di interruzione gestisce il problema automaticamente. In questo caso, gli utenti non ricevono un messaggio e-mail relativo all’esecuzione non riuscita.

Quando &quot;Esecuzione automatica completa&quot; è disattivato, l’esecuzione viene contrassegnata come &quot;Avviso&quot;.

Esistono alcune eccezioni alle esecuzioni memorizzate in Esecuzioni incomplete e, con alcuni tipi di errore, non è possibile ritentare automaticamente l’esecuzione di uno scenario.

Per ulteriori informazioni, consulta [Consenti l’archiviazione di esecuzioni incomplete](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) nell’articolo [Pannello delle impostazioni dello scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Per ulteriori informazioni, consulta [Gestione avanzata degli errori in Adobe Workfront Fusion](../../workfront-fusion/errors/advanced-error-handling.md).
