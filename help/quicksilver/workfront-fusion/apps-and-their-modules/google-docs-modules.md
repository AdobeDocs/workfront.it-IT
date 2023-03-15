---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Google Docs
description: Adobe Workfront Fusion [!DNL Google Docs] i moduli consentono di monitorare, creare, modificare e recuperare i documenti [!DNL Google Docs] e [!DNL Google Docs] (per gli utenti di [!DNL G Suite]).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '4042'
ht-degree: 0%

---

# [!DNL Google Docs] moduli

La [!DNL Adobe Workfront Fusion] [!DNL Google Docs] i moduli consentono di monitorare, creare, modificare e recuperare i documenti [!DNL Google Docs] e [!DNL Google Docs] (per [!DNL G Suite] utenti).

Per utilizzare [!DNL Google Docs] con [!DNL Adobe Workfront Fusion], è necessario disporre di un [!DNL Google] conto. Se non hai un [!DNL Google] tuttavia, è possibile crearne una nella [!DNL Google] Pagina della guida dell’account.

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o superiore</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr>
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Per utilizzare [!DNL Google Docs] moduli, è necessario disporre di un account Google.

## [!DNL Google Docs] moduli e relativi campi

Quando si configura [!DNL Google Docs] moduli, [!UICONTROL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Google Docs] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Documento

* [[!UICONTROL Controlla documenti]](#watch-documents)
* [[!UICONTROL Elenca documenti]](#list-documents)
* [[!UICONTROL Ottenere il contenuto di un documento]](#get-content-of-a-document)
* [[!UICONTROL Creare un documento]](#create-a-document)
* [[!UICONTROL Creare un documento da un modello]](#create-a-document-from-a-template)
* [[!UICONTROL Inserire un paragrafo in un documento]](#insert-a-paragraph-to-a-document)
* [[!UICONTROL Inserire un&#39;immagine in un documento]](#insert-an-image-to-a-document)
* [[!UICONTROL Sostituire un’immagine con una nuova immagine]](#replace-an-image-with-a-new-image)
* [[!UICONTROL Sostituire il testo in un documento]](#replace-text-in-a-document)
* [[!UICONTROL Scaricare un documento]](#download-a-document)
* [[!UICONTROL Eliminare un documento]](#delete-a-document)

#### [!UICONTROL Controlla documenti]

Questo modulo di attivazione restituisce i dettagli del documento quando un nuovo documento viene creato o modificato nella cartella selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Guarda i documenti]</td> 
   <td> <p style="color: #000000;">Seleziona se visualizzare i documenti creati ([!UICONTROL By Created Date]) o modificati ([!UICONTROL By Modified Date]).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Selezionare il tipo di unità da monitorare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selezionare la cartella da controllare per i documenti creati o modificati.</p> </li> 
     <li> <p><strong>[!UICONTROL Condiviso Con Me]</strong> </p> <p>Selezionare la cartella da controllare per i documenti creati o modificati.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unità condivisa]</strong> (disponibile per [!DNL G Suite] solo utenti)</p> <p>Seleziona se desideri [!UICONTROL Utilizzare l’accesso amministratore di dominio]. Selezionando [!UICONTROL Sì] la richiesta viene generata come amministratore di dominio e vengono restituite tutte le unità condivise in cui il richiedente è un amministratore.</p> <p>Selezionare l'unità condivisa che si desidera controllare.</p> <p>Nota: Se hai selezionato la [!DNL Google Shared Drive] in questo campo e non sei un [!DNL G Suite] utente, errore <code>[400] Invalid Value</code> viene restituito .</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Imposta il numero massimo di documenti restituiti da Workfront Fusion in un unico ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenca documenti]

Questo modulo di azione recupera un elenco di documenti dalla cartella selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Selezionare il tipo di unità da cui si desidera elencare i documenti.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selezionare la cartella da cui si desidera elencare i documenti.</p> </li> 
     <li> <p><strong>[!UICONTROL Condiviso Con Me]</strong> </p> <p>Selezionare la cartella da cui si desidera elencare i documenti.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unità condivisa]</strong> (disponibile per [!DNL G Suite] solo utenti)</p> <p>Seleziona se desideri [!UICONTROL Utilizzare l’accesso amministratore di dominio]. Selezionando [!UICONTROL Sì] la richiesta viene generata come amministratore di dominio e vengono restituite tutte le unità condivise in cui il richiedente è un amministratore.</p> <p>Selezionare l'unità condivisa da cui si desidera elencare i documenti.</p> <p>Nota: Se hai selezionato la [!DNL Google Docs] in questo campo e non sei un [!DNL G Suite] utente, errore <code>[400] Invalid Value</code> viene restituito .</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Imposta il numero massimo di documenti [!DNL Workfront Fusion] restituisce in un ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottenere il contenuto di un documento]

Questo modulo di azione recupera un documento specificato.

Potrebbe essere necessario estendere le autorizzazioni.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ottieni contenuto di un documento]</td> 
   <td> <p>Selezionare se si desidera mappare l'ID documento del documento o selezionare manualmente il documento dal menu a discesa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Selezionare il tipo di unità contenente il documento che si desidera recuperare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selezionare la cartella contenente il documento che si desidera recuperare.</p> </li> 
     <li> <p><strong>[!UICONTROL Condiviso Con Me]</strong> </p> <p>Selezionare la cartella contenente il documento che si desidera recuperare.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unità condivisa]</strong> (disponibile per [!DNL G Suite] solo utenti)</p> <p>Seleziona se desideri [!UICONTROL Utilizzare l’accesso amministratore di dominio]. Selezionando [!UICONTROL Sì] la richiesta viene generata come amministratore di dominio e vengono restituite tutte le unità condivise in cui il richiedente è un amministratore.</p> <p>Selezionare l'unità condivisa contenente il documento che si desidera recuperare.</p> <p>Nota: Se hai selezionato la [!DNL Google Docs] in questo campo e non sei un [!DNL G Suite] utente, errore <code>[400] Invalid Value</code> viene restituito .</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Selezionare l'oggetto che si desidera restituire nell'output del modulo.</p> 
    <ul> 
     <li>[!UICONTROL Image] (predefinito)</li> 
     <li>[!UICONTROL Drawing]</li> 
     <li>Grafico</li> 
    </ul> <p>Nota:  <p>Per ulteriori mappature di questi oggetti, utilizza il valore [!UICONTROL Inline Objects Array] nell’output di questo modulo (invece di [!UICONTROL inlineObjects]).</p> <p>Gli oggetti [!UICONTROL Inline Objects Array] vengono ordinati nello stesso ordine in cui vengono visualizzati nel documento. L'elaborazione risulterà più semplice.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare un documento]

Questo modulo di azione consente di creare un nuovo documento nella cartella selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Immettere il nome del documento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content]</td> 
   <td> <p>Inserire il contenuto del documento. HTML è supportato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Selezionare il tipo di unità in cui si desidera creare un documento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selezionare la cartella in cui si desidera creare un documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Condiviso Con Me]</strong> </p> <p>Selezionare la cartella in cui si desidera creare un documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unità condivisa]</strong> (disponibile per [!DNL G Suite] solo utenti)</p> <p>Seleziona se desideri [!UICONTROL Utilizzare l’accesso amministratore di dominio]. Selezionando [!UICONTROL Sì] la richiesta viene generata come amministratore di dominio e vengono restituite tutte le unità condivise in cui il richiedente è un amministratore.</p> <p>Selezionare l'unità condivisa in cui si desidera creare un documento.</p> <p>Nota: Se hai selezionato la [!DNL Google Docs] in questo campo e non sei un [!DNL G Suite] utente, errore <code>[400] Invalid Value</code> viene restituito .</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserire un’intestazione]</td> 
   <td> <p> Abilitare questa opzione per inserire l’intestazione nel documento, quindi immettere o mappare il testo dell’intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserire un piè di pagina] </td> 
   <td> <p>Selezionare questa opzione per inserire il piè di pagina nel documento, quindi immettere o mappare il testo dell'intestazione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare un documento da un modello]

Questo modulo di azione crea una copia di un documento modello esistente e sostituisce eventuali tag. Questo modulo consente inoltre agli utenti di sostituire le immagini con nuove immagini tramite URL.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Creare un documento da un modello]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Selezionare questa opzione per mappare il modello di documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br>Selezionare questa opzione per scegliere il modello di documento dal menu a discesa.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Selezionare il tipo di unità in cui si trova il modello. Questa opzione è disponibile se hai selezionato [!UICONTROL By Dropdown] nel campo precedente.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Seleziona la cartella in cui si trova il modello.</p> </li> 
     <li> <p><strong>[!UICONTROL Condiviso Con Me]</strong> </p> <p>Seleziona la cartella in cui si trova il modello.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unità condivisa]</strong> (disponibile per [!DNL G Suite] solo utenti)</p> <p>Seleziona se desideri [!UICONTROL Utilizzare l’accesso amministratore di dominio]. Selezionando [!UICONTROL Sì] la richiesta viene generata come amministratore di dominio e vengono restituite tutte le unità condivise in cui il richiedente è un amministratore.</p> <p>Selezionare l'unità condivisa in cui si trova il modello.</p> <p>Nota: Se hai selezionato la [!DNL Google Docs] in questo campo e non sei un [!DNL G Suite] utente, errore <code>[400] Invalid Value</code> viene restituito .</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>Immettere i valori che verranno immessi al posto delle variabili nel nuovo documento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Tags]</strong> <br>Immettere i tag contenuti nel modello di documento. Non utilizzare <code>&#123;&#123;&#125;&#125;</code>. Esempio: use <code>name</code> anziché <code>&#123;&#123;name&#125;&#125;</code>.</li> 
     <li><strong>[!UICONTROL Valore Sostituito]</strong><br>Immetti il valore del tag .</li> 
    </ul> <p>Ad esempio,<code> &#123;&#123;name&#125;&#125;</code> nel documento di origine verrà visualizzata come campo nome, in cui è possibile inserire il valore, ad esempio <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Immagini sostitutive]</p> </td> 
   <td> <p>Immetti il collegamento all’ [!UICONTROL Image Object ID] e all’ [!UICONTROL Image URL] che sostituiranno l’immagine corrente.</p> <p>Nota: È possibile recuperare gli ID immagine utilizzando il modulo [!UICONTROL Get a Document], in cui gli ID sono contenuti nella matrice [!UICONTROL Inline Object Array].</p> <p>È consigliabile aggiungere testo ALT alle immagini nel [!DNL Google] documento. </p> <p>Per aggiungere un testo ALT alla tabella [!DNL Google Docs] immagine:</p> 
    <ol> 
     <li value="1">Fai clic con il pulsante destro del mouse sull'immagine.</li> 
     <li value="2">Selezionare l’opzione [!UICONTROL ALT text].</li> 
     <li value="3">Inserisci il testo ALT nel campo [!UICONTROL Title] e fai clic su [!UICONTROL OK].</li> 
    </ol> <p>Dopo aver aggiunto il testo ALT all'immagine, il testo ALT viene visualizzato tra parentesi nel nome del campo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title] </td> 
   <td> <p>Immettere il nome del nuovo documento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Selezionare il tipo di unità in cui si trova il modello. Questa opzione è disponibile se hai selezionato [!UICONTROL By Dropdown] nel campo precedente.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selezionare la cartella in cui si desidera creare il documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Condiviso Con Me]</strong> </p> <p>Selezionare la cartella in cui si desidera creare il documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unità condivisa]</strong> (disponibile per [!DNL G Suite] solo utenti)</p> <p>Seleziona se desideri [!UICONTROL Utilizzare l’accesso amministratore di dominio]. Selezionando [!UICONTROL Sì] la richiesta viene generata come amministratore di dominio e vengono restituite tutte le unità condivise in cui il richiedente è un amministratore.</p> <p>Selezionare l'unità condivisa in cui si desidera creare il documento.</p> <p>Nota: Se hai selezionato la [!DNL Google Docs] in questo campo e non sei un [!DNL G Suite] utente, errore <code>[400] Invalid Value</code> viene restituito .</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Inserire un paragrafo in un documento]

Questo modulo di azione aggiunge o inserisce un nuovo paragrafo a un documento esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Selezionare un documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Selezionare questa opzione per mappare il documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Selezionare questa opzione per scegliere il documento dal menu a discesa.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Selezionare il tipo di unità in cui si trova il documento a cui si desidera aggiungere un paragrafo. Questa opzione è disponibile se hai selezionato [!UICONTROL By Dropdown] nel campo precedente.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selezionare la cartella in cui si trova il documento a cui si desidera aggiungere un paragrafo, quindi selezionare il documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Condiviso Con Me]</strong> </p> <p>Selezionare la cartella in cui si trova il documento a cui si desidera aggiungere un paragrafo, quindi selezionare il documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unità condivisa]</strong> (disponibile per [!DNL G Suite] solo utenti)</p> <p>Seleziona se desideri [!UICONTROL Utilizzare l’accesso amministratore di dominio]. Selezionando [!UICONTROL Sì] la richiesta viene generata come amministratore di dominio e vengono restituite tutte le unità condivise in cui il richiedente è un amministratore.</p> <p>Selezionare l'unità condivisa in cui si trova il documento a cui si desidera aggiungere un paragrafo, quindi selezionare il documento.</p> <p>Nota: Se hai selezionato la [!DNL Google Docs] in questo campo e non sei un [!DNL G Suite] utente, errore <code>[400] Invalid Value</code> viene restituito .</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Inserire un paragrafo]</p> </td> 
   <td> <p>Selezionare la modalità di inserimento del nuovo testo nel documento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Per specifica di posizione]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL By index]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Immettere il numero di indice in cui si desidera inserire il testo. È possibile utilizzare il modulo [!UICONTROL Get a Document] per recuperare il numero di indice.</p> <p>Per visualizzare tutti i caratteri (anche nascosti) nel documento, puoi utilizzare il componente aggiuntivo [!UICONTROL Show]. Puoi trovare il componente aggiuntivo in [!UICONTROL Add-ons] &gt; [!UICONTROL Get add-ons]. Cerca [!UICONTROL Show] e installa il componente aggiuntivo [!UICONTROL Show].</p> </li> 
         <li> <p><strong>[!UICONTROL Testo inserito]</strong> </p> <p>Immettere il testo che si desidera inserire nel documento.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL Per ID segmento]</strong> </p> <p>Selezionare l’intestazione e il piè di pagina in cui si desidera inserire il contenuto di testo e immettere il testo da inserire nei campi corrispondenti.</p> <p>Se l’intestazione o il piè di pagina contengono già del testo, il nuovo testo verrà aggiunto prima del testo esistente.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Aggiungendo al corpo del documento]</strong> </p> <p>Aggiunge il testo immesso alla fine del contenuto corporeo del documento.</p> <p>Lo stile del nuovo paragrafo viene copiato dal paragrafo nella posizione dell’indice di inserimento corrente, inclusi elenchi e punti elenco.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Aggiungendo alla fine del segmento (intestazione e piè di pagina)]</strong> </p> <p>Selezionare l’intestazione e il piè di pagina in cui si desidera inserire il contenuto di testo e immettere il testo da inserire nei campi corrispondenti.</p> <p>Se l’intestazione o il piè di pagina contengono già del testo, il nuovo testo verrà aggiunto dopo il testo esistente.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Testo aggiunto [!UICONTROL]</td> 
   <td>Immettere o mappare il testo da aggiungere al documento</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Inserire un&#39;immagine in un documento]

Questo modulo di azione inserisce un’immagine dall’URL al documento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Selezionare un documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Selezionare questa opzione per mappare il modello di documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Selezionare questa opzione per scegliere il documento dal menu a discesa.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Selezionare il tipo di unità in cui si trova il documento a cui si desidera aggiungere un'immagine. Questa opzione è disponibile se hai selezionato [!UICONTROL By Dropdown] nel campo precedente.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selezionare la cartella in cui si trova il documento a cui si desidera aggiungere un'immagine, quindi selezionare il documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Condiviso Con Me]</strong> </p> <p>Selezionare la cartella in cui si trova il documento a cui si desidera aggiungere un'immagine, quindi selezionare il documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unità condivisa]</strong> (disponibile per [!DNL G Suite] solo utenti)</p> <p>Seleziona se desideri [!UICONTROL Utilizzare l’accesso amministratore di dominio]. Selezionando [!UICONTROL Sì] la richiesta viene generata come amministratore di dominio e vengono restituite tutte le unità condivise in cui il richiedente è un amministratore.</p> <p>Selezionare l'unità condivisa in cui si trova il documento a cui si desidera aggiungere un'immagine, quindi selezionare il documento.</p> <p>Nota: Se hai selezionato la [!DNL Google Docs] in questo campo e non sei un [!DNL G Suite] utente, errore <code>[400] Invalid Value</code> viene restituito .</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Inserire un’immagine]</p> </td> 
   <td> <p>Selezionare la modalità di inserimento della nuova immagine nel documento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Per specifica di posizione]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL By index]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Immettere il numero di indice in cui si desidera inserire l'immagine. Puoi utilizzare il modulo [!UICONTROL Get a Document] per recuperare il numero di indice [!UICONTROL Index Number].</p> <p>Per visualizzare tutti i caratteri (anche nascosti) nel documento, puoi utilizzare il componente aggiuntivo [!UICONTROL Show]. Puoi trovare il componente aggiuntivo in [!UICONTROL Add-ons] &gt; [!UICONTROL Get add-ons]. Cerca [!UICONTROL Show] e installa il componente aggiuntivo [!UICONTROL Show].</p> </li> 
         <li> <p><strong>[!UICONTROL URL immagine]</strong> </p> <p>Immettere l'URL dell'immagine che si desidera inserire nel documento.</p> <p>La dimensione massima dell'immagine è 50 MB. Non deve superare i 25 megapixel. È supportato solo il formato PNG, JPEG o GIF.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL Per ID segmento]</strong> </p> <p>Selezionare l’intestazione e il piè di pagina a cui si desidera inserire l’immagine e immettere l’URL dell’immagine nei campi corrispondenti.</p> <p>La dimensione massima dell'immagine è 50 MB. L'immagine non deve superare i 25 megapixel. È supportato solo il formato PNG, JPEG o GIF.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Aggiungendo al corpo del documento]</strong> </p> <p>Aggiunge un'immagine specifica alla fine del contenuto del corpo del documento.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Aggiungendo alla fine del segmento (intestazione e piè di pagina)]</strong> </p> <p>Selezionare l’intestazione e il piè di pagina a cui si desidera inserire un’immagine e immettere l’URL immagine da inserire nei campi corrispondenti.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Altezza in punti/ampiezza in punti]</p> </td> 
   <td> <p>Definisci le dimensioni dell’immagine inserita. Il rapporto di formato sarà mantenuto.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sostituire un’immagine con una nuova immagine]

Questo modulo di azione sostituisce un’immagine esistente. Le proporzioni dell&#39;immagine originale vengono mantenute.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Selezionare un documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Selezionare questa opzione per mappare il modello di documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Selezionare questa opzione per scegliere il documento dal menu a discesa.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Selezionare il tipo di unità in cui si trova il documento che si desidera sostituire. Questa opzione è disponibile se hai selezionato [!UICONTROL By Dropdown] nel campo precedente.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selezionare la cartella in cui si trova il documento che si desidera sostituire, quindi selezionare il documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Condiviso Con Me]</strong> </p> <p>Selezionare la cartella in cui si trova il documento che si desidera sostituire, quindi selezionare il documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unità condivisa]</strong> (disponibile per [!DNL G Suite] solo utenti)</p> <p>Seleziona se desideri [!UICONTROL Utilizzare l’accesso amministratore di dominio]. Selezionando [!UICONTROL Sì] la richiesta viene generata come amministratore di dominio e vengono restituite tutte le unità condivise in cui il richiedente è un amministratore.</p> <p>Selezionare l'unità condivisa in cui si trova il documento che si desidera sostituire, quindi selezionare il documento.</p> <p>Nota: Se hai selezionato la [!DNL Google Docs] in questo campo e non sei un [!DNL G Suite] utente, errore <code>[400] Invalid Value</code> viene restituito .</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL immagine]</p> </td> 
   <td> <p>Immetti o mappa l’URL della nuova immagine che sostituirà l’immagine esistente.</p> <p>Le immagini vengono elencate nell’ordine in cui appaiono nel documento. Ad esempio: <code>Body: Image No. 1</code> è la prima immagine del documento.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sostituire il testo in un documento]

Questo modulo di azione sostituisce il testo in un documento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Selezionare un documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Selezionare questa opzione per mappare il modello di documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Selezionare questa opzione per scegliere il documento dal menu a discesa.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Selezionare il tipo di unità in cui si trova il documento a cui si desidera aggiungere testo. Questa opzione è disponibile se hai selezionato [!UICONTROL By Dropdown] nel campo precedente.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selezionare la cartella in cui si trova il documento a cui si desidera aggiungere testo, quindi selezionare il documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Condiviso Con Me]</strong> </p> <p>Selezionare la cartella in cui si trova il documento a cui si desidera aggiungere testo, quindi selezionare il documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unità condivisa]</strong> (disponibile per [!DNL G Suite] solo utenti)</p> <p>Seleziona se desideri [!UICONTROL Utilizzare l’accesso amministratore di dominio]. Selezionando [!UICONTROL Sì] la richiesta viene generata come amministratore di dominio e vengono restituite tutte le unità condivise in cui il richiedente è un amministratore.</p> <p>Selezionare l'unità condivisa in cui si trova il documento a cui si desidera aggiungere testo, quindi selezionare il documento.</p> <p>Nota: Se hai selezionato la [!DNL Google Docs] in questo campo e non sei un [!DNL G Suite] utente, errore <code>[400] Invalid Value</code> viene restituito .</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sostituire un testo]</p> </td> 
   <td> <p>Aggiungere ogni testo da sostituire.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Testo precedente da sostituire]</strong> </p> <p>Immettere il testo che si desidera sostituire.</p> </li> 
     <li> <p><strong>[!UICONTROL Nuovo testo da inserire]</strong> </p> <p>Inserisci il nuovo testo.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scaricare un documento]

Questo modulo di azione converte e scarica il documento selezionato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Selezionare il tipo di unità in cui si trova il documento da scaricare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selezionare la cartella in cui si trova il documento da scaricare, quindi selezionare il documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Condiviso Con Me]</strong> </p> <p>Selezionare la cartella in cui si trova il documento da scaricare, quindi selezionare il documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unità condivisa]</strong> (disponibile per [!DNL G Suite] solo utenti)</p> <p>Seleziona se desideri [!UICONTROL Utilizzare l’accesso amministratore di dominio]. Selezionando [!UICONTROL Sì] la richiesta viene generata come amministratore di dominio e vengono restituite tutte le unità condivise in cui il richiedente è un amministratore.</p> <p>Selezionare l'unità condivisa in cui si trova il documento da scaricare, quindi selezionare il documento.</p> <p>Nota: Se hai selezionato la [!DNL Google Docs] in questo campo e non sei un [!DNL G Suite] utente, errore <code>[400] Invalid Value</code> viene restituito .</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type] </p> </td> 
   <td> <p>Selezionare il formato del file di destinazione del documento scaricato.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un documento]

Questo modulo di azione elimina un documento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Selezionare il tipo di unità in cui si trova il documento da eliminare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selezionare la cartella in cui si trova il documento da eliminare, quindi selezionare il documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Condiviso Con Me]</strong> </p> <p>Selezionare la cartella in cui si trova il documento da eliminare, quindi selezionare il documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unità condivisa]</strong> (disponibile per [!DNL G Suite] solo utenti)</p> <p>Seleziona se desideri [!UICONTROL Utilizzare l’accesso amministratore di dominio]. Selezionando [!UICONTROL Sì] la richiesta viene generata come amministratore di dominio e vengono restituite tutte le unità condivise in cui il richiedente è un amministratore.</p> <p>Selezionare l'unità condivisa in cui si trova il documento da eliminare, quindi selezionare il documento.</p> <p>Nota: Se hai selezionato la [!DNL Google Docs] in questo campo e non sei un [!DNL G Suite] utente, errore <code>[400] Invalid Value</code> viene restituito .</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Unità condivisa]</td> 
   <td> <p>Selezionare l'unità contenente il documento che si desidera scaricare, quindi selezionare un documento. Questa opzione è disponibile se hai selezionato [!DNL Google Docs] nel campo [!UICONTROL Scegli un'unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Document ID]</td> 
   <td> <p> Selezionare o mappare il documento in cui si desidera sostituire una o più immagini.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Altro

* [[!UICONTROL Effettuare una chiamata API]](#make-an-api-call)
* [[!UICONTROL Fare clic su tutti i collegamenti di un documento]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL Effettuare una chiamata API]

Questo modulo di azione ti consente di eseguire una chiamata API personalizzata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Immettere un percorso relativo a <code>https://docs.googleapis.com/</code>. Esempio: <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Metodo]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard. Ad esempio, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] aggiunge le intestazioni di autorizzazione per te.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Immetti la stringa di query della richiesta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Esempio:** La seguente chiamata API recupera i dettagli del documento specificato nei documenti Google:

**URL:**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**Metodo:**

[!UICONTROL GET]

![](assets/api-call-example.png)

I dettagli del documento recuperato sono disponibili in Output del modulo in [!UICONTROL Bundle] > [!UICONTROL Corpo].

![](assets/api-output.png)

#### [!UICONTROL Fare clic su tutti i collegamenti di un documento]

Questo modulo di azione individua tutti i collegamenti presenti nel documento e li rende cliccabili.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Creare tutti i collegamenti in un documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Selezionare questa opzione per mappare il modello di documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Selezionare questa opzione per scegliere il documento dal menu a discesa.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Selezionare il tipo di unità in cui si trova il documento su cui si desidera rendere cliccabili i collegamenti. Questa opzione è disponibile se hai selezionato [!UICONTROL By Dropdown] nel campo precedente.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selezionare la cartella in cui si trova il documento in cui si desidera rendere cliccabili i collegamenti, quindi selezionare il documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Condiviso Con Me]</strong> </p> <p>Selezionare la cartella in cui si trova il documento in cui si desidera rendere cliccabili i collegamenti, quindi selezionare il documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unità condivisa]</strong> (disponibile per [!DNL G Suite] solo utenti)</p> <p>Seleziona se desideri [!UICONTROL Utilizzare l’accesso amministratore di dominio]. Selezionando [!UICONTROL Sì] la richiesta viene generata come amministratore di dominio e vengono restituite tutte le unità condivise in cui il richiedente è un amministratore.</p> <p>Selezionare l'unità condivisa in cui si trova il documento su cui si desidera rendere cliccabili i collegamenti, quindi selezionare il documento.</p> <p>Nota: Se hai selezionato la [!DNL Google Docs] in questo campo e non sei un [!DNL G Suite] utente, errore <code>[400] Invalid Value</code> viene restituito .</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Unità condivisa]</td> 
   <td> <p>Selezionare l'unità contenente il documento in cui si desidera aggiornare i collegamenti, quindi selezionare un documento. Questa opzione è disponibile se hai selezionato [!DNL Google Docs] nel [!UICONTROL Scegli un'unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Document ID]</td> 
   <td> <p> Selezionare o mappare il documento in cui si desidera aggiornare i collegamenti.</p> </td> 
  </tr> 
 </tbody> 
</table>
