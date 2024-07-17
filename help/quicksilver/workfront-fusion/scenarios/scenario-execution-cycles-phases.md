---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Esecuzione, cicli e fasi dello scenario in [!DNL Adobe Workfront Fusion]
description: In questo articolo vengono descritti gli eventi che si verificano durante l'esecuzione di uno scenario  [!DNL Adobe Workfront Fusion] , ad esempio l'inizializzazione, le operazioni, i commit e i rollback.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# Esecuzione, cicli e fasi dello scenario in [!DNL Adobe Workfront Fusion]

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
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Inizializzazione

Durante la fase di inizializzazione, vengono create tutte le connessioni necessarie (connessione a un database, servizio e-mail e così via). Vengono inoltre verificati se ogni modulo è in grado di eseguire le operazioni a cui è destinato.

## Cicli

Ogni ciclo rappresenta un&#39;unità di lavoro indissociabile composta da una serie di operazioni. È possibile impostare il numero massimo di cicli nel pannello [!UICONTROL impostazioni scenario]. Il numero predefinito è 1.

Per ulteriori informazioni, vedere [Pannello impostazioni scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Operazione

Durante la fase di funzionamento si esegue la lettura e/o la scrittura:

* L’operazione di lettura consiste nell’ottenere dati da un servizio che viene quindi elaborato da altri moduli in base a uno scenario predefinito. Il modulo [!UICONTROL Dropbox] >[!UICONTROL File di controllo], ad esempio, restituisce nuovi bundle (file) creati dall&#39;ultima esecuzione dello scenario.
* L’operazione di scrittura consiste nell’inviare dati a un determinato servizio per un’ulteriore elaborazione. Ad esempio, il modulo [!DNL Dropbox] >[!UICONTROL Carica un file] carica un file in una cartella [!DNL Dropbox].

## Conferma

Se la fase operativa ha esito positivo per tutti i moduli, inizia la fase di commit durante la quale vengono eseguite tutte le operazioni eseguite dai moduli. [!DNL Workfront Fusion] invia quindi informazioni sul completamento a tutti i servizi coinvolti nella fase operativa.

## Rollback

Se si verifica un errore durante la fase di operazione o commit di un modulo, la fase viene interrotta e viene avviata la fase di rollback, rendendo vuote tutte le operazioni durante il ciclo specificato. Alcuni moduli non supportano il rollback e le operazioni eseguite da questi moduli non possono essere ripristinate. Per ulteriori informazioni, consulta la sezione [Moduli ACID](#acid-modules).

## Finalizzazione

Durante la fase di finalizzazione, le connessioni aperte (ad esempio le connessioni FTP, le connessioni al database e così via) vengono chiuse e lo scenario viene completato.

## Moduli ACID

Tutti i moduli [!DNL Workfront Fusion] che supportano il rollback (noto anche come transazionale) sono contrassegnati con il tag ACID.

![](assets/acid-modules-350x189.png)

I moduli non contrassegnati con questo tag non possono essere ripristinati allo stato iniziale quando si verificano errori in altri moduli. Un esempio tipico di modulo non-ACID è l&#39;azione [!UICONTROL E-mail] >[!UICONTROL Invia e-mail]. Una volta inviata l’e-mail, non puoi annullare l’invio.
