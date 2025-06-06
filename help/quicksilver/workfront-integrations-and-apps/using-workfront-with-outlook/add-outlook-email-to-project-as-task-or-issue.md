---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Aggiungere un messaggio e-mail di Outlook a un progetto come attività o problema
description: Puoi convertire le e-mail in [!DNL Adobe Workfront] attività o problemi. Dopo la conversione di un’e-mail, l’attività o il problema viene visualizzato sul progetto selezionato durante la conversione.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 00755c27-9fc9-4357-a39b-4f9772484252
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# Aggiungere un&#39;e-mail di [!DNL Outlook] a un progetto come attività o problema

>[!IMPORTANT]
>
>Microsoft [È in corso la disabilitazione del supporto per i token online di Exchange legacy](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), attualmente utilizzati dal componente aggiuntivo di Workfront Outlook per l&#39;autenticazione. Questa modifica di Microsoft ha già iniziato a interessare i clienti e continuerà a essere implementata in più fasi fino a ottobre 2025.
>
>* **Dopo la completa disattivazione di questi token da parte di Microsoft, l&#39;integrazione di Workfront per Microsoft Outlook non funzionerà più.**
>
>Come parte di questa modifica, Microsoft ha deciso di cambiare il modo in cui i token vengono riabilitati. Dopo il **30 giugno 2025**, gli amministratori non saranno più in grado di riabilitare i token personalmente. Solo il supporto Microsoft può concedere eccezioni. **Il 1° ottobre 2025, i token legacy verranno disattivati per tutti i tenant. Le eccezioni non verranno concesse.**


È possibile convertire le e-mail in [!DNL Adobe Workfront] attività o problemi. Dopo la conversione di un’e-mail, l’attività o il problema viene visualizzato sul progetto selezionato durante la conversione.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Lavoro], [!UICONTROL Piano]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## Prerequisiti

L&#39;amministratore di [!DNL Workfront] deve abilitare [!DNL Outlook for Office] con [!DNL Workfront] prima di poter utilizzare questa integrazione.

## Aggiungi un&#39;e-mail [!DNL Outlook] a un progetto come attività o problema

1. Selezionare l&#39;e-mail all&#39;interno di [!DNL Outlook] che si desidera convertire in un&#39;attività o in un problema.
1. Fare clic sull&#39;icona **[!DNL Workfront]** nell&#39;angolo superiore destro del messaggio di posta elettronica per visualizzare il componente aggiuntivo Workfront.

   Per accedere all&#39;icona di [!DNL Workfront], potrebbe essere necessario fare clic sulla freccia rivolta verso il basso in alto a destra nell&#39;e-mail.

1. Fai clic sull&#39;icona **[!UICONTROL Menu]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) per visualizzare l&#39;elenco delle opzioni [!DNL Workfront] disponibili.



1. Fai clic su **[!UICONTROL Aggiungi a lavoro]**.

1. Selezionare il campo **[!UICONTROL Aggiungi al progetto]**.
1. Inizia a digitare il nome di un progetto nel campo **[!UICONTROL Progetto]**, quindi selezionalo quando viene visualizzato nell&#39;elenco.
1. Selezionare il pulsante di opzione **[!UICONTROL Attività]** se si desidera aggiungere un&#39;attività al progetto selezionato.

   Oppure

   Per aggiungere un problema al progetto selezionato, seleziona il pulsante di opzione **[!UICONTROL Problema]**.

1. (Facoltativo) Specifica a chi è assegnata questa attività o problema nel campo **[!UICONTROL Assegna a]**.

   >[!TIP]
   >
   >Puoi assegnare l’attività o il problema a un team se desideri che più persone ne siano consapevoli. Se i membri del team hanno le notifiche e-mail abilitate, riceveranno un’e-mail relativa alla nuova attività o al problema loro assegnato.


1. (Facoltativo) Specifica **[!UICONTROL Scadenza]**. Questa diventa la [!UICONTROL Data di completamento pianificata] dell&#39;attività o del problema.
1. (Facoltativo) Aggiorna le seguenti informazioni dall&#39;e-mail prima di salvarla come attività o problema (i campi obbligatori sono preceduti da un asterisco).

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Nome attività o problema]</td>
        <td>Per impostazione predefinita, il nome dell’attività corrisponde all’oggetto dell’e-mail. È possibile modificare il nome dell'attività come desiderato.</td>
        <td></td>
      </tr>
      <tr>
        <td>[!UICONTROL Descrizione]</td>
        <td>Per impostazione predefinita, la descrizione è la stessa del corpo dell’e-mail. Puoi modificare la descrizione come desiderato.</td>
      </tr>
      <tr>
        <td>[!UICONTROL Allegati]</td>
        <td>Tutti gli allegati e-mail vengono salvati nell'area [!UICONTROL Documents] dell'attività o del problema. Puoi eliminare tutti gli allegati prima di salvare l’e-mail come attività o problema.</td>
      </tr>
   </table>

1. Fare clic su **[!UICONTROL Aggiungi]**.

   L&#39;attività o il problema viene aggiunto al progetto specificato

1. (Facoltativo) Fare clic su **[!UICONTROL Visualizza in[!DNL Workfront]]** per visualizzare l&#39;attività nell&#39;applicazione [!DNL Workfront] in una nuova scheda.

1. (Facoltativo) Torna a [!DNL Outlook] e seleziona l&#39;e-mail convertita.

   Nella parte superiore del pannello del componente aggiuntivo [!DNL Workfront], notare la conferma con un collegamento che indica che l&#39;e-mail è stata aggiunta a [!DNL Workfront] come attività o problema. Il collegamento include la data in cui è stato convertito.



