---
title: 23.2 - Miglioramenti per la gestione delle risorse
description: 23.2 - Miglioramenti per la gestione delle risorse
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b225ae19-eee7-4329-a42d-2a2bf9adad01
TQID: https://experienceleague.adobe.com/QzjHfD9RX0nF8Bk84Rq3yFTJvQpKMJPq9YmIXjJ9QJw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 277
ht-degree: 8%

---

# 23.2 - Miglioramenti per la gestione delle risorse

Questa pagina descrive tutti i miglioramenti alla gestione delle risorse apportati con la versione 23.2 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione con la versione 23.2.

Per un elenco di tutte le modifiche disponibili a questo punto del ciclo di rilascio 23.2, vedere [Panoramica sulla versione 23.2](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Introduzione del campo Tempo di lavoro per calcolare con precisione la capacità dell&#39;utente

>[!NOTE]
>
>Versione di anteprima: 16 febbraio 2023; versione di produzione pianificata: 2 marzo 2023

Per consentire ai responsabili delle risorse di calcolare con precisione la disponibilità dei loro utenti e tenere conto del tempo che gli utenti dedicano al lavoro effettivo relativo al progetto, stiamo introducendo il concetto di orario di lavoro in Adobe Workfront.

È possibile definire il valore del campo Tempo di lavoro per ogni utente al momento della creazione o della modifica del profilo. Per ulteriori informazioni, vedere [Modificare il profilo di un utente](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Il campo Tempo di lavoro rappresenta la percentuale di tempo equivalente a tempo pieno (FTE) disponibile per il lavoro effettivo, esclusi i costi comuni. L&#39;orario di lavoro deve essere un numero decimale con un valore compreso tra 0 e 1. Ad esempio, una disponibilità del 20% per il lavoro effettivo sarebbe 0,2.

Il valore predefinito del campo è 1, che indica che un utente spende l’intero FTE per il lavoro effettivo relativo al progetto.

In seguito a questo aggiornamento, Workfront calcola la disponibilità dell&#39;utente utilizzando le formule seguenti, a seconda della selezione effettuata nell&#39;area delle preferenze Gestione risorse:

* Pianificazione predefinita:
* Capacità utente = [(Ore programmate - Eccezioni programmate) `*` FTE - Indisponibilità] `*` Orario di lavoro
* Pianificazione utente:
* Capacità utente = (Ore programmate - Eccezioni programmate - Indisponibilità) `*` orario di lavoro.

Per ulteriori informazioni, vedere [Configurare le [!UICONTROL preferenze per la gestione delle risorse]](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3415608/){target=_blank}
