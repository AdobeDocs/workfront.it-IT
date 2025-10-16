---
product-area: enterprise-scenario-planner-product-area
keywords: piano,autorizzazioni,condivisione,iniziative,scenari,scenario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Condividere un piano nella Pianificazione scenario
description: Puoi condividere un piano creato in Adobe Workfront Scenario Planner con altri utenti.
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 2%

---

# Condividi un piano in [!DNL Scenario Planner]

<!--Audited: 07/2024-->

È possibile condividere un piano in [!DNL Adobe Workfront Scenario Planner] con altri utenti, in modo che possano collaborare allo stesso lavoro svolto.

>[!TIP]
>
>Se si invia ad altri un collegamento a un piano, è necessario condividere il piano con loro affinché possano visualizzarlo.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] pacchetto</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>NOTA</b></p>
<p>Se hai un pacchetto Workfront diverso, contatta il rappresentante Workfront.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licenza</p> </td> 
   <td> <p>[!UICONTROL Light] o versione successiva</p> 
   <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
    <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di [!UICONTROL Edit] al [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorizzazioni oggetto </p> </td> 
   <td> <p>Autorizzazioni [!UICONTROL Manage] per un piano</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni sull&#39;accesso alla Pianificazione scenario, vedere [Accesso necessario per utilizzare la [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Per informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso alla documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Prerequisiti

* Gli utenti a cui sono state assegnate le autorizzazioni per il piano devono avere accesso all&#39;area [!DNL Scenario Planner] nei propri livelli di accesso, come concesso dall&#39;amministratore [!DNL Workfront], per poter ricevere le autorizzazioni per un piano.

  Ad esempio, [!UICONTROL I richiedenti] non possono visualizzare, creare o modificare i piani. Tieni presente questo aspetto quando condividi un piano con un utente che dispone di una licenza Requestor.

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

Per ulteriori informazioni sull&#39;accesso a [!DNL Scenario Planner] per vari tipi di licenza, vedere [Concedere l&#39;accesso a  [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## Considerazioni sulla condivisione dei piani

* Tutti gli utenti, inclusi gli amministratori di sistema, possono accedere solo ai piani creati.
* È possibile condividere un singolo piano oppure più piani in blocco.
* Non è possibile visualizzare i piani non creati o non condivisi con l&#39;utente.
* È possibile condividere un piano solo con altri utenti. Non è possibile condividere i piani con gruppi, team o aziende.
* È necessario salvare un piano prima di poterlo condividere.
* Puoi condividere un URL di un piano con un altro utente. Se l’utente non dispone delle autorizzazioni necessarie per visualizzare almeno il piano, può richiedere l’accesso al piano a un altro utente quando riceve l’URL. Per informazioni sulla richiesta di accesso a un piano, vedere [Richiedere l&#39;accesso a un piano in [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
* Quando si condividono più piani già condivisi con altri utenti, gli utenti condivisi non vengono sostituiti ma aggiunti agli utenti esistenti di ogni piano selezionato.

## Opzioni di autorizzazione del piano

Nella tabella seguente sono elencate le autorizzazioni che è possibile concedere durante la condivisione di un piano. Per ulteriori informazioni sull&#39;accesso degli utenti in base alla licenza, vedere [Concedere l&#39;accesso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Azioni</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Gestisci]</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL View]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Visualizza piano </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Visualizza iniziative </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Visualizza scenari</td> 
   <td>✓</td> 
   <td><span style="font-weight: normal;">✓</span> </td> 
  </tr> 
  <tr> 
   <td>Visualizza mansioni</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Visualizza informazioni su costi e budget*</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>Gestione delle informazioni su costi e budget*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Creare iniziative</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Creare scenari</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Elimina iniziative o scenari</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Copia scenari</td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Pubblica scenari**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*È necessario avere accesso ai dati finanziari per poter visualizzare o gestire le informazioni finanziarie sui piani, anche se si dispone delle autorizzazioni di gestione per i piani. Per informazioni sull&#39;accesso ai dati finanziari, vedere [Concedere l&#39;accesso ai dati finanziari](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

**Per pubblicare scenari, devi disporre dell’accesso Crea e delle autorizzazioni per gestire i progetti.

Per informazioni sul livello di accesso al progetto, vedere [Concedere l&#39;accesso ai progetti](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Per informazioni sulle autorizzazioni del progetto, vedere [Condividere un progetto in [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

## Condividere i piani

{{step1-to-scenario-planner}}

1. Fare clic sul nome di un piano per aprirlo

   Oppure

   Selezionare diversi piani per condividerli in blocco.

   >[!TIP]
   >
   >Per condividere un piano, fare clic sugli avatar degli utenti con cui è condiviso nell&#39;angolo superiore destro dell&#39;intestazione del piano.

1. (Condizionale) Se hai aperto un piano, fai clic sull&#39;icona **[!UICONTROL Altro]** ![Altro](assets/more-icon.png) a destra del nome del [!UICONTROL Piano], quindi fai clic su **[!UICONTROL Condividi]**

   Oppure

   Se hai selezionato diversi piani per condividerli in blocco, fai clic sull&#39;icona **[!UICONTROL Condividi]** ![](assets/share-icon-26x26.png) nella parte superiore dell&#39;elenco dei piani per aprire la casella di accesso [!UICONTROL Piano].

   >[!TIP]
   >
   >* Gli utenti che dispongono delle autorizzazioni per tutti i piani selezionati vengono visualizzati nella casella di accesso [!UICONTROL Piano].
   >* Eventuali utenti aggiuntivi vengono aggiunti a e non sostituiscono gli utenti esistenti in tutti i piani selezionati.

1. Nel campo **[!UICONTROL Concedi l&#39;accesso al piano a]**, inizia a digitare il nome degli utenti con cui vuoi condividere il piano, quindi selezionali quando compaiono nell&#39;elenco.
1. Dal menu a discesa delle autorizzazioni a destra del nome utente, selezionare il livello di autorizzazione che si desidera concedere al piano.
1. Selezionare una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visualizzazione </td> 
      <td>Gli utenti con cui condividi il piano disporranno delle autorizzazioni necessarie per visualizzarlo. Non possono modificare le informazioni sul piano, aggiungere iniziative, scenari o pubblicare scenari. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Gestisci]</td> 
      <td> <p>Gli utenti che condividono il piano dispongono delle autorizzazioni necessarie per gestirlo, ad esempio per modificare le informazioni, aggiungere iniziative, scenari e pubblicare il piano. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >È possibile eliminare un piano solo quando è stato creato. Non è possibile eliminare i piani condivisi con l&#39;utente.

1. Fai clic su **[!UICONTROL Salva]**.

   Il piano è ora condiviso con gli utenti specificati.

   È possibile visualizzare gli utenti che dispongono delle autorizzazioni per il piano nella colonna Condiviso con me in un elenco di piani o nell&#39;angolo superiore destro dell&#39;intestazione del piano.

   >[!TIP]
   >
   >Puoi visualizzare i piani condivisi con te applicando il filtro [!UICONTROL Condivisi con me] in un elenco di piani.


