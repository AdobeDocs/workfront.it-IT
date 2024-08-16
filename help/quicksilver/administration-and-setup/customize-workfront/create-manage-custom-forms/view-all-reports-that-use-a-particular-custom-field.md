---
title: Visualizza tutti i report che utilizzano un particolare campo personalizzato o widget
description: Nell’area Forms personalizzata è possibile aggiungere una visualizzazione personalizzata che mostra quali rapporti utilizzano un particolare campo personalizzato o widget. Questa funzione è utile quando devi modificare o eliminare il campo o il widget, perché potrebbe già essere implementato in uno o più rapporti. È importante valutare se quei rapporti avranno bisogno di aggiustamenti per continuare a funzionare correttamente.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: c1bc2832d1c52885e737056172e7aec93a951e6c
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 0%

---

# Visualizzare tutti i rapporti che utilizzano un particolare campo personalizzato o widget

Nell’area Forms personalizzata è possibile aggiungere una visualizzazione personalizzata che mostra quali rapporti utilizzano un particolare campo personalizzato o widget. Questa funzione è utile quando devi modificare o eliminare il campo o il widget, perché potrebbe già essere implementato in uno o più rapporti. È importante valutare se quei rapporti avranno bisogno di aggiustamenti per continuare a funzionare correttamente.

Per informazioni sui campi personalizzati e i widget nei moduli personalizzati, vedere [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>piano Adobe Workfront</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Nuovo: Standard</p>
   <p>oppure</p>
   <p>Corrente: Piano</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Elencare i rapporti che utilizzano un particolare campo personalizzato o widget

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Forms personalizzato**.
1. Fai clic su **Campi** per visualizzare un report in cui sono elencati tutti i campi e i widget personalizzati nella tua istanza di Workfront.

1. Fai clic sul menu **Visualizza**, quindi controlla eventuali viste personalizzate nell&#39;elenco che includono la colonna **Rapporti** (che non è una colonna predefinita in questa scheda).

   Nella colonna Rapporti è possibile visualizzare i rapporti che utilizzano ogni campo personalizzato e widget aggiunto a un modulo personalizzato nel sistema. È possibile che un utente abbia già creato una visualizzazione che include la colonna **Report**.

1. Se non vedi una visualizzazione che include la colonna **Report**, crea una nuova visualizzazione che la include:

   1. Fai clic sul menu **Visualizza**, quindi fai clic su **Nuova visualizzazione**.

   1. Nella pagina **Nuova visualizzazione** visualizzata, nella casella accanto all&#39;angolo superiore sinistro sostituire **Nuova visualizzazione parametri** con un nome descrittivo per la visualizzazione, ad esempio *Campi e widget*.

   1. Fai clic su **Aggiungi colonna** nell&#39;angolo inferiore destro.
   1. Nella casella **Mostra in questa colonna** visualizzata nell&#39;angolo superiore sinistro, inizia a digitare *report*, quindi seleziona **Report** quando viene visualizzato nell&#39;elenco sotto la casella.

   1. (Condizionale) Se vuoi spostare la colonna **Rapporti** che hai appena aggiunto in una posizione orizzontale diversa, trascina la relativa intestazione nell&#39;area **Anteprima colonna** nella parte inferiore della pagina.

   1. Fai clic su **Fine**, quindi fai clic su **Salva visualizzazione**.

1. Fai clic sul menu a discesa **Visualizza**, quindi seleziona il nome della visualizzazione personalizzata appena creata.
1. Nella colonna **Nome**, individua il campo personalizzato o il widget che intendi modificare o eliminare, quindi controlla la colonna **Rapporti** in quella riga per vedere quali rapporti lo utilizzano, se presenti.

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
   > 1. Nel menu principale, fare clic su **Report**.
   > 1. Fai clic su **Nuovo report** nell&#39;angolo in alto a sinistra, quindi fai clic su **Parametro** nell&#39;elenco visualizzato.
   > 1. Fai clic su **Aggiungi colonna** nell&#39;angolo inferiore destro.
   > 1. Nella casella **Mostra in questa colonna** visualizzata nell&#39;angolo superiore sinistro, inizia a digitare *report*, quindi seleziona **Report** quando viene visualizzato nell&#39;elenco sotto la casella.
   > 1. (Condizionale) Se vuoi spostare la colonna **Rapporti** che hai appena aggiunto in una posizione orizzontale diversa, trascina la relativa intestazione nell&#39;area **Anteprima colonna** nella parte inferiore della pagina.
   > 1. Fai clic su **Fine**, quindi su **Salva+Chiudi**.
   > 1. Digitare un nome descrittivo per il report, ad esempio *Campi e widget*.
