---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Panoramica sulle richieste del team
description: Le richieste del team si trovano nell'area Team nel menu principale.
author: Lisa
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: 9693ac3792fec3eca6218a228f2067519ed433ac
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Panoramica sulle richieste del team

## Comprendere le richieste del team

Le richieste del team si trovano in [!UICONTROL Team] nella zona [!UICONTROL Menu principale]. Fai clic sul pulsante [!UICONTROL Richieste del team] icona ![Icona della richiesta](assets/request-icon.png) nel pannello a sinistra per visualizzare le richieste del team.

>[!NOTE]
>
>I team Agile non dispongono di richieste team.

La [!UICONTROL Richieste del team] mostra le richieste in attesa di assegnazione per il team attualmente selezionato nell’elenco a discesa. Il numero tra parentesi indica quanti elementi sono pronti per essere lavorati.

Una richiesta del team rappresenta un elemento di lavoro in sospeso non assegnato a un utente specifico. Al contrario, viene assegnato a un team, e qualsiasi membro del team può volontariamente accettare la responsabilità per l&#39;oggetto. Se un utente si offre volontario per lavorare su una richiesta del team, l&#39;utente accetta l&#39;assegnazione del lavoro come proprio. L’attività viene assegnata al singolo utente oltre al team.

>[!NOTE]
>
>Non utilizzare una richiesta team per le assegnazioni di attività collaborative. Se è necessario assegnare più utenti per lavorare insieme a un&#39;attività, eseguire questa operazione tramite [!UICONTROL Assegnazioni avanzate] e non tramite richieste Team. Per ulteriori informazioni, consulta [Creazione di assegnazioni avanzate](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Comprendere il [!UICONTROL Pronto per l&#39;inizio] e [!UICONTROL Tutto] options

Nella parte superiore della sezione Richieste team sono disponibili due opzioni: [!UICONTROL Pronto per l&#39;inizio] e [!UICONTROL Tutto].

La [!UICONTROL Pronto per l&#39;inizio] mostra solo le attività e i problemi che soddisfano tutti i seguenti criteri:

* Tutti i predecessori hanno soddisfatto le condizioni per i tipi di dipendenza precedenti.\
   Ad esempio, se il tipo di relazione predecessore è [!UICONTROL Fine-Inizio] (l&#39;attività predecessore deve terminare prima dell&#39;avvio dell&#39;attività dipendente), il predecessore deve essere contrassegnato come [!UICONTROL Completa]. (Per ulteriori informazioni sui tipi di dipendenza predecessore, consulta [Panoramica dei tipi di dipendenza dell&#39;attività](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).)

* L&#39;utente connesso è la persona assegnata a queste attività e a questi problemi (per le richieste di lavoro), oppure il team selezionato viene assegnato a queste attività e a questi problemi (per le richieste del team).
* Lo stato del progetto è in uno stato [!UICONTROL Corrente].
* La [!UICONTROL Data di inizio prevista] o [!UICONTROL Data di inizio prevista] è passato o è previsto che inizi entro due settimane dalla data odierna (o no [!UICONTROL Data di inizio prevista] o [!UICONTROL Data di inizio prevista] è stato definito).
* La [!UICONTROL Data di consegna] si è già verificato o si verificherà entro due settimane dalla data corrente.

>[!NOTE]
>
>Se l’attività soddisfa i primi tre criteri e ha una data di fine entro due settimane dalla data corrente, verrà visualizzata come [!UICONTROL Pronto per l&#39;inizio] anche se le date previste/previste sono oltre le due settimane. Se l&#39;attività non dispone di una data di consegna, le date previste/previste devono essere entro due settimane dalla data corrente.

La [!UICONTROL Tutto] mostra tutte le attività e i problemi relativi ai progetti correnti assegnati all&#39;utente connesso o a tutte le attività o problemi assegnati al team.
