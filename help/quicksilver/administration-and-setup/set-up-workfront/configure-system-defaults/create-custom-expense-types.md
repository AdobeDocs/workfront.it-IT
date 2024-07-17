---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Creare tipi di spesa personalizzati
description: In qualità di amministratore  [!DNL Adobe Workfront] , puoi creare tipi di spesa personalizzati per definire e tenere traccia delle spese associate alle attività e ai progetti. Le spese sono costi non di manodopera che possono essere associati ad attività o progetti.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 1%

---

# Creare tipi di spesa personalizzati

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

In qualità di amministratore [!DNL Adobe Workfront], puoi creare tipi di spesa personalizzati per definire e tenere traccia delle spese associate alle attività e ai progetti. Le spese sono costi non di manodopera che possono essere associati ad attività o progetti.

Puoi modificare o eliminare qualsiasi tipo di spesa creato. Impossibile eliminare o modificare i tipi di spesa [!DNL Workfront] predefiniti.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore [!DNL Workfront].</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipi di spesa predefiniti

I Tipi di Spesa che sono in [!DNL Workfront] per impostazione predefinita non possono essere eliminati o modificati includono:

* [!UICONTROL Advertising]
* [!UICONTROL Consulenza]
* [!UICONTROL Intrattenimento]
* [!UICONTROL Generale]
* [!UICONTROL Materiali]
* [!UICONTROL Viaggi]

## Creare tipi di spesa personalizzati

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe Workfront].
1. Fare clic su **[!UICONTROL Tipi di spesa]**.
1. Fare clic su **[!UICONTROL Nuovo tipo di spesa]**.
1. Nella casella **[!UICONTROL Nuovo tipo di spesa]** visualizzata, specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Specifica un nome per la spesa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td>Specifica una descrizione della spesa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Unità Calcolata]</td> 
      <td> <p>Selezionare l'unità di misura per il tipo di spesa dall'elenco a discesa.</p> <p>Sono disponibili le seguenti unità di misura:</p> 
       <ul> 
        <li>Miglia</li> 
        <li>Chilometro</li> 
        <li>Chilogrammo</li> 
        <li>Dollaro</li> 
        <li>Dollaro</li> 
        <li>Giorno</li> 
        <li>Altro - Se si seleziona questa opzione, viene richiesto di denominare l'unità di misura e di definirla in modo che sia familiare all'organizzazione.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Trfa</td> 
      <td> <p>Specifica il prezzo unitario. Questo campo è formattato come valuta e rappresenta il costo di ogni unità stabilita nel campo <strong>[!UICONTROL Unità calcolata]</strong>. </p> <p>Il tasso può contenere un valore numerico con un massimo di 4 numeri dopo il decimale. Ad esempio, 1,0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Crea tipo di spesa]**.\
   Il tipo di spesa è ora disponibile per gli utenti per associarlo alle spese relative ai progetti e alle attività.

## Modifica tipi di spesa personalizzati

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe Workfront].
1. Fare clic su **[!UICONTROL Tipi di spesa]**.
1. Selezionare il tipo di spesa da modificare, quindi fare clic su **[!UICONTROL Modifica]**.

   Viene visualizzata la finestra di dialogo **[!UICONTROL Modifica tipo di spesa]**.

1. Apporta le modifiche desiderate, quindi fai clic su **[!UICONTROL Salva modifiche]**.\
   Il tipo di spesa è ora disponibile per gli utenti per associarlo alle spese relative ai progetti e alle attività.

Per ulteriori informazioni su come utilizzare le spese e su come possono influenzare il costo di un progetto, vedere l&#39;articolo [Gestione delle spese del progetto](../../../manage-work/projects/project-finances/manage-project-expenses.md).
