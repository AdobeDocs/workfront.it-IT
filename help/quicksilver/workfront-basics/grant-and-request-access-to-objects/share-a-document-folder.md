---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Condividere una cartella documenti
description: È possibile condividere una cartella e il relativo contenuto dall'area Documenti.
author: Alina
feature: Get Started with Workfront
exl-id: c0d318a8-b1cf-4522-b478-acf092687658
source-git-commit: 3bd377ba2dec29bb956632cf3e9e3e33afe4305d
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# Condividere una cartella documenti

È possibile condividere una cartella e il relativo contenuto dall&#39;area Documenti.

>[!NOTE]
>
>* La cartella deve trovarsi nei primi cinque livelli di una gerarchia di cartelle su un oggetto. Ogni cartella al sesto livello o inferiore eredita le configurazioni di condivisione dalla cartella direttamente al di sopra di essa.
>
>  Per informazioni sull&#39;aggiunta di sottocartelle per creare una gerarchia di cartelle, vedere la sezione [Creare cartelle e sottocartelle](../../documents/organizing-documents/create-documents-folder.md#creating-folders) nell&#39;articolo [Creare cartelle di documenti](../../documents/organizing-documents/create-documents-folder.md).
>
>* Impossibile condividere le cartelle avanzate.
>* Se si configurano le opzioni di condivisione per una cartella documenti all&#39;interno di un modello e successivamente viene creato un progetto da tale modello, le configurazioni di condivisione non vengono trasferite alla cartella documenti nel nuovo progetto.
>* Se si configurano le opzioni di condivisione per una cartella di documento all&#39;interno di un elemento di lavoro e quindi si copia l&#39;elemento di lavoro, le configurazioni di condivisione non vengono trasferite alla cartella di documento nel nuovo elemento di lavoro.
>

## Requisiti di accesso

<!--drafted for P&P
(I am putting Contributor and higher here because this is what I found in testing. Normally, Review equals Light but I found out that Contributor can also have manage rights to documents and can share them.)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Review or higher</p>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Documents</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to an object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Visualizza accesso ai documenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di visualizzazione a un oggetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Condividere una cartella

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Documenti**.

   Oppure

   Con un oggetto Workfront aperto, fai clic su **Documenti** nel pannello a sinistra.

1. Selezionare la cartella, quindi fare clic sull&#39;icona Condividi ![](assets/share-icon.png) nella barra degli strumenti.

   La cartella deve trovarsi nei primi cinque livelli di una gerarchia di cartelle su un oggetto e non può essere una cartella avanzata.

1. Nella casella visualizzata, in **Concedi l&#39;accesso alla cartella a**, inizia a digitare il nome dell&#39;utente, del team, della mansione, del gruppo o della società con cui vuoi condividere la cartella, quindi premi **Invio** quando viene visualizzato il nome.
1. Per regolare l’accesso per l’utente, il team, la mansione, il gruppo o la società appena aggiunti, fai clic sul menu a discesa a destra del nome, quindi configura una delle seguenti opzioni disponibili e le relative impostazioni avanzate:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visualizzare</td> 
      <td> <p>Possibilità di visualizzare la cartella e il suo contenuto.</p> <p>Fare clic su <strong>Impostazioni avanzate</strong> per specificare se si desidera consentire quanto segue:</p> 
       <ul> 
        <li><strong>Download</strong>: possibilità di scaricare la cartella e il relativo contenuto come file ZIP</li> 
        <li> <p><strong>Condividi</strong>: possibilità di condividere la cartella con altri utenti nel sistema</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gestire</td> 
      <td> <p>Possibilità di visualizzare e modificare la cartella e il suo contenuto</p> <p>Fare clic su <strong>Impostazioni avanzate</strong> per specificare se si desidera consentire agli utenti di eseguire le operazioni seguenti:</p> 
       <ul> 
        <li><strong>Elimina</strong>: elimina la cartella e il relativo contenuto dal sistema</li> 
        <li><b>Scarica</b>: scarica la cartella e il suo contenuto come file ZIP</li> 
        <li><strong>Condividi</strong>: condividi la cartella e il relativo contenuto con altri utenti nel sistema</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Ripeti i passaggi 3-4 per aggiungere altri nomi all’elenco e configurarne le opzioni.
1. (Facoltativo) Se desideri che tutti gli utenti del sistema possano visualizzare la cartella e il suo contenuto, fai clic sull&#39;icona a forma di ingranaggio ![](assets/gear-icon-settings-with-dn-arrow.jpg) nell&#39;angolo superiore destro della casella di condivisione, quindi fai clic su **Rendi visibile a livello di sistema.**

   Se cambi idea, puoi fare clic su **Rimuovi accesso a livello di sistema** (opzione predefinita).

## Modalità di accesso degli utenti al contenuto di una cartella condivisa con loro

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Delete these 2 paragraphs when the story &nbsp;<a href="https://hub.workfront.com/task/622f8d6f000897c9a4a11bdfd9b2cf34/overview">Handle email notification content when a folder is shared</a> goes to Preview:</p>
-->

Attualmente, quando si condivide una cartella, i destinatari non la visualizzano nell&#39;area Documenti. Tuttavia, possono accedere ai relativi documenti eseguendo un rapporto sui documenti.

Per informazioni sull&#39;esecuzione di un report, vedere la sezione [Report sugli oggetti](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) nell&#39;articolo [Comprendere gli oggetti in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md). Vedi anche [Creare un rapporto personalizzato](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Workfront sends a notification email when someone shares a document folder on an object with a user or a team. To access the folder from the email, recipients can click the folder title or the "See it in Workfront" link.</p> <note type="note">
<ul class="preview">
<li> <p>The email notification "Someone shares an object with me" or "Someone shares an object with my team" must be enabled in order for a user or team to receive a notification email about a shared folder.</p> </li>
<li> <p>When someone shares a document folder from the global Documents area, the links in the notification email take the recipient to the global Documents area. Because folders in this area are private, the shared folder is not displayed there, but the recipient can access its documents by creating a document report. </p> <p>For information about running a report, see the section <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects" class="MCXref xref">Report on objects</a> in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. Also see <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li>
<li> <p>Currently, it is not possible to share folders with external users.</p> </li>
</ul>
</note>
</div>
-->

## Autorizzazioni ereditate quando si condivide un oggetto contenente una cartella

Quando si condivide un oggetto che ha una cartella documenti, i destinatari possono accedere anche alla cartella:

* Se concedi ai destinatari l’accesso in visualizzazione all’oggetto principale, avranno l’accesso in visualizzazione alla cartella.
* Se concedi ai destinatari l’accesso Contribute o Manage all’oggetto principale, questi dispongono dell’accesso Manage alla cartella.
* Se si concede un tipo di accesso (Visualizza, Contribute o Gestisci) all&#39;oggetto padre e un altro tipo alla cartella, i destinatari disporranno del più alto di questi due tipi di accesso ai documenti della cartella

  Ad esempio, se condividi l’oggetto principale con accesso in visualizzazione e la cartella con accesso in gestione, i destinatari dispongono di accesso in gestione ai documenti della cartella.

  >[!NOTE]
  >
  >Un documento allegato eredita le autorizzazioni solo dall&#39;oggetto a cui è stato associato. Se si crea una cartella sull&#39;oggetto e si sposta il documento nella cartella, questa eredita le autorizzazioni della cartella. Tuttavia, se si crea una cartella su un oggetto padre o padre e si sposta il documento in tale cartella, questa non eredita le autorizzazioni della cartella.

* Se nel livello di accesso del destinatario è abilitata l’opzione &quot;Non ereditare mai l’accesso ai documenti da progetti, attività, problemi, ecc.&quot;, il destinatario non erediterà le autorizzazioni per i documenti in una cartella condivisa con lui. Per consentire l&#39;accesso a un documento nella cartella, è necessario condividere il documento.

  Per informazioni sull&#39;opzione &quot;Mai ereditare&quot;, vedere [Configurare l&#39;accesso ad Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

  Per informazioni sulla condivisione di un documento, vedere [Condividere un documento](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).
