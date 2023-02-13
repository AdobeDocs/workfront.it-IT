---
user-type: administrator
content-type: overview
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Panoramica del firewall
description: Poiché Adobe Workfront comunica con la rete dell’organizzazione, per consentire tale comunicazione è necessario configurare il firewall dell’organizzazione. I firewall sono misure di sicurezza altamente efficaci che funzionano separando la rete di un'organizzazione da Internet. Garantiscono che solo i dati selezionati e il traffico di rete possano entrare o uscire dalla rete dell'organizzazione. Il firewall consente o blocca i dati in base al sito che invia o riceve i dati. In qualità di amministratore di Adobe Workfront, devi assicurarti che i dati inviati a o da Workfront possano passare attraverso il firewall dell’organizzazione.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 172999e7-fb05-49a6-ad57-84b59e80a28e
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# Panoramica del firewall

Poiché Adobe Workfront comunica con la rete dell’organizzazione, per consentire tale comunicazione è necessario configurare il firewall dell’organizzazione. I firewall sono misure di sicurezza altamente efficaci che funzionano separando la rete di un&#39;organizzazione da Internet. Garantiscono che solo i dati selezionati e il traffico di rete possano entrare o uscire dalla rete dell&#39;organizzazione. Il firewall consente o blocca i dati in base al sito che invia o riceve i dati. In qualità di amministratore di Adobe Workfront, devi assicurarti che i dati inviati a o da Workfront possano passare attraverso il firewall dell’organizzazione.

Questo viene eseguito tramite un inserì nell&#39;elenco Consentiti, che è essenzialmente un &quot;elenco&quot; di siti che sono &quot;autorizzati&quot; a inviare o ricevere dati attraverso il firewall. I siti possono essere identificati in uno dei due modi seguenti:

* **Indirizzo IP**: una serie di numeri quali 52.31.132.175
* **Dominio**: parte di un URL, ad esempio &quot;questo dominio&quot; in www.thisdomain.com

Workfront utilizza indirizzi IP e domini specifici per la comunicazione web. Devono essere aggiunti all’inserire nell&#39;elenco Consentiti dell’organizzazione prima di poter utilizzare Workfront nell’organizzazione.

In genere, un amministratore di rete configura un inserì nell&#39;elenco Consentiti. Rivolgiti all’amministratore di rete della tua organizzazione per verificare che il firewall consenta tali indirizzi IP. Se non sai chi sia l&#39;amministratore di rete, il reparto IT della tua organizzazione può indirizzarti nella direzione giusta.

>[!IMPORTANT]
>
>In qualità di amministratore di Workfront, devi accertarti che questi indirizzi IP e domini siano aggiunti all’inserire nell&#39;elenco Consentiti della tua organizzazione. Questo è vero anche se non li aggiungi tu stesso. Workfront non può configurare l&#39;inserire nell&#39;elenco Consentiti dell&#39;organizzazione.

## Raccolta di informazioni per la configurazione del firewall

Per configurare il firewall per Workfront, l’amministratore di rete deve sapere quali indirizzi IP e domini aggiungere. Alcune di queste informazioni sono disponibili solo per un amministratore Workfront. In qualità di amministratore di Workfront, è necessario individuare queste informazioni e fornirle all&#39;amministratore di rete.

>[!NOTE]
>
>La best practice per la sicurezza consiste nell’aggiungere solo gli indirizzi IP e i domini che si connettono alla funzionalità che la tua organizzazione utilizza attivamente. Fornendo queste informazioni, puoi garantire che questa best practice sia seguita.

Fornisci all’amministratore di rete le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Indirizzi IP e domini specifici per consentire</td> 
   <td> <p>L'articolo <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">Configurare l’inserire nell'elenco Consentiti del firewall</a> contiene l’elenco degli indirizzi IP e dei domini che la tua organizzazione deve aggiungere al proprio inserire nell'elenco Consentiti. </p> <p>L'amministratore di rete potrebbe non avere accesso all'articolo "Configurare il firewall". In tal caso, devi fornirlo a loro. Si sconsiglia di stampare una copia cartacea. Una copia digitale consente all’amministratore di rete di copiare e incollare gli indirizzi, in modo più rapido e preciso rispetto alla digitazione da una copia cartacea.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Il cluster</td> 
   <td>Per individuare il cluster dell'organizzazione, vedi <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Visualizza il cluster della tua organizzazione e il piano Workfront</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Il piano Workfront</td> 
   <td> <p>Il piano della tua organizzazione è uno dei seguenti:</p> 
    <ul> 
     <li> <p>Enterprise </p> </li> 
     <li> <p>Business </p> </li> 
     <li> <p>Pro </p> </li> 
     <li> <p>Team </p> </li> 
    </ul> <p>Per individuare il piano, vedi <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Visualizza il cluster della tua organizzazione e il piano Workfront.</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Il tuo dominio</td> 
   <td> <p>Per individuare il dominio, controllare l'indirizzo Web utilizzato per la connessione a Workfront.</p> <p>Esempio: all'indirizzo web <code>greatcompany.my.workfront.com</code>, il dominio è "azienda grandiosa"</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Altri prodotti Adobe Workfront</td> 
   <td> <p>Informare l'amministratore di rete se si dispone di licenze per uno dei seguenti casi:</p> 
    <ul> 
     <li> <p>Prova Adobe Workfront</p> </li> 
     <li> <p>Adobe Workfront Fusion </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Integrazioni Adobe Workfront</td> 
   <td>Informare l'amministratore di rete se si utilizza una delle seguenti opzioni:
    <ul>
     <li><p><p>Workfront per Jira</p></p></li>
     <li><p>Workfront per G Suite</p></li>
     <li><p>Workfront per Microsoft Teams</p></li>
     <li><p>Workfront per Outlook</p></li>
     <li><p>Workfront per Salesforce</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Funzionalità aggiuntive</td> 
   <td> <p>Informare l'amministratore di rete se si utilizza una delle seguenti opzioni:</p> 
    <ul> 
     <li> <p>Un'unità di prova Workfront</p> </li> 
     <li> <p>Workfront Ascent</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>Se aggiungi uno qualsiasi di questi prodotti, integrazioni o funzionalità in un secondo momento, contatta l’amministratore di rete in modo che possa regolare l’inserire nell&#39;elenco Consentiti.

### Visualizza il cluster della tua organizzazione e il piano Workfront {#view-your-organization-s-cluster-and-workfront-plan}

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Sistema** nel pannello a sinistra
1. Per visualizzare il cluster, seleziona **Informazioni cliente**.

   Il cluster viene visualizzato in alto a destra **Informazioni di base** sezione .

   ![](assets/locate-cluster.png)

1. Per visualizzare il piano Workfront, seleziona **Licenze**.

   Il piano viene visualizzato nella parte inferiore della pagina.

   ![](assets/locate-plan.png)
