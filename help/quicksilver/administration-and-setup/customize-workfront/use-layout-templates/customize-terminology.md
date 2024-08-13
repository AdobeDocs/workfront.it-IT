---
title: Personalizzare la terminologia dell’interfaccia utente utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un modello di layout per modificare le etichette di alcuni oggetti visualizzati in Workfront in modo che corrispondano ai termini utilizzati nell’organizzazione.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: a8214d9e10363881afbc2bd71f78f46cb6a25880
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 2%

---

# Personalizzare la terminologia dell’interfaccia utente utilizzando un modello di layout

In qualità di amministratore di Adobe Workfront, puoi utilizzare un modello di layout per modificare le etichette di alcuni oggetti visualizzati in Workfront in modo che corrispondano ai termini utilizzati nell’organizzazione.

Dopo aver salvato un modello di layout in cui è stata modificata la terminologia, quindi disconnettersi da Workfront e accedere nuovamente, le etichette modificate vengono visualizzate nella maggior parte delle aree di Workfront:

* Menu principale
* Tutte le aree a cui si accede dal menu principale
* Tutte le schede
* Tutti i menu
* Elementi di Report Builder e reporting (visualizzazioni, filtri e raggruppamenti)
* Pulsanti Salva
* File esportati
* E-mail
* App mobili

>[!NOTE]
>
>* Nell&#39;area Componente aggiuntivo di Outlook non vengono visualizzate le etichette personalizzate.
>* È possibile che si verifichino problemi grammaticali o di altro tipo quando si personalizzano le etichette. Ad esempio, se modifichi &quot;Problema&quot; in &quot;Richiesta&quot;, nell’interfaccia utente potrebbero essere presenti posizioni in cui viene visualizzata la frase &quot;Una richiesta&quot;. Per ulteriori informazioni, vedere [Implicazioni della personalizzazione dei nomi degli oggetti](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) nell&#39;articolo [Informazioni sugli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>

Per ulteriori informazioni sui modelli di layout, vedere [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Per informazioni sui modelli di layout per i gruppi, vedere [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Dopo aver configurato un modello di layout, è necessario assegnarlo agli utenti affinché le modifiche apportate siano visibili agli altri utenti. Per informazioni sull&#39;assegnazione di un modello di layout agli utenti, vedere [Assegnare gli utenti a un modello di layout](../use-layout-templates/assign-users-to-layout-template.md).

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
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.
Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Personalizzare la terminologia dell’interfaccia utente

1. Iniziare a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Fai clic su **Imposta terminologia** nell&#39;angolo superiore destro della pagina.
1. Effettua una delle seguenti operazioni:

   * Per utilizzare un termine alternativo fornito da Workfront, fare clic sulla freccia giù ![](assets/dropdown-arrow.png) accanto all&#39;etichetta, quindi selezionare l&#39;etichetta alternativa desiderata nell&#39;elenco a discesa.

     >[!NOTE]
     >
     >Le etichette alternative fornite negli elenchi a discesa sono supportate nelle versioni di Workfront localizzate per lingue diverse dall’inglese.

   * Per fornire un&#39;alternativa personalizzata per l&#39;etichetta visualizzata per un oggetto, fare clic su **Imposta nome personalizzato** a destra dell&#39;etichetta, quindi digitare i moduli **Singolare** e **Plurale** del termine personalizzato. Puoi fare clic su **Reimposta** se cambi idea.

     È possibile personalizzare i seguenti nomi di oggetto:

     <table style="table-layout:auto">
      <col>
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><p>Oggetti Workfront</p></td>
        <td>
          <p>Portfolio</p>
          <p>Programma</p>
          <p>Progetto</p>
          <p>Attività</p>
          <p>Problema</p>
          <p>Obiettivo</p>
          <p>Risultato</p>
          <p>Attività</p>
         </ul></td>
        <td><p>Per ulteriori informazioni su questi oggetti, vedere <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Informazioni sugli oggetti in Adobe Workfront</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Oggetti Obiettivi Workfront</p></td>
        <td>
         <ul>
          <p>Obiettivo</p>
          <p>Risultato</p>
          <p>Attività</p>
         </ul></td>
        <td><p>Questi oggetti richiedono una licenza aggiuntiva. Per ulteriori informazioni, consulta <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Panoramica sugli obiettivi di Adobe Workfront</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Oggetti Workfront Scenario Planner</p></td>
        <td>
         <ul>
          <p>Iniziativa</p>
          <p>Scenario</p>
          <p>Piano </p>
         </ul></td>
        <td><p>Questi oggetti richiedono una licenza aggiuntiva. Per informazioni, vedere <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">Introduzione alla Pianificazione scenario</a>.</p></td>
       </tr>
      </tbody>
     </table>

1. Al termine, fare clic su **Fine**.

   >[!TIP]
   >
   >Dopo aver fatto clic su Fine (e anche dopo aver salvato il modello di layout), è sempre possibile tornare alle impostazioni Terminologia e fare clic su Reimposta accanto ai termini personalizzati per riportarli allo stato predefinito.

1. Continuate a personalizzare il modello di layout.

   Oppure

   Se hai completato la personalizzazione, fai clic su **Salva**.

1. Per visualizzare le modifiche terminologiche:

   1. Esci e accedi di nuovo a Workfront.
   1. Chiudi tutte le schede del browser aperte per l’ambiente Workfront.

   >[!IMPORTANT]
   >
   >Questo è necessario anche per tutti coloro che hanno utilizzato il modello di layout prima di apportare modifiche terminologiche.

Per ulteriori informazioni sui modelli di layout, vedere [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
