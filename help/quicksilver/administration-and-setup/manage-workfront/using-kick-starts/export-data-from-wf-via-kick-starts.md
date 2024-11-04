---
user-type: administrator
product-area: system-administration
keywords: kick-start, kick-start, kick-start, kick-start
navigation-topic: use-kick-starts
title: Esportare dati da Workfront tramite Kick-Start
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare la funzione di esportazione dati di Kick-Start per esportare dati da Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 7b9989b73f7be46690073f323203ae2d9ca1a4b5
workflow-type: tm+mt
source-wordcount: '1028'
ht-degree: 7%

---

# Esportare dati da Workfront tramite Kick-Start

<!-- Audited: 2/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

{{highlighted-preview}}

In qualità di amministratore di Adobe Workfront, puoi utilizzare la funzione di esportazione dati di Kick-Start per esportare dati da Workfront. Puoi utilizzarlo in altre applicazioni dopo averlo esportato.

L&#39;esportazione dei dati tramite Kick-Start è utile anche per comprendere quali campi sono associati a ciascun oggetto, come questi campi sono codificati e come i valori di questi campi sono formattati nel database.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td>
   <p>Nuovo: Standard</p>
   Oppure
   <p>Corrente: Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vantaggi e svantaggi dell’utilizzo dei kick-start per esportare i dati

Esistono due modi per esportare i dati in Workfront:

* Esportazione di dati da un report o da un elenco

  Per ulteriori informazioni sull&#39;esportazione di dati da un report o da un elenco, vedere [Esporta dati](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* Esportazione di dati tramite kick-start

La tabella seguente mostra i vantaggi e gli svantaggi di ciascun metodo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>I dati esportati includono i valori degli oggetti e dei campi</p> </th> 
   <th> <p>Possibilità di esportare dati su più tipi di oggetti contemporaneamente</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Esportazione di dati da una visualizzazione elenco</strong> </p> <p>Per ulteriori informazioni sull'esportazione di dati da un elenco, vedere <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Esporta dati</a></p> </td> 
   <td> <p>Sì</p> <p>Vengono esportati sia i campi nativi di Workfront che i campi personalizzati associati agli oggetti.</p> </td> 
   <td> <p>No</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Esportazione di dati tramite Kick-Start</strong> </p> </td> 
   <td> <p>Sì (limitato)</p> <p>La maggior parte dei campi nativi di Workfront associati agli oggetti viene esportata, ma alcuni non lo sono. Ad esempio, non è possibile esportare i campi Pianificazione, Proprietario progetto o Sponsor progetto tramite un’esportazione di avvio del progetto.</p> <p>In un progetto a cui è allegato un modulo personalizzato, tutti i dati immessi nei campi del modulo non vengono esportati.</p> <p>È tuttavia possibile esportare un modulo personalizzato. Nel file risultante sono elencati i campi configurati nel modulo, ad esempio caselle di testo e pulsanti di scelta.</p> </td> 
   <td> <p>Sì</p> <p>L'utilizzo di Kick-Start per esportare i dati di Workfront consente di esportare dati relativi a più tipi di oggetti in un'unica esportazione. Ad esempio, puoi includere attività, problemi e progetti in una singola esportazione.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Limiti di esportazione

Esistono le seguenti limitazioni quando si esportano dati tramite avvii (i dati vengono esportati in un formato di file Excel):

* **50.000 righe:** il numero di righe consentito nel file.
* **65.530 collegamenti ipertestuali:** Si tratta di un limite imposto da Excel ai documenti che contengono più di 65.530 collegamenti ipertestuali. Non è possibile aprire questi documenti dopo averli esportati. Si noti che un documento di Excel può contenere solo 200 righe di dati, ma se il documento contiene più di 65.530 collegamenti, il documento non si apre.

## Esportare i dati tramite kick-start

{{step-1-to-setup}}

1. Fai clic su **Sistema** > **Avvii,** quindi fai clic su **Esporta dati.**

1. Selezionare l&#39;oggetto da esportare. Per impostazione predefinita, i seguenti oggetti sono visualizzati in **Cosa includere**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Oggetto</strong> </p> </th> 
      <th> <p><strong>Fogli esportati del file di Excel</strong> </p> </th> 
      <th> <p> <strong>Formato esportazione</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>Dashboard</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>Parametro<br>Opzione Parametro<br>Gruppo Parametri<br>Parametro Categoria<br>Categoria<br>Report<br>Sezione Scheda Portale<br>Dashboard<br>Preferenze</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Rapporto</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">Parametro<br>Opzione Parametro<br>Gruppo Parametri<br>Parametro Categoria<br>Categoria<br>Rapporto<br>Preferenze</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Approvazione</p> </td> 
      <td scope="col" valign="top"> <p>Approvatore passaggio<br>Passaggio approvazione<br>Approvazione<br>Processo approvazione<br>Preferenze</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Dati personalizzati</p> </td> 
      <td scope="col" valign="top"> <p>Parametro<br>Opzione Parametro<br>Gruppo Parametri<br>Parametro Categoria<br>Categoria<br>Preferenze</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Tipo di spesa</p> </td> 
      <td valign="top"> <p>Tipo di spesa<br>Preferenze</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Tipo di ora</p> </td> 
      <td valign="top"> <p>Tipo di Ora<br>Preferenze</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Team</p> </td> 
      <td valign="top"> Membro team<br>Team<br>Preferenze </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Utente</p> </td> 
      <td valign="top"> <p>Utente<br>Preferenze</p> </td> 
      <td valign="top"> <p> Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Altre opzioni** per visualizzare l&#39;elenco completo degli oggetti.

   Tutti gli oggetti elencati possono essere utilizzati anche per importare dati in Workfront.

   L&#39;unica eccezione è l&#39;oggetto **Access Levels**. La scheda dati Livelli di accesso inclusa in un&#39;esportazione viene fornita solo a scopo di riferimento. Consente di assegnare un livello di accesso a un nuovo account utente in base all’ID.

   Per ulteriori informazioni sull&#39;importazione di dati in Workfront tramite l&#39;avvio automatico, vedere [Importare dati in Adobe Workfront utilizzando un modello di avvio](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). Di seguito è riportato un elenco di tutti gli oggetti che possono essere esportati tramite kick-start:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>Oggetto</p> </th> 
      <th> <p>Fogli esportati del file Excel</p> </th> 
      <th> <p>Formato di esportazione</p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top">Livello di accesso</td> 
      <td scope="col" valign="top">Livello d'Accesso<br>Preferenze</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Assegnazione</td> 
      <td scope="col" valign="top">Assegnazione<br>Preferenze</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Azienda</td> 
      <td scope="col" valign="top"> Società<br>Preferenze </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Modello e-mail</td> 
      <td scope="col" valign="top"> Preferenze modello e-mail<br> </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Spesa</td> 
      <td valign="top"> Preferenze <br> spese </td> 
      <td scope="col" valign="top"> Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Pagina Esterna</td> 
      <td valign="top"> Pagina esterna<br>Preferenze </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Filtro</td> 
      <td valign="top"> Filtra<br>Preferenze </td> 
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
      <td valign="top"> Hour<br>Preferenze </td> 
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
      <td valign="top"> Percorso Milestone<br>Milestone<br>Preferenze </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Nota</td> 
      <td valign="top"> Note<br>Preferenze </td> 
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
      <td valign="top"> Stima risorse<br>Preferenze </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Gruppo di risorse</td> 
      <td valign="top"> Preferenze del Pool di Risorse<br> </td> 
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
      <td valign="top">Domande Scorecard<br>Opzione Scorecard<br>Scorecard<br>Preferenze </td> 
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
      <td valign="top"> Profilo scheda orario<br>Scheda orario<br>Preferenze </td> 
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

   Il file di avvio esportato viene scaricato nel computer come file Excel o come file . file zip contenente più file Excel e proprietà. Ogni file di Excel è un insieme di fogli, in cui ogni foglio rappresenta un campo associato all&#39;oggetto selezionato. A ogni esportazione è associato un foglio **Proprietà**.

   Le opzioni **Dashboard** e **Report** consentono di selezionare dashboard e report specifici da includere nel download. Puoi esportare solo dashboard condivisi a livello di sistema.

   Non è possibile esportare report matrice. Per ulteriori informazioni sui report matrice, vedere [Creare un report matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   Kick-Start non supporta i filtri o i raggruppamenti in modalità testo. Per un’esportazione corretta, i filtri e i raggruppamenti per reporting devono essere commutati in modalità Standard.

   Puoi selezionare fino a 100 dashboard e 100 rapporti in una singola esportazione.

   <span class="preview">Immagine di esempio nell&#39;ambiente di anteprima:</span>
   ![Esportazione Kick-Start](assets/kickstart-export-spreadsheet-options.png)

   Immagine di esempio nell’ambiente di produzione:
   ![Esportazione Kick-Start](assets/kickstart-export-350x381.png)

   È possibile esportare più oggetti contemporaneamente.

1. (Consigliato) Analizza i dati esportati per assicurarti che tutte le informazioni che prevedi di visualizzare siano state esportate.

   Per le esportazioni di grandi dimensioni, Workfront lavora in background per produrre il file Excel e ti fornisce un messaggio di avviso relativo al ritardo. Al termine del download, il file di avvio viene inviato all’utente tramite e-mail.

