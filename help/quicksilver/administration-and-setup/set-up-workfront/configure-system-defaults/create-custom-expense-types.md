---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Crea tipi di spesa personalizzati
description: Come [!DNL Adobe Workfront] amministratore, è possibile creare tipi di spesa personalizzati per definire e tenere traccia delle spese associate alle attività e ai progetti. Le spese sono costi non lavorativi che possono essere associati a attività o progetti.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 3%

---

# Crea tipi di spesa personalizzati

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Come [!DNL Adobe Workfront] amministratore, è possibile creare tipi di spesa personalizzati per definire e tenere traccia delle spese associate alle attività e ai progetti. Le spese sono costi non lavorativi che possono essere associati a attività o progetti.

È possibile modificare o eliminare qualsiasi tipo di spesa creato. Non è possibile eliminare o modificare il componente incorporato [!DNL Workfront] tipi di spesa.

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore.</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipi di spesa predefiniti

Tipi di spesa in [!DNL Workfront] per impostazione predefinita non è possibile eliminare o modificare i seguenti elementi:

* [!UICONTROL Pubblicità]
* [!UICONTROL Consulenza]
* [!UICONTROL Intrattenimento]
* [!UICONTROL Generale]
* [!UICONTROL Materiali]
* [!UICONTROL Viaggi]

## Crea tipi di spesa personalizzati

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront].
1. Fai clic su **[!UICONTROL Tipi di spesa]**.
1. Fai clic su **[!UICONTROL Nuovo tipo di spesa]**.
1. In **[!UICONTROL Nuovo tipo di spesa]** casella visualizzata, specificare le informazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Specificare un nome per la spesa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td>Specificare una descrizione della spesa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Unità calcolata]</td> 
      <td> <p>Selezionare l'unità di misura per il tipo di spesa dall'elenco a discesa.</p> <p>Sono disponibili le seguenti unità di misura:</p> 
       <ul> 
        <li>Miglia</li> 
        <li>Chilometro</li> 
        <li>Chilogrammo</li> 
        <li>Dollaro</li> 
        <li>Dollaro</li> 
        <li>giorno</li> 
        <li>Altro: quando si seleziona questa opzione è necessario denominare l’unità di misura e definire l’unità di misura come qualcosa di familiare all’organizzazione.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Trfa</td> 
      <td> <p>Specifica il prezzo per unità. Si tratta di un campo formattato per la valuta e rappresenta il costo di ogni unità stabilita nel <strong>[!UICONTROL Unità calcolata]</strong> campo . </p> <p>La velocità può contenere un valore numerico con fino a 4 numeri dopo il decimale. Ad esempio, 1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Crea tipo di spesa]**.\
   Il tipo di spesa è ora disponibile per consentire agli utenti di associarlo alle spese relative a progetti e attività.

## Modifica tipi di spesa personalizzati

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront].
1. Fai clic su **[!UICONTROL Tipi di spesa]**.
1. Selezionare il tipo di spesa che si desidera modificare, quindi fare clic su **[!UICONTROL Modifica]**.

   La **[!UICONTROL Modifica tipo di spesa]** viene visualizzata la finestra di dialogo.

1. Apporta le modifiche desiderate, quindi fai clic su **[!UICONTROL Salva modifiche]**.\
   Il tipo di spesa è ora disponibile per consentire agli utenti di associarlo alle spese relative a progetti e attività.

Per ulteriori informazioni su come utilizzare le spese e come possono influenzare il costo di un progetto, consulta l’articolo [Gestione delle spese di progetto](../../../manage-work/projects/project-finances/manage-project-expenses.md).
