---
user-type: administrator
product-area: system-administration;setup
title: Visualizzare e gestire la cronologia modifiche
description: La cronologia modifiche consente di visualizzare un registro delle modifiche apportate a oggetti e campi di Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 1e06115eb5688271e2a6f4c8a41647eb644d8292
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 5%

---

# Visualizzare e gestire la cronologia delle modifiche

{{preview-fast-release-general}}

La cronologia delle modifiche consente all’amministratore di sistema di configurare e tenere traccia delle modifiche apportate a oggetti e campi specifici in Adobe Workfront. La configurazione flessibile consente all’amministratore di impostare esattamente quali oggetti e campi vengono tracciati.

La cronologia delle modifiche consente di tenere traccia dei seguenti tipi di dati definiti:

* Attività nell’area Configura, ad esempio creazione o eliminazione di un livello di accesso o di una mansione
* Aggiornamenti a livello di campo, ad esempio la modifica della descrizione di un progetto o del modello di layout di un utente
* Aggiornamenti degli oggetti, ad esempio aggiornamento dello stato di un progetto o aggiunta di un modulo personalizzato a un&#39;attività
* <span class="preview">Attività del flusso di lavoro di revisione e approvazione unificata, inclusi partecipanti e decisioni</span>

Per informazioni sulla definizione degli oggetti e dei campi tracciati, vedere [Configurare i campi da tracciare nella cronologia delle modifiche](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/configure-fields-in-change-history.md).

Nell&#39;elenco Cronologia modifiche è possibile visualizzare il registro delle modifiche apportate agli oggetti di Workfront, inclusi attributi quali:

* Nome oggetto
* Tipo di oggetto
* Tipo di modifica (operazione)
* Data e ora della modifica
* Source della modifica, ad esempio utenti specifici, API, Workfront Fusion, AI LLM o Workfront

>[!NOTE]
>
>Quando si accede a Cronologia modifiche, le revisioni vengono visualizzate solo per i campi per i quali si dispone delle autorizzazioni di visualizzazione.
>Se ad esempio si tiene traccia dei dati finanziari nei progetti e non si ha accesso ai dati finanziari, i campi finanziari non verranno visualizzati nell&#39;elenco Cronologia modifiche.

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
   <td><span class="preview">Accesso amministrativo alla cronologia delle modifiche</span></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare l&#39;elenco Cronologia modifiche

Puoi visualizzare i registri della cronologia delle modifiche nell’area Configurazione.

L&#39;elenco Cronologia modifiche è un elenco avanzato e include filtri, colonne, altezza riga, selezione data e barra di ricerca.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Tracciamento modifiche > Elenco cronologia modifiche**.

   Viene visualizzato l&#39;elenco Cronologia modifiche (Change History List).

1. Per modificare le date per le quali vengono visualizzate le modifiche, fai clic sul selettore di date e seleziona le nuove date.

   Le modifiche sono disponibili per gli ultimi 90 giorni.

1. Per cercare un termine specifico, fare clic nella casella di ricerca e immettere il termine desiderato. I risultati vengono evidenziati nell&#39;elenco durante la digitazione.
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



