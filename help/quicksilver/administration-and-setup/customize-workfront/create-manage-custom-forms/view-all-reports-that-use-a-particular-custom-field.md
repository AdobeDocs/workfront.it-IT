---
title: Visualizzare tutti i rapporti che utilizzano un campo personalizzato o un widget particolare
description: È possibile aggiungere una visualizzazione personalizzata nell'area Forms personalizzata che mostri quali report utilizzano un campo o un widget personalizzato specifico. Questa funzione è utile quando devi modificare o eliminare il campo o il widget, perché potrebbe essere già implementato in uno o più rapporti. È importante valutare se tali rapporti avranno bisogno di aggiustamenti per poter continuare a funzionare correttamente.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Visualizzare tutti i rapporti che utilizzano un campo personalizzato o un widget particolare

È possibile aggiungere una visualizzazione personalizzata nell&#39;area Forms personalizzata che mostri quali report utilizzano un campo o un widget personalizzato specifico. Questa funzione è utile quando devi modificare o eliminare il campo o il widget, perché potrebbe essere già implementato in uno o più rapporti. È importante valutare se tali rapporti avranno bisogno di aggiustamenti per poter continuare a funzionare correttamente.

Per informazioni sui campi e i widget personalizzati nei moduli personalizzati, consultare [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Aggiunta o modifica di un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni su come gli amministratori di Workfront concedono questo accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o configurazioni del livello di accesso si dispone, contattare l&#39;amministratore Workfront.

## Elencare i rapporti che utilizzano un campo personalizzato o un widget particolare

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Forms personalizzato**.
1. Apri **Campi** per visualizzare un elenco di tutti i campi e widget personalizzati nella tua istanza Workfront.

   ![](assets/fields-tab.png)

1. Fai clic sul pulsante **Visualizza** menu a discesa nell’intestazione nella parte superiore dell’elenco, quindi controlla eventuali viste personalizzate nell’elenco che includono **Rapporti** (che non è una colonna predefinita in questa scheda).

   Nella colonna Rapporti è possibile vedere quali rapporti utilizzano ogni campo e widget personalizzato aggiunto a un modulo personalizzato nel sistema. È possibile che qualcuno abbia già creato una visualizzazione che include **Rapporti** colonna.

1. Se non visualizzi una visualizzazione che include **Rapporti** crea una nuova visualizzazione che la include:

   1. Fai clic sul pulsante **Visualizza** menu a discesa, quindi fai clic su **Nuova vista**.

   1. Sulla **Nuova vista** nella casella posta nell&#39;angolo in alto a sinistra, sostituire **Nuova vista parametro** con un nome descrittivo per la visualizzazione, ad esempio *Campi e widget*.

   1. Fai clic su **Aggiungi colonna** nell&#39;angolo in basso a destra.
   1. In **Mostra in questa colonna** casella visualizzata nell&#39;angolo superiore sinistro, inizia a digitare *rapporto*, quindi seleziona **Rapporti** quando appare nell&#39;elenco sotto la casella.

   1. (Condizionale) Per spostare il **Rapporti** colonna appena aggiunta in una posizione orizzontale diversa, trascina l’intestazione nella **Anteprima a colonne** nella parte inferiore della pagina.

   1. Fai clic su **Fine**, quindi fai clic su **Salva visualizzazione**.

1. Fai clic sul pulsante **Visualizza** dal menu a discesa, quindi seleziona il nome della visualizzazione personalizzata appena creata.
1. In **Nome** trova il campo personalizzato o il widget che intendi modificare o eliminare, quindi osserva **Rapporti** in quella riga per vedere quali report lo utilizzano, se presenti.

   Per trovare le informazioni per questa colonna, Workfront cerca i campi e i widget personalizzati in tutti i filtri, le visualizzazioni e i raggruppamenti dei rapporti.

   Se viene visualizzato un segno più, è possibile fare clic sulla riga di testo per visualizzare una casella in cui sono elencati tutti i rapporti aggiuntivi che utilizzano il campo o il widget.

   >[!NOTE]
   >
   >Il tempo di caricamento iniziale per questo strumento può richiedere da 10 a 2,5 minuti, a seconda della quantità di dati nel sistema.

   >[!TIP]
   >
   >Se non hai il tempo di esaminare i rapporti che utilizzano il campo o il widget personalizzato, puoi fare clic su Esporta per creare un file in cui includerli. Puoi condividere questo file con tutti coloro che possiedono un rapporto che utilizza il campo o il widget e discutere le modifiche necessarie, l&#39;impatto che potrebbe avere sul rapporto e cosa deve essere fatto per garantire che il rapporto continui a funzionare correttamente.
   >
   >Questa visualizzazione è disponibile anche in un rapporto Parametro :
   >      
   > 1. Nel menu principale, fai clic su **Rapporti**.
   > 1. Fai clic su nell’angolo in alto a sinistra **Nuovo rapporto**, quindi fai clic su **Parametro** nell’elenco visualizzato.
   > 1. Fai clic su **Aggiungi colonna** nell&#39;angolo in basso a destra.
   > 1. In **Mostra in questa colonna** casella visualizzata nell&#39;angolo superiore sinistro, inizia a digitare *rapporto*, quindi seleziona **Rapporti** quando appare nell&#39;elenco sotto la casella.
   > 1. (Condizionale) Per spostare il **Rapporti** colonna appena aggiunta in una posizione orizzontale diversa, trascina l’intestazione nella **Anteprima a colonne** nella parte inferiore della pagina.
   > 1. Fai clic su **Fine**, quindi fai clic su **Salva e chiudi**.
   > 1. Inserisci un nome descrittivo per il rapporto, ad esempio *Campi e widget*.

