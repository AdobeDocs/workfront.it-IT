---
content-type: reference
navigation-topic: announcements
title: Nuovo sistema gestito da Adobe Workfront per sostituire POP Email per le code delle richieste con 21.1
description: Stiamo sostituendo l’opzione e-mail POP per le code di richieste con un nuovo sistema gestito da Adobe Workfront. Sarà comunque possibile inviare le richieste tramite e-mail, ma sarà necessario impostare un nuovo indirizzo e-mail gestito da Workfront nell’area Coda richieste.
author: Luke
feature: Product Announcements
exl-id: d7147641-ba36-422b-a9b2-3c2f4ab609d8
TQID: https://experienceleague.adobe.com/zzr53eiyA6o-VpZQnFQt-xCXZBKaScZUz8jDmOgX-Ns
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 332
ht-degree: 4%

---

# Nuovo sistema gestito da Adobe Workfront per sostituire POP email for Request Queues con 21.1

Stiamo sostituendo l’opzione e-mail POP per le code di richieste con un nuovo sistema gestito da Adobe Workfront. Sarà comunque possibile inviare le richieste tramite e-mail, ma sarà necessario impostare un nuovo indirizzo e-mail gestito da Workfront nell’area Coda richieste.

## Perché stai rimuovendo l’opzione POP email?

La tecnologia POP è un&#39;opzione e-mail inaffidabile e meno sicura. Inoltre, vediamo un sacco di problemi dei clienti relativi specificamente alla POP email. Passare a un sistema gestito da Workfront offre un&#39;esperienza più affidabile.

## Quale azione devo intraprendere?

Devi impostare un nuovo indirizzo e-mail per ogni coda di richieste configurata con POP email nell’ambiente di produzione e distribuire il nuovo indirizzo e-mail in base alle esigenze. Per ulteriori informazioni, vedere [Consentire agli utenti di inviare un problema tramite e-mail a un progetto della coda richieste](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Qual è il piano di transizione?

A partire dalla versione 21.1 di inizio febbraio, gli utenti avranno 60 giorni di tempo per passare al nuovo indirizzo e-mail *@intake.workfront.com* creato. Durante il periodo di 60 giorni, l’e-mail POP utilizzata in precedenza continuerà a funzionare.

## Come posso eseguire il test in Anteprima?

Per verificare questa modifica nell’anteprima, devi abilitare le e-mail nell’ambiente di anteprima. A questo scopo, segui le istruzioni riportate nella sezione Gestione delle e-mail in anteprima in [Abilita la consegna di e-mail dall&#39;ambiente Sandbox di anteprima](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!IMPORTANT]
>
>Ciò che hai impostato qui non verrà trasferito all&#39;ambiente di produzione. Dovrai eseguire di nuovo questo processo dopo aver rilasciato la funzionalità in Produzione.
