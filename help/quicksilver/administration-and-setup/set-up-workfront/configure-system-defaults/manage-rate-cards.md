---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Gestire le schede delle tariffe
description: Le schede tariffa consentono di definire più tariffe di fatturazione per ruolo, in base alla posizione.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: a61635022da9eed7c2fc61bad1cbca0f7f23d7ec
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# Gestire le schede delle tariffe

{{highlighted-preview-article-level}}

Le schede tariffa consentono di definire più tariffe di fatturazione per ruolo, in base alla posizione. Potresti avere un lavoro di Designer con sede a Parigi e un secondo Designer con sede a New York, ciascuno con tariffe di fatturazione diverse. Tuttavia, non è necessario specificare una posizione per le mansioni su una scheda tariffaria. Una tariffa di fatturazione per una mansione (e possibilmente l&#39;ubicazione) su una scheda della tariffa può includere anche date di validità.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td><p>Nuovo piano: [!UICONTROL Standard] </p>
       <p>oppure</p> 
       <p>Piano corrente: [!UICONTROL Plan] </p>
   </td>    
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a [!UICONTROL Financial Data]</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Per modificare una scheda delle tariffe condivisa con te, devi disporre delle autorizzazioni di gestione per tale scheda.</td> 
  </tr> 
 </tbody> 
</table>

## Aggiungi una scheda tariffa

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su [!UICONTROL **Classifica schede**].
1. Clic [!UICONTROL **Nuova scheda tariffaria**], quindi digita un nome per la scheda delle tariffe nel [!UICONTROL Nuova scheda tariffaria] per sostituire &quot;Tasso senza titolo&quot;.
1. (Facoltativo) Nella schermata Dettagli scheda tariffa, aggiungi un [!UICONTROL **Descrizione**].
1. (Facoltativo) Per allegare un modulo personalizzato alla scheda delle tariffe, fai clic sul pulsante [!UICONTROL **Aggiungi modulo personalizzato**] nell&#39;angolo superiore destro e selezionare un modulo personalizzato dall&#39;elenco visualizzato.

   Per ulteriori informazioni su come allegare un modulo personalizzato, consulta [Aggiungere un modulo personalizzato a un oggetto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Clic [!UICONTROL **Ruoli e tassi**] nel pannello di navigazione a sinistra.
1. Nella schermata Rate Card Job Roles and Rates (Ruoli e tariffe delle schede di tariffa), fare clic su [!UICONTROL **Aggiungi mansione**].
1. Nella finestra di dialogo, seleziona una [!UICONTROL **Ruolo**] per definire le tariffe di fatturazione per.

   Nel campo Tariffa di fatturazione predefinita viene visualizzata la tariffa a livello di sistema per questa mansione, se definita.

   ![Finestra di dialogo Nuova tariffa di fatturazione](assets/location-rate-for-rate-card.png)

1. Seleziona un [!UICONTROL **Valuta**] per il ruolo.
1. (Facoltativo) Seleziona un [!UICONTROL **Posizione**] per il ruolo.
1. In [!UICONTROL **Tariffa di fatturazione 1**] , immettere la tariffa di fatturazione per questa ubicazione. Quindi, fai clic su [!UICONTROL **Salva**] per sostituire una sola volta la tariffa di fatturazione.

   Oppure

   Clic [!UICONTROL **Aggiungi tariffa**] per aggiungere altre tariffe di fatturazione specifiche per l’ubicazione con date di validità.

1. (Condizionale) Se si stanno aggiungendo più tariffe di fatturazione per questa ubicazione, inserire le seguenti informazioni:

   * **[!UICONTROL Tariffa di fatturazione 1], 2, ecc.:** Il valore della tariffa di fatturazione per il periodo di tempo.
   * **[!UICONTROL Data di inizio]:** Data di inizio della sostituzione della tariffa.
   * **[!UICONTROL Data di fine]:** Data di fine della sostituzione della tariffa.

     La tariffa di fatturazione 1 non avrà una data di inizio e l&#39;ultima tariffa di fatturazione non avrà una data di fine. Alcune date vengono aggiunte automaticamente. Ad esempio, se la tariffa di fatturazione 1 non ha una data di fine e si aggiunge la tariffa di fatturazione 2 con una data di inizio del 1° maggio 2023, alla tariffa di fatturazione 1 viene aggiunta una data di fine del 30 aprile 2023 in modo che non esistano spazi vuoti.

1. Fai clic su [!UICONTROL **Salva**].
1. (Facoltativo) Per aggiungere un’altra tariffa di fatturazione, per la stessa mansione in un’altra posizione o per una mansione separata, fai clic su [!UICONTROL **Aggiungi mansione**].
1. (Facoltativo) Per modificare una scheda tariffa, fare clic sul nome della scheda tariffa nell&#39;elenco Schede tariffa in Configurazione. Per modificare una tariffa di fatturazione, fai clic su [!UICONTROL **Ruoli e tassi**] nel pannello di navigazione a sinistra della scheda tariffa. Quindi, seleziona la tariffa e fai clic su **Modifica** icona ![Icona Modifica](assets/edit-icon.png).

## Copiare una scheda tariffa

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su [!UICONTROL **Classifica schede**].
1. Seleziona la casella di controllo accanto alla scheda delle tariffe nell’elenco e fai clic su **Copia** icona ![Icona Copia](assets/copy-icon.png).
1. Digita un nome per la scheda della tariffa nel [!UICONTROL Copia scheda della tariffa] per sostituire &quot;Tasso senza titolo&quot;. Quindi, fai clic su **Salva**.

   La nuova scheda tariffe viene salvata. Modifica i dettagli della scheda della tariffa, le mansioni e le tariffe in base alle esigenze.

## Eliminare un&#39;intera scheda tariffaria

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su [!UICONTROL **Classifica schede**].
1. Selezionare la casella di controllo accanto alla scheda delle tariffe nell&#39;elenco e fare clic sul pulsante **Elimina** icona ![Icona Elimina](assets/delete.png).

   >[!NOTE]
   >
   >Una scheda di tariffa allegata a un progetto verrà eliminata dal progetto.
