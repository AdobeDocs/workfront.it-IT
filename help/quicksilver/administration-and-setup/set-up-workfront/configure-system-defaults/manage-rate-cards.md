---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Gestire le schede delle tariffe
description: Le schede tariffa consentono di definire più tariffe di fatturazione per ruolo, in base alla posizione.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 1517e3e28fe536a8a72d2802919c8b8819e9ea1a
workflow-type: tm+mt
source-wordcount: '532'
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
   <td><p>Piano legacy: [!UICONTROL Plan]</p>
       <p>Piano corrente: [!UICONTROL Standard]</p></td> 
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
1. Clic [!UICONTROL **Nuova scheda tariffaria**], quindi immettere il nome e la descrizione della scheda tariffaria nell&#39;elenco.
1. Per aggiungere le tariffe di fatturazione, fai clic sul nome della scheda delle tariffe nell’elenco.
1. Nella schermata della scheda, fai clic su [!UICONTROL **Nuova tariffa di fatturazione**].
1. Nella finestra di dialogo Nuova tariffa di fatturazione, seleziona una [!UICONTROL **Ruolo**] per definire le tariffe di fatturazione per.

   Nel campo Tariffa di fatturazione predefinita viene visualizzata la tariffa a livello di sistema per questa mansione.

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
1. (Facoltativo) Per aggiungere un’altra tariffa di fatturazione, per la stessa mansione in un’altra posizione o per una mansione separata, fai clic su [!UICONTROL **Nuova tariffa di fatturazione**].

## Copiare una scheda tariffa

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su [!UICONTROL **Classifica schede**].
1. Seleziona la casella di controllo accanto alla scheda di valutazione nell’elenco e fai clic su **Copia** icona ![Icona Copia](assets/copy-icon.png).

   Viene aggiunta una scheda di frequenza duplicata. Fare clic sul nome della scheda della tariffa nell&#39;elenco per modificarlo.

## Eliminare una scheda tariffa

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su [!UICONTROL **Classifica schede**].
1. Seleziona la casella di controllo accanto alla scheda delle tariffe nell’elenco e fai clic su **Elimina** icona ![Icona Elimina](assets/delete.png).

   >[!NOTE]
   >
   >Una scheda di tariffa allegata a un progetto verrà eliminata dal progetto.
