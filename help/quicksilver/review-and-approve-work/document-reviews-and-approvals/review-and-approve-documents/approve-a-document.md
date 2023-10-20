---
product-area: projects
navigation-topic: approvals
title: Approvare un documento
description: Se si è assegnati come approvatori a un documento, è possibile prendere una decisione in diversi modi.
author: Nolan
feature: Work Management, Digital Content and Documents
exl-id: 5490973b-99a7-4790-9d89-bf8f16ff5765
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 0%

---

# Approvare un documento

Se si è assegnati come approvatori a un documento, è possibile prendere una decisione in diversi modi.

Per informazioni sulla creazione di una nuova approvazione del documento, vedere [Creare un’approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>Il contenuto di questo articolo fa riferimento alla funzionalità di approvazione dei documenti aggiornata, disponibile solo per account specifici. Per informazioni sui processi di approvazione standard, vedi gli articoli elencati in [Approvazioni lavoro](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso di visualizzazione o accesso successivo agli oggetti associati alle approvazioni</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per gli oggetti associati alle approvazioni</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Approvare un documento dalla Home

1. Fai clic su **Home** icona ![](../assets/home-icon-30x29.png) nell’angolo in alto a sinistra di Adobe Workfront.

   >[!NOTE]
   >
   >L’amministratore di Workfront potrebbe apportare le seguenti modifiche all’icona Home nel tuo ambiente:
   >
   >* Sostituiscilo con un’immagine personalizzata per illustrare la tua organizzazione. In questo caso, l’icona avrà un aspetto diverso da quello mostrato in questo articolo.
   >
   >* Sostituisci la pagina collegata con un’altra pagina. In questo caso, fai clic su **Menu principale** ![](../assets/main-menu-icon.png) nell’angolo superiore destro della pagina, quindi fai clic su **Home**.

1. Clic **Filtri** in alto a sinistra nella pagina e assicurati che **Approvazioni** è selezionato.

   Tutti gli elementi di lavoro che richiedono la tua approvazione vengono visualizzati nell’elenco.

   >[!NOTE]
   >
   >Le approvazioni assegnate a Ruoli o Gruppi non sono elencate nella Home. Le approvazioni assegnate ai team vengono visualizzate nel raggruppamento Richiesta team in Work List (Elenco di lavoro).

1. Fare clic sull&#39;approvazione del documento nell&#39;elenco per il quale si desidera prendere una decisione di approvazione. Le informazioni relative all’approvazione verranno visualizzate sul lato destro della pagina.

1. Fai clic su una delle due opzioni di approvazione seguenti nell’angolo in alto a destra della pagina:

   * Il **Approva** Il menu a discesa contiene due opzioni:

      * **Approva** indica che non sono necessarie modifiche per questa versione del documento e che viene concessa l&#39;approvazione.

      * **Approva con modifiche** indica che nel documento sono ancora necessarie alcune piccole modifiche, ma l&#39;approvazione viene concessa a condizione che tali modifiche vengano apportate. Se si seleziona questa opzione, verrà visualizzata una finestra contenente una casella di testo denominata **Passaggi successivi** dove è possibile specificare le modifiche necessarie per approvare il documento. Immettere tali informazioni e fare clic su **Aggiungi messaggio** oppure puoi fare clic su **Ignora** inviare la decisione di approvazione senza ulteriori informazioni.

   * **Necessità di lavoro** indica che la versione del documento non è approvata e richiede modifiche significative.

   Quando visualizzi le approvazioni dei documenti nella Home, tieni presente quanto segue:

   * Il nome dell’utente che ha richiesto l’approvazione viene visualizzato sopra il nome del documento nella Home con il testo &quot;*Utente A* desidera la tua approvazione per...&quot;, nonché in **Inviato da** nelle informazioni sull’approvazione visualizzate a destra dopo aver selezionato un’approvazione.

   * Dopo aver preso una decisione su un’approvazione, l’approvazione rimane nella scheda Approvazioni personali con il testo &quot;Presa di decisione&quot; fino a quando non fai clic su **Aggiorna** o fino all&#39;aggiornamento della pagina del browser.

## Approvare un documento dalla pagina del documento

1. Passare alla pagina del documento facendo clic sul nome del documento.

1. Selezionare la versione del documento in attesa di approvazione nel menu a discesa versione accanto al nome del documento. Per impostazione predefinita, viene selezionata la versione più recente.

   Se la versione attualmente selezionata del documento ha un&#39;approvazione in sospeso, i pulsanti di decisione di approvazione vengono visualizzati nell&#39;angolo in alto a destra della pagina. Se altre versioni del documento hanno approvazioni in sospeso, il menu a discesa della versione visualizza un punto rosso.

   <!--
   ![](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. Fai clic su una delle due opzioni di approvazione seguenti nell’angolo in alto a destra della pagina:

   * Il **Approva** Il menu a discesa contiene due opzioni:

      * **Approva** indica che non sono necessarie modifiche per questa versione del documento e che viene concessa l&#39;approvazione.

      * **Approva con modifiche** indica che nel documento sono ancora necessarie alcune piccole modifiche, ma l&#39;approvazione viene concessa a condizione che tali modifiche vengano apportate. Se si seleziona questa opzione, verrà visualizzata una finestra contenente una casella di testo denominata **Passaggi successivi** dove è possibile specificare le modifiche necessarie per approvare il documento. Immettere tali informazioni e fare clic su **Aggiungi messaggio** oppure puoi fare clic su **Ignora** inviare la decisione di approvazione senza ulteriori informazioni.

   * **Necessità di lavoro** indica che la versione del documento non è approvata e richiede modifiche significative.

## Approvare un documento dal riquadro Riepilogo documento

1. Vai al progetto, all’attività o al problema che contiene il documento, quindi seleziona **Documenti**.

1. Fare clic sul documento che richiede l&#39;approvazione e verrà aperto il riquadro Riepilogo documento.

1. Seleziona la versione del documento da rivedere nel menu a discesa della versione. Per impostazione predefinita, viene selezionata la versione più recente.

   Se la versione attualmente selezionata del documento ha un&#39;approvazione in sospeso, i pulsanti di decisione di approvazione vengono visualizzati nell&#39;angolo in alto a destra del riquadro Riepilogo documento. Se altre versioni del documento hanno approvazioni in sospeso, il menu a discesa della versione visualizza un punto rosso.

   <!--
   ![](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. Fare clic su una delle due opzioni di approvazione seguenti nell&#39;angolo superiore destro del riquadro Riepilogo documento:

   * Il **Approva** Il menu a discesa contiene due opzioni:

      * **Approva** indica che non sono necessarie modifiche per questa versione del documento e che viene concessa l&#39;approvazione.

      * **Approva con modifiche** indica che nel documento sono ancora necessarie alcune piccole modifiche, ma l&#39;approvazione viene concessa a condizione che tali modifiche vengano apportate. Se si seleziona questa opzione, verrà visualizzata una finestra contenente una casella di testo denominata **Passaggi successivi** dove è possibile specificare le modifiche necessarie per approvare il documento. Immettere tali informazioni e fare clic su **Aggiungi messaggio** oppure puoi fare clic su **Ignora** inviare la decisione di approvazione senza ulteriori informazioni.

   * **Necessità di lavoro** indica che la versione del documento non è approvata e richiede modifiche significative.
