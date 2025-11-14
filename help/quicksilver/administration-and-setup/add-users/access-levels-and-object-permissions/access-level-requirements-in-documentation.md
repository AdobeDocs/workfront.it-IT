---
title: Requisiti di accesso nella documentazione di Workfront
content-type: reference
product-area: system-administration
keywords: accesso,livello,sistema,amministratore,planner,lavoratore,revisore,richiedente,esterno,utente
navigation-topic: access-levels
description: Gli articoli descrittivi della documentazione di Workfront contengono una tabella che spiega gli accessi e le autorizzazioni necessari per tale procedura. Questo articolo illustra più dettagliatamente la tabella dei requisiti di accesso e contiene collegamenti per ulteriori informazioni.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 39ea0d53-ec31-4644-b772-cfe260b8e013
source-git-commit: c1c30696dc9ef324103467f3bdcb83609cf5d1d8
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 1%

---

# Requisiti di accesso nella documentazione di Workfront

Gli articoli descrittivi della documentazione di Workfront contengono una tabella che spiega i requisiti di accesso e autorizzazioni necessari per tale procedura. Questa tabella dei requisiti di accesso consente di capire se è possibile eseguire una determinata azione in Workfront o perché non è possibile eseguirla. Questo articolo illustra ogni elemento della tabella dei requisiti di accesso e fornisce suggerimenti per la risoluzione dei problemi e collegamenti a informazioni più approfondite.

Se una riga è assente dalla tabella dei requisiti di accesso in un determinato articolo, non vi sono requisiti di quel tipo per tale azione.

>[!NOTE]
>
>Per ulteriori informazioni sulle modalità di applicazione dei campi di questa tabella, contattare l&#39;amministratore di Workfront.

## Tabella dei requisiti di accesso

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> I pacchetti Adobe Workfront si riferiscono al set di funzioni acquistate dalla tua organizzazione. La maggior parte delle funzionalità di Workfront è disponibile in tutti i pacchetti, con alcune eccezioni, per lo più relative alla pianificazione strategica e ai controlli aziendali. <p>I pacchetti esistenti prima del 2022 non sono elencati.</p>
   <p>I pacchetti Workfront sono suddivisi in tre aree. Alcune aree offrono pacchetti diversi, ad esempio Select, Prime e Ultimate.<p>
   <ul>
   <li><b>Flusso di lavoro di Workfront</b>: include funzionalità relative alle operazioni, ad esempio gestione delle attività, approvazioni e schede attività. Questo pacchetto è ulteriormente suddiviso in pacchetti Workflow Select, Workflow Prime e Workflow Ultimate.</li>
   <li><b>Pianificazione Workfront</b>: include funzionalità relative alla pianificazione strategica. Questo pacchetto è ulteriormente suddiviso in Planning Select, Planning Prime e Planning Ultimate.</li>
   <li><b>Automazione e integrazione di Workfront</b>: include funzionalità relative all'automazione dei processi e all'integrazione con altre applicazioni.</li>
   </ul>
  <p>È possibile che la tua organizzazione abbia acquistato un pacchetto Workfront in una o più di queste aree.</p>
  <p>In precedenza, Workfront offriva pacchetti Workfront Select, Workfront Prime e Workfront Ultimate, senza distinguere tra flusso di lavoro, pianificazione e automazione e integrazione. La tua organizzazione potrebbe utilizzare uno di questi pacchetti legacy. 
   <ul><li>Per informazioni sul pacchetto Adobe Workfront utilizzato dalla tua organizzazione, compreso se l’organizzazione si trova nel modello di pacchetto corrente o legacy, contatta l’amministratore Workfront.</li>
   <li>Per istruzioni su come un amministratore di Workfront può individuare il pacchetto Workfront della tua organizzazione, consulta <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">Visualizzare il cluster e il pacchetto Workfront della tua organizzazione</a>.</li><li>Per ulteriori informazioni sui pacchetti Workfront, vedere <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront pricing and package</a>.</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> Le licenze di Adobe Workfront si riferiscono al set di funzioni di Workfront incluse nella licenza assegnata all’utente. Ad esempio, un utente potrebbe disporre di una licenza che include la contrassegnazione degli elementi di lavoro completati e del tempo di registrazione, mentre un altro utente potrebbe disporre di una licenza che consente loro di approvare solo le risorse o inviare richieste. <p> 
   <ul>
   <li>Per individuare la licenza assegnata, contattare l'amministratore di Workfront.</li>
   <li>Per informazioni sulle licenze, consulta:
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Panoramica sulle nuove licenze</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica sulle licenze</a></li></ul></li>
   <li>Se disponi del livello di accesso corretto e non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td><p>Poiché Workfront lavora a stretto contatto con altri prodotti Adobe, alcune procedure in Workfront interagiscono direttamente con tali prodotti. Per seguire tali procedure, l’organizzazione deve aver acquistato quel prodotto. Ad esempio, per utilizzare una funzionalità che consente a Workfront di interagire con Adobe Experience Manager Assets, la tua organizzazione deve aver acquistato Adobe Experience Manager Assets.</p>
   <p>Gli articoli che descrivono le procedure eseguite con prodotti aggiuntivi elencano il prodotto richiesto nella linea Prodotto di questa tabella.</p>
   <p>Per verificare se la tua organizzazione ha acquistato uno di questi prodotti aggiuntivi, contatta l’amministratore Workfront.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso</td> 
   <td> I livelli di accesso sono insiemi di autorizzazioni per le azioni che è possibile eseguire in Workfront, impostate dall'amministratore di Workfront. <p>Workfront dispone di livelli di accesso incorporati corrispondenti alle licenze Workfront, ma l’amministratore di Workfront può creare livelli di accesso più elevati per riflettere in modo più preciso i set di autorizzazioni necessari nell’organizzazione.</p>
   <ul>
    <li>Per informazioni sui livelli di accesso, vedere:
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">Panoramica dei nuovi livelli di accesso</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">Panoramica dei livelli di accesso</a></li></ul></li>
    <li>Per informazioni dettagliate sul livello di accesso, contattare l'amministratore Workfront</li>
    <li>Se sei un amministratore di Workfront, consulta <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurare l'accesso ad Adobe Workfront</a> per ulteriori informazioni sulla concessione dell'accesso a oggetti specifici nel livello di accesso.</li>  
   <li>Se disponi del livello di accesso corretto e non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td><p>Le autorizzazioni per gli oggetti si riferiscono all'accesso ai singoli oggetti di Workfront quando vengono creati o condivisi con l'utente. Ad esempio, per visualizzare un progetto specifico è necessario disporre dell'accesso di visualizzazione, anche se il proprio livello di accesso consente di visualizzare i progetti. Questa sezione della tabella dei requisiti di accesso descrive tutte le autorizzazioni specifiche per gli oggetti necessarie per eseguire l'azione descritta nell'articolo.</p>
   <p>Per informazioni sulla richiesta di accesso aggiuntivo a un oggetto, vedere <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti</a>.</p><p>Per informazioni sulla condivisione di un oggetto, vedere <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md" class="MCXref xref">Condividere un oggetto</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Modello layout</td> 
   <td><p>I modelli di layout controllano ciò che è possibile visualizzare nel menu principale e sono configurati dall’amministratore di Workfront. Questa riga indica le aree specifiche di Workfront che devono essere incluse nel menu principale per eseguire l’azione.</p><p>In generale, se un articolo indica di fare clic su un'area del menu principale che non è visibile nel menu principale, contattare l'amministratore di Workfront per determinare se tale area può essere resa disponibile.</p><p>
   Per informazioni su come un amministratore di Workfront può configurare il menu principale, vedere <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref">Personalizzare il menu principale utilizzando un modello di layout</a>.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront Fusion</td> 
   <td>Adobe Workfront Fusion dispone di un modello di licenza separato rispetto a Workfront. 
   <ul><li>Il modello di licenza corrente si basa sul numero di operazioni eseguite e non ha limitazioni sulle azioni che un'organizzazione può eseguire. </li>
   <li>Le licenze legacy si basano sulla capacità degli scenari di connettersi ad applicazioni di terze parti o sull’utilizzo degli scenari solo per l’automazione di Workfront. </li>
   </ul>
   Per informazioni sulle licenze Fusion, vedere <a href="https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration" class="MCXref xref">Licenze Workfront Fusion</a>.
   </td> 
  </tr> 
 </tbody> 
</table>
