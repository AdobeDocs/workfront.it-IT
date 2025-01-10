---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Configurare l’indisponibilità personale
description: È importante indicare in Adobe Workfront quando si verifica l’assenza approvata, perché influisce sulla pianificazione e sulle date di completamento pianificate delle attività a cui sei assegnato.
author: Courtney
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: fa5a59c15395f825ad73d889d4d877224a676891
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Configurare l’indisponibilità personale

<!-- Audited: 12/2023 -->

[!DNL Adobe Workfront] non è progettato per replicare o sostituire i sistemi esistenti per gestire, accantonare e tenere traccia delle indisponibilità personali.

Tuttavia, è importante indicare quando si verifica l&#39;assenza approvata, perché ciò influisce sia sulla pianificazione che sulle [!UICONTROL date di completamento pianificate] delle attività assegnate.

Se ad esempio si è assegnati a un&#39;attività per la quale è previsto un periodo di due settimane e si prevede di prendere tre giorni di ferie durante tale periodo, [!DNL Workfront] aggiunge tre giorni alla sequenza temporale dell&#39;attività per tenere conto del periodo di ferie.

Gli strumenti di gestione delle risorse utilizzano anche il proprio tempo libero personale per indicare quando si è disponibili per essere programmati per il lavoro.

>[!NOTE]
>
>Per evitare incoerenze con le date per le quali pianifichi le ferie, consigliamo che il fuso orario del profilo utente corrisponda a quello della pianificazione. Per ulteriori informazioni, consulta i seguenti articoli:
>
>* [Crea una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Modifica il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
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
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> <p>Nuovo: Standard (per configurare il proprio tempo libero personale)</p>
        <p>oppure</p>
        <p>Corrente: Lavoro o versione successiva (per configurare il proprio tempo libero personale)</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Accesso a [!UICONTROL Manager] con [!UICONTROL Modifica utente] (per apportare modifiche al calendario di indisponibilità di altri utenti)<br>
   <strong>NOTA:</strong> se un manager modifica il calendario personale di ferie per un altro utente, tutte le voci vengono visualizzate nel fuso orario dell'utente e non in quello del manager.</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Configura indisponibilità personale in [!DNL Workfront]

{{step1-click-profile-pic}}

>[!NOTE]
>
>Se ti trovi in Adobe Unified Experience, puoi accedere al tuo profilo Workfront facendo clic sul menu dell’account Adobe (immagine del tuo profilo) nell’area di navigazione superiore, quindi scegliendo Profilo Workfront.
>
>![profilo Workfront](assets/aue-profile.png)


1. Nel pannello a sinistra, fai clic su **[!UICONTROL Indisponibilità]**.
1. Seleziona la data desiderata per il tuo tempo libero personale.

   ![Calendario personale per ferie](assets/personal-time-off-calendar.png)

1. Seleziona **[!UICONTROL Tutto il giorno]** se stai prendendo una giornata libera.

   Lasciare deselezionata la casella di controllo se si sta prendendo meno di un giorno intero di ferie e indicare l&#39;ora di inizio e di fine del periodo di ferie.

1. Fai clic su **[!UICONTROL Salva]**.

   Il tuo tempo libero è ora visibile nel sistema [!DNL Workfront] negli strumenti di gestione delle risorse come la pianificazione delle risorse e il bilanciatore dei carichi di lavoro. Quando ti viene assegnato un lavoro durante questo periodo, una descrizione comando informa l’utente che hai pianificato un’indisponibilità.
