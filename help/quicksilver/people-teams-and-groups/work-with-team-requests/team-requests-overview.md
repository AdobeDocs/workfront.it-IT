---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Panoramica delle richieste di team
description: Le richieste dei team si trovano nell’area Team nel menu principale.
author: Courtney
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/usIfdIZm77U8ltA5lj37cqAp7uHoSSnRD4wuPx863ZM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 486
ht-degree: 0%

---

# Panoramica delle richieste dei team

## Comprendere le richieste del team

Richieste team trovate nell&#39;area [!UICONTROL Team] nel [!UICONTROL Menu principale]. Fai clic sull&#39;icona [!UICONTROL Richieste team] ![Icona richiesta](assets/request-icon.png) nel pannello a sinistra per visualizzare le richieste team.

>[!NOTE]
>
>I team Agile non dispongono di richieste team.

La scheda [!UICONTROL Richieste team] mostra le richieste in attesa di assegnazione per il team attualmente selezionato nell&#39;elenco a discesa. Il numero tra parentesi indica il numero di elementi pronti per essere lavorati. La scheda [!UICONTROL Richieste team] può visualizzare fino a 2.000 richieste per un team.

Una richiesta team rappresenta un elemento di lavoro in sospeso non assegnato a un utente specifico. Viene invece assegnato a un team, e qualsiasi membro di quel team può offrirsi volontario per accettare la responsabilità per l’elemento. Se un utente si offre volontario per lavorare su una richiesta del team, accetta l’assegnazione del lavoro come propria. L’attività viene assegnata al singolo utente oltre che al team.

>[!NOTE]
>
>Non utilizzare una richiesta team per assegnazioni di attività collaborative. Se devi assegnare più utenti per lavorare insieme su un&#39;attività, esegui questa operazione tramite [!UICONTROL Assegnazioni avanzate] e non tramite richieste del team. Per ulteriori informazioni, vedere [Creare assegnazioni avanzate](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Comprendere le opzioni [!UICONTROL Pronto per iniziare] e [!UICONTROL Tutti]

Nella parte superiore della sezione Richieste team sono disponibili due opzioni: [!UICONTROL Pronto per iniziare] e [!UICONTROL Tutto].

L&#39;opzione [!UICONTROL Pronto per l&#39;avvio] mostra solo le attività e i problemi che soddisfano tutti i criteri seguenti:

* Tutti i predecessori hanno soddisfatto le condizioni per i tipi di dipendenza predecessori.\
  Ad esempio, se il tipo di relazione predecessore è [!UICONTROL Fine-Inizio] (l&#39;attività predecessore deve terminare prima che l&#39;attività dipendente possa iniziare), il predecessore deve essere contrassegnato come [!UICONTROL Completo]. Per ulteriori informazioni sui tipi di relazione predecessore, vedere [Panoramica sui tipi di relazione attività](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

* L’utente connesso è la persona assegnata a queste attività e problemi (per le richieste di lavoro), oppure il team selezionato è assegnato a queste attività e problemi (per le richieste di team).
* Lo stato del progetto è [!UICONTROL Corrente].
* La [!UICONTROL Data inizio prevista] o la [!UICONTROL Data inizio prevista] è passata o è prevista entro due settimane dalla data odierna (oppure non è stata definita alcuna [!UICONTROL Data inizio prevista] o [!UICONTROL Data inizio prevista]).
* La [!UICONTROL Data handoff] si è già verificata o si verificherà entro due settimane dalla data corrente.

>[!NOTE]
>
>Se l&#39;attività soddisfa i primi tre criteri e ha una data di handoff entro due settimane dalla data corrente, verrà visualizzata come [!UICONTROL Pronta per iniziare] anche se le date pianificate/previste sono più di due settimane. Se l&#39;attività non ha una data Handoff, le date Pianificato/Previsto devono essere entro due settimane dalla data corrente.

L&#39;opzione [!UICONTROL Tutte] mostra tutte le attività e i problemi dei progetti correnti assegnati all&#39;utente connesso o tutte le attività o i problemi assegnati al team.
