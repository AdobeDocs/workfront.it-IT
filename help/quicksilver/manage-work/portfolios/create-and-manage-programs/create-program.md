---
product-area: programs
navigation-topic: create and manage programs
title: Crea un programma
description: Un programma rappresenta una raccolta di progetti che condividono una strategia, un obiettivo o un obiettivo comuni che trascendono i confini del progetto. I programmi non possono esistere al di fuori di un portfolio.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 6ec353c2-2241-47c2-8c59-1d8ddc43781e
source-git-commit: 93c36a87667097729e89a61f68cc17e9c861d547
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 1%

---

# Crea un programma

Un programma rappresenta una raccolta di progetti che condividono una strategia, un obiettivo o un obiettivo comuni che trascendono i confini del progetto. I programmi non possono esistere al di fuori di un portfolio.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Business] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a Portfoli e programmi con [!UICONTROL Edit] </p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di gestione per il portfolio</p> <p>Dopo aver creato un programma, per impostazione predefinita disponi di autorizzazioni di gestione [!UICONTROL] per</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Crea un programma

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Esegui una delle operazioni seguenti.

   * Crea un programma da [!UICONTROL Programmi] area:

      1. Fai clic su **[!UICONTROL Programmi]** nel menu principale.
      1. Fai clic su **[!UICONTROL Nuovo programma]**.
      1. Nella casella visualizzata, digitare il nome di un Portfolio esistente nella **[!UICONTROL Seleziona Portfolio]** campo .
      1. Digitare il nome del nuovo programma nel **[!UICONTROL Nome]** campo .
      1. Fai clic su **[!UICONTROL Salva]**.
   * Crea un programma da [!UICONTROL Portfoli] area:

      1. Fai clic su **[!UICONTROL Portfoli]** in [!UICONTROL Menu principale], quindi fai clic su un portfolio.
      1. Nel pannello a sinistra, fai clic su **[!UICONTROL Programmi]**.
      1. Fai clic sul pulsante **[!UICONTROL Nuovo programma]** menu a discesa, quindi **[!UICONTROL Nuovo programma]**.


1. Specifica il nome del programma nella **[!UICONTROL Programma senza titolo]** campo .

   Il nome può contenere fino a 255 caratteri.

1. (Facoltativo) Fai clic su **[!UICONTROL Responsabile del programma]** nell&#39;intestazione del programma per aggiornarlo.

   >[!TIP]
   >
   >In qualità di creatore del programma, per impostazione predefinita è impostato come responsabile del programma.

1. Fai clic su **[!UICONTROL Dettagli del programma]** nel pannello a sinistra.
1. Fai doppio clic su un campo per aggiornare le informazioni nel **[!UICONTROL Panoramica]** area.
1. Specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Campo</th> 
      <th>Descrizione</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td> <p>Specifica una descrizione del programma.</p> <p>La descrizione viene visualizzata nella pagina di destinazione del programma.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Program Manager]</td> 
      <td> <p>Inizia a digitare il nome dell’utente che desideri utilizzare come gestore programmi, quindi fai clic sul nome dell’utente quando viene visualizzato nell’elenco a discesa. È lo stesso del [!UICONTROL Program Owner]. </p> <p>Suggerimento: È inoltre possibile aggiornare Program Manager nell'intestazione del programma. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Group] </td> 
      <td> <p>Aggiungi il nome di un singolo gruppo se il gruppo è proprietario del programma o è responsabile del suo completamento. </p> <p>Per selezionare il gruppo di destra, posiziona il cursore sopra di esso e fai clic sull’icona [!UICONTROL information] <img src="assets/info-icon.png"> viene visualizzato accanto a esso. Viene visualizzata una descrizione comandi che elenca le informazioni sul gruppo, ad esempio la gerarchia dei gruppi al di sopra di esso e i relativi amministratori.</p> 
       <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
        <img src="assets/group-details-widget-programs-350x268.png" style="width: 350;height: 268;"> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo e condizionale) Fai clic all’interno del **[!UICONTROL Aggiungi modulo personalizzato]** per selezionare un modulo personalizzato per il portfolio e aggiornare i campi personalizzati.

   >[!TIP]
   >
   >È necessario che i moduli personalizzati del programma siano già stati creati prima di poterli allegare ai programmi.

1. (Facoltativo) Fare doppio clic su un campo per aggiornare le informazioni sul modulo personalizzato.
1. Fai clic su **[!UICONTROL Progetti]** nel pannello a sinistra, quindi **[!UICONTROL Aggiungi progetti]** per aggiungere progetti al programma.

   Per informazioni sull’aggiunta di progetti ai programmi, consulta [Aggiungere un progetto a un programma](../../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

1. Fai clic su **[!UICONTROL Salva modifiche]**.
1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Menu Altro]** ![](assets/more-icon.png) accanto al nome del programma e fai clic su **[!UICONTROL Disattiva programma]**.

   Quando si disattiva un programma, il programma non viene più visualizzato in un elenco di programmi quando gli utenti tentano di aggiungerlo a un progetto. È ancora possibile accedere al programma dal [!UICONTROL Programmi] area.

## Panoramica dell&#39;intestazione del programma

Puoi trovare informazioni limitate sul programma nella relativa intestazione.

Nell&#39;intestazione di un programma vengono visualizzate le informazioni seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Informazioni intestazione</td> 
   <td> <p><strong>Note</strong> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Breadcrumb con il nome del portafoglio</td> 
   <td>Puoi accedere al portfolio a cui appartiene il programma dall’intestazione del programma. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del programma</td> 
   <td>È possibile modificare il nome del programma nell'intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto e dello stato di attivazione</td> 
   <td>La parola "Programma" viene visualizzata in una struttura verde quando si visualizza un programma. Accanto alla parola "[!UICONTROL Disattivato]" viene visualizzato il contorno grigio se il programma non è contrassegnato come [!UICONTROL Active]. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Settore azioni del programma </td> 
   <td> <p>Fare clic su una delle seguenti opzioni per accedere a ulteriori informazioni o opzioni di modifica per il programma:</p> 
    <ul> 
     <li>Icona a forma di stella per aggiungere il programma all'elenco dei Preferiti</li> 
     <li> <p>Menu [!UICONTROL Altro] <img src="assets/qs-more-menu.png"> per effettuare una delle seguenti operazioni: </p> 
      <ul> 
       <li>Modifica del programma</li> 
       <li>Disattivala. Quando un programma è disattivato, non è più possibile associarlo a progetti a livello di progetto. </li> 
       <li> <p>La elimini. L'eliminazione del programma non comporta l'eliminazione dei progetti nel programma. Rimuove l'associazione dei progetti al programma. </p> </li> 
       <li>Condividi con altri</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percent Complete]</td> 
   <td> <p>Non è possibile modificare la percentuale di completamento del programma nell'intestazione. Queste informazioni vengono aggiornate dai progetti del programma. Per impostazione predefinita, la percentuale di completamento del programma è una media della percentuale di completamento dei progetti in uno stato [!UICONTROL Current] e [!UICONTROL Approved] che appartiene al programma.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Manager]</td> 
   <td> <p>È possibile modificare Gestione programmi nell’intestazione. È lo stesso del [!UICONTROL Program Owner]. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di completamento pianificata]</td> 
   <td>Non è possibile modificare la percentuale di completamento del programma nell'intestazione. La percentuale di completamento del programma corrisponde alla media della percentuale di completamento dei progetti nell'intestazione. I progetti qui rappresentati sono progetti con stato [!UICONTROL Current] e [!UICONTROL Approved]. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Active Projects Condition]</td> 
   <td>Questo è un calcolo della percentuale di progetti nel programma con [!UICONTROL Condition] impostato come [!UICONTROL On Target], [!UICONTROL At Risk] o [!UICONTROL In Trouble]. I progetti qui rappresentati sono progetti con stato [!UICONTROL Current] e [!UICONTROL Approved]. </td> 
  </tr> 
 </tbody> 
</table>

## Spostare un programma

Puoi aggiungere programmi esistenti a un portfolio. Poiché i programmi non possono esistere in due portafogli diversi, l’aggiunta di un programma esistente lo sposta in modo permanente da un portfolio all’altro.

Per ulteriori informazioni, consulta [Aggiungi un programma esistente a un portfolio](../../../manage-work/portfolios/create-and-manage-programs/move-program.md).
