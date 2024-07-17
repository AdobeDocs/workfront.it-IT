---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Aggiungi un’attività secondaria a una storia esistente sulla bacheca Scrum
description: Quando create sottoattività per i brani esistenti, tenete presente l'impostazione Modalità di completamento per il progetto, poiché questo influisce sul modo in cui i brani vengono aggiornati.
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 0%

---

# Aggiungi un&#39;attività secondaria a una storia esistente nella bacheca [!UICONTROL Scrum]

Quando create sottoattività per i brani esistenti, tenete presente quanto segue:

**Quando l&#39;impostazione della [!UICONTROL Modalità di completamento] per il progetto è impostata su [!UICONTROL Manuale]:**

* Se si sposta una storia padre con sottoattività in [!UICONTROL Complete], la storia padre viene aggiornata al 100% e lo stato [!UICONTROL Status] in [!UICONTROL Complete]. Le sottoattività non vengono aggiornate.
* Per aggiornare la [!UICONTROL Percentuale completata] per la storia, è necessario aggiornarla dalla scheda [!UICONTROL Storie] o dalla pagina [!UICONTROL Dettagli] dell&#39;oggetto.

**Quando l&#39;impostazione [!UICONTROL Modalità di completamento] per il progetto è impostata su [!UICONTROL Automatico]**:

* Se si sposta una storia padre con sottoattività in [!UICONTROL Complete], la storia padre viene aggiornata al 100% e lo stato [!UICONTROL Status] in [!UICONTROL Complete]. Anche le sottoattività vengono aggiornate al 100% e lo [!UICONTROL Stato] viene aggiornato a [!UICONTROL Completo].
* Per aggiornare [!UICONTROL Percent Complete] per la storia, è necessario aggiornare [!UICONTROL Percent Complete] per le sottoattività. La [!UICONTROL Percentuale completata] per il brano viene calcolata in base alla [!UICONTROL Percentuale completata] di tutte le sottoattività.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Work] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o versione successiva</p> <p>Nota: se non disponi ancora dell'accesso, chiedi all'amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Accesso [!UICONTROL Contribute] o [!UICONTROL Gestisci] all'attività su cui si trova la sottoattività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## Aggiungi un’attività secondaria a una storia esistente sulla bacheca Scrum

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.

1. Passare all&#39;iterazione o al progetto agile contenente il brano in cui si desidera aggiungere un&#39;attività secondaria. Per informazioni su come passare a un&#39;iterazione, vedere [Visualizzare un&#39;iterazione](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. Passare alla sezione del brano sullo storyboard in cui si desidera aggiungere un&#39;attività secondaria.
1. Fai clic su **[!UICONTROL Aggiungi sottoattività]** nella scheda del brano principale per creare una sottoattività al brano.

   ![Aggiungi sottoattività](assets/agile-story-addsubtask-NWE.png)

   Oppure

   Fare clic su **[!UICONTROL Aggiungi sottoattività]** in un riquadro di sottoattività per creare una sottoattività per la sottoattività.

   [!DNL Workfront] supporta un numero infinito di livelli di sottoattività, ma solo due livelli (sottoattività di sottoattività) vengono visualizzati nello storyboard agile.

   ![Aggiungi sottoattività](assets/agile-story-addsubtask2-NWE.png)

   Quando si aggiunge un&#39;attività secondaria a un brano che al momento non ha una corsia di scorrimento, l&#39;attività principale viene promossa alla colonna [!UICONTROL Storia principale] e la sottoattività si sposta all&#39;interno della corsia di spostamento.

1. Specifica le seguenti informazioni:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nome sottoattività]</strong></td>
      <td> Specificare un nome per la sottoattività.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Descrizione]</strong></td>
      <td>Specificare una descrizione per la sottoattività.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Stima]</strong></td>
      <td>Specifica la stima per l’attività secondaria.<br><p>Quando crei delle stime, tieni presente quanto segue:</p>
       <ul>
        <li>Se il team agile è configurato per stimare le storie in punti, per impostazione predefinita 1 punto equivale a 8 ore. Le stime vengono aggiunte come [!UICONTROL Lavoro Necessario] alla storia.</li>
        <li>Le stime combinate per tutte le sottoattività determinano la stima del brano padre. Per ulteriori informazioni, vedere <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">Aggiornare lo stato delle storie e delle sottoattività sulla bacheca Scrum</a>.</li>
        <li>Quando si crea una nuova sottoattività, il campo [!UICONTROL Stima] è già impostato. Se si reimposta la stima per l'attività secondaria, si reimposta la stima per la storia padre (perché la storia padre è la somma di tutte le relative sottoattività).</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Lavoro Necessario]</strong></td>
      <td> (Disponibile solo nei progetti) Specifica il numero di ore pianificate per l'attività.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignment]</strong></td>
      <td>Iniziare a digitare il nome del team a cui si desidera assegnare la sottoattività, quindi fare clic su di esso quando viene visualizzato nell'elenco a discesa.</td>
     </tr>
    </tbody>
   </table>

1. Fai clic su **[!UICONTROL Crea]**.
