---
navigation-topic: get-started-with-workfront
title: Personalizzare le colonne dell’elenco di lavoro Priorità
description: È possibile personalizzare le colonne dell’elenco lavori in Priorità per supportare il modo in cui si lavora.
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: e4232fbe-1b5c-4614-8613-3b0e25ffee46
TQID: https://experienceleague.adobe.com/YIqeZbiTZH00yXJ6LnQrpEZuHvW4Y5QZVkYU3OquWqE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1880d4370059ad654f91c6f40a0a787c51c1e54e
workflow-type: tm+mt
source-wordcount: 437
ht-degree: 10%

---

# Personalizzare le colonne dell’elenco di lavoro Priorità

{{preview-fast-release-general}}

<!--I think this article can point to the Enhanced lists article for managing the view-->

<!--
<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->


È possibile personalizzare le colonne dell’elenco lavori in Priorità per supportare il modo in cui si lavora.

In Priorità vengono visualizzati gli elementi di lavoro assegnati all&#39;utente. Non è possibile visualizzare gli elementi di lavoro assegnati al team.

<!--
>[!NOTE]
>
>You cannot add custom data to columns at this time.
-->

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Pacchetto Adobe Workfront</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza di Adobe Workfront</strong></td> 
   <td> 
   <p>Revisore o versione successiva</p>
   <p>Chiaro o superiore</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso</strong></td> 
   <td> <p>Accesso di visualizzazione o modifica per l'oggetto su cui si trova l'aggiornamento</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni sugli oggetti</strong></td> 
   <td> <p>Accesso di visualizzazione all'oggetto</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizzare le colonne dell’elenco di lavoro Priorità

### Attiva o disattiva colonne

{{step1-to-priorities}}

1. Fai clic su **Colonne** nella parte sinistra della schermata.

   <span class="preview">Immagine di esempio nell&#39;ambiente di anteprima:</span>
   ![Colonne](assets/columns-new-060226.png)

   Immagine di esempio nell’ambiente di produzione:
   ![Colonne](assets/columns-new.png)

1. Utilizzare gli interruttori per visualizzare o nascondere le colonne nell&#39;elenco lavori.

### Riordinare le colonne

{{step1-to-priorities}}

1. Fai clic su **Colonne** nella parte sinistra della schermata.
1. Fai clic sull&#39;icona **Trascina** e sposta la colonna nella posizione desiderata. Spostamento automatico degli aggiornamenti delle colonne nell&#39;elenco lavori.
   ![Riordina colonne](assets/reorder-columns-new.png)

>[!NOTE]
>
>La colonna Nome è fissa e non può essere spostata.

<div class="preview">

### Aggiungere e rimuovere colonne con Gestione colonne

{{step1-to-priorities}}

1. Fai clic sull&#39;icona + nell&#39;angolo superiore destro dell&#39;elenco per aprire la casella **Gestione colonne**.
1. Aggiungere o rimuovere colonne, quindi fare clic su **Salva**.

   >[!NOTE]
   >
   >È possibile aggiungere solo campi esistenti alla visualizzazione elenco. Sono disponibili campi nativi e personalizzati per attività e problemi da aggiungere come colonne.

Per ulteriori informazioni sul gestore colonne, vedere la sezione [Aggiungere e rimuovere colonne con il gestore colonne](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager) nell&#39;articolo [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

</div>

### Modificare l&#39;altezza della riga nell&#39;elenco delle priorità

{{step1-to-priorities}}

1. Fai clic sull&#39;icona **Altezza riga**.

   La lunghezza verticale di una riga viene aggiornata. Scegli una tra le opzioni seguenti:

   * Piccola
   * Standard. Questa è la scelta predefinita.
   * Canale
   * Alta

   L’elenco viene aggiornato immediatamente.

<div class="preview">

## Gestire le visualizzazioni per l&#39;elenco delle priorità

Una vista definisce le colonne, i filtri e i raggruppamenti nell’elenco con le impostazioni predefinite.

All&#39;elenco delle priorità viene assegnata una vista predefinita. Puoi anche creare e condividere le tue viste.

{{step1-to-priorities}}

1. Espandere il menu delle viste a discesa nell&#39;angolo superiore sinistro dell&#39;elenco per selezionare un&#39;altra vista oppure fare clic su **Nuova vista** per crearne un&#39;altra.
1. Aggiornare le colonne, i filtri e i raggruppamenti che si desidera includere nella visualizzazione.

   Le modifiche alle viste vengono salvate automaticamente. Alla successiva applicazione di questa visualizzazione, le impostazioni delle colonne e dei filtri rimangono invariate.

Per ulteriori informazioni sulle visualizzazioni, vedere la sezione [Aggiornare gli elementi dell&#39;elenco avanzato](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#update-enhanced-list-elements) nell&#39;articolo [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

</div>
