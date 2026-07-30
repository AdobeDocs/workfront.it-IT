---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Cronologia modifiche
description: La cronologia modifiche consente di visualizzare un registro delle modifiche apportate agli oggetti di Workfront
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: de1f426630b8c99cfaca07dafb9c2de0f16f263f
workflow-type: tm+mt
source-wordcount: '737'
ht-degree: 4%

---

# Visualizzare e gestire la cronologia delle modifiche

{{preview-fast-release-general}}

Puoi visualizzare la cronologia delle modifiche, inclusi i registri di audit, nell’area Tracciamento delle modifiche di Configurazione.

* **I registri di controllo** sono modifiche attivate dagli utenti.
Per ulteriori informazioni sui registri di controllo e sull&#39;area Registri di controllo, vedere [Panoramica dei registri di controllo](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/audit-logs.md) e [Visualizzare ed esportare i registri di controllo](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).
* **Configurazione** visualizza i campi tracciati per l&#39;elenco della cronologia delle modifiche.
  <span class="preview">In qualità di amministratore di Workfront, puoi configurare i campi oggetto e le azioni di cui Workfront tiene traccia. Workfront, ad esempio, può tenere traccia di tutte le modifiche apportate dagli utenti ai nomi dei problemi all&#39;interno del sistema. Qualsiasi modifica al nome del problema viene quindi visualizzata come una voce nel registro della cronologia modifiche.</span>

* **Elenco cronologia modifiche** consente di visualizzare un registro delle modifiche apportate agli oggetti di Workfront, inclusi attributi quali:

  * Oggetto
  * Tipo di oggetto
  * Tipo di modifica (operazione)
  * Source della modifica, ad esempio utenti specifici, API, Workfront Fusion, AI LLM o Workfront

  <span class="preview">L&#39;attività del flusso di lavoro di revisione e approvazione unificata viene registrata nella Cronologia modifiche, inclusi i partecipanti e le decisioni.</span>

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td><p>Amministratore di sistema</p>
       <p><span class="preview">Per visualizzare la cronologia modifiche: accesso amministrativo alla cronologia modifiche</span></p>
       <p><span class="preview">Per configurare i campi tracciati: amministratore di sistema</span></p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<div class="preview">

## Aggiungi i campi di cui vuoi tenere traccia

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Tracciamento modifiche > Configurazione**.
1. Nella schermata Configurazione, fare clic su **Aggiungi campo**.
1. Nella casella **Aggiungi campi** selezionare un oggetto. È possibile iniziare a digitare il nome dell&#39;oggetto, quindi selezionarlo quando viene visualizzato nell&#39;elenco.
1. Quindi, selezionare i nomi dei campi di cui si desidera tenere traccia per l&#39;oggetto. È possibile digitare il nome del campo e selezionarlo quando viene visualizzato nell&#39;elenco.

   Per l’oggetto sono disponibili sia campi personalizzati che campi nativi.
   I campi già tracciati vengono visualizzati come selezionati nell’elenco.

   ![Aggiungi campi per rilevamento modifiche](assets/change-history-config-add-fields.png)

1. Dopo aver selezionato tutti i campi da monitorare, fai clic su **Aggiungi**.

   I campi vengono aggiunti all&#39;elenco Campi tracciati.

## Rimuovi i campi che non desideri più tracciare

È possibile rimuovere i campi di cui non si desidera tenere traccia per un particolare tipo di oggetto nell&#39;interfaccia di Workfront.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Tracciamento modifiche > Configurazione**.
1. Nella schermata Configuration, seleziona il campo o i campi che desideri interrompere il tracciamento.

   È possibile che lo stesso nome di campo venga visualizzato più volte. I campi sono raggruppati per oggetto, in modo da poter individuare il campo corretto. Puoi anche utilizzare la casella di ricerca nella parte superiore dello schermo.

1. Seleziona **Elimina** nella barra delle azioni nella parte inferiore dello schermo.
1. Fai clic su **Rimuovi** nel messaggio di conferma.

   I campi vengono rimossi dall&#39;elenco Campi tracciati.

</div>

## Visualizza l&#39;area di configurazione per il rilevamento delle modifiche

>[!NOTE]
>
>Nell’ambiente di produzione, Configuration è attualmente disponibile solo come informazione e non può essere modificato. La possibilità di modificare i campi tracciati sarà disponibile nel prossimo futuro.

Per visualizzare i tipi di modifiche tracciate:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Traccia delle revisioni >** Configurazione**.

   I campi vengono visualizzati raggruppati per tipo di oggetto.

1. Per visualizzare i campi sotto un oggetto specifico, fare clic sulla freccia a discesa accanto al tipo di oggetto.

## Visualizzare l&#39;elenco Cronologia modifiche

Gli amministratori di Workfront possono visualizzare la cronologia delle modifiche nell’area Configurazione.

L&#39;elenco Cronologia modifiche è un elenco avanzato e include filtri, colonne, altezza riga, selezione data e barra di ricerca.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Tracciamento modifiche > Elenco cronologia modifiche**.

   Viene visualizzato l&#39;elenco Cronologia modifiche (Change History List).

1. Per modificare le date per le quali vengono visualizzate le modifiche, fai clic sul selettore di date e seleziona le nuove date.

   Le modifiche sono disponibili per gli ultimi 90 giorni.

1. Per cercare un termine specifico, fare clic sulla barra di ricerca e immettere il termine desiderato. I risultati vengono evidenziati nell&#39;elenco durante la digitazione.
1. (Facoltativo) Per filtrare in base a una colonna, vedi [Filtrare gli elementi in un elenco avanzato](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list) nell&#39;articolo [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Facoltativo) Per nascondere, visualizzare o riordinare le colonne, vedere [Personalizzare le colonne](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns) nell&#39;articolo [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Facoltativo)Per aggiungere o rimuovere colonne, vedere [Aggiungere e rimuovere colonne con Gestione colonne](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager) nell&#39;articolo [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Facoltativo)Per regolare l&#39;altezza delle righe, vedere [Modificare l&#39;altezza delle righe in una visualizzazione](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view) nell&#39;articolo [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Esporta cronologia modifiche

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Tracciamento modifiche > Elenco cronologia modifiche**.
1. Filtrare l&#39;elenco per visualizzare gli elementi da esportare.
1. Fai clic sull&#39;icona **Esporta** ![Icona Esporta](assets/export-icon.png) e seleziona se desideri salvare in formato XLSX o CSV.

   Viene visualizzata la casella Salva file (Save file), che consente di salvare il file esportato sul computer.
   Completate il salvataggio del file esportato. Ora è possibile trovarlo nel computer e condividerlo con altri utenti.



