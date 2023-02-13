---
title: Personalizzare la terminologia dell’interfaccia utente utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un modello di layout per modificare le etichette di alcuni oggetti che vengono visualizzate in Workfront in modo che corrispondano ai termini utilizzati nell’organizzazione.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 3%

---

# Personalizzare la terminologia dell’interfaccia utente utilizzando un modello di layout

In qualità di amministratore di Adobe Workfront, puoi utilizzare un modello di layout per modificare le etichette di alcuni oggetti che vengono visualizzate in Workfront in modo che corrispondano ai termini utilizzati nell’organizzazione.

Dopo aver salvato un modello di layout in cui è stata modificata la terminologia, disconnettiti da Workfront e accedi di nuovo, le etichette modificate vengono visualizzate nella posizione in cui apparirebbero le etichette predefinite nella maggior parte delle aree di Workfront:

* Menu principale
* Tutte le aree accessibili dal menu principale
* Tutte le schede
* Tutti i menu
* Report Builder e elementi di reporting (viste, filtri e raggruppamenti)
* Pulsanti Salva
* File esportati
* E-mail
* App mobili

>[!NOTE]
>
>* L&#39;area del componente aggiuntivo di Outlook non visualizza le etichette personalizzate.
>* È possibile che si verifichino problemi di grammatica e di altro tipo quando si personalizzano le etichette. Ad esempio, se cambi &quot;Problema&quot; in &quot;Richiesta&quot;, potrebbero esserci dei punti nell’interfaccia utente in cui viene visualizzata la frase &quot;Richiesta&quot;. Per ulteriori informazioni, consulta [Implicazioni della personalizzazione dei nomi degli oggetti](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) nell&#39;articolo [Comprendere gli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>


Per informazioni sui modelli di layout per gruppi, consulta [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

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
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.
Per eseguirle per un gruppo, devi essere un responsabile di quel gruppo.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizzare la terminologia dell’interfaccia utente

1. Inizia a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Fai clic su **Imposta terminologia** nell’angolo superiore destro della pagina.
1. Effettua una delle seguenti operazioni:

   * Per utilizzare un termine alternativo fornito da Workfront, fai clic sulla freccia giù  ![](assets/dropdown-arrow.png) accanto all’etichetta, fai clic sull’etichetta alternativa desiderata nell’elenco a discesa.

      >[!NOTE]
      >
      >Le etichette alternative fornite negli elenchi a discesa sono supportate nelle versioni di Workfront localizzate per le lingue non inglesi.

   * Per fornire un&#39;alternativa personalizzata per l&#39;etichetta visualizzata per un oggetto, fare clic su **Imposta nome personalizzato** a destra dell’etichetta, quindi digita il **Singolare** e **Plurale** moduli del termine personalizzato. Puoi fare clic su **Reimposta** se cambi idea.

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
        <td><p>Per ulteriori informazioni su questi oggetti, vedere <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Comprendere gli oggetti in Adobe Workfront</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Oggetti Workfront</p></td>
        <td>
         <ul>
          <p>Obiettivo</p>
          <p>Risultato</p>
          <p>Attività</p>
         </ul></td>
        <td><p>Questi oggetti richiedono una licenza aggiuntiva. Per ulteriori informazioni, consulta <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Panoramica sugli obiettivi di Adobe Workfront</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Oggetti di Workfront Scenario Planner</p></td>
        <td>
         <ul>
          <p>Iniziativa</p>
          <p>Scenario</p>
          <p>Piano </p>
         </ul></td>
        <td><p>Questi oggetti richiedono una licenza aggiuntiva. Per informazioni, consulta <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">Guida introduttiva a Scenario Planner</a>.</p></td>
       </tr>
      </tbody>
     </table>

1. Al termine, fai clic su **Fine**.

   >[!TIP]
   >
   >Dopo aver fatto clic su Fine (e anche dopo aver salvato il modello di layout), puoi sempre tornare alle impostazioni Imposta terminologia e fare clic su Ripristina accanto a qualsiasi termine personalizzato per riportarli al loro stato predefinito.

1. Continua a personalizzare il modello di layout.

   Oppure

   Al termine della personalizzazione, fai clic su **Salva**.

1. Per visualizzare le modifiche terminologiche:

   1. Disconnettiti e accedi nuovamente a Workfront.
   1. Chiudi tutte le schede del browser aperte per l’ambiente Workfront.

   >[!IMPORTANT]
   >
   >Questo è necessario anche per gli utenti che hanno utilizzato il modello di layout prima di apportare modifiche terminologiche.

Per ulteriori informazioni sui modelli di layout, consulta [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
