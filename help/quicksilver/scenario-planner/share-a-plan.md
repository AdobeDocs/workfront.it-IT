---
product-area: enterprise-scenario-planner-product-area
keywords: piano,autorizzazioni,condivisione,iniziative,scenari,scenario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Condividere un piano nella Pianificazione scenario
description: Puoi condividere un piano creato in Adobe Workfront Scenario Planner con altri utenti.
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Condividi un piano in [!DNL Scenario Planner]

È possibile condividere un piano in [!DNL Adobe Workfront Scenario Planner] con altri utenti, in modo che possano collaborare allo stesso lavoro svolto.

>[!TIP]
>
>Se si invia ad altri un collegamento a un piano, è necessario condividere il piano con loro affinché possano visualizzarlo.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> piano*</b> </p> </td> 
   <td>[!UICONTROL Business] o versione successiva</td> 
  </tr> 
  <tr> 
   <td> <p>Licenza [!DNL Adobe Workfront]<b>*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td><b>Prodotto</b> </td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alla funzionalità descritta in questo articolo.</p> <p>Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedere <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurazioni del livello di accesso*</strong> </td> 
   <td> <p>Accesso di [!UICONTROL Edit] al [!DNL Scenario Planner]</p> <p>Se non disponi ancora dell'accesso, chiedi all'amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il livello di accesso, vedere <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p> Autorizzazioni [!UICONTROL Manage] per il piano
     <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedere <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">[!UICONTROL Request] accesso a un piano in [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront.

## Prerequisiti

* Gli utenti a cui sono state assegnate le autorizzazioni per il piano devono avere accesso all&#39;area [!DNL Scenario Planner] nei propri livelli di accesso, come concesso dall&#39;amministratore [!DNL Workfront], per poter ricevere le autorizzazioni per un piano.

  Ad esempio, [!UICONTROL I richiedenti] non possono visualizzare, creare o modificare i piani. Tieni presente questo aspetto quando condividi un piano con un utente che dispone di una licenza Requestor.

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

Per ulteriori informazioni sull&#39;accesso a [!DNL Scenario Planner] per vari tipi di licenza, vedere [Concedere l&#39;accesso a  [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## Considerazioni sulla condivisione dei piani

* È possibile condividere un singolo piano oppure più piani in blocco.
* Non è possibile visualizzare i piani non creati o non condivisi con l&#39;utente.
* È possibile condividere un piano solo con altri utenti. Non è possibile condividere i piani con gruppi, team o aziende.
* È necessario salvare un piano prima di poterlo condividere.
* Puoi condividere un URL di un piano con un altro utente. Se l’utente non dispone delle autorizzazioni necessarie per visualizzare almeno il piano, può richiedere l’accesso al piano a un altro utente quando riceve l’URL. Per informazioni sulla richiesta di accesso a un piano, vedere [Richiedere l&#39;accesso a un piano in [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
* Quando si condividono più piani già condivisi con altri utenti, gli utenti condivisi non vengono sostituiti ma aggiunti agli utenti esistenti di ogni piano selezionato.

## Condividere i piani

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di Workfront, quindi fai clic su **[!UICONTROL Scenari]**.
1. Fare clic sul nome di un piano per aprirlo

   Oppure

   Selezionare diversi piani per condividerli in blocco.

   >[!TIP]
   >
   >Per condividere un piano, fare clic sugli avatar degli utenti con cui è condiviso nell&#39;angolo superiore destro dell&#39;intestazione del piano.

1. (Condizionale) Se hai aperto un piano, fai clic sull&#39;icona **[!UICONTROL Altro]** ![](assets/more-icon.png) a destra del nome del [!UICONTROL Piano], quindi fai clic su **[!UICONTROL Condividi]**

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
      <td role="rowheader">Visualizzazione [!UICONTROL]</td> 
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
   <td>✓ <span style="font-weight: normal;"></span> </td> 
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
   <td>Scenari Publish**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*È necessario avere accesso ai dati finanziari per poter visualizzare o gestire le informazioni finanziarie sui piani, anche se si dispone delle autorizzazioni di gestione per i piani. Per informazioni sull&#39;accesso ai dati finanziari, vedere [Concedere l&#39;accesso ai dati finanziari](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

**Per pubblicare scenari, devi disporre dell’accesso Crea e delle autorizzazioni per gestire i progetti.

Per informazioni sul livello di accesso al progetto, vedere [Concedere l&#39;accesso ai progetti](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Per informazioni sulle autorizzazioni del progetto, vedere [Condividere un progetto in [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
