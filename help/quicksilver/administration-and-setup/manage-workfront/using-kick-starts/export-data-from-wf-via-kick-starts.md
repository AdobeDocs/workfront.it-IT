---
user-type: administrator
product-area: system-administration
keywords: kickstart, calcio d'inizio, kickstart, calcio d'inizio
navigation-topic: use-kick-starts
title: Esportare dati da Adobe Workfront tramite Kick-Starts
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare l’esportatore di dati Kick-Starts per esportare dati da Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1101'
ht-degree: 9%

---

# Esportare dati da Adobe Workfront tramite Kick-Starts

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

In qualità di amministratore di Adobe Workfront, puoi utilizzare l’esportatore di dati Kick-Starts per esportare dati da Workfront. Puoi utilizzarlo in altre applicazioni dopo averlo esportato.

L’esportazione dei dati tramite Kick-Starts è utile anche per comprendere quali campi sono associati a ciascun oggetto, come questi campi sono codificati e come i valori di questi campi vengono formattati nel database.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Vantaggi e svantaggi dell&#39;utilizzo di calcio per esportare i dati

In Workfront sono disponibili due modi per esportare i dati:

* Esportazione di dati da un report o da un elenco

   Per ulteriori informazioni sull&#39;esportazione di dati da un report o da un elenco, consulta [Esportare i dati](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* Esportazione di dati tramite gli avvii

La tabella seguente mostra i vantaggi e gli svantaggi di ciascun metodo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>I dati esportati includono valori oggetto e campo</p> </th> 
   <th> <p>Possibilità di esportare contemporaneamente i dati su più tipi di oggetti</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Esportazione di dati da una vista a elenco</strong> </p> <p>Per ulteriori informazioni sull’esportazione di dati da un elenco, consulta <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Esportare i dati</a></p> </td> 
   <td> <p>Sì</p> <p>Vengono esportati sia i campi nativi di Workfront che i campi personalizzati associati agli oggetti.</p> </td> 
   <td> <p>No</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Esportazione di dati tramite Kick-Starts</strong> </p> </td> 
   <td> <p>Sì (limitato)</p> <p>La maggior parte dei campi nativi di Workfront associati agli oggetti viene esportata, ma alcuni no. Ad esempio, non è possibile esportare i campi Pianificazione, Proprietario progetto o Sponsor di progetto tramite un'esportazione di avvio del progetto.</p> <p>In un progetto a cui è allegato un modulo personalizzato, i dati immessi nei campi del modulo non vengono esportati.</p> <p>È tuttavia possibile esportare un modulo personalizzato. Nel file risultante sono elencati i campi configurati nel modulo, ad esempio caselle di testo e pulsanti di scelta.</p> </td> 
   <td> <p>Sì</p> <p>L’utilizzo di Kick-Starts per esportare i dati di Workfront consente di esportare i dati relativi a più tipi di oggetti in una singola esportazione. Ad esempio, puoi includere attività, problemi e progetti in un’unica esportazione.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Limiti di esportazione

Durante l’esportazione dei dati tramite i avvii esistono le seguenti limitazioni (i dati vengono esportati in un formato file Excel):

* **50.000 righe:** Numero di righe consentite nel file.
* **65.530 collegamenti ipertestuali:** Questo è un limite imposto da Excel sui documenti che contengono più di 65.530 collegamenti ipertestuali. Non è possibile aprire questi documenti dopo l’esportazione. Si noti che un documento Excel può contenere solo 200 righe di dati, ma se il documento contiene più di 65.530 collegamenti, il documento non viene aperto.

## Esportare i dati tramite gli avvii

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Sistema** > **Kick-Starts,** quindi fai clic su **Esporta dati.**

1. Selezionare l’oggetto da esportare.
1. Fai clic su **Altre opzioni** per visualizzare l’elenco completo degli oggetti.

   Tutti gli oggetti elencati qui possono essere utilizzati anche per importare dati in Workfront.

   L&#39;unica eccezione è la **Livelli di accesso** oggetto. Il foglio dati dei livelli di accesso incluso in un&#39;esportazione viene fornito solo a scopo di riferimento. Ti consente di assegnare un livello di accesso a un nuovo account utente tramite ID.

   Per ulteriori informazioni sull’importazione di dati in Workfront tramite i Avvio rapido, vedi [Importare dati in Adobe Workfront utilizzando un modello Click-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). Di seguito è riportato un elenco di tutti gli oggetti che possono essere esportati tramite i brani di avvio:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>Oggetto</p> </th> 
      <th> <p>Fogli esportati del file Excel</p> </th> 
      <th> <p>Formato esportazione</p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top">Livello di accesso</td> 
      <td scope="col" valign="top">Livello di accesso<br>Preferenze</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Assegnazione</td> 
      <td scope="col" valign="top">Assegnazione<br>Preferenze</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Azienda</td> 
      <td scope="col" valign="top"> Azienda<br>Preferenze </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Modello e-mail</td> 
      <td scope="col" valign="top"> Modello e-mail<br>Preferenze </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Spesa</td> 
      <td valign="top"> Spese<br>Preferenze </td> 
      <td scope="col" valign="top"> Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Pagina Esterna</td> 
      <td valign="top"> Pagina esterna<br>Preferenze </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Filtro</td> 
      <td valign="top"> Filtro<br>Preferenze </td> 
      <td valign="top">ZIP </td> 
     </tr> 
     <tr> 
      <td valign="top">Gruppo</td> 
      <td valign="top"> Gruppo<br>Preferenze  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Raggruppamento</td> 
      <td valign="top"> Raggruppamento<br>Preferenze </td> 
      <td valign="top">ZIP</td> 
     </tr> 
     <tr> 
      <td valign="top">Ora</td> 
      <td valign="top"> Ora<br>Preferenze </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Problema</td> 
      <td valign="top"> Problema<br>Preferenze </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Ruolo</td> 
      <td valign="top"> Ruolo<br>Preferenze </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Percorso milestone</td> 
      <td valign="top"> Milestone<br>Percorso Milestone<br>Preferenze </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Nota</td> 
      <td valign="top"> Nota<br>Preferenze </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Portfolio</td> 
      <td valign="top"> Portfolio<br>Preferenze  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Progetto</td> 
      <td valign="top"> Coda<br>Progetto<br>Regola di routing<br>Argomento coda<br>Preferenze </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Stima Risorse</td> 
      <td valign="top"> Stima risorsa<br>Preferenze </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Gruppo di risorse</td> 
      <td valign="top"> Pool di risorse<br>Preferenze </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Rischio</td> 
      <td valign="top"> Rischio<br>Preferenze  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Tipo Rischio</td> 
      <td valign="top"> Tipo di rischio<br>Preferenze  </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Scorecard</td> 
      <td valign="top">Domande sulla scorecard<br>Opzione Scorecard<br>Scorecard<br>Preferenze </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Attività</td> 
      <td valign="top"> Attività<br>Preferenze </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Modello</td> 
      <td valign="top"> Coda<br>Modello<br>Regola di routing<br>Argomento coda<br>Preferenze </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top">Assegnazione Modello</td> 
      <td valign="top"> Assegnazione modello<br>Preferenze </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Attività modello</td> 
      <td valign="top"> Attività modello<br>Preferenze </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Scheda orario</td> 
      <td valign="top"> Profilo scheda attività<br>Scheda attività<br>Preferenze </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top"> Visualizza </td> 
      <td valign="top"> Visualizza<br>Preferenze  </td> 
      <td valign="top">ZIP</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Scarica.**

   Il file di avvio esportato viene scaricato sul computer come file Excel o come file . file zip contenente più file Excel e proprietà. Ogni file Excel è una raccolta di fogli, in cui ogni foglio rappresenta un campo associato all&#39;oggetto selezionato. C&#39;è una **Proprietà** foglio associato a ogni esportazione.

   La **Dashboard** e **Rapporto** le opzioni consentono di selezionare dashboard e rapporti specifici da includere nel download. Puoi esportare solo le dashboard condivise a livello di sistema.

   Non è possibile esportare rapporti sulle matrici. Per ulteriori informazioni sui rapporti sulle matrici, vedi [Creare un rapporto sulla matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   Puoi selezionare fino a 100 dashboard e 100 rapporti in un’unica esportazione.

   ![](assets/kickstart-export-350x381.png)

   È possibile esportare più oggetti contemporaneamente.

   Per impostazione predefinita, sotto la **Cosa includere** etichetta (prima di fare clic su **Altre opzioni**):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Oggetto</strong> </p> </th> 
      <th> <p><strong>Fogli esportati del file Excel</strong> </p> </th> 
      <th> <p> <strong>Formato esportazione</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>Dashboard</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>Parametro<br>Opzione parametro<br>Gruppo di parametri<br>Parametro categoria<br>Categoria<br>Rapporto<br>Sezione della scheda Portale<br>Dashboard<br>Preferenze</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Rapporto</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">Parametro<br>Opzione parametro<br>Gruppo di parametri<br>Parametro categoria<br>Categoria<br>Rapporto<br>Preferenze</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Approval</p> </td> 
      <td scope="col" valign="top"> <p>Approvatore del passaggio<br>Passaggio di approvazione<br>Approvazione<br>Processo di approvazione<br>Preferenze</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Dati personalizzati</p> </td> 
      <td scope="col" valign="top"> <p>Parametro<br>Opzione parametro<br>Gruppo di parametri<br>Parametro categoria<br>Categoria<br>Preferenze</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Tipo di Spesa</p> </td> 
      <td valign="top"> <p>Tipo di spesa<br>Preferenze</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Tipo di ora</p> </td> 
      <td valign="top"> <p>Tipo ora<br>Preferenze</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Team</p> </td> 
      <td valign="top"> Membro del team<br>Team<br>Preferenze </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Utente</p> </td> 
      <td valign="top"> <p>Utente<br>Preferenze</p> </td> 
      <td valign="top"> <p> Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong></strong> </p> </th> 
      <th> <p><strong>Fogli esportati del file Excel</strong> </p> </th> 
      <th> <p> <strong>Formato esportazione</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>Dashboard</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>Parametro<br>Opzione parametro<br>Gruppo di parametri<br>Parametro categoria<br>Categoria<br>Rapporto<br>Sezione della scheda Portale<br>Dashboard<br>Preferenze</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Rapporto</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">Parametro<br>Opzione parametro<br>Gruppo di parametri<br>Parametro categoria<br>Categoria<br>Rapporto<br>Preferenze</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Approval</p> </td> 
      <td scope="col" valign="top"> <p>Approvatore del passaggio<br>Passaggio di approvazione<br>Approvazione<br>Processo di approvazione<br>Preferenze</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Dati personalizzati</p> </td> 
      <td scope="col" valign="top"> <p>Parametro<br>Opzione parametro<br>Gruppo di parametri<br>Parametro categoria<br>Categoria<br>Preferenze</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Tipo di Spesa</p> </td> 
      <td valign="top"> <p>Tipo di spesa<br>Preferenze</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Tipo di ora</p> </td> 
      <td valign="top"> <p>Tipo ora<br>Preferenze</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Team</p> </td> 
      <td valign="top"> Membro del team<br>Team<br>Preferenze </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Utente</p> </td> 
      <td valign="top"> <p>Utente<br>Preferenze</p> </td> 
      <td valign="top"> <p>Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Consigliato) Analizza i dati esportati per garantire che tutte le informazioni che ti aspetti di vedere siano state esportate.

   Per le esportazioni di grandi dimensioni, Workfront funziona in background per produrre il file Excel e fornisce un messaggio di avviso sul ritardo. Il file di avvio viene inviato via e-mail al termine del download.

   ![](assets/large-kick-start-file-warning-350x65.png)
