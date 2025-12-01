---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Configurare l’indisponibilità personale
description: È importante indicare in Adobe Workfront quando si verifica l’assenza approvata, perché influisce sulla pianificazione e sulle date di completamento pianificate delle attività a cui sei assegnato.
author: Becky
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: 0e37a5a519770d3d48192f1799491aa53a871508
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 4%

---

# Configurare l’indisponibilità personale

<!-- Audited: 12/2025 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

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

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col>
 <tbody> 
  <tr> 
   <td> Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td> <p>Per configurare il proprio periodo di inattività personale, è necessario disporre di:</p>
        <p>Standard (per configurare il proprio tempo libero personale)</p>
        <p>Lavoro o superiore (per configurare il proprio tempo libero personale)</p> </td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td><p>Per apportare modifiche al calendario delle ferie di un altro utente, è necessario essere il manager dell'utente e disporre dell'accesso Modifica utente.</p>
   <p><strong>NOTA:</strong> se un manager modifica il calendario personale di ferie per un altro utente, tutte le voci vengono visualizzate nel fuso orario dell'utente e non in quello del manager.</p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configura indisponibilità personale in [!DNL Workfront]

{{step1-click-profile-pic}}

>[!NOTE]
>
>Se la tua organizzazione si trova nell&#39;esperienza unificata di Adobe, fai clic sul menu dell&#39;account **Adobe** (immagine del tuo profilo) nell&#39;angolo superiore destro dell&#39;area di navigazione superiore, quindi fai clic su **Profilo Workfront**.
>
>![profilo Workfront](assets/aue-profile.png)

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Indisponibilità]**.
1. Seleziona la data desiderata per il tuo tempo libero personale.

   ![Calendario personale per ferie](assets/personal-time-off-calendar-0925.png)

   <!--Sample image in the Production environment:
   ![Personal time off calendar](assets/personal-time-off-calendar.png)-->

1. Seleziona **[!UICONTROL Tutto il giorno]** se stai prendendo una giornata libera.

   Lasciare deselezionata la casella di controllo se si sta prendendo meno di un giorno intero di ferie e indicare l&#39;ora di inizio e di fine del periodo di ferie.

1. Fai clic su **[!UICONTROL Salva]**.

   Il tuo tempo libero è ora visibile nel sistema [!DNL Workfront] negli strumenti di gestione delle risorse come la pianificazione delle risorse e il bilanciatore dei carichi di lavoro. Quando ti viene assegnato un lavoro durante questo periodo, una descrizione comando informa l’utente che hai pianificato un’indisponibilità.
