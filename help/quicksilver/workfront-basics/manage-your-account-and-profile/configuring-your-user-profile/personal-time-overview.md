---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Configurare l’indisponibilità personale
description: È importante indicare in Adobe Workfront quando si verifica l’assenza approvata, perché influisce sulla pianificazione e sulle date di completamento pianificate delle attività a cui sei assegnato.
author: Lisa
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: 6d2494f1ccb2f9b222a953ed8bae922bd0f26389
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# Configurare l’indisponibilità personale

[!DNL Adobe Workfront] non è progettato per replicare o sostituire i sistemi esistenti per gestire, accantonare e tenere traccia del tempo di inattività personale.

Tuttavia, è importante indicare quando si verifica l’assenza approvata, perché questo influisce sia sulla pianificazione che sul [!UICONTROL Date di completamento pianificate] delle attività che ti sono state assegnate.

Se, ad esempio, si è assegnati a un&#39;attività per la quale è programmato un periodo di due settimane e si prevede di prendere tre giorni di ferie durante tale periodo, [!DNL Workfront] aggiunge tre giorni alla sequenza temporale dell&#39;attività per tenere conto del tempo libero.

Gli strumenti di gestione delle risorse utilizzano anche il proprio tempo libero personale per indicare quando si è disponibili per essere programmati per il lavoro.

>[!NOTE]
>
>Per evitare incoerenze con le date per le quali pianifichi le ferie, consigliamo che il fuso orario del profilo utente corrisponda a quello della pianificazione. Per ulteriori informazioni, consulta i seguenti articoli:
>
>* [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>Nuovo: Standard (per configurare il proprio tempo libero personale)</p>
        <p>oppure</p>
        <p>Corrente: Lavoro o versione successiva (per configurare il proprio tempo libero personale)</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td>[!UICONTROL Manager] con accesso a [!UICONTROL Modifica utente] (per apportare modifiche al calendario delle ferie degli altri utenti)<br>
   <strong>NOTA:</strong> Se un manager modifica il calendario personale di ferie dell'utente, tutte le voci vengono visualizzate nel fuso orario dell'utente e non in quello del manager.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Configurare il tempo libero personale in [!DNL Workfront]

{{step1-click-profile-pic}}

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Indisponibilità]**.
1. Seleziona la data desiderata per il tuo tempo libero personale.

   ![Calendario personale delle ferie](assets/personal-time-off-calendar.png)

1. Seleziona **[!UICONTROL Tutto il giorno]**, se sta prendendo un giorno intero di ferie.

   Lasciare deselezionata la casella di controllo se si sta prendendo meno di un giorno intero di ferie e indicare l&#39;ora di inizio e di fine del periodo di ferie.

1. Fai clic su **[!UICONTROL Salva]**.

   Il tempo libero è ora visibile in [!DNL Workfront] negli strumenti di gestione delle risorse, come la pianificazione delle risorse e il bilanciatore dei carichi di lavoro. Quando ti viene assegnato un lavoro durante questo periodo, una descrizione comando informa l’utente che hai pianificato un’indisponibilità.
