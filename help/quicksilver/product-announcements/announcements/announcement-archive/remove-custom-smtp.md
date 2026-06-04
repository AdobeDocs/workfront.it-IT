---
content-type: reference
navigation-topic: announcements
title: Rimuovere l’SMTP personalizzato come opzione e-mail in uscita
description: Con la versione 20.3 (prevista per agosto 2020), Adobe Workfront sta passando a un nuovo sistema e-mail che migliorerà notevolmente l’affidabilità della consegna e-mail per gli aggiornamenti e le notifiche di Workfront. Di conseguenza, i clienti non potranno più utilizzare il proprio server di posta elettronica SMTP per inoltrare la propria e-mail dalla piattaforma Workfront al destinatario desiderato. Tutte le e-mail verranno inviate direttamente dal server di Workfront Mail.
author: Luke
feature: Product Announcements
exl-id: 73abd185-81c6-43fc-b8b0-cad14d15b348
TQID: https://experienceleague.adobe.com/q3IdES8LZlJDDBjUqTkHmWqjtVdMV-w80o7wC-uRSXg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 306
ht-degree: 7%

---

# Rimuovere l’SMTP personalizzato come opzione e-mail in uscita

>[!NOTE]
>
>La funzionalità descritta in questo articolo non è più disponibile e l&#39;articolo verrà rimosso a breve.

Con la versione 20.3 (prevista per agosto 2020), Adobe Workfront sta passando a un nuovo sistema e-mail che migliorerà notevolmente l’affidabilità della consegna e-mail per gli aggiornamenti e le notifiche di Workfront. Di conseguenza, i clienti non potranno più utilizzare il proprio server di posta elettronica SMTP per inoltrare la propria e-mail dalla piattaforma Workfront al destinatario desiderato. Tutte le e-mail verranno inviate direttamente dal server di Workfront Mail.

Per accedere a questa funzione, accedi come amministratore di sistema e seleziona Configurazione > E-mail > Configurazione. Ecco una schermata che evidenzia la funzione:

![Impostazioni server e-mail](assets/email-server-settings-350x226.png)

L’impostazione evidenziata in questa schermata passerà automaticamente all’opzione Workfront Mail Server con la versione 20.3.

Se hai configurato un server di posta SMTP personalizzato, **ti consigliamo vivamente di contattare il tuo team IT** per assicurarti che l&#39;e-mail da notifications@my.workfront.com non venga bloccata per le e-mail in arrivo nel tuo sistema. Puoi anche fare riferimento a Configurazione del firewall per i dettagli sugli indirizzi IP da cui provengono il traffico e l’e-mail.

Per ulteriori domande o dubbi, contattare il [team di supporto Workfront](https://experienceleague.adobe.com/?support-tab=home&lang=it#support).
