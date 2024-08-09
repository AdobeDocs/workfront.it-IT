---
user-type: administrator
content-type: overview
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Panoramica del firewall
description: Poiché Adobe Workfront comunica con la rete della tua organizzazione, il firewall di quest’ultima deve essere configurato in modo da consentire tale comunicazione. I firewall sono misure di sicurezza altamente efficaci che funzionano separando la rete di un'organizzazione da Internet. Garantiscono che solo i dati e il traffico di rete selezionati possano essere spostati all’interno o all’esterno della rete dell’organizzazione. Il firewall consente o blocca i dati in base al sito che invia o riceve i dati. In qualità di amministratore di Adobe Workfront, devi assicurarti che i dati inviati a o da Workfront possano passare attraverso il firewall dell’organizzazione.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 172999e7-fb05-49a6-ad57-84b59e80a28e
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# Panoramica del firewall

Poiché Adobe Workfront comunica con la rete della tua organizzazione, il firewall di quest’ultima deve essere configurato in modo da consentire tale comunicazione. I firewall sono misure di sicurezza altamente efficaci che funzionano separando la rete di un&#39;organizzazione da Internet. Garantiscono che solo i dati e il traffico di rete selezionati possano essere spostati all’interno o all’esterno della rete dell’organizzazione. Il firewall consente o blocca i dati in base al sito che invia o riceve i dati. In qualità di amministratore di Adobe Workfront, devi assicurarti che i dati inviati a o da Workfront possano passare attraverso il firewall dell’organizzazione.

Ciò viene realizzato attraverso un inserisco nell&#39;elenco Consentiti di, che è essenzialmente un &quot;elenco&quot; di siti che sono &quot;autorizzati&quot; a inviare o ricevere dati attraverso il firewall. I siti possono essere identificati in due modi:

* **Indirizzo IP**: una serie di numeri come 52.31.132.175
* **Dominio**: parte di un URL, ad esempio &quot;thisdomain&quot; in www.thisdomain.com

Workfront utilizza indirizzi IP e domini specifici per la comunicazione web. Per poter utilizzare Workfront nell’organizzazione, è necessario aggiungerle al inserisco nell&#39;elenco Consentiti di dell’organizzazione.

In genere, un amministratore di rete configura un inserisco nell&#39;elenco Consentiti di rete. Rivolgiti all’amministratore di rete della tua organizzazione per assicurarti che il firewall consenta tali indirizzi IP. Se non si conosce il nome dell&#39;amministratore di rete, il reparto IT dell&#39;organizzazione può indirizzare l&#39;utente nella giusta direzione.

>[!IMPORTANT]
>
>In qualità di amministratore di Workfront, devi assicurarti che tali indirizzi IP e domini vengano aggiunti al inserisco nell&#39;elenco Consentiti di gestione dei della tua organizzazione. Questo vale anche se non li aggiungi tu stesso. Workfront non è in grado di configurare il inserisco nell&#39;elenco Consentiti di della tua organizzazione.

## Raccolta di informazioni per la configurazione del firewall

Per configurare il firewall per Workfront, l&#39;amministratore di rete deve sapere quali indirizzi IP e domini aggiungere. Alcune di queste informazioni sono disponibili solo per un amministratore di Workfront. In qualità di amministratore di Workfront, è necessario individuare queste informazioni e fornirle all&#39;amministratore di rete.

>[!NOTE]
>
>La best practice per la sicurezza prevede l’aggiunta di solo gli indirizzi IP e i domini che si connettono alle funzionalità utilizzate attivamente dalla tua organizzazione. Fornendo queste informazioni, puoi assicurarti di seguire questa best practice.

Fornire all&#39;amministratore di rete le informazioni seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Indirizzi IP e domini specifici da consentire</td> 
   <td> <p>L'articolo <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">Configurare il inserisco nell'elenco Consentiti di del firewall</a> contiene l'elenco degli indirizzi IP e dei domini che l'organizzazione deve aggiungere al proprio inserisco nell'elenco Consentiti di. </p> <p>È possibile che l'amministratore di rete non abbia accesso all'articolo "Configurare il inserisco nell'elenco Consentiti di configurazione del firewall" per il sistema di protezione. In tal caso, devi fornirlo a loro. Si sconsiglia di stampare una copia cartacea. Una copia digitale consente all'amministratore di rete di copiare e incollare gli indirizzi, in modo più rapido e preciso rispetto alla digitazione da una copia cartacea.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Il cluster</td> 
   <td>Per individuare il cluster dell'organizzazione, vedere <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Visualizzare il cluster e il piano Workfront dell'organizzazione</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Piano Workfront</td> 
   <td> <p>Per individuare il piano dell'organizzazione, vedere <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Visualizzare il cluster e il piano Workfront dell'organizzazione.</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Il tuo dominio</td> 
   <td> <p>Per individuare il dominio, controllare l'indirizzo Web utilizzato per la connessione a Workfront.</p> <p>Esempio: nell'indirizzo Web <code>greatcompany.my.workfront.com</code>, il dominio è "grand company"</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Altri prodotti Adobe Workfront</td> 
   <td> <p>Informare l'amministratore di rete se si dispone di licenze per uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Bozza di Adobe Workfront</p> </li> 
     <li> <p>Adobe Workfront Fusion </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Integrazioni Adobe Workfront</td> 
   <td>Informare l'amministratore di rete se si utilizza uno dei seguenti elementi:
    <ul>
     <li><p>Workfront per Jira</p></li>
     <li><p>Workfront per Google Workspace</p></li>
     <li><p>Workfront per Microsoft Teams</p></li>
     <li><p>Workfront per Outlook</p></li>
     <li><p>Workfront per Salesforce</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Funzionalità aggiuntive</td> 
   <td> <p>Informare l'amministratore di rete se si utilizza quanto segue:</p> 
    <ul> 
     <li> <p>Un'unità di prova Workfront</p> </li> 
    </ul> </td>
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>Se aggiungi uno di questi prodotti, integrazioni o funzionalità in una data successiva, devi contattare l’amministratore di rete in modo che possa regolare il inserisco nell&#39;elenco Consentiti di.

### Visualizza il piano Workfront e il cluster della tua organizzazione {#view-your-organization-s-cluster-and-workfront-plan}

{{step-1-to-setup}}

1. Fai clic su **Sistema** nel pannello a sinistra
1. Per Visualizzare Il Cluster, Selezionare **Informazioni Cliente**.

   Il cluster viene visualizzato nella parte superiore destra della sezione **Informazioni di base**.

   ![](assets/locate-cluster.png)

1. Per visualizzare il piano Workfront, selezionare **Licenze**.

   Il piano viene visualizzato nell’angolo superiore destro della pagina.

   ![](assets/locate-plan.png)
