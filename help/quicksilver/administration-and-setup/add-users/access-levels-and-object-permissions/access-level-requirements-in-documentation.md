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
source-git-commit: cb38223c4dd8048fd2ab105abce2c9a79b84c43f
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 1%

---

# Requisiti di accesso nella documentazione di Workfront

Gli articoli descrittivi della documentazione di Workfront contengono una tabella che spiega i requisiti di accesso e autorizzazioni necessari per tale procedura. Questa tabella dei requisiti di accesso consente di capire se è possibile eseguire una determinata azione in Workfront o perché non è possibile eseguirla. Questo articolo illustra ogni elemento della tabella dei requisiti di accesso e fornisce suggerimenti per la risoluzione dei problemi e collegamenti a informazioni più approfondite.

Se una riga è assente dalla tabella dei requisiti di accesso in un determinato articolo, non vi sono requisiti di quel tipo per tale azione.

Alcune righe contengono informazioni etichettate come &quot;Nuovo&quot; e &quot;Corrente&quot;. Questo perché Workfront sta passando a un nuovo modello di prezzi e imballaggio, con alcune organizzazioni che operano con il nuovo modello e altre che utilizzano ancora il modello corrente. Per individuare il modello utilizzato dall’organizzazione, contatta l’amministratore di Workfront. Puoi trovare dettagli e collegamenti alle informazioni nella sezione [Tabella dei requisiti di accesso](#the-access-requirements-table) di questo articolo.

>[!NOTE]
>
>Per ulteriori informazioni sulle modalità di applicazione dei campi di questa tabella, contattare l&#39;amministratore di Workfront.

## Tabella dei requisiti di accesso

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> I piani di Adobe Workfront si riferiscono all’insieme di funzioni acquistate dalla tua organizzazione. La maggior parte delle funzionalità di Workfront è disponibile in tutti i piani, con alcune eccezioni, per lo più relative alla pianificazione strategica e ai controlli aziendali. 
   <ul><li>Per informazioni sul piano Adobe Workfront utilizzato dalla tua organizzazione, compreso se l’organizzazione si trova nel modello di packaging nuovo o corrente, contatta l’amministratore Workfront.</li>
   <li>Per istruzioni su come un amministratore di Workfront può individuare il piano Workfront della tua organizzazione, consulta <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan" class="MCXref xref">Visualizzare il piano Workfront e il cluster della tua organizzazione</a>.</li><li>Per ulteriori informazioni sui nuovi piani di Workfront, vedere <a href="https://business.adobe.com/products/workfront/pricing.html">Determinazione prezzi e creazione pacchetti di Adobe Workfront</a>.</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> Le licenze di Adobe Workfront si riferiscono al set di funzioni di Workfront incluse nella licenza assegnata all’utente. Ad esempio, un utente potrebbe disporre di una licenza che include la contrassegnazione degli elementi di lavoro completati e del tempo di registrazione, mentre un altro utente potrebbe disporre di una licenza che consente loro di approvare solo le risorse o inviare richieste. <p> 
   <ul>
   <li>Per individuare la licenza assegnata, contattare l'amministratore di Workfront.</li>
   <li>Adobe Workfront sta passando a un nuovo modello di prezzi e packaging. Per informazioni sulle licenze, consulta:
   <ul>
   <li>Nuovo: <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Panoramica nuove licenze</a></li>
   <li>Corrente: <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica licenze</a></li></ul></li>
   <li>Se disponi del livello di accesso corretto e non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>Workfront offre alcuni prodotti che possono essere acquistati oltre a Workfront.
   <p>Gli articoli che descrivono le procedure eseguite all’interno di questi prodotti aggiuntivi elencano qui il prodotto richiesto.</p>
   <ul>
   <li>ADOBE EXPERIENCE MANAGER ASSETS o ASSETS ESSENTIALS </li>
   <li>Workfront Fusion</li>
   <li>Workfront Goals</li>
   <li>Pianificazione scenario in Workfront</li>
   <li>Pianificazione Workfront</li>
   </ul>
   <p>Per verificare se la tua organizzazione ha acquistato uno di questi prodotti aggiuntivi, contatta l’amministratore Workfront.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso</td> 
   <td> I livelli di accesso sono insiemi di autorizzazioni per le azioni che è possibile eseguire in Workfront, impostate dall'amministratore di Workfront. <p>Workfront dispone di livelli di accesso incorporati corrispondenti alle licenze Workfront, ma l’amministratore di Workfront può creare livelli di accesso più elevati per riflettere in modo più preciso i set di autorizzazioni necessari nell’organizzazione.</p>
   <ul>
    <li>Adobe Workfront sta passando a un nuovo modello di prezzi e packaging. Per informazioni sui livelli di accesso per ciascun modello, consulta:
   <ul>
   <li>Nuovo: <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">Panoramica sui nuovi livelli di accesso</a></li>
   <li>Corrente: <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">Panoramica dei livelli di accesso</a></li></ul></li>
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
   <td role="rowheader">Modello di layout</td> 
   <td><p>I modelli di layout controllano ciò che è possibile visualizzare nel menu principale e sono configurati dall’amministratore di Workfront. Questa riga indica le aree specifiche di Workfront che devono essere incluse nel menu principale per eseguire l’azione.</p><p>In generale, se un articolo indica di fare clic su un'area del menu principale che non è visibile nel menu principale, contattare l'amministratore di Workfront per determinare se tale area può essere resa disponibile.</p><p>
   Per informazioni su come un amministratore di Workfront può configurare il menu principale, vedere <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref">Personalizzare il menu principale utilizzando un modello di layout</a>.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront Fusion</td> 
   <td>Adobe Workfront Fusion dispone di un modello di licenza separato rispetto a Workfront. 
   <ul><li>Corrente: il modello di licenza corrente si basa sul numero di operazioni eseguite e non ha limitazioni sulle azioni che un'organizzazione può eseguire. </li>
   <li>Legacy: le licenze legacy si basano sulla capacità degli scenari di connettersi ad applicazioni di terze parti o sull’utilizzo degli scenari solo per l’automazione di Workfront. </li>
   </ul>
   Per informazioni sulle licenze Fusion, vedere <a href="https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration" class="MCXref xref">Licenze Workfront Fusion</a>.
   </td> 
  </tr> 
 </tbody> 
</table>
