---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Aggiungi una sottoattività a una storia esistente sulla scheda Scrum
description: Durante la creazione di sottoattività per i brani esistenti, ricorda l’impostazione Modalità completamento per il progetto, in quanto questo influisce sul modo in cui i brani vengono aggiornati.
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# Aggiungi una sottoattività a una storia esistente nella [!UICONTROL Scratto] bacheca

Durante la creazione di sottoattività per i brani esistenti, tenere presente quanto segue:

**Quando il [!UICONTROL Modalità completamento] per il progetto è impostata su [!UICONTROL Manuale]:**

* Spostamento di un brano principale con sottoattività in [!UICONTROL Completa] aggiorna il brano principale al 100% e la [!UICONTROL Stato] a [!UICONTROL Completa]. Le sottoattività non vengono aggiornate.
* Per aggiornare [!UICONTROL Percentuale completata] per la storia, devi aggiornarla dal [!UICONTROL Storie] o dalla scheda [!UICONTROL Dettagli] della pagina dell&#39;oggetto.

**Quando il [!UICONTROL Modalità completamento] per il progetto è impostata su [!UICONTROL Automatico]**:

* Spostamento di un brano principale con sottoattività in [!UICONTROL Completa] aggiorna il brano principale al 100% e la [!UICONTROL Stato] a [!UICONTROL Completa]. Le sottoattività vengono inoltre aggiornate al 100% e [!UICONTROL Stato] è stato aggiornato a [!UICONTROL Completa].
* Per aggiornare [!UICONTROL Percentuale completata] per la storia, devi aggiornare il [!UICONTROL Percentuale completata] per tutte le sottoattività. La [!UICONTROL Percentuale completata] per la storia viene calcolata in base al [!UICONTROL Percentuale completata] di tutte le sottoattività.

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
   <td> <p>[!UICONTROL Work] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o superiore</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>[!UICONTROL Contribute] o [!UICONTROL Gestisci] accesso all'attività su cui si trova la sottoattività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Aggiungi una sottoattività a una storia esistente sulla scheda Scrum

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.

1. Passa all’iterazione agile o al progetto che contiene il brano in cui desideri aggiungere una sottoattività. Per informazioni su come passare a un&#39;iterazione, consulta [Visualizzare un’iterazione](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. Passa alla sezione del racconto sulla bacheca in cui desideri aggiungere una sottoattività.
1. Fai clic su **[!UICONTROL Aggiungi sottoattività]** sulla scheda del brano principale per creare una sottoattività al brano.

   ![Aggiungi sottoattività](assets/agile-story-addsubtask-NWE.png)

   Oppure

   Fai clic su **[!UICONTROL Aggiungi sottoattività]** in un riquadro attività secondaria per creare una sottoattività per la sottoattività.

   [!DNL Workfront] supporta infiniti livelli di sottoattività, ma solo due livelli (sottoattività delle sottoattività) vengono visualizzati sulla bacheca di storie agili.

   ![Aggiungi sottoattività](assets/agile-story-addsubtask2-NWE.png)

   Quando si aggiunge una sottoattività a un brano che al momento non ha una corsia, l&#39;attività principale viene promossa alla [!UICONTROL Storia principale] e la sottoattività si sposta all’interno della corsia.

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
      <td role="rowheader"><strong>[!UICONTROL Estimate]</strong></td>
      <td>Specificare la stima per la sottoattività.<br><p>Quando crei stime, tieni presente quanto segue:</p>
       <ul>
        <li>Se il team agile è configurato per stimare le storie in punti, per impostazione predefinita 1 punto è uguale a 8 ore. Le stime vengono aggiunte come [!UICONTROL Pianifica ore] sulla storia.</li>
        <li>Le stime combinate per tutte le sottoattività determinano la stima del racconto principale. Per ulteriori informazioni, consulta <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">Aggiornare lo stato dei racconti e delle sottoattività sulla scheda Scrum</a>.</li>
        <li>Quando crei una nuova sottoattività, il campo Stima [!UICONTROL] è già impostato. Se si reimposta la stima sull'attività secondaria, si reimposta la stima sul brano padre (perché il brano padre è la somma di tutte le sue sottoattività).</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Orario pianificato]</strong></td>
      <td> (Disponibile solo nei progetti) Specifica il numero di ore pianificate per l’attività.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignment]</strong></td>
      <td>Iniziare a digitare il nome del team in cui si desidera assegnare il sottotask, quindi fare clic su di esso quando viene visualizzato nell'elenco a discesa.</td>
     </tr>
    </tbody>
   </table>

1. Fai clic su **[!UICONTROL Crea]**.
