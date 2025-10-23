---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Configurare l’indisponibilità personale
description: È importante indicare in Adobe Workfront quando si verifica l’assenza approvata, perché influisce sulla pianificazione e sulle date di completamento pianificate delle attività a cui sei assegnato.
author: Becky
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: e25ea757129e9645f7b5f0729cd498d5947f49f2
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Configurare l’indisponibilità personale

<!-- Audited: 12/2023 -->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambiente Sandbox di anteprima ed è in fase di rilascio in un rollout graduale in produzione.</span>

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

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
>Se ti trovi nell’esperienza unificata di Adobe, per accedere al tuo profilo Workfront fai clic sul menu dell’account Adobe (immagine del tuo profilo) nell’area di navigazione superiore, quindi scegli Profilo Workfront.
>
>![profilo Workfront](assets/aue-profile.png)

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Indisponibilità]**.
1. Seleziona la data desiderata per il tuo tempo libero personale.

   <span class="preview">Immagine di esempio nell&#39;ambiente di anteprima:</span>
   ![Calendario personale per ferie](assets/personal-time-off-calendar-0925.png)

   Immagine di esempio nell’ambiente di produzione:
   ![Calendario personale per ferie](assets/personal-time-off-calendar.png)

1. Seleziona **[!UICONTROL Tutto il giorno]** se stai prendendo una giornata libera.

   Lasciare deselezionata la casella di controllo se si sta prendendo meno di un giorno intero di ferie e indicare l&#39;ora di inizio e di fine del periodo di ferie.

1. Fai clic su **[!UICONTROL Salva]**.

   Il tuo tempo libero è ora visibile nel sistema [!DNL Workfront] negli strumenti di gestione delle risorse come la pianificazione delle risorse e il bilanciatore dei carichi di lavoro. Quando ti viene assegnato un lavoro durante questo periodo, una descrizione comando informa l’utente che hai pianificato un’indisponibilità.
