---
title: Moduli MariaDB
description: In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL MariaDB], oltre a collegarlo a più applicazioni e servizi di terze parti.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 1%

---

# [!DNL MariaDB] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL MariaDB], oltre a collegarlo a più applicazioni e servizi di terze parti.

Per istruzioni sulla creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o versione successiva</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
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

## Prerequisiti

Da utilizzare [!DNL MariaDB] moduli, è necessario disporre di un [!DNL MariaDB] account.

## Connetti [!DNL MariaDB] a [!DNL Workfront Fusion]

Puoi creare una connessione al tuo [!DNL MariaDB] account direttamente dall&#39;interno di un [!DNL MariaDB] modulo.

1. In qualsiasi [!DNL MariaDB] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo.
1. Configura i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome connessione]</p> </td> 
      <td> <p>Immettere un nome per la nuova connessione.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Host]</td> 
      <td> <p>Immettere l'indirizzo IP o il nome host dell'istanza di database. L'host deve essere accessibile dall'esterno della rete.</p> <p>Esempio: <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Porta [!UICONTROL]</td> 
      <td>La porta predefinita è 3306. Se si utilizza una porta non standard, impostare questo numero sulla porta. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome Database]</td> 
      <td>Immettere il nome del database con cui si desidera interagire.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Username]</td> 
      <td>Immetti il nome utente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Password]</td> 
      <td>Immetti la password.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

## [!DNL MariaDB] Moduli e relativi campi

Quando si configura [!DNL MariaDB] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL MariaDB] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Eseguire una query (avanzata)

Questo modulo di azione recupera le informazioni dal database in base a una query fornita dall&#39;utente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla connessione [!DNL MariaDB] account a [!DNL Workfront Fusion], vedi <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Connetti [!DNL MariaDB] a [!DNL Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td> <p>Immettere la query SQL che si desidera venga utilizzata dal modulo per recuperare i dati.</p> <p>Importante: le variabili utilizzate nella query non vengono bonificate. Assicurati di bonificare correttamente le variabili per evitare l’iniezione SQL.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Seleziona righe da una tabella (avanzate)]

Questo modulo legge i record dal database.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla connessione [!DNL MariaDB] account a [!DNL Workfront Fusion], vedi <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Connetti [!DNL MariaDB] a [!DNL Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tabella [!UICONTROL]</td> 
   <td> <p>Selezionare la tabella contenente i record che si desidera leggere.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Imposta il filtro in base al quale desideri selezionare le righe</p> 
    <ul> 
     <li> <p>Selezionare il campo in base al quale si desidera eseguire la ricerca</p> </li> 
     <li> <p>Seleziona l’operatore da utilizzare per la ricerca</p> </li> 
     <li> <p>Immettere o mappare il valore che si desidera cercare.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort] </td> 
   <td> <p>Per ogni livello in cui si desidera ordinare i risultati, fare clic su <strong>[!UICONTROL Add item]</strong>, quindi selezionare il campo in base al quale si desidera ordinare i risultati e se si desidera ordinare in modo crescente o decrescente</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>
