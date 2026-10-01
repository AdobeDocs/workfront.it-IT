---
user-type: administrator
product-area: system-administration;setup
title: Configurare la localizzazione personalizzata
description: La localizzazione personalizzata consente di definire termini e frasi personalizzati in lingue diverse. Workfront visualizza quindi questi termini nella lingua impostata nelle impostazioni del browser.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bdc6d5ee-2037-4d0b-bf18-3e6cc9cb078e
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: b077c95d8bb795fcd7c0983c78b7533cb8167270
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 5%
---
# Configurare la localizzazione personalizzata

{{highlighted-preview}}

La localizzazione personalizzata consente di <span class="preview"> utilizzare l&#39;intelligenza artificiale</span> per definire termini e frasi personalizzati in lingue diverse. Workfront visualizza questi termini nella lingua impostata nelle impostazioni Adobe Identity Management (IMS) dell’utente.

Ad esempio, l’etichetta &quot;Pubblico di destinazione&quot; può essere localizzata nella parola tedesca &quot;Zielgruppe&quot;. Qualsiasi utente che utilizza come lingua principale del browser il tedesco vede la parola &quot;Zielgruppe&quot; come un’etichetta per qualsiasi campo etichettato &quot;Target Audience&quot; in inglese.

Puoi configurare le traduzioni in più lingue. Le lingue attualmente disponibili includono:

* Cinese (tradizionale)
* Cinese (semplificato)
* Francese
* Tedesco
* Italiano
* Giapponese
* Coreano
* Portoghese (Brasile)
* Spagnolo

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Prime flusso di lavoro o superiore </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Standard</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Per configurare le traduzioni è necessario essere un amministratore di Workfront.</p>  </td> 
  </tr>
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni durante l’impostazione della localizzazione

Quando configuri la localizzazione, tieni presente quanto segue:

* Puoi configurare un termine per la traduzione in più lingue.
* La localizzazione si applica alle etichette dei campi personalizzati (anche quando vengono utilizzate come intestazione di colonna) e alle descrizioni.
* La localizzazione personalizzata può essere applicata ai messaggi generati da Regole aziendali, ma deve essere abilitata nella Regola aziendale.

  Per istruzioni, vedere [Abilitare la localizzazione in una regola business](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md#using-custom-localization-with-business-rules) nell&#39;articolo Creare e modificare le regole business.

## Configurare le traduzioni

Le traduzioni vengono configurate nell’area Configurazione.

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic sull&#39;icona **[!UICONTROL Setup]** ![Setup](/help/_includes/assets/gear-icon-setup.png).
1. Nell&#39;area Configura fare clic su **Localizzazione** nel pannello di navigazione a sinistra.
1. Per aggiungere una nuova traduzione, fare clic su **Nuova riga**.
1. Nella colonna **Inglese** immettere il termine inglese da tradurre.
1. Nella colonna relativa alla lingua in cui si desidera tradurre il termine, immettere il termine nella lingua di destinazione.
1. (Facoltativo) Per tradurre la parola in lingue aggiuntive, aggiungi la traduzione nella colonna della lingua appropriata.
1. (Facoltativo) Per riordinare le colonne della lingua, fai clic sull’intestazione di una colonna da spostare e trascinala nella posizione desiderata.
1. (Facoltativo) Per eliminare le traduzioni per un termine, fai clic sulla casella di controllo accanto al termine, quindi fai clic su **Elimina** nella barra blu nella parte inferiore della pagina.

<div class="preview">

## Localizzare il testo personalizzato non tradotto utilizzando le traduzioni basate su IA

Puoi utilizzare l’intelligenza artificiale per localizzare il testo personalizzato. Seleziona il termine e le lingue e puoi approvare le traduzioni prima che vengano applicate.

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic sull&#39;icona **[!UICONTROL Setup]** ![Setup](/help/_includes/assets/gear-icon-setup.png).
1. Nell&#39;area Configura fare clic su **Localizzazione** nel pannello di navigazione a sinistra.
1. Nell&#39;area Localizzazione selezionare la scheda **Testo personalizzato non tradotto**.

   Viene visualizzato un elenco di testo personalizzato non tradotto. Sono inclusi testo come etichette di campo e messaggi di regole personalizzati.

1. Selezionare uno o più termini da localizzare.
1. Nella barra blu nella parte inferiore dello schermo, seleziona **Traduci con IA**.

   Viene visualizzata la finestra Genera traduzioni.

1. Fare clic sulle lingue in cui si desidera tradurre il termine o i termini. Per selezionare rapidamente tutte le lingue, fare clic su **Seleziona tutto**.
1. (Facoltativo) Per fornire indicazioni più specifiche per la traduzione, immetti le istruzioni nel campo &quot;Istruzioni per IA&quot;.
1. Fai clic su **Genera**.

   L&#39;intelligenza artificiale inizia a generare le traduzioni.

   Viene visualizzata la finestra Rivedi traduzioni.

1. (Facoltativo) Per modificare le traduzioni o aggiungere una traduzione personalizzata, fai clic su nel quadrato appropriato della tabella e digita la traduzione desiderata.
1. Fai clic su **Salva**.

## Tradurre un termine localizzato in altre lingue

Puoi tradurre un termine localizzato in precedenza in nuove lingue utilizzando l’intelligenza artificiale, oppure fornire una traduzione personalizzata.

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic sull&#39;icona **[!UICONTROL Setup]** ![Setup](/help/_includes/assets/gear-icon-setup.png).
1. Nell&#39;area Configura fare clic su **Localizzazione** nel pannello di navigazione a sinistra.
1. Nell&#39;area Localizzazione selezionare la scheda **Traduzioni**.

   Viene visualizzato un elenco dei termini tradotti in precedenza e delle relative traduzioni.

1. (Facoltativo) Per modificare o immettere direttamente una traduzione, fai clic sulla casella appropriata nella tabella e digita la traduzione desiderata.
1. Selezionare i termini per i quali si desidera generare traduzioni aggiuntive facendo clic sulle caselle di controllo accanto a tali termini.
1. Nella barra blu nella parte inferiore della pagina, fai clic su **Compila con AI**.


   Viene visualizzata la finestra Genera traduzioni.

1. Fare clic sulle lingue in cui si desidera tradurre il termine o i termini. Per selezionare rapidamente tutte le lingue, fare clic su **Seleziona tutto**.
1. (Facoltativo) Per fornire indicazioni più specifiche per la traduzione, immetti le istruzioni nel campo &quot;Istruzioni per IA&quot;.
1. Fai clic su **Genera**.

   L&#39;intelligenza artificiale inizia a generare le traduzioni.

   Viene visualizzata la finestra Rivedi traduzioni.

1. (Facoltativo) Per modificare le traduzioni o aggiungere una traduzione personalizzata, fai clic su nel quadrato appropriato della tabella e digita la traduzione desiderata.
1. Fai clic su **Salva**.
1. (Facoltativo) Per eliminare tutte le traduzioni per un termine, fai clic sulla casella di controllo accanto al termine, quindi fai clic su **Elimina** nella barra blu nella parte inferiore della pagina.


</div>
