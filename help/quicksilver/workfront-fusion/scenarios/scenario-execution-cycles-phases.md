---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]
description: Questo articolo descrive gli eventi che si verificano durante un [!DNL Adobe Workfront Fusion] lo scenario è in esecuzione, ad esempio inizializzazione, operazioni, commit e rollback.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 1%

---

# Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] è un sistema transazionale simile ai database relazionali. Ogni esecuzione dello scenario inizia con la fase di inizializzazione, continua con almeno un ciclo composto dalle fasi di operazione e commit/rollback e termina con la fase di finalizzazione:

>[!INFO]
>
>**Esempio**
>
>Inizializzazione
>
>#1 ciclo
>
>Funzionamento (lettura o scrittura)
>
>Conferma o rollback
>
>#2 ciclo
>
>Funzionamento (lettura o scrittura)
>
>Conferma o rollback
>
>...
>
>#N ciclo
>
>Funzionamento (lettura o scrittura)
>
>Conferma o rollback
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
  <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
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

## Inizializzazione

Durante la fase di inizializzazione, vengono create tutte le connessioni necessarie (connessione a un database, servizio e-mail e così via). Vengono inoltre verificati se ogni modulo è in grado di eseguire le operazioni a cui è destinato.

## Cicli

Ogni ciclo rappresenta un&#39;unità di lavoro indissociabile composta da una serie di operazioni. È possibile impostare il numero massimo di cicli nel [!UICONTROL impostazioni scenario] pannello. Il numero predefinito è 1.

Per ulteriori informazioni, consulta [Il pannello delle impostazioni dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Operazione

Durante la fase di funzionamento si esegue la lettura e/o la scrittura:

* L’operazione di lettura consiste nell’ottenere dati da un servizio che viene quindi elaborato da altri moduli in base a uno scenario predefinito. Ad esempio, il [!UICONTROL Dropbox] >[!UICONTROL Guarda i file] Il modulo restituisce nuovi bundle (file) creati dall’ultima esecuzione dello scenario.
* L’operazione di scrittura consiste nell’inviare dati a un determinato servizio per un’ulteriore elaborazione. Ad esempio, il [!DNL Dropbox] >[!UICONTROL Carica un file] il modulo carica un file in un [!DNL Dropbox] cartella.

## Conferma

Se la fase operativa ha esito positivo per tutti i moduli, inizia la fase di commit durante la quale vengono eseguite tutte le operazioni eseguite dai moduli. Ciò significa che [!DNL Workfront Fusion] invia a tutti i servizi coinvolti nella fase operativa informazioni sul suo successo.

## Rollback

Se si verifica un errore durante la fase di operazione o commit di un modulo, la fase viene interrotta e viene avviata la fase di rollback, rendendo vuote tutte le operazioni durante il ciclo specificato. Alcuni moduli non supportano il rollback e le operazioni eseguite da questi moduli non possono essere ripristinate. Per ulteriori informazioni, consulta [Moduli ACID](#acid-modules) sezione.

## Finalizzazione

Durante la fase di finalizzazione, le connessioni aperte (ad esempio le connessioni FTP, le connessioni al database e così via) vengono chiuse e lo scenario viene completato.

## Moduli ACID

Tutti [!DNL Workfront Fusion] I moduli che supportano il rollback (noto anche come transazionale) sono contrassegnati con il tag ACID.

![](assets/acid-modules-350x189.png)

I moduli non contrassegnati con questo tag non possono essere ripristinati allo stato iniziale quando si verificano errori in altri moduli. Un esempio tipico di modulo non-ACID è il [!UICONTROL E-mail] >[!UICONTROL Inviare un’e-mail] azione. Una volta inviata l’e-mail, non puoi annullare l’invio.
