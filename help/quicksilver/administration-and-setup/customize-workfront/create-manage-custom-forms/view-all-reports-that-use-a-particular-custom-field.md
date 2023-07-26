---
title: Visualizzare tutti i rapporti che utilizzano un particolare campo personalizzato o widget
description: Nell’area Forms personalizzata è possibile aggiungere una visualizzazione personalizzata che mostra quali rapporti utilizzano un particolare campo personalizzato o widget. Questa funzione è utile quando devi modificare o eliminare il campo o il widget, perché potrebbe già essere implementato in uno o più rapporti. È importante valutare se quei rapporti avranno bisogno di aggiustamenti per continuare a funzionare correttamente.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Visualizzare tutti i rapporti che utilizzano un particolare campo personalizzato o widget

Nell’area Forms personalizzata è possibile aggiungere una visualizzazione personalizzata che mostra quali rapporti utilizzano un particolare campo personalizzato o widget. Questa funzione è utile quando devi modificare o eliminare il campo o il widget, perché potrebbe già essere implementato in uno o più rapporti. È importante valutare se quei rapporti avranno bisogno di aggiustamenti per continuare a funzionare correttamente.

Per informazioni sui campi personalizzati e i widget nei moduli personalizzati, vedi [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Aggiungere o modificare un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni sulle modalità di concessione dell'accesso da parte degli amministratori di Workfront, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sulle configurazioni di piano, tipo di licenza o livello di accesso disponibili, contattare l&#39;amministratore Workfront.

## Elencare i rapporti che utilizzano un particolare campo personalizzato o widget

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Forms personalizzato**.
1. Apri **Campi** per visualizzare un rapporto che elenca tutti i campi personalizzati e i widget nell’istanza Workfront.

   ![](assets/fields-tab.png)

1. Fai clic su **Visualizza** nell’intestazione nella parte superiore dell’elenco, quindi controlla eventuali viste personalizzate nell’elenco che includono **Rapporti** (che non è una colonna predefinita in questa scheda).

   Nella colonna Rapporti è possibile visualizzare i rapporti che utilizzano ogni campo personalizzato e widget aggiunto a un modulo personalizzato nel sistema. È possibile che un utente abbia già creato una visualizzazione che include **Rapporti** colonna.

1. Se non viene visualizzata una visualizzazione che include **Rapporti** , crea una nuova visualizzazione che la includa:

   1. Fai clic su **Visualizza** menu a discesa, quindi fai clic su **Nuova visualizzazione**.

   1. Il giorno **Nuova visualizzazione** pagina visualizzata, nella casella accanto all&#39;angolo superiore sinistro sostituire **Nuova vista parametro** con un nome descrittivo per la visualizzazione, ad esempio *Campi e widget*.

   1. Clic **Aggiungi colonna** nell&#39;angolo inferiore destro.
   1. In **Mostra in questa colonna** che viene visualizzata vicino all&#39;angolo superiore sinistro, inizia a digitare *rapporto*, quindi seleziona **Rapporti** quando viene visualizzato nell’elenco sotto la casella.

   1. (Condizionale) Se desideri spostare il **Rapporti** colonna appena aggiunta a una diversa posizione orizzontale, trascina la relativa intestazione nella **Anteprima colonna** nella parte inferiore della pagina.

   1. Clic **Fine**, quindi fai clic su **Salva visualizzazione**.

1. Fai clic su **Visualizza** , quindi selezionare il nome della visualizzazione personalizzata appena creata.
1. In **Nome** , trovare il campo personalizzato o il widget che si intende modificare o eliminare, quindi esaminare **Rapporti** nella riga per vedere quali rapporti la utilizzano, se presenti.

   Per trovare le informazioni per questa colonna, Workfront cerca i campi personalizzati e i widget in tutti i filtri, le visualizzazioni e i raggruppamenti dei rapporti.

   Se viene visualizzato un segno più, è possibile fare clic su tale riga di testo per visualizzare una casella in cui sono elencati tutti i report aggiuntivi che utilizzano il campo o il widget.

   >[!NOTE]
   >
   >Il tempo di caricamento iniziale di questo strumento può richiedere da 10 secondi a 2,5 minuti, a seconda della quantità di dati nel sistema.

   >[!TIP]
   >
   >Se non hai tempo di analizzare i rapporti che utilizzano il campo personalizzato o il widget, puoi fare clic su Esporta per creare un file che li elenca. Puoi condividere questo file con chiunque possieda un report che utilizza il campo o il widget e discutere delle modifiche che devono essere apportate, dell’impatto che potrebbe avere sul report e di ciò che deve essere fatto per garantire che il report continui a funzionare correttamente.
   >
   >Questa vista è disponibile anche in un rapporto Parametro:
   >      
   > 1. Nel menu principale, fare clic su **Rapporti**.
   > 1. Fai clic su in alto a sinistra **Nuovo rapporto**, quindi fai clic su **Parametro** nell’elenco visualizzato.
   > 1. Clic **Aggiungi colonna** nell&#39;angolo inferiore destro.
   > 1. In **Mostra in questa colonna** che viene visualizzata vicino all&#39;angolo superiore sinistro, inizia a digitare *rapporto*, quindi seleziona **Rapporti** quando viene visualizzato nell’elenco sotto la casella.
   > 1. (Condizionale) Se desideri spostare il **Rapporti** colonna appena aggiunta a una diversa posizione orizzontale, trascina la relativa intestazione nella **Anteprima colonna** nella parte inferiore della pagina.
   > 1. Clic **Fine**, quindi fai clic su **Salva+Chiudi**.
   > 1. Digita un nome descrittivo per il rapporto, ad esempio *Campi e widget*.
