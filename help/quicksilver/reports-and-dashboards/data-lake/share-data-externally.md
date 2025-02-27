---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Stabilire una connessione a Workfront Data Connect
description: Workfront Data Connect consente di utilizzare i dati Workfront della propria organizzazione con strumenti di business intelligence o di memorizzarli in un data warehouse esterno.
author: Nolan
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: ea9c674b798c48927c7a0a542d36d5ded15ea3f1
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 1%

---

# Stabilire una connessione a Workfront Data Connect

Workfront Data Connect consente di utilizzare i dati Workfront della propria organizzazione con strumenti di business intelligence o di memorizzarli in un data warehouse esterno.

Per collegare il data lake Data Connect a un prodotto esterno, è necessario innanzitutto creare una connessione come descritto in [Creare un account o una connessione di lettura per Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md). Quindi, devi aggiungere tutti gli IP richiesti al inserisco nell&#39;elenco Consentiti di come descritto in [Aggiungere gli IP al inserisco nell&#39;elenco Consentiti di](#add-ips-to-the-allowlist) di seguito.

La maggior parte dei prodotti richiede le seguenti informazioni sul data lake per stabilire una connessione:

| Nome campo | Valore |
|---------------|-------------|
| Server | L&#39;URL per la connessione, senza la porzione `https://` (trovata nella pagina **Connessione dati** in Workfront*) |
| Porta | `443` |
| Database | `WORKFRONT` |
| Data warehouse | `READER_WH` |
| Schema | `WF` |
| Ruolo | `READER_ROLE` |
| Nome utente | Il nome utente scelto durante la creazione della connessione (trovato nella pagina **Connessione dati** in Workfront*) |
| Password | La password scelta al primo accesso a Snowflake* |

*Per informazioni su dove trovare la pagina **Connessione dati** contenente le connessioni, vedere [Creare un account o una connessione di lettura per Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Una volta aggiunta una voce al inserisco nell&#39;elenco Consentiti di, tutti gli altri indirizzi IP non sono più consentiti. Prima di utilizzare lo strumento, assicurati di aver inserito tutti gli indirizzi IP richiesti, sia per la creazione che per la lettura dello strumento di visualizzazione. In caso contrario, potrebbe verificarsi un errore relativo alle credenziali non valide.
>
>Se nel elenco Consentiti non è incluso alcun indirizzo IP ma si verificano ancora problemi di connessione a uno strumento BI, controllare la configurazione del server proxy per lo strumento BI.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td><p>Incluso nei seguenti piani:</p>
    <ul>
        <li><p>Ultimate</p></li> 
    </ul>    
   <!--<p>Can be purchased as an add-on to the following plans:</p> 
    <ul>
        <li>Select</li> 
        <li>Prime</li>
    </ul>--> 
    <p>Workfront Data Connect non è disponibile per i piani Workfront legacy.</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungere IP al inserisco nell&#39;elenco Consentiti di

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **Setup**.

1. Nel pannello a sinistra, fai clic su **Sistema** > **Connessione dati**.

1. Fai clic sulla scheda **IP consentiti**, quindi fai clic sul pulsante **Aggiungi un indirizzo IP al tuo Inserisco nell&#39;elenco Consentiti di**.

1. Immettere un nome per l&#39;indirizzo IP in **Descrizione indirizzo IP** e immettere l&#39;indirizzo IP (o blocco CIDR) per lo strumento che si desidera utilizzare in **Indirizzo IP**, quindi fare clic su **Aggiungi IP da Inserire nell&#39;elenco Consentiti**.

   ![Aggiungi indirizzo IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Rimozione di un indirizzo IP dal inserisco nell&#39;elenco Consentiti di

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **Setup**.

1. Nel pannello a sinistra, fai clic su **Sistema** > **Connessione dati**.

1. Fai clic sulla scheda **IP consentiti**, quindi fai clic sull&#39;icona cestino ![icona Elimina](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) a destra dell&#39;indirizzo IP che desideri rimuovere.

1. Nella finestra visualizzata, selezionare la casella per confermare e quindi fare clic su **Elimina**.

## Condividere i dati con gli strumenti di Business Intelligence

Di seguito sono elencati alcuni strumenti comuni di business intelligence. Per ulteriori informazioni sulla connessione al data lake, visita i relativi siti di documentazione.

* Tableau
* Power BI
* Domo
* SAP HANA

## Archiviare dati in un data warehouse esterno

Di seguito sono elencati alcuni data warehouse comuni; visita i relativi siti di documentazione per ulteriori informazioni sulla connessione al data lake.

* Database
* AWS Redshift
