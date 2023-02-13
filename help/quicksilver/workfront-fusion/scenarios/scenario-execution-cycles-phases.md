---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]
description: Questo articolo descrive gli eventi che si verificano durante un [!DNL Adobe Workfront Fusion] scenario in esecuzione, ad esempio inizializzazione, operazioni, commit e rollback.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] è un sistema transazionale simile ai database relazionali. L&#39;esecuzione di ogni scenario inizia con la fase di inizializzazione, continua con almeno un ciclo composto dalle fasi di operazione e commit/rollback e termina con la fase di finalizzazione:

>[!INFO]
>
>**Esempio**
>
>Inizializzazione
>
>Ciclo 1
>
>Operazione (lettura o scrittura)
>
>Commit o rollback
>
>Ciclo 2
>
>Operazione (lettura o scrittura)
>
>Commit o rollback
>
>...
>
>Ciclo N
>
>Operazione (lettura o scrittura)
>
>Commit o rollback
>
>Finalizzazione

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Inizializzazione

Durante la fase di inizializzazione vengono create tutte le connessioni necessarie (connessione a un database, servizio e-mail e così via). Vengono inoltre controllati se ogni modulo è in grado di eseguire le operazioni previste.

## Cicli

Ogni ciclo rappresenta un&#39;unità di lavoro non divisibile composta da una serie di operazioni. È possibile impostare il numero massimo di cicli nel [!UICONTROL impostazioni dello scenario] pannello. Il numero predefinito è 1.

Per ulteriori informazioni, consulta [Il pannello delle impostazioni dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Operazione

Durante la fase operativa viene eseguita l&#39;operazione di lettura e/o scrittura:

* L’operazione di lettura consiste nell’ottenere i dati da un servizio che viene quindi elaborato da altri moduli in base a uno scenario predefinito. Ad esempio, il [!UICONTROL Dropbox] >[!UICONTROL File di controllo] Il modulo restituisce nuovi bundle (file) creati dall&#39;ultima esecuzione dello scenario.
* L’operazione di scrittura consiste nell’invio di dati a un determinato servizio per un ulteriore trattamento. Ad esempio, il [!DNL Dropbox] >[!UICONTROL Caricare un file] il modulo carica un file in un [!DNL Dropbox] cartella.

## Conferma

Se la fase di funzionamento ha esito positivo per tutti i moduli, la fase di commit inizia durante la quale vengono eseguite tutte le operazioni dei moduli. Ciò significa che [!DNL Workfront Fusion] invia a tutti i servizi coinvolti nella fase operativa informazioni sul suo successo.

## Ripristino

Se si verifica un errore durante l&#39;operazione o la fase di commit su qualsiasi modulo, la fase viene interrotta e la fase di rollback viene avviata, rendendo tutte le operazioni durante il ciclo inattive. Alcuni moduli non supportano il rollback e le operazioni eseguite da questi moduli non possono essere ripristinate. Per ulteriori informazioni, consulta la sezione [Moduli ACID](#acid-modules) sezione .

## Finalizzazione

Durante la fase di finalizzazione, le connessioni aperte (ad esempio, connessioni FTP, connessioni al database e così via) vengono chiuse e lo scenario viene completato.

## Moduli ACID

Tutto [!DNL Workfront Fusion] i moduli che supportano il rollback (noto anche come transazionale) sono contrassegnati con il tag ACID.

![](assets/acid-modules-350x189.png)

I moduli non contrassegnati con questo tag non possono essere ripristinati al loro stato iniziale quando si verificano errori in altri moduli. Un esempio tipico di modulo non ACID è il [!UICONTROL E-mail] >[!UICONTROL Invia un messaggio e-mail] azione. Dopo l’invio dell’e-mail non puoi annullare l’invio.
