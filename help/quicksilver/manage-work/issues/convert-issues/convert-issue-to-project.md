---
product-area: projects
navigation-topic: convert-issues
title: Convertire un problema in un progetto in Adobe Workfront
description: Convertire un problema in un progetto in Adobe Workfront
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: f4ef463ebdc9a4a7a0802e5394d7820ebc447aa9
workflow-type: tm+mt
source-wordcount: '1472'
ht-degree: 0%

---

# Convertire un problema in un progetto in Adobe Workfront

Se è necessario fare di più per completare un problema dopo l’invio del problema, puoi convertire il problema in un progetto.

È possibile convertire un problema in un nuovo progetto oppure convertirlo in un progetto utilizzando un modello. Questo articolo descrive entrambi i modi per convertire i problemi in progetti.

>[!IMPORTANT]
>
>Per informazioni generali sulla conversione dei problemi, si consiglia di leggere anche l’articolo [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Durante la creazione di un progetto a partire da un problema, alcuni campi del progetto si popolano da altri oggetti. Per ulteriori informazioni, consulta la sezione &quot;Nuove impostazioni predefinite del progetto&quot; nell’articolo [Creare un progetto](../../../manage-work/projects/create-projects/create-project.md).

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
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Issues, Tasks, and Projects</p> <p>Modifica l'accesso ai dati finanziari per aggiornare le informazioni finanziarie per un progetto convertito dall'emissione</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni per il problema</p> <p>Ottieni le autorizzazioni di gestione per il progetto dopo la conversione del problema</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront.

## Convertire un problema in un progetto

È possibile convertire un problema in un progetto vuoto o convertirlo in un progetto utilizzando un modello.

1. Vai a un progetto e fai clic su **[!UICONTROL Problemi]** nel pannello a sinistra.
1. Nell’elenco dei problemi visualizzato, effettua una delle seguenti operazioni:

   * Per convertire un problema in un progetto vuoto, fai clic sul nome del problema, quindi sulla **[!UICONTROL Altro]** menu ![](assets/more-icon.png) a destra del nome del problema, quindi fai clic su **[!UICONTROL Converti in progetto vuoto]**.


     Oppure

     Seleziona il problema nell’elenco dei problemi, fai clic su **[!UICONTROL Altro]** menu ![](assets/more-icon.png) nella parte superiore dell’elenco, quindi fai clic su **[!UICONTROL Converti in progetto vuoto]**.

     >[!IMPORTANT]
     >
     >L’opzione Converti in progetto vuoto viene visualizzata solo quando l’amministratore di sistema o di gruppo ha abilitato l’opzione [!UICONTROL Consenti agli utenti di creare progetti senza utilizzare un modello] preferenza in [!UICONTROL Configurazione] area. Per ulteriori informazioni, consulta [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


     Dopo aver convertito il problema, è necessario aggiungere manualmente le attività al progetto o allegare un modello al progetto.

     Procedi con il passaggio 3e seguente.

     <!--
     Is this accurate?
     -->

     >[!TIP]
     >   
     >* Se il problema è stato creato utilizzando una coda di richieste, il nuovo progetto eredita il Gruppo della coda di richieste.
     >* Se il problema è stato creato aggiungendolo alla sezione Problemi del progetto, il nuovo progetto eredita il Gruppo del progetto del problema.

   * Per convertire un problema in un progetto utilizzando un modello, effettuare una delle seguenti operazioni:

      * Fai clic sul nome di un problema, quindi fai clic su [!UICONTROL **Altro**] menu ![](assets/more-icon.png) a destra del nome del problema

        ![](assets/issue-more-menu-expanded-with-convert-to-project-options-nwe-350x213.png)

        Oppure

      * Seleziona il problema nell’elenco dei problemi, in un rapporto o in un dashboard, fai clic su **Altro** menu ![](assets/more-icon.png) nella parte superiore dell’elenco, quindi fai clic su **Converti in progetto da modello** e inizia a digitare il nome di un modello nel **Cerca modello** , quindi fare clic sul nome del modello visualizzato nell&#39;elenco. Continuare con il passaggio 3.

        <!--      
        (is this accurate?)      
        -->

     >[!TIP]
     >
     >Se sono stati aggiunti modelli all&#39;elenco Preferiti, è possibile passare il puntatore del mouse sull&#39;icona [!UICONTROL **Modelli preferiti**] e fare clic sul modello che si desidera utilizzare.

     Viene visualizzata la casella Nuovo progetto da modello (New Project from Template).

     ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

     >[!TIP]
     >
     >Se il problema è associato a un processo di approvazione o è già associato a un oggetto di risoluzione, Workfront visualizza un avviso nella parte superiore della casella Converti in progetto per avvisarti che l’approvazione verrà rimossa o che l’oggetto di risoluzione verrà sovrascritto durante la conversione. Per ulteriori informazioni, consulta [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. (Condizionale) Se hai selezionato di convertire il problema in un progetto utilizzando un modello, continua con i seguenti passaggi:

   1. Rivedi i dettagli del modello a destra.

      I dettagli del modello includono quanto segue:

      * Durata modello
      * Proprietario del modello
      * Numero di attività di primo livello che includono i nomi delle tre attività principali
      * Numero di tutte le attività nel modello
      * Nomi dei moduli personalizzati del modello

   1. (Facoltativo) Passa il puntatore del mouse sul nome di un modello e fai clic sull&#39;icona Preferiti ![](assets/favorites-icon-small.png) per contrassegnarlo come preferito per un utilizzo futuro.

      >[!TIP]
      >
      >Puoi avere fino a 40 elementi Workfront contrassegnati come preferiti. Ciò include modelli e altri elementi.

   1. Clic [!UICONTROL **Usa modello**] per selezionare un modello.

      Il [!UICONTROL Converti in progetto] viene visualizzata la casella.

      ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

   1. Se un campo è già popolato nel modello, il campo viene prepopolato in [!UICONTROL Converti in progetto] casella. Puoi modificare i valori precompilati in modo che corrispondano meglio al tuo progetto. Per ulteriori informazioni, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >* L’amministratore del sistema o del gruppo può aggiungere o rimuovere campi nel [!UICONTROL Casella Converti in progetto] aggiornando le informazioni di Project Details (Dettagli progetto) in [!UICONTROL Modello di layout].
      >
      >* Per aggiornare i campi in [!UICONTROL Finanza] sezione nella sezione [!UICONTROL Converti in progetto] casella che devi avere [!UICONTROL Modifica] accesso a [!UICONTROL Dati finanziari] nel tuo livello di accesso. Se è stato [!UICONTROL Visualizza] accesso a [!UICONTROL Dati finanziari] nel tuo livello di accesso tutte le informazioni finanziarie del modello vengono trasferite al nuovo progetto e non puoi modificarle mentre converti il problema. Per informazioni, consulta [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) e [Condividere un modello](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   1. (Facoltativo e condizionale) Fai clic su [!UICONTROL **Opzioni**] nel pannello a sinistra, seleziona una delle opzioni disponibili:

      * [!UICONTROL **Mantieni il problema originale e collegane la risoluzione a questo progetto**]

        Se questa opzione è deselezionata, il problema originale viene eliminato.

        >[!NOTE]
        >
        >Gli utenti che non dispongono dell’accesso o delle autorizzazioni necessarie per eliminare un problema non potranno eliminarlo mentre lo stanno convertendo, indipendentemente dallo stato di questa impostazione. Per informazioni sull’accesso e le autorizzazioni per i problemi, consulta:
        >
        >* [Concedere l’accesso ai problemi](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
        > 
        >* [Condividere un problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

      * [!UICONTROL **Consenti a (Nome utente) di accedere a questo progetto**]

        Se non è selezionata, il [!UICONTROL Contatto principale] non ha accesso alla nuova attività.

        >[!NOTE]
        >
        >Le opzioni disponibili dipendono dal modo in cui l’amministratore di Workfront le ha configurate per tutti gli utenti del sistema o per il gruppo. Per ulteriori informazioni, consulta [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
        >
        >
        >Oppure, se i gruppi di livello superiore dell’organizzazione li hanno configurati separatamente, le opzioni disponibili dipendono dal gruppo selezionato per il nuovo progetto al passaggio 6. Per ulteriori informazioni, consulta [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   1. Clic [!UICONTROL **Forms personalizzato**] ed effettuare una delle seguenti operazioni:

      * Esamina i moduli personalizzati allegati al modello. Si trasferiranno al nuovo progetto.
      * Assicurati che tutti i campi obbligatori contengano informazioni valide.
      * Ridisporre i moduli personalizzati trascinandoli ![](assets/drag-object-icon.png) dove li volete.
      * Fai clic su **x** a destra di qualsiasi modulo che non si desidera trasferire al progetto.
      * Se necessario, trasferisci le informazioni del modulo personalizzato dal problema al progetto.

        >[!TIP]
        >
        >* Se un modulo personalizzato con più oggetti allegato al problema è configurato per l’utilizzo sia con problemi che con progetti, tutte le informazioni salvate nel modulo vengono mantenute quando si effettua la conversione, se i campi sono presenti sia sul problema che nei moduli personalizzati del progetto.
        >* Se al problema e al progetto è allegato un modulo personalizzato con più oggetti con un campo calcolato, il problema e il progetto devono essere compatibili con tutti i campi a cui si fa riferimento nei campi personalizzati calcolati del modulo. In caso di incompatibilità, un messaggio ti avvisa di apportare le modifiche necessarie. Per ulteriori informazioni, consulta la sezione &quot;Campi personalizzati calcolati nei moduli personalizzati con più oggetti&quot; in [Aggiungere dati calcolati a un modulo personalizzato con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
        >* Se utilizzi un modello per la conversione e un modulo personalizzato allegato al modello contiene un campo personalizzato che si trova anche in un modulo personalizzato allegato al problema, per il nuovo progetto viene utilizzato il valore del campo del problema. Tuttavia, se il campo personalizzato è vuoto nel problema, viene utilizzato il valore del modello.

   1. Clic [!UICONTROL **Converti in progetto**].

      >[!TIP]
      >
      >Se hai deciso di eliminare il problema originale, ora il problema è un progetto.
      >   
      >Oppure
      >  
      >Se hai deciso di mantenere il problema originale, questo ora è collegato al nuovo progetto e verrà completato al termine del progetto.
      >
      >Alcuni campi dei problemi vengono trasferiti al progetto. La maggior parte dei campi definiti nel modello viene trasferita automaticamente al nuovo progetto creato se non sono stati modificati nei passaggi precedenti. Per informazioni, consulta [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. (Facoltativo) Se necessario, imposta ulteriori dettagli &#x200B; progetto (proprietario del progetto, date del progetto) e attività.
1. Clic [!UICONTROL **Converti in progetto**].

   Il problema ora viene convertito in un progetto.

1. Clic [!UICONTROL **Vai al progetto**] all&#39;interno del [!UICONTROL Completato] nell’angolo superiore destro della pagina. Viene visualizzata la pagina del progetto.
